# Comparing `tmp/geeViz-2023.7.5.tar.gz` & `tmp/geeViz-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.7.5.tar", last modified: Fri Jul 28 17:23:01 2023, max compression
+gzip compressed data, was "geeViz-2023.8.1.tar", last modified: Thu Aug  3 19:21:09 2023, max compression
```

## Comparing `geeViz-2023.7.5.tar` & `geeViz-2023.8.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.224322 geeViz-2023.7.5/
--rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.7.5/LICENSE
--rw-rw-rw-   0        0        0     3851 2023-07-28 17:23:01.221329 geeViz-2023.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.7.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:00.907172 geeViz-2023.7.5/geeViz/
--rw-rw-rw-   0        0        0      127 2023-07-28 17:18:20.000000 geeViz-2023.7.5/geeViz/__init__.py
--rw-rw-rw-   0        0        0    23538 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.120598 geeViz-2023.7.5/geeViz/examples/
--rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      127 2023-07-28 17:18:12.000000 geeViz-2023.7.5/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/foliumViewerExample.py
--rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/gee2PandasExample.ipynb
--rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14302 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11478 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12263 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/foliumView.py
--rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/gcpLib.py
--rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/gee2Pandas.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.155503 geeViz-2023.7.5/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.158528 geeViz-2023.7.5/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.7.5/geeViz/geeView/css/style.min.css
--rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/foliumView.html
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.202384 geeViz-2023.7.5/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.7.5/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.218336 geeViz-2023.7.5/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.7.5/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0     1465 2023-07-28 17:17:53.000000 geeViz-2023.7.5/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    16877 2023-07-28 17:13:30.000000 geeViz-2023.7.5/geeViz/geeView.py
--rw-rw-rw-   0        0        0   175797 2023-07-24 21:29:01.000000 geeViz-2023.7.5/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:23:00.954043 geeViz-2023.7.5/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3851 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:23:01.224322 geeViz-2023.7.5/setup.cfg
--rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.915890 geeViz-2023.8.1/
+-rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.8.1/LICENSE
+-rw-rw-rw-   0        0        0     3851 2023-08-03 19:21:09.914888 geeViz-2023.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:08.893822 geeViz-2023.8.1/geeViz/
+-rw-rw-rw-   0        0        0      121 2023-08-03 17:05:51.000000 geeViz-2023.8.1/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    24675 2023-08-03 19:18:16.000000 geeViz-2023.8.1/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.462829 geeViz-2023.8.1/geeViz/examples/
+-rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      127 2023-08-03 17:05:44.000000 geeViz-2023.8.1/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14302 2023-08-03 17:05:12.000000 geeViz-2023.8.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11478 2023-08-03 16:58:50.000000 geeViz-2023.8.1/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12128 2023-08-03 17:04:31.000000 geeViz-2023.8.1/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.525310 geeViz-2023.8.1/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.540936 geeViz-2023.8.1/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.8.1/geeViz/geeView/css/style.min.css
+-rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/foliumView.html
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.624734 geeViz-2023.8.1/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.8.1/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.911203 geeViz-2023.8.1/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.8.1/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0   450001 2023-08-03 17:05:30.000000 geeViz-2023.8.1/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    16877 2023-07-28 17:13:30.000000 geeViz-2023.8.1/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   176095 2023-08-03 16:54:44.000000 geeViz-2023.8.1/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:21:08.934713 geeViz-2023.8.1/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3851 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:21:09.916889 geeViz-2023.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.8.1/setup.py
```

### Comparing `geeViz-2023.7.5/LICENSE` & `geeViz-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/PKG-INFO` & `geeViz-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.5
+Version: 2023.8.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.5/README.md` & `geeViz-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/assetManagerLib.py` & `geeViz-2023.8.1/geeViz/assetManagerLib.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,33 +17,31 @@
 
 """
 
 #--------------------------------------------------------------------------
 #           ASSETMANAGERLIB.PY
 #--------------------------------------------------------------------------
 
+import geeViz.geeView 
 import sys, ee, os, shutil, subprocess, datetime, calendar, json,glob
 import time, logging, pdb
-try:
-    z = ee.Number(1).getInfo()
-except:
-    print('Initializing GEE')
-    ee.Initialize()
-
 taskLimit = 10
 
 #############################################################################################
 #               Functions to update ACL
 #############################################################################################
 
 #Function for updating ACL for a given GEE asset path
 def updateACL(assetName,writers = [],all_users_can_read = True,readers = []):
     print('Updating permissions for: ',assetName)
-    ee.data.setAssetAcl(assetName, json.dumps({u'writers': writers, u'all_users_can_read': all_users_can_read, u'readers': readers}))
-
+    try:
+        ee.data.setAssetAcl(assetName, json.dumps({u'writers': writers, u'all_users_can_read': all_users_can_read, u'readers': readers}))
+    except Exception as E:
+        print('Could not update permissions for: ',assetName)
+        print(E)
 #--------------------------------------------------------------------------------------------
 
 #Function for updating all assets under a given folder level in GEE
 def batchUpdateAcl(folder,writers = [],all_users_can_read = True,readers = []):
     # Update ACL for folders first, then find all images within them.
     assets = ee.data.listAssets({'parent': folder})['assets']
     folders = [a for a in assets if a['type'] == 'FOLDER']
@@ -116,48 +114,59 @@
             print( out)
             try:
                 ee.data.copyAsset(image,out)
             except:
                 print( out,'Error: May already exist')
 #---------------------------------------------------------------------------------------------
 
-def moveImages(images,toFolder):
+def moveImages(images,toFolder,delete_original = False):
     create_image_collection(toFolder)
     for image in images:
         print ('Copying',base(image))
         out = toFolder + '/' + base(image)
-        try:
-            ee.data.copyAsset(image,out)
-            #ee.data.deleteAsset(image)
-        except:
-            print (out,'already exists')
+        if not ee_asset_exists(out):
+            try:
+                ee.data.copyAsset(image,out)
+                if delete_original:
+                    ee.data.deleteAsset(image)
+            except Exception as E:
+                print('Error copying:', image)
+                print(E)
 
 #---------------------------------------------------------------------------------------------
 # types = 'imageCollection' or 'tables'
 def batchDelete(Collection, type = 'imageCollection'):
 
     if type == 'imageCollection':
         images = walkFolders(Collection)
     elif type == 'tables':
         images = walkFoldersTables(Collection) 
 
     for image in images:
         print('Deleting: '+ Collection +'/'+ base(image))
-        ee.data.deleteAsset(image)
+        try:
+            ee.data.deleteAsset(image)
+        except Exception as E:
+            print('Could not delete: ',image)
+            print(E)
 
 def deleteByName(Collection, nameIdentifier, type='imageCollection'):
     if type == 'imageCollection':
         images = walkFolders(Collection)
     elif type == 'tables':
         images = walkFoldersTables(Collection) 
 
     for image in images:
         if nameIdentifier in image:
             print('Deleting: '+ Collection +'/'+ base(image))
-            ee.data.deleteAsset(image)
+            try:
+                ee.data.deleteAsset(image)
+            except Exception as E:
+                print('Could not delete: ',image)
+                print(E)
 #############################################################################################
 #       Asset Info Queries
 #############################################################################################
 
 # Adapted from Samapriya Roy's assetsize.py (https://github.com/samapriya/Planet-GEE-Pipeline-CLI)
 suffixes = ['B', 'KB', 'MB', 'GB', 'TB', 'PB']
 def humansize(nbytes):
@@ -187,16 +196,15 @@
     elif header =="FOLDER":
         b=subprocess.check_output("earthengine du "+asset+" -s",shell=True)
         num=subprocess.check_output("earthengine ls "+asset,shell=True)
         size=humansize(float(b.strip().split(' ')[0]))
         print('')
         print(str(asset)+" ===> "+str(size))
         print('Total number of items in folder: '+str(len(num.split('\n'))-1))
-if __name__ == '__main__':
-    assetsize(None)
+
 #############################################################################################
 #       Functions to Upload to Google Cloud Storage and Google Earth Engine Repository
 #############################################################################################
 #Wrapper function to upload to google cloudStorage
 #Bucket must already exist
 def upload_to_gcs(image_dir,gs_bucket,image_extension = '.tif',copy_or_sync = 'copy'):
     if copy_or_sync == 'copy':
@@ -396,16 +404,33 @@
 
 #Adapted from: https://github.com/tracek/gee_asset_manager/blob/master/geebam/helper_functions.py
 #Author: Lukasz Tracewski
 def create_image_collection(full_path_to_collection):
     if ee_asset_exists(full_path_to_collection):
         print("Collection "+full_path_to_collection+" already exists")
     else:
-        ee.data.createAsset({'type': ee.data.ASSET_TYPE_IMAGE_COLL}, full_path_to_collection)
-        print('New collection '+full_path_to_collection+' created')
+        try:
+            ee.data.createAsset({'type': ee.data.ASSET_TYPE_IMAGE_COLL}, full_path_to_collection)
+            print('New collection '+full_path_to_collection+' created')
+        except Exception as E:
+            print('Could not create: ',full_path_to_collection)
+            print(E)
+            
+# More general function to create asset collecctions or folders
+# asset_type can be one of ee.data.ASSET_TYPE_FOLDER or ee.data.ASSET_TYPE_IMAGE_COLL
+def create_asset(asset_path,asset_type = ee.data.ASSET_TYPE_FOLDER):
+    if ee_asset_exists(asset_path):
+        print("Asset "+asset_path+" already exists")
+    else:
+        try:
+            ee.data.createAsset({'type': asset_type}, asset_path)
+            print('New asset '+asset_path+' created')
+        except Exception as E:
+            print('Could not create: ',asset_path)
+            print(E)
 
 def verify_path(path):
     response = ee.data.getInfo(path)
     if not response:
         logging.error('%s is not a valid destination. Make sure full path is provided e.g. users/user/nameofcollection '
                       'or projects/myproject/myfolder/newcollection and that you have write access there.', path)
         sys.exit(1)
```

### Comparing `geeViz-2023.7.5/geeViz/changeDetectionLib.py` & `geeViz-2023.8.1/geeViz/changeDetectionLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/CCDCViz.py` & `geeViz-2023.8.1/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.8.1/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.8.1/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.8.1/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/foliumViewerExample.py` & `geeViz-2023.8.1/geeViz/examples/foliumViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/gee2PandasExample.ipynb` & `geeViz-2023.8.1/geeViz/examples/gee2PandasExample.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/geeViewExample.py` & `geeViz-2023.8.1/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.8.1/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.8.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 startJulian = 152
 endJulian = 273
 
 # Specify start and end years for all analyses
 # More than a 3 year span should be provided for time series methods to work 
 # well. If providing pre-computed stats for cloudScore and TDOM, this does not 
 # matter
-startYear = 2018
-endYear = 2022
+startYear = 2020
+endYear = 2023
 
 # Specify an annual buffer to include imagery from the same season 
 # timeframe from the prior and following year. timeBuffer = 1 will result 
 # in a 3 year moving window. If you want single-year composites, set to 0
 timebuffer =0
 
 # Specify the weights to be used for the moving window created by timeBuffer
```

### Comparing `geeViz-2023.7.5/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.8.1/geeViz/examples/getLandsatWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 endJulian = 273
 
 # Specify start and end years for all analyses
 # More than a 3 year span should be provided for time series methods to work 
 # well. If providing pre-computed stats for cloudScore and TDOM, this does not 
 # matter
 startYear = 2015
-endYear = 2022
+endYear = 2023
 
 # Specify an annual buffer to include imagery from the same season 
 # timeframe from the prior and following year. timeBuffer = 1 will result 
 # in a 3 year moving window. If you want single-year composites, set to 0
 timebuffer =0
 
 # Specify the weights to be used for the moving window created by timeBuffer
```

### Comparing `geeViz-2023.7.5/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.8.1/geeViz/examples/getSentinel2Wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 endJulian = 273
 
 # Specify start and end years for all analyses
 # More than a 3 year span should be provided for time series methods to work 
 # well. If using Fmask as the cloud/cloud shadow masking method, or providing
 # pre-computed stats for cloudScore and TDOM, this does not 
 # matter
-startYear = 2018
-endYear = 2022
+startYear = 2020
+endYear = 2023
 
 # Specify an annual buffer to include imagery from the same season 
 # timeframe from the prior and following year. timeBuffer = 1 will result 
 # in a 3 year moving window. If you want single-year composites, set to 0
 timebuffer =0
 
 # Specify the weights to be used for the moving window created by timeBuffer
@@ -226,17 +226,15 @@
 processedScenes = s2sAndTs['processedScenes']
 processedComposites = s2sAndTs['processedComposites']
 
 # Indicate what type of image is being added to speed up map service creation
 getImagesLib.vizParamsFalse['layerType']= 'geeImage';
 
 Map.addLayer(processedComposites.select(['NDVI','NBR']),{'addToLegend':False,'layerType':'geeImageCollection'},'Time Series (NBR and NDVI)',False)
-for year in range(startYear + timebuffer      ,endYear + 1 - timebuffer ):
-     t = processedComposites.filter(ee.Filter.calendarRange(year,year,'year')).first()
-     Map.addLayer(t,getImagesLib.vizParamsFalse,str(year),False)
+Map.addTimeLapse(processedComposites,getImagesLib.vizParamsFalse,'Composite Timelapse',False)
 ####################################################################################################
 # Load the study region
 Map.addLayer(studyArea, {'strokeColor': '0000FF'}, "Study Area", True)
 Map.centerObject(studyArea)
 ####################################################################################################
 ####################################################################################################
 # View map
```

### Comparing `geeViz-2023.7.5/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.8.1/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.8.1/geeViz/examples/lcmsViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.8.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.8.1/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.8.1/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/examples/timeLapseExample.py` & `geeViz-2023.8.1/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/foliumView.py` & `geeViz-2023.8.1/geeViz/foliumView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/gcpLib.py` & `geeViz-2023.8.1/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/gee2Pandas.py` & `geeViz-2023.8.1/geeViz/gee2Pandas.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/css/style.min.css` & `geeViz-2023.8.1/geeViz/geeView/css/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/foliumView.html` & `geeViz-2023.8.1/geeViz/geeView/foliumView.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.8.1/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/GEE.png` & `geeViz-2023.8.1/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.8.1/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.8.1/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.8.1/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.8.1/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.8.1/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.8.1/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.8.1/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/index.html` & `geeViz-2023.8.1/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.8.1/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.8.1/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView/js/load.min.js` & `geeViz-2023.8.1/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/geeView.py` & `geeViz-2023.8.1/geeViz/geeView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/getImagesLib.py` & `geeViz-2023.8.1/geeViz/getImagesLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -4691,6298 +4691,6316 @@
 00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012530: 2020 2020 2020 6d61 7850 6978 656c 7320        maxPixels 
 00012540: 3d20 3165 3133 290d 0a20 2020 2070 7269  = 1e13)..    pri
 00012550: 6e74 2827 4578 706f 7274 696e 673a 272c  nt('Exporting:',
 00012560: 6173 7365 744e 616d 6529 0d0a 2020 2020  assetName)..    
 00012570: 7072 696e 7428 7429 0d0a 2020 2020 742e  print(t)..    t.
 00012580: 7374 6172 7428 290d 0a20 2065 6c73 653a  start()..  else:
-00012590: 0d0a 2020 2020 7072 696e 7428 2741 7373  ..    print('Ass
-000125a0: 6574 2063 7572 7265 6e74 6c79 2065 7869  et currently exi
-000125b0: 7374 7320 6f72 2069 7320 6265 696e 6720  sts or is being 
-000125c0: 6578 706f 7274 6564 2061 6e64 206f 7665  exported and ove
-000125d0: 7277 7269 7465 203d 2046 616c 7365 2e20  rwrite = False. 
-000125e0: 4578 706f 7274 206e 6f74 2073 7461 7274  Export not start
-000125f0: 6564 2e20 5365 7420 6f76 6572 7769 7465  ed. Set overwite
-00012600: 203d 2054 7275 6520 6966 2079 6f75 2077   = True if you w
-00012610: 6f75 6c64 206c 696b 6520 746f 206f 7665  ould like to ove
-00012620: 7277 6974 6520 616e 7920 6578 6973 7469  rwite any existi
-00012630: 6e67 2061 7373 6574 206f 7220 6173 7365  ng asset or asse
-00012640: 7420 6578 706f 7274 696e 6720 7461 736b  t exporting task
-00012650: 2729 0d0a 2020 2320 4d61 702e 6164 644c  ')..  # Map.addL
-00012660: 6179 6572 2869 6d61 6765 466f 7245 7870  ayer(imageForExp
-00012670: 6f72 742c 7669 7a50 6172 616d 7346 616c  ort,vizParamsFal
-00012680: 7365 2c61 7373 6574 4e61 6d65 290d 0a65  se,assetName)..e
-00012690: 7870 6f72 7454 6f41 7373 6574 5772 6170  xportToAssetWrap
-000126a0: 7065 7233 203d 2065 7870 6f72 7454 6f41  per3 = exportToA
-000126b0: 7373 6574 5772 6170 7065 720d 0a65 7870  ssetWrapper..exp
-000126c0: 6f72 7454 6f41 7373 6574 5772 6170 7065  ortToAssetWrappe
-000126d0: 7232 203d 2065 7870 6f72 7454 6f41 7373  r2 = exportToAss
-000126e0: 6574 5772 6170 7065 720d 0a23 2323 2323  etWrapper..#####
-000126f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012590: 0d0a 2020 2020 7072 696e 7428 6627 7b61  ..    print(f'{a
+000125a0: 7373 6574 4e61 6d65 7d20 6375 7272 656e  ssetName} curren
+000125b0: 746c 7920 6578 6973 7473 206f 7220 6973  tly exists or is
+000125c0: 2062 6569 6e67 2065 7870 6f72 7465 6420   being exported 
+000125d0: 616e 6420 6f76 6572 7772 6974 6520 3d20  and overwrite = 
+000125e0: 4661 6c73 652e 2045 7870 6f72 7420 6e6f  False. Export no
+000125f0: 7420 7374 6172 7465 642e 2053 6574 206f  t started. Set o
+00012600: 7665 7277 6974 6520 3d20 5472 7565 2069  verwite = True i
+00012610: 6620 796f 7520 776f 756c 6420 6c69 6b65  f you would like
+00012620: 2074 6f20 6f76 6572 7769 7465 2061 6e79   to overwite any
+00012630: 2065 7869 7374 696e 6720 6173 7365 7420   existing asset 
+00012640: 6f72 2061 7373 6574 2065 7870 6f72 7469  or asset exporti
+00012650: 6e67 2074 6173 6b27 290d 0a20 2023 204d  ng task')..  # M
+00012660: 6170 2e61 6464 4c61 7965 7228 696d 6167  ap.addLayer(imag
+00012670: 6546 6f72 4578 706f 7274 2c76 697a 5061  eForExport,vizPa
+00012680: 7261 6d73 4661 6c73 652c 6173 7365 744e  ramsFalse,assetN
+00012690: 616d 6529 0d0a 6578 706f 7274 546f 4173  ame)..exportToAs
+000126a0: 7365 7457 7261 7070 6572 3320 3d20 6578  setWrapper3 = ex
+000126b0: 706f 7274 546f 4173 7365 7457 7261 7070  portToAssetWrapp
+000126c0: 6572 0d0a 6578 706f 7274 546f 4173 7365  er..exportToAsse
+000126d0: 7457 7261 7070 6572 3220 3d20 6578 706f  tWrapper2 = expo
+000126e0: 7274 546f 4173 7365 7457 7261 7070 6572  rtToAssetWrapper
+000126f0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
 00012700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012730: 2323 2323 0d0a 6465 6620 6578 706f 7274  ####..def export
-00012740: 546f 4472 6976 6557 7261 7070 6572 2869  ToDriveWrapper(i
-00012750: 6d61 6765 466f 7245 7870 6f72 742c 6f75  mageForExport,ou
-00012760: 7470 7574 4e61 6d65 2c64 7269 7665 466f  tputName,driveFo
-00012770: 6c64 6572 4e61 6d65 2c72 6f69 2c73 6361  lderName,roi,sca
-00012780: 6c65 3d20 4e6f 6e65 2c63 7273 203d 204e  le= None,crs = N
-00012790: 6f6e 652c 7472 616e 7366 6f72 6d20 3d20  one,transform = 
-000127a0: 4e6f 6e65 2c6f 7574 7075 744e 6f44 6174  None,outputNoDat
-000127b0: 6120 3d20 2d33 3237 3638 293a 0d0a 2020  a = -32768):..  
-000127c0: 6f75 7470 7574 4e61 6d65 203d 206f 7574  outputName = out
-000127d0: 7075 744e 616d 652e 7265 706c 6163 6528  putName.replace(
-000127e0: 222f 5c73 2b2f 6722 2c27 2d27 2923 4765  "/\s+/g",'-')#Ge
-000127f0: 7420 7269 6420 6f66 2061 6e79 2073 7061  t rid of any spa
-00012800: 6365 730d 0a0d 0a20 2023 5075 6c6c 2067  ces....  #Pull g
-00012810: 656f 6d65 7472 7920 6966 2066 6561 7475  eometry if featu
-00012820: 7265 206f 7220 6665 6174 7572 6543 6f6c  re or featureCol
-00012830: 6c65 6374 696f 6e0d 0a20 2074 7279 3a0d  lection..  try:.
-00012840: 0a20 2020 2072 6f69 203d 2072 6f69 2e67  .    roi = roi.g
-00012850: 656f 6d65 7472 7928 290d 0a20 2065 7863  eometry()..  exc
-00012860: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00012870: 2065 3a0d 0a20 2020 2078 203d 2065 0d0a   e:..    x = e..
-00012880: 0d0a 2020 234d 616b 6520 7375 7265 2069  ..  #Make sure i
-00012890: 6d61 6765 2069 7320 636c 6970 7065 6420  mage is clipped 
-000128a0: 746f 2072 6f69 2069 6e20 6361 7365 2069  to roi in case i
-000128b0: 7427 7320 6120 6d75 6c74 692d 7061 7274  t's a multi-part
-000128c0: 2070 6f6c 7967 6f6e 0d0a 2020 696d 6167   polygon..  imag
-000128d0: 6546 6f72 4578 706f 7274 203d 2069 6d61  eForExport = ima
-000128e0: 6765 466f 7245 7870 6f72 742e 636c 6970  geForExport.clip
-000128f0: 2872 6f69 292e 756e 6d61 736b 286f 7574  (roi).unmask(out
-00012900: 7075 744e 6f44 6174 612c 4661 6c73 6529  putNoData,False)
-00012910: 0d0a 0d0a 2020 6966 2074 7261 6e73 666f  ....  if transfo
-00012920: 726d 2021 3d20 4e6f 6e65 2061 6e64 2028  rm != None and (
-00012930: 7374 7228 7479 7065 2874 7261 6e73 666f  str(type(transfo
-00012940: 726d 2929 203d 3d20 223c 7479 7065 2027  rm)) == "<type '
-00012950: 6c69 7374 273e 2220 6f72 2073 7472 2874  list'>" or str(t
-00012960: 7970 6528 7472 616e 7366 6f72 6d29 2920  ype(transform)) 
-00012970: 3d3d 2022 3c63 6c61 7373 2027 6c69 7374  == "<class 'list
-00012980: 273e 2229 3a0d 0a20 2020 2074 7261 6e73  '>"):..    trans
-00012990: 666f 726d 203d 2073 7472 2874 7261 6e73  form = str(trans
-000129a0: 666f 726d 290d 0a0d 0a0d 0a20 2023 456e  form)......  #En
-000129b0: 7375 7265 2062 6f75 6e64 7320 6172 6520  sure bounds are 
-000129c0: 696e 2065 7870 6f72 7420 7072 6f6a 6563  in export projec
-000129d0: 7469 6f6e 0d0a 2020 6f75 7452 6567 696f  tion..  outRegio
-000129e0: 6e20 3d20 726f 692e 626f 756e 6473 2831  n = roi.bounds(1
-000129f0: 3030 2c63 7273 290d 0a0d 0a20 2023 204d  00,crs)....  # M
-00012a00: 6170 2e61 6464 4c61 7965 7228 696d 6167  ap.addLayer(imag
-00012a10: 6546 6f72 4578 706f 7274 2c7b 7d2c 6f75  eForExport,{},ou
-00012a20: 7470 7574 4e61 6d65 2c46 616c 7365 290d  tputName,False).
-00012a30: 0a20 2074 203d 2065 652e 6261 7463 682e  .  t = ee.batch.
-00012a40: 4578 706f 7274 2e69 6d61 6765 2e74 6f44  Export.image.toD
-00012a50: 7269 7665 2869 6d61 6765 466f 7245 7870  rive(imageForExp
-00012a60: 6f72 742c 206f 7574 7075 744e 616d 652c  ort, outputName,
-00012a70: 2064 7269 7665 466f 6c64 6572 4e61 6d65   driveFolderName
-00012a80: 2c20 6f75 7470 7574 4e61 6d65 2c20 4e6f  , outputName, No
-00012a90: 6e65 2c20 6f75 7452 6567 696f 6e2c 2073  ne, outRegion, s
-00012aa0: 6361 6c65 2c20 6372 732c 2074 7261 6e73  cale, crs, trans
-00012ab0: 666f 726d 2c20 3165 3133 290d 0a20 2070  form, 1e13)..  p
-00012ac0: 7269 6e74 2827 4578 706f 7274 696e 673a  rint('Exporting:
-00012ad0: 272c 6f75 7470 7574 4e61 6d65 290d 0a20  ',outputName).. 
-00012ae0: 2074 2e73 7461 7274 2829 0d0a 2323 2323   t.start()..####
-00012af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012730: 2323 2323 2323 2323 2323 230d 0a64 6566  ###########..def
+00012740: 2065 7870 6f72 7454 6f44 7269 7665 5772   exportToDriveWr
+00012750: 6170 7065 7228 696d 6167 6546 6f72 4578  apper(imageForEx
+00012760: 706f 7274 2c6f 7574 7075 744e 616d 652c  port,outputName,
+00012770: 6472 6976 6546 6f6c 6465 724e 616d 652c  driveFolderName,
+00012780: 726f 692c 7363 616c 653d 204e 6f6e 652c  roi,scale= None,
+00012790: 6372 7320 3d20 4e6f 6e65 2c74 7261 6e73  crs = None,trans
+000127a0: 666f 726d 203d 204e 6f6e 652c 6f75 7470  form = None,outp
+000127b0: 7574 4e6f 4461 7461 203d 202d 3332 3736  utNoData = -3276
+000127c0: 3829 3a0d 0a20 206f 7574 7075 744e 616d  8):..  outputNam
+000127d0: 6520 3d20 6f75 7470 7574 4e61 6d65 2e72  e = outputName.r
+000127e0: 6570 6c61 6365 2822 2f5c 732b 2f67 222c  eplace("/\s+/g",
+000127f0: 272d 2729 2347 6574 2072 6964 206f 6620  '-')#Get rid of 
+00012800: 616e 7920 7370 6163 6573 0d0a 0d0a 2020  any spaces....  
+00012810: 2350 756c 6c20 6765 6f6d 6574 7279 2069  #Pull geometry i
+00012820: 6620 6665 6174 7572 6520 6f72 2066 6561  f feature or fea
+00012830: 7475 7265 436f 6c6c 6563 7469 6f6e 0d0a  tureCollection..
+00012840: 2020 7472 793a 0d0a 2020 2020 726f 6920    try:..    roi 
+00012850: 3d20 726f 692e 6765 6f6d 6574 7279 2829  = roi.geometry()
+00012860: 0d0a 2020 6578 6365 7074 2045 7863 6570  ..  except Excep
+00012870: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+00012880: 7820 3d20 650d 0a0d 0a20 2023 4d61 6b65  x = e....  #Make
+00012890: 2073 7572 6520 696d 6167 6520 6973 2063   sure image is c
+000128a0: 6c69 7070 6564 2074 6f20 726f 6920 696e  lipped to roi in
+000128b0: 2063 6173 6520 6974 2773 2061 206d 756c   case it's a mul
+000128c0: 7469 2d70 6172 7420 706f 6c79 676f 6e0d  ti-part polygon.
+000128d0: 0a20 2069 6d61 6765 466f 7245 7870 6f72  .  imageForExpor
+000128e0: 7420 3d20 696d 6167 6546 6f72 4578 706f  t = imageForExpo
+000128f0: 7274 2e63 6c69 7028 726f 6929 2e75 6e6d  rt.clip(roi).unm
+00012900: 6173 6b28 6f75 7470 7574 4e6f 4461 7461  ask(outputNoData
+00012910: 2c46 616c 7365 290d 0a0d 0a20 2069 6620  ,False)....  if 
+00012920: 7472 616e 7366 6f72 6d20 213d 204e 6f6e  transform != Non
+00012930: 6520 616e 6420 2873 7472 2874 7970 6528  e and (str(type(
+00012940: 7472 616e 7366 6f72 6d29 2920 3d3d 2022  transform)) == "
+00012950: 3c74 7970 6520 276c 6973 7427 3e22 206f  <type 'list'>" o
+00012960: 7220 7374 7228 7479 7065 2874 7261 6e73  r str(type(trans
+00012970: 666f 726d 2929 203d 3d20 223c 636c 6173  form)) == "<clas
+00012980: 7320 276c 6973 7427 3e22 293a 0d0a 2020  s 'list'>"):..  
+00012990: 2020 7472 616e 7366 6f72 6d20 3d20 7374    transform = st
+000129a0: 7228 7472 616e 7366 6f72 6d29 0d0a 0d0a  r(transform)....
+000129b0: 0d0a 2020 2345 6e73 7572 6520 626f 756e  ..  #Ensure boun
+000129c0: 6473 2061 7265 2069 6e20 6578 706f 7274  ds are in export
+000129d0: 2070 726f 6a65 6374 696f 6e0d 0a20 206f   projection..  o
+000129e0: 7574 5265 6769 6f6e 203d 2072 6f69 2e62  utRegion = roi.b
+000129f0: 6f75 6e64 7328 3130 302c 6372 7329 0d0a  ounds(100,crs)..
+00012a00: 0d0a 2020 2320 4d61 702e 6164 644c 6179  ..  # Map.addLay
+00012a10: 6572 2869 6d61 6765 466f 7245 7870 6f72  er(imageForExpor
+00012a20: 742c 7b7d 2c6f 7574 7075 744e 616d 652c  t,{},outputName,
+00012a30: 4661 6c73 6529 0d0a 2020 7420 3d20 6565  False)..  t = ee
+00012a40: 2e62 6174 6368 2e45 7870 6f72 742e 696d  .batch.Export.im
+00012a50: 6167 652e 746f 4472 6976 6528 696d 6167  age.toDrive(imag
+00012a60: 6546 6f72 4578 706f 7274 2c20 6f75 7470  eForExport, outp
+00012a70: 7574 4e61 6d65 2c20 6472 6976 6546 6f6c  utName, driveFol
+00012a80: 6465 724e 616d 652c 206f 7574 7075 744e  derName, outputN
+00012a90: 616d 652c 204e 6f6e 652c 206f 7574 5265  ame, None, outRe
+00012aa0: 6769 6f6e 2c20 7363 616c 652c 2063 7273  gion, scale, crs
+00012ab0: 2c20 7472 616e 7366 6f72 6d2c 2031 6531  , transform, 1e1
+00012ac0: 3329 0d0a 2020 7072 696e 7428 2745 7870  3)..  print('Exp
+00012ad0: 6f72 7469 6e67 3a27 2c6f 7574 7075 744e  orting:',outputN
+00012ae0: 616d 6529 0d0a 2020 742e 7374 6172 7428  ame)..  t.start(
+00012af0: 290d 0a23 2323 2323 2323 2323 2323 2323  )..#############
 00012b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012b30: 2323 2323 230d 0a64 6566 2065 7870 6f72  #####..def expor
-00012b40: 7454 6f43 6c6f 7564 5374 6f72 6167 6557  tToCloudStorageW
-00012b50: 7261 7070 6572 2869 6d61 6765 466f 7245  rapper(imageForE
-00012b60: 7870 6f72 742c 6f75 7470 7574 4e61 6d65  xport,outputName
-00012b70: 2c62 7563 6b65 744e 616d 652c 726f 692c  ,bucketName,roi,
-00012b80: 7363 616c 653d 204e 6f6e 652c 6372 7320  scale= None,crs 
-00012b90: 3d20 4e6f 6e65 2c74 7261 6e73 666f 726d  = None,transform
-00012ba0: 203d 204e 6f6e 652c 6f75 7470 7574 4e6f   = None,outputNo
-00012bb0: 4461 7461 203d 202d 3332 3736 3829 3a0d  Data = -32768):.
-00012bc0: 0a20 206f 7574 7075 744e 616d 6520 3d20  .  outputName = 
-00012bd0: 6f75 7470 7574 4e61 6d65 2e72 6570 6c61  outputName.repla
-00012be0: 6365 2822 2f5c 732b 2f67 222c 272d 2729  ce("/\s+/g",'-')
-00012bf0: 2347 6574 2072 6964 206f 6620 616e 7920  #Get rid of any 
-00012c00: 7370 6163 6573 0d0a 0d0a 2020 2350 756c  spaces....  #Pul
-00012c10: 6c20 6765 6f6d 6574 7279 2069 6620 6665  l geometry if fe
-00012c20: 6174 7572 6520 6f72 2066 6561 7475 7265  ature or feature
-00012c30: 436f 6c6c 6563 7469 6f6e 0d0a 2020 7472  Collection..  tr
-00012c40: 793a 0d0a 2020 2020 726f 6920 3d20 726f  y:..    roi = ro
-00012c50: 692e 6765 6f6d 6574 7279 2829 0d0a 2020  i.geometry()..  
-00012c60: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00012c70: 2061 7320 653a 0d0a 2020 2020 7820 3d20   as e:..    x = 
-00012c80: 650d 0a0d 0a20 2023 4d61 6b65 2073 7572  e....  #Make sur
-00012c90: 6520 696d 6167 6520 6973 2063 6c69 7070  e image is clipp
-00012ca0: 6564 2074 6f20 726f 6920 696e 2063 6173  ed to roi in cas
-00012cb0: 6520 6974 2773 2061 206d 756c 7469 2d70  e it's a multi-p
-00012cc0: 6172 7420 706f 6c79 676f 6e0d 0a20 2069  art polygon..  i
-00012cd0: 6d61 6765 466f 7245 7870 6f72 7420 3d20  mageForExport = 
-00012ce0: 696d 6167 6546 6f72 4578 706f 7274 2e63  imageForExport.c
-00012cf0: 6c69 7028 726f 6929 2e75 6e6d 6173 6b28  lip(roi).unmask(
-00012d00: 6f75 7470 7574 4e6f 4461 7461 2c46 616c  outputNoData,Fal
-00012d10: 7365 290d 0a0d 0a20 2069 6620 7472 616e  se)....  if tran
-00012d20: 7366 6f72 6d20 213d 204e 6f6e 6520 616e  sform != None an
-00012d30: 6420 2873 7472 2874 7970 6528 7472 616e  d (str(type(tran
-00012d40: 7366 6f72 6d29 2920 3d3d 2022 3c74 7970  sform)) == "<typ
-00012d50: 6520 276c 6973 7427 3e22 206f 7220 7374  e 'list'>" or st
-00012d60: 7228 7479 7065 2874 7261 6e73 666f 726d  r(type(transform
-00012d70: 2929 203d 3d20 223c 636c 6173 7320 276c  )) == "<class 'l
-00012d80: 6973 7427 3e22 293a 0d0a 2020 2020 7472  ist'>"):..    tr
-00012d90: 616e 7366 6f72 6d20 3d20 7374 7228 7472  ansform = str(tr
-00012da0: 616e 7366 6f72 6d29 0d0a 0d0a 0d0a 2020  ansform)......  
-00012db0: 2345 6e73 7572 6520 626f 756e 6473 2061  #Ensure bounds a
-00012dc0: 7265 2069 6e20 6578 706f 7274 2070 726f  re in export pro
-00012dd0: 6a65 6374 696f 6e0d 0a20 206f 7574 5265  jection..  outRe
-00012de0: 6769 6f6e 203d 2072 6f69 2e62 6f75 6e64  gion = roi.bound
-00012df0: 7328 3130 302c 6372 7329 0d0a 0d0a 2020  s(100,crs)....  
-00012e00: 7420 3d20 6565 2e62 6174 6368 2e45 7870  t = ee.batch.Exp
-00012e10: 6f72 742e 696d 6167 652e 746f 436c 6f75  ort.image.toClou
-00012e20: 6453 746f 7261 6765 2869 6d61 6765 466f  dStorage(imageFo
-00012e30: 7245 7870 6f72 742c 206f 7574 7075 744e  rExport, outputN
-00012e40: 616d 652c 2062 7563 6b65 744e 616d 652c  ame, bucketName,
-00012e50: 206f 7574 7075 744e 616d 652c 204e 6f6e   outputName, Non
-00012e60: 652c 206f 7574 5265 6769 6f6e 2c20 7363  e, outRegion, sc
-00012e70: 616c 652c 2063 7273 2c20 7472 616e 7366  ale, crs, transf
-00012e80: 6f72 6d2c 2031 6531 3329 0d0a 2020 7072  orm, 1e13)..  pr
-00012e90: 696e 7428 2745 7870 6f72 7469 6e67 3a27  int('Exporting:'
-00012ea0: 2c6f 7574 7075 744e 616d 6529 0d0a 2020  ,outputName)..  
-00012eb0: 7072 696e 7428 7429 0d0a 2020 742e 7374  print(t)..  t.st
-00012ec0: 6172 7428 290d 0a0d 0a0d 0a23 2323 2323  art()......#####
-00012ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012b30: 2323 2323 2323 2323 2323 2323 0d0a 6465  ############..de
+00012b40: 6620 6578 706f 7274 546f 436c 6f75 6453  f exportToCloudS
+00012b50: 746f 7261 6765 5772 6170 7065 7228 696d  torageWrapper(im
+00012b60: 6167 6546 6f72 4578 706f 7274 2c6f 7574  ageForExport,out
+00012b70: 7075 744e 616d 652c 6275 636b 6574 4e61  putName,bucketNa
+00012b80: 6d65 2c72 6f69 2c73 6361 6c65 3d20 4e6f  me,roi,scale= No
+00012b90: 6e65 2c63 7273 203d 204e 6f6e 652c 7472  ne,crs = None,tr
+00012ba0: 616e 7366 6f72 6d20 3d20 4e6f 6e65 2c6f  ansform = None,o
+00012bb0: 7574 7075 744e 6f44 6174 6120 3d20 2d33  utputNoData = -3
+00012bc0: 3237 3638 293a 0d0a 2020 6f75 7470 7574  2768):..  output
+00012bd0: 4e61 6d65 203d 206f 7574 7075 744e 616d  Name = outputNam
+00012be0: 652e 7265 706c 6163 6528 222f 5c73 2b2f  e.replace("/\s+/
+00012bf0: 6722 2c27 2d27 2923 4765 7420 7269 6420  g",'-')#Get rid 
+00012c00: 6f66 2061 6e79 2073 7061 6365 730d 0a0d  of any spaces...
+00012c10: 0a20 2023 5075 6c6c 2067 656f 6d65 7472  .  #Pull geometr
+00012c20: 7920 6966 2066 6561 7475 7265 206f 7220  y if feature or 
+00012c30: 6665 6174 7572 6543 6f6c 6c65 6374 696f  featureCollectio
+00012c40: 6e0d 0a20 2074 7279 3a0d 0a20 2020 2072  n..  try:..    r
+00012c50: 6f69 203d 2072 6f69 2e67 656f 6d65 7472  oi = roi.geometr
+00012c60: 7928 290d 0a20 2065 7863 6570 7420 4578  y()..  except Ex
+00012c70: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00012c80: 2020 2078 203d 2065 0d0a 0d0a 2020 234d     x = e....  #M
+00012c90: 616b 6520 7375 7265 2069 6d61 6765 2069  ake sure image i
+00012ca0: 7320 636c 6970 7065 6420 746f 2072 6f69  s clipped to roi
+00012cb0: 2069 6e20 6361 7365 2069 7427 7320 6120   in case it's a 
+00012cc0: 6d75 6c74 692d 7061 7274 2070 6f6c 7967  multi-part polyg
+00012cd0: 6f6e 0d0a 2020 696d 6167 6546 6f72 4578  on..  imageForEx
+00012ce0: 706f 7274 203d 2069 6d61 6765 466f 7245  port = imageForE
+00012cf0: 7870 6f72 742e 636c 6970 2872 6f69 292e  xport.clip(roi).
+00012d00: 756e 6d61 736b 286f 7574 7075 744e 6f44  unmask(outputNoD
+00012d10: 6174 612c 4661 6c73 6529 0d0a 0d0a 2020  ata,False)....  
+00012d20: 6966 2074 7261 6e73 666f 726d 2021 3d20  if transform != 
+00012d30: 4e6f 6e65 2061 6e64 2028 7374 7228 7479  None and (str(ty
+00012d40: 7065 2874 7261 6e73 666f 726d 2929 203d  pe(transform)) =
+00012d50: 3d20 223c 7479 7065 2027 6c69 7374 273e  = "<type 'list'>
+00012d60: 2220 6f72 2073 7472 2874 7970 6528 7472  " or str(type(tr
+00012d70: 616e 7366 6f72 6d29 2920 3d3d 2022 3c63  ansform)) == "<c
+00012d80: 6c61 7373 2027 6c69 7374 273e 2229 3a0d  lass 'list'>"):.
+00012d90: 0a20 2020 2074 7261 6e73 666f 726d 203d  .    transform =
+00012da0: 2073 7472 2874 7261 6e73 666f 726d 290d   str(transform).
+00012db0: 0a0d 0a0d 0a20 2023 456e 7375 7265 2062  .....  #Ensure b
+00012dc0: 6f75 6e64 7320 6172 6520 696e 2065 7870  ounds are in exp
+00012dd0: 6f72 7420 7072 6f6a 6563 7469 6f6e 0d0a  ort projection..
+00012de0: 2020 6f75 7452 6567 696f 6e20 3d20 726f    outRegion = ro
+00012df0: 692e 626f 756e 6473 2831 3030 2c63 7273  i.bounds(100,crs
+00012e00: 290d 0a0d 0a20 2074 203d 2065 652e 6261  )....  t = ee.ba
+00012e10: 7463 682e 4578 706f 7274 2e69 6d61 6765  tch.Export.image
+00012e20: 2e74 6f43 6c6f 7564 5374 6f72 6167 6528  .toCloudStorage(
+00012e30: 696d 6167 6546 6f72 4578 706f 7274 2c20  imageForExport, 
+00012e40: 6f75 7470 7574 4e61 6d65 2c20 6275 636b  outputName, buck
+00012e50: 6574 4e61 6d65 2c20 6f75 7470 7574 4e61  etName, outputNa
+00012e60: 6d65 2c20 4e6f 6e65 2c20 6f75 7452 6567  me, None, outReg
+00012e70: 696f 6e2c 2073 6361 6c65 2c20 6372 732c  ion, scale, crs,
+00012e80: 2074 7261 6e73 666f 726d 2c20 3165 3133   transform, 1e13
+00012e90: 290d 0a20 2070 7269 6e74 2827 4578 706f  )..  print('Expo
+00012ea0: 7274 696e 673a 272c 6f75 7470 7574 4e61  rting:',outputNa
+00012eb0: 6d65 290d 0a20 2070 7269 6e74 2874 290d  me)..  print(t).
+00012ec0: 0a20 2074 2e73 7461 7274 2829 0d0a 0d0a  .  t.start()....
+00012ed0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
 00012ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012f10: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
+00012f10: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
 00012f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00012f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012f50: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00012f60: 0a23 4675 6e63 7469 6f6e 2066 6f72 2077  .#Function for w
-00012f70: 7261 7070 696e 6720 6461 7465 7320 7768  rapping dates wh
-00012f80: 656e 2074 6865 2073 7461 7274 4a75 6c69  en the startJuli
-00012f90: 616e 203c 2065 6e64 4a75 6c69 616e 0d0a  an < endJulian..
-00012fa0: 2343 6865 636b 7320 666f 7220 7965 6172  #Checks for year
-00012fb0: 2077 6974 6820 6d61 6a6f 7269 7479 206f   with majority o
-00012fc0: 6620 7468 6520 6461 7973 2061 6e64 2074  f the days and t
-00012fd0: 6865 2077 7261 704f 6666 7365 740d 0a64  he wrapOffset..d
-00012fe0: 6566 2077 7261 7044 6174 6573 2873 7461  ef wrapDates(sta
-00012ff0: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
-00013000: 616e 293a 0d0a 2020 2353 6574 2075 7020  an):..  #Set up 
-00013010: 6461 7465 2077 7261 7070 696e 670d 0a20  date wrapping.. 
-00013020: 2077 7261 704f 6666 7365 7420 3d20 300d   wrapOffset = 0.
-00013030: 0a20 2079 6561 7257 6974 684d 616a 6f72  .  yearWithMajor
-00013040: 6974 7920 3d20 300d 0a20 2069 6620 7374  ity = 0..  if st
-00013050: 6172 744a 756c 6961 6e20 3e20 656e 644a  artJulian > endJ
-00013060: 756c 6961 6e3a 0d0a 2020 2020 7772 6170  ulian:..    wrap
-00013070: 4f66 6673 6574 203d 2033 3635 0d0a 2020  Offset = 365..  
-00013080: 2020 7931 4e44 6179 7320 3d20 3336 352d    y1NDays = 365-
-00013090: 7374 6172 744a 756c 6961 6e0d 0a20 2020  startJulian..   
-000130a0: 2079 324e 4461 7973 203d 2065 6e64 4a75   y2NDays = endJu
-000130b0: 6c69 616e 0d0a 2020 2020 6966 2079 324e  lian..    if y2N
-000130c0: 4461 7973 203e 2079 314e 4461 7973 3a0d  Days > y1NDays:.
-000130d0: 0a20 2020 2020 2079 6561 7257 6974 684d  .      yearWithM
-000130e0: 616a 6f72 6974 7920 3d20 310d 0a0d 0a20  ajority = 1.... 
-000130f0: 2072 6574 7572 6e20 5b77 7261 704f 6666   return [wrapOff
-00013100: 7365 742c 7965 6172 5769 7468 4d61 6a6f  set,yearWithMajo
-00013110: 7269 7479 5d0d 0a0d 0a23 2323 2323 2323  rity]....#######
+00012f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012f60: 2323 2323 2323 0d0a 2346 756e 6374 696f  ######..#Functio
+00012f70: 6e20 666f 7220 7772 6170 7069 6e67 2064  n for wrapping d
+00012f80: 6174 6573 2077 6865 6e20 7468 6520 7374  ates when the st
+00012f90: 6172 744a 756c 6961 6e20 3c20 656e 644a  artJulian < endJ
+00012fa0: 756c 6961 6e0d 0a23 4368 6563 6b73 2066  ulian..#Checks f
+00012fb0: 6f72 2079 6561 7220 7769 7468 206d 616a  or year with maj
+00012fc0: 6f72 6974 7920 6f66 2074 6865 2064 6179  ority of the day
+00012fd0: 7320 616e 6420 7468 6520 7772 6170 4f66  s and the wrapOf
+00012fe0: 6673 6574 0d0a 6465 6620 7772 6170 4461  fset..def wrapDa
+00012ff0: 7465 7328 7374 6172 744a 756c 6961 6e2c  tes(startJulian,
+00013000: 656e 644a 756c 6961 6e29 3a0d 0a20 2023  endJulian):..  #
+00013010: 5365 7420 7570 2064 6174 6520 7772 6170  Set up date wrap
+00013020: 7069 6e67 0d0a 2020 7772 6170 4f66 6673  ping..  wrapOffs
+00013030: 6574 203d 2030 0d0a 2020 7965 6172 5769  et = 0..  yearWi
+00013040: 7468 4d61 6a6f 7269 7479 203d 2030 0d0a  thMajority = 0..
+00013050: 2020 6966 2073 7461 7274 4a75 6c69 616e    if startJulian
+00013060: 203e 2065 6e64 4a75 6c69 616e 3a0d 0a20   > endJulian:.. 
+00013070: 2020 2077 7261 704f 6666 7365 7420 3d20     wrapOffset = 
+00013080: 3336 350d 0a20 2020 2079 314e 4461 7973  365..    y1NDays
+00013090: 203d 2033 3635 2d73 7461 7274 4a75 6c69   = 365-startJuli
+000130a0: 616e 0d0a 2020 2020 7932 4e44 6179 7320  an..    y2NDays 
+000130b0: 3d20 656e 644a 756c 6961 6e0d 0a20 2020  = endJulian..   
+000130c0: 2069 6620 7932 4e44 6179 7320 3e20 7931   if y2NDays > y1
+000130d0: 4e44 6179 733a 0d0a 2020 2020 2020 7965  NDays:..      ye
+000130e0: 6172 5769 7468 4d61 6a6f 7269 7479 203d  arWithMajority =
+000130f0: 2031 0d0a 0d0a 2020 7265 7475 726e 205b   1....  return [
+00013100: 7772 6170 4f66 6673 6574 2c79 6561 7257  wrapOffset,yearW
+00013110: 6974 684d 616a 6f72 6974 795d 0d0a 0d0a  ithMajority]....
 00013120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013160: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+00013160: 2323 2323 2323 2323 230d 0a23 2323 2323  #########..#####
 00013170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000131a0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-000131b0: 4372 6561 7465 2063 6f6d 706f 7369 7465  Create composite
-000131c0: 7320 666f 7220 6561 6368 2079 6561 7220  s for each year 
-000131d0: 7769 7468 696e 2073 7461 7274 5965 6172  within startYear
-000131e0: 2061 6e64 2065 6e64 5965 6172 2072 616e   and endYear ran
-000131f0: 6765 0d0a 6465 6620 636f 6d70 6f73 6974  ge..def composit
-00013200: 6554 696d 6553 6572 6965 7328 0d0a 2020  eTimeSeries(..  
-00013210: 2020 2020 6c73 2c0d 0a20 2020 2020 2073      ls,..      s
-00013220: 7461 7274 5965 6172 2c0d 0a20 2020 2020  tartYear,..     
-00013230: 2065 6e64 5965 6172 2c0d 0a20 2020 2020   endYear,..     
-00013240: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
-00013250: 2020 2020 2065 6e64 4a75 6c69 616e 2c0d       endJulian,.
-00013260: 0a20 2020 2020 2074 696d 6562 7566 6665  .      timebuffe
-00013270: 7220 3d20 302c 0d0a 2020 2020 2020 7765  r = 0,..      we
-00013280: 6967 6874 7320 3d20 5b31 5d2c 0d0a 2020  ights = [1],..  
-00013290: 2020 2020 636f 6d70 6f73 6974 696e 674d      compositingM
-000132a0: 6574 686f 6420 3d20 4e6f 6e65 2c0d 0a20  ethod = None,.. 
-000132b0: 2020 2020 2063 6f6d 706f 7369 7469 6e67       compositing
-000132c0: 5265 6475 6365 7220 3d20 4e6f 6e65 293a  Reducer = None):
-000132d0: 0d0a 0d0a 2020 6172 6773 203d 2066 6f72  ....  args = for
-000132e0: 6d61 7441 7267 7328 6c6f 6361 6c73 2829  matArgs(locals()
-000132f0: 290d 0a20 2069 6620 2761 7267 7327 2069  )..  if 'args' i
-00013300: 6e20 6172 6773 2e6b 6579 7328 293a 0d0a  n args.keys():..
-00013310: 2020 2020 6465 6c20 6172 6773 5b27 6172      del args['ar
-00013320: 6773 275d 0d0a 0d0a 2020 6475 6d6d 7949  gs']....  dummyI
-00013330: 6d61 6765 203d 2065 652e 496d 6167 6528  mage = ee.Image(
-00013340: 6c73 2e66 6972 7374 2829 290d 0a0d 0a20  ls.first()).... 
-00013350: 2064 6174 6557 7261 7070 696e 6720 3d20   dateWrapping = 
-00013360: 7772 6170 4461 7465 7328 7374 6172 744a  wrapDates(startJ
-00013370: 756c 6961 6e2c 656e 644a 756c 6961 6e29  ulian,endJulian)
-00013380: 0d0a 2020 7772 6170 4f66 6673 6574 203d  ..  wrapOffset =
-00013390: 2064 6174 6557 7261 7070 696e 675b 305d   dateWrapping[0]
-000133a0: 0d0a 2020 7965 6172 5769 7468 4d61 6a6f  ..  yearWithMajo
-000133b0: 7269 7479 203d 2064 6174 6557 7261 7070  rity = dateWrapp
-000133c0: 696e 675b 315d 0d0a 0d0a 0d0a 0d0a 2020  ing[1]........  
-000133d0: 6465 6620 7965 6172 436f 6d70 6f73 6974  def yearComposit
-000133e0: 6547 6574 7465 7228 7965 6172 293a 0d0a  eGetter(year):..
-000133f0: 0d0a 2020 2020 2353 6574 2075 7020 6461  ..    #Set up da
-00013400: 7465 730d 0a20 2020 2073 7461 7274 5965  tes..    startYe
-00013410: 6172 5420 3d20 7965 6172 2d74 696d 6562  arT = year-timeb
-00013420: 7566 6665 720d 0a20 2020 2065 6e64 5965  uffer..    endYe
-00013430: 6172 5420 3d20 7965 6172 2b74 696d 6562  arT = year+timeb
-00013440: 7566 6665 720d 0a20 2020 2073 7461 7274  uffer..    start
-00013450: 4461 7465 5420 3d20 6565 2e44 6174 652e  DateT = ee.Date.
-00013460: 6672 6f6d 594d 4428 7374 6172 7459 6561  fromYMD(startYea
-00013470: 7254 2c31 2c31 292e 6164 7661 6e63 6528  rT,1,1).advance(
-00013480: 7374 6172 744a 756c 6961 6e2d 312c 2764  startJulian-1,'d
-00013490: 6179 2729 0d0a 2020 2020 656e 6444 6174  ay')..    endDat
-000134a0: 6554 203d 2065 652e 4461 7465 2e66 726f  eT = ee.Date.fro
-000134b0: 6d59 4d44 2865 6e64 5965 6172 542c 312c  mYMD(endYearT,1,
-000134c0: 3129 2e61 6476 616e 6365 2865 6e64 4a75  1).advance(endJu
-000134d0: 6c69 616e 2d31 2b77 7261 704f 6666 7365  lian-1+wrapOffse
-000134e0: 742c 2764 6179 2729 0d0a 0d0a 0d0a 2020  t,'day')......  
-000134f0: 2020 2370 7269 6e74 2879 6561 722c 7374    #print(year,st
-00013500: 6172 7444 6174 6554 2c65 6e64 4461 7465  artDateT,endDate
-00013510: 5429 0d0a 0d0a 2020 2020 2353 6574 2075  T)....    #Set u
-00013520: 7020 7765 6967 6874 6564 206d 6f76 696e  p weighted movin
-00013530: 6720 7769 646f 770d 0a20 2020 2079 6561  g widow..    yea
-00013540: 7273 5420 3d20 6565 2e4c 6973 742e 7365  rsT = ee.List.se
-00013550: 7175 656e 6365 2873 7461 7274 5965 6172  quence(startYear
-00013560: 542c 656e 6459 6561 7254 290d 0a0d 0a20  T,endYearT).... 
-00013570: 2020 2064 6566 207a 6970 7065 7228 6929     def zipper(i)
-00013580: 3a0d 0a20 2020 2020 2069 203d 2065 652e  :..      i = ee.
-00013590: 4c69 7374 2869 290d 0a20 2020 2020 2072  List(i)..      r
-000135a0: 6574 7572 6e20 6565 2e4c 6973 742e 7265  eturn ee.List.re
-000135b0: 7065 6174 2869 2e67 6574 2830 292c 692e  peat(i.get(0),i.
-000135c0: 6765 7428 3129 290d 0a0d 0a20 2020 207a  get(1))....    z
-000135d0: 203d 2079 6561 7273 542e 7a69 7028 7765   = yearsT.zip(we
-000135e0: 6967 6874 7329 0d0a 0d0a 2020 2020 7965  ights)....    ye
-000135f0: 6172 7354 5420 3d20 7a2e 6d61 7028 7a69  arsTT = z.map(zi
-00013600: 7070 6572 292e 666c 6174 7465 6e28 290d  pper).flatten().
-00013610: 0a0d 0a20 2020 2023 2070 7269 6e74 2827  ...    # print('
-00013620: 5765 6967 6874 6564 2063 6f6d 706f 7369  Weighted composi
-00013630: 7465 2079 6561 7273 2066 6f72 2079 6561  te years for yea
-00013640: 723a 272c 7965 6172 2c79 6561 7273 5454  r:',year,yearsTT
-00013650: 2e67 6574 496e 666f 2829 290d 0a0d 0a20  .getInfo()).... 
-00013660: 2020 2023 4974 6572 6174 6520 6163 726f     #Iterate acro
-00013670: 7373 2065 6163 6820 7965 6172 2069 6e20  ss each year in 
-00013680: 6c69 7374 0d0a 2020 2020 6465 6620 7972  list..    def yr
-00013690: 4765 7474 6572 2879 7229 3a0d 0a20 2020  Getter(yr):..   
-000136a0: 2020 2023 5365 7420 7570 2064 6174 6573     #Set up dates
-000136b0: 0d0a 2020 2020 2020 7374 6172 7444 6174  ..      startDat
-000136c0: 6554 203d 2065 652e 4461 7465 2e66 726f  eT = ee.Date.fro
-000136d0: 6d59 4d44 2879 722c 312c 3129 2e61 6476  mYMD(yr,1,1).adv
-000136e0: 616e 6365 2873 7461 7274 4a75 6c69 616e  ance(startJulian
-000136f0: 2d31 2c27 6461 7927 290d 0a20 2020 2020  -1,'day')..     
-00013700: 2065 6e64 4461 7465 5420 3d20 6565 2e44   endDateT = ee.D
-00013710: 6174 652e 6672 6f6d 594d 4428 7972 2c31  ate.fromYMD(yr,1
-00013720: 2c31 292e 6164 7661 6e63 6528 656e 644a  ,1).advance(endJ
-00013730: 756c 6961 6e2d 312b 7772 6170 4f66 6673  ulian-1+wrapOffs
-00013740: 6574 2c27 6461 7927 290d 0a0d 0a20 2020  et,'day')....   
-00013750: 2020 2023 4669 6c74 6572 2069 6d61 6765     #Filter image
-00013760: 7320 666f 7220 6769 7665 6e20 6461 7465  s for given date
-00013770: 2072 616e 6765 0d0a 2020 2020 2020 6c73   range..      ls
-00013780: 5420 3d20 6c73 2e66 696c 7465 7244 6174  T = ls.filterDat
-00013790: 6528 7374 6172 7444 6174 6554 2c65 6e64  e(startDateT,end
-000137a0: 4461 7465 542e 6164 7661 6e63 6528 312c  DateT.advance(1,
-000137b0: 2764 6179 2729 290d 0a20 2020 2020 206c  'day'))..      l
-000137c0: 7354 203d 2066 696c 6c45 6d70 7479 436f  sT = fillEmptyCo
-000137d0: 6c6c 6563 7469 6f6e 7328 6c73 542c 6475  llections(lsT,du
-000137e0: 6d6d 7949 6d61 6765 290d 0a20 2020 2020  mmyImage)..     
-000137f0: 2072 6574 7572 6e20 6c73 540d 0a20 2020   return lsT..   
-00013800: 2069 6d61 6765 7320 3d20 7965 6172 7354   images = yearsT
-00013810: 542e 6d61 7028 7972 4765 7474 6572 290d  T.map(yrGetter).
-00013820: 0a20 2020 206c 7354 203d 2065 652e 496d  .    lsT = ee.Im
-00013830: 6167 6543 6f6c 6c65 6374 696f 6e28 6565  ageCollection(ee
-00013840: 2e46 6561 7475 7265 436f 6c6c 6563 7469  .FeatureCollecti
-00013850: 6f6e 2869 6d61 6765 7329 2e66 6c61 7474  on(images).flatt
-00013860: 656e 2829 290d 0a0d 0a20 2020 2063 6f75  en())....    cou
-00013870: 6e74 203d 206c 7354 2e73 656c 6563 7428  nt = lsT.select(
-00013880: 5b30 5d29 2e63 6f75 6e74 2829 2e72 656e  [0]).count().ren
-00013890: 616d 6528 5b27 636f 6d70 6f73 6974 654f  ame(['compositeO
-000138a0: 6273 436f 756e 7427 5d29 0d0a 2020 2020  bsCount'])..    
-000138b0: 2343 6f6d 7075 7465 206d 6564 6961 6e20  #Compute median 
-000138c0: 6f72 206d 6564 6f69 6420 6f72 2061 7070  or medoid or app
-000138d0: 6c79 2072 6564 7563 6572 0d0a 2020 2020  ly reducer..    
-000138e0: 6966 2063 6f6d 706f 7369 7469 6e67 5265  if compositingRe
-000138f0: 6475 6365 7220 213d 204e 6f6e 653a 0d0a  ducer != None:..
-00013900: 2020 2020 2020 636f 6d70 6f73 6974 6520        composite 
-00013910: 3d20 6c73 542e 7265 6475 6365 2863 6f6d  = lsT.reduce(com
-00013920: 706f 7369 7469 6e67 5265 6475 6365 7229  positingReducer)
-00013930: 0d0a 2020 2020 656c 6966 2063 6f6d 706f  ..    elif compo
-00013940: 7369 7469 6e67 4d65 7468 6f64 2e6c 6f77  sitingMethod.low
-00013950: 6572 2829 203d 3d20 276d 6564 6961 6e27  er() == 'median'
-00013960: 3a0d 0a20 2020 2020 2063 6f6d 706f 7369  :..      composi
-00013970: 7465 203d 206c 7354 2e6d 6564 6961 6e28  te = lsT.median(
-00013980: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
-00013990: 2020 2020 636f 6d70 6f73 6974 6520 3d20      composite = 
-000139a0: 6d65 646f 6964 4d6f 7361 6963 4d53 4428  medoidMosaicMSD(
-000139b0: 6c73 542c 5b27 6772 6565 6e27 2c27 7265  lsT,['green','re
-000139c0: 6427 2c27 6e69 7227 2c27 7377 6972 3127  d','nir','swir1'
-000139d0: 2c27 7377 6972 3227 5d29 0d0a 2020 2020  ,'swir2'])..    
-000139e0: 636f 6d70 6f73 6974 6520 3d20 636f 6d70  composite = comp
-000139f0: 6f73 6974 652e 6164 6442 616e 6473 2863  osite.addBands(c
-00013a00: 6f75 6e74 292e 666c 6f61 7428 290d 0a0d  ount).float()...
-00013a10: 0a20 2020 2072 6574 7572 6e20 636f 6d70  .    return comp
-00013a20: 6f73 6974 652e 7365 7428 7b27 7379 7374  osite.set({'syst
-00013a30: 656d 3a74 696d 655f 7374 6172 7427 3a65  em:time_start':e
-00013a40: 652e 4461 7465 2e66 726f 6d59 4d44 2879  e.Date.fromYMD(y
-00013a50: 6561 722b 2079 6561 7257 6974 684d 616a  ear+ yearWithMaj
-00013a60: 6f72 6974 792c 362c 3129 2e6d 696c 6c69  ority,6,1).milli
-00013a70: 7328 292c 5c0d 0a20 2020 2020 2020 2020  s(),\..         
-00013a80: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013a90: 7374 6172 7444 6174 6527 3a73 7461 7274  startDate':start
-00013aa0: 4461 7465 542e 6d69 6c6c 6973 2829 2c5c  DateT.millis(),\
-00013ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013ac0: 2020 2020 2020 2020 2020 2765 6e64 4461            'endDa
-00013ad0: 7465 273a 656e 6444 6174 6554 2e6d 696c  te':endDateT.mil
-00013ae0: 6c69 7328 292c 5c0d 0a20 2020 2020 2020  lis(),\..       
+000131a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000131b0: 2323 2323 0d0a 2343 7265 6174 6520 636f  ####..#Create co
+000131c0: 6d70 6f73 6974 6573 2066 6f72 2065 6163  mposites for eac
+000131d0: 6820 7965 6172 2077 6974 6869 6e20 7374  h year within st
+000131e0: 6172 7459 6561 7220 616e 6420 656e 6459  artYear and endY
+000131f0: 6561 7220 7261 6e67 650d 0a64 6566 2063  ear range..def c
+00013200: 6f6d 706f 7369 7465 5469 6d65 5365 7269  ompositeTimeSeri
+00013210: 6573 280d 0a20 2020 2020 206c 732c 0d0a  es(..      ls,..
+00013220: 2020 2020 2020 7374 6172 7459 6561 722c        startYear,
+00013230: 0d0a 2020 2020 2020 656e 6459 6561 722c  ..      endYear,
+00013240: 0d0a 2020 2020 2020 7374 6172 744a 756c  ..      startJul
+00013250: 6961 6e2c 0d0a 2020 2020 2020 656e 644a  ian,..      endJ
+00013260: 756c 6961 6e2c 0d0a 2020 2020 2020 7469  ulian,..      ti
+00013270: 6d65 6275 6666 6572 203d 2030 2c0d 0a20  mebuffer = 0,.. 
+00013280: 2020 2020 2077 6569 6768 7473 203d 205b       weights = [
+00013290: 315d 2c0d 0a20 2020 2020 2063 6f6d 706f  1],..      compo
+000132a0: 7369 7469 6e67 4d65 7468 6f64 203d 204e  sitingMethod = N
+000132b0: 6f6e 652c 0d0a 2020 2020 2020 636f 6d70  one,..      comp
+000132c0: 6f73 6974 696e 6752 6564 7563 6572 203d  ositingReducer =
+000132d0: 204e 6f6e 6529 3a0d 0a0d 0a20 2061 7267   None):....  arg
+000132e0: 7320 3d20 666f 726d 6174 4172 6773 286c  s = formatArgs(l
+000132f0: 6f63 616c 7328 2929 0d0a 2020 6966 2027  ocals())..  if '
+00013300: 6172 6773 2720 696e 2061 7267 732e 6b65  args' in args.ke
+00013310: 7973 2829 3a0d 0a20 2020 2064 656c 2061  ys():..    del a
+00013320: 7267 735b 2761 7267 7327 5d0d 0a0d 0a20  rgs['args'].... 
+00013330: 2064 756d 6d79 496d 6167 6520 3d20 6565   dummyImage = ee
+00013340: 2e49 6d61 6765 286c 732e 6669 7273 7428  .Image(ls.first(
+00013350: 2929 0d0a 0d0a 2020 6461 7465 5772 6170  ))....  dateWrap
+00013360: 7069 6e67 203d 2077 7261 7044 6174 6573  ping = wrapDates
+00013370: 2873 7461 7274 4a75 6c69 616e 2c65 6e64  (startJulian,end
+00013380: 4a75 6c69 616e 290d 0a20 2077 7261 704f  Julian)..  wrapO
+00013390: 6666 7365 7420 3d20 6461 7465 5772 6170  ffset = dateWrap
+000133a0: 7069 6e67 5b30 5d0d 0a20 2079 6561 7257  ping[0]..  yearW
+000133b0: 6974 684d 616a 6f72 6974 7920 3d20 6461  ithMajority = da
+000133c0: 7465 5772 6170 7069 6e67 5b31 5d0d 0a0d  teWrapping[1]...
+000133d0: 0a0d 0a0d 0a20 2064 6566 2079 6561 7243  .....  def yearC
+000133e0: 6f6d 706f 7369 7465 4765 7474 6572 2879  ompositeGetter(y
+000133f0: 6561 7229 3a0d 0a0d 0a20 2020 2023 5365  ear):....    #Se
+00013400: 7420 7570 2064 6174 6573 0d0a 2020 2020  t up dates..    
+00013410: 7374 6172 7459 6561 7254 203d 2079 6561  startYearT = yea
+00013420: 722d 7469 6d65 6275 6666 6572 0d0a 2020  r-timebuffer..  
+00013430: 2020 656e 6459 6561 7254 203d 2079 6561    endYearT = yea
+00013440: 722b 7469 6d65 6275 6666 6572 0d0a 2020  r+timebuffer..  
+00013450: 2020 7374 6172 7444 6174 6554 203d 2065    startDateT = e
+00013460: 652e 4461 7465 2e66 726f 6d59 4d44 2873  e.Date.fromYMD(s
+00013470: 7461 7274 5965 6172 542c 312c 3129 2e61  tartYearT,1,1).a
+00013480: 6476 616e 6365 2873 7461 7274 4a75 6c69  dvance(startJuli
+00013490: 616e 2d31 2c27 6461 7927 290d 0a20 2020  an-1,'day')..   
+000134a0: 2065 6e64 4461 7465 5420 3d20 6565 2e44   endDateT = ee.D
+000134b0: 6174 652e 6672 6f6d 594d 4428 656e 6459  ate.fromYMD(endY
+000134c0: 6561 7254 2c31 2c31 292e 6164 7661 6e63  earT,1,1).advanc
+000134d0: 6528 656e 644a 756c 6961 6e2d 312b 7772  e(endJulian-1+wr
+000134e0: 6170 4f66 6673 6574 2c27 6461 7927 290d  apOffset,'day').
+000134f0: 0a0d 0a0d 0a20 2020 2023 7072 696e 7428  .....    #print(
+00013500: 7965 6172 2c73 7461 7274 4461 7465 542c  year,startDateT,
+00013510: 656e 6444 6174 6554 290d 0a0d 0a20 2020  endDateT)....   
+00013520: 2023 5365 7420 7570 2077 6569 6768 7465   #Set up weighte
+00013530: 6420 6d6f 7669 6e67 2077 6964 6f77 0d0a  d moving widow..
+00013540: 2020 2020 7965 6172 7354 203d 2065 652e      yearsT = ee.
+00013550: 4c69 7374 2e73 6571 7565 6e63 6528 7374  List.sequence(st
+00013560: 6172 7459 6561 7254 2c65 6e64 5965 6172  artYearT,endYear
+00013570: 5429 0d0a 0d0a 2020 2020 6465 6620 7a69  T)....    def zi
+00013580: 7070 6572 2869 293a 0d0a 2020 2020 2020  pper(i):..      
+00013590: 6920 3d20 6565 2e4c 6973 7428 6929 0d0a  i = ee.List(i)..
+000135a0: 2020 2020 2020 7265 7475 726e 2065 652e        return ee.
+000135b0: 4c69 7374 2e72 6570 6561 7428 692e 6765  List.repeat(i.ge
+000135c0: 7428 3029 2c69 2e67 6574 2831 2929 0d0a  t(0),i.get(1))..
+000135d0: 0d0a 2020 2020 7a20 3d20 7965 6172 7354  ..    z = yearsT
+000135e0: 2e7a 6970 2877 6569 6768 7473 290d 0a0d  .zip(weights)...
+000135f0: 0a20 2020 2079 6561 7273 5454 203d 207a  .    yearsTT = z
+00013600: 2e6d 6170 287a 6970 7065 7229 2e66 6c61  .map(zipper).fla
+00013610: 7474 656e 2829 0d0a 0d0a 2020 2020 2320  tten()....    # 
+00013620: 7072 696e 7428 2757 6569 6768 7465 6420  print('Weighted 
+00013630: 636f 6d70 6f73 6974 6520 7965 6172 7320  composite years 
+00013640: 666f 7220 7965 6172 3a27 2c79 6561 722c  for year:',year,
+00013650: 7965 6172 7354 542e 6765 7449 6e66 6f28  yearsTT.getInfo(
+00013660: 2929 0d0a 0d0a 2020 2020 2349 7465 7261  ))....    #Itera
+00013670: 7465 2061 6372 6f73 7320 6561 6368 2079  te across each y
+00013680: 6561 7220 696e 206c 6973 740d 0a20 2020  ear in list..   
+00013690: 2064 6566 2079 7247 6574 7465 7228 7972   def yrGetter(yr
+000136a0: 293a 0d0a 2020 2020 2020 2353 6574 2075  ):..      #Set u
+000136b0: 7020 6461 7465 730d 0a20 2020 2020 2073  p dates..      s
+000136c0: 7461 7274 4461 7465 5420 3d20 6565 2e44  tartDateT = ee.D
+000136d0: 6174 652e 6672 6f6d 594d 4428 7972 2c31  ate.fromYMD(yr,1
+000136e0: 2c31 292e 6164 7661 6e63 6528 7374 6172  ,1).advance(star
+000136f0: 744a 756c 6961 6e2d 312c 2764 6179 2729  tJulian-1,'day')
+00013700: 0d0a 2020 2020 2020 656e 6444 6174 6554  ..      endDateT
+00013710: 203d 2065 652e 4461 7465 2e66 726f 6d59   = ee.Date.fromY
+00013720: 4d44 2879 722c 312c 3129 2e61 6476 616e  MD(yr,1,1).advan
+00013730: 6365 2865 6e64 4a75 6c69 616e 2d31 2b77  ce(endJulian-1+w
+00013740: 7261 704f 6666 7365 742c 2764 6179 2729  rapOffset,'day')
+00013750: 0d0a 0d0a 2020 2020 2020 2346 696c 7465  ....      #Filte
+00013760: 7220 696d 6167 6573 2066 6f72 2067 6976  r images for giv
+00013770: 656e 2064 6174 6520 7261 6e67 650d 0a20  en date range.. 
+00013780: 2020 2020 206c 7354 203d 206c 732e 6669       lsT = ls.fi
+00013790: 6c74 6572 4461 7465 2873 7461 7274 4461  lterDate(startDa
+000137a0: 7465 542c 656e 6444 6174 6554 2e61 6476  teT,endDateT.adv
+000137b0: 616e 6365 2831 2c27 6461 7927 2929 0d0a  ance(1,'day'))..
+000137c0: 2020 2020 2020 6c73 5420 3d20 6669 6c6c        lsT = fill
+000137d0: 456d 7074 7943 6f6c 6c65 6374 696f 6e73  EmptyCollections
+000137e0: 286c 7354 2c64 756d 6d79 496d 6167 6529  (lsT,dummyImage)
+000137f0: 0d0a 2020 2020 2020 7265 7475 726e 206c  ..      return l
+00013800: 7354 0d0a 2020 2020 696d 6167 6573 203d  sT..    images =
+00013810: 2079 6561 7273 5454 2e6d 6170 2879 7247   yearsTT.map(yrG
+00013820: 6574 7465 7229 0d0a 2020 2020 6c73 5420  etter)..    lsT 
+00013830: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
+00013840: 7469 6f6e 2865 652e 4665 6174 7572 6543  tion(ee.FeatureC
+00013850: 6f6c 6c65 6374 696f 6e28 696d 6167 6573  ollection(images
+00013860: 292e 666c 6174 7465 6e28 2929 0d0a 0d0a  ).flatten())....
+00013870: 2020 2020 636f 756e 7420 3d20 6c73 542e      count = lsT.
+00013880: 7365 6c65 6374 285b 305d 292e 636f 756e  select([0]).coun
+00013890: 7428 292e 7265 6e61 6d65 285b 2763 6f6d  t().rename(['com
+000138a0: 706f 7369 7465 4f62 7343 6f75 6e74 275d  positeObsCount']
+000138b0: 290d 0a20 2020 2023 436f 6d70 7574 6520  )..    #Compute 
+000138c0: 6d65 6469 616e 206f 7220 6d65 646f 6964  median or medoid
+000138d0: 206f 7220 6170 706c 7920 7265 6475 6365   or apply reduce
+000138e0: 720d 0a20 2020 2069 6620 636f 6d70 6f73  r..    if compos
+000138f0: 6974 696e 6752 6564 7563 6572 2021 3d20  itingReducer != 
+00013900: 4e6f 6e65 3a0d 0a20 2020 2020 2063 6f6d  None:..      com
+00013910: 706f 7369 7465 203d 206c 7354 2e72 6564  posite = lsT.red
+00013920: 7563 6528 636f 6d70 6f73 6974 696e 6752  uce(compositingR
+00013930: 6564 7563 6572 290d 0a20 2020 2065 6c69  educer)..    eli
+00013940: 6620 636f 6d70 6f73 6974 696e 674d 6574  f compositingMet
+00013950: 686f 642e 6c6f 7765 7228 2920 3d3d 2027  hod.lower() == '
+00013960: 6d65 6469 616e 273a 0d0a 2020 2020 2020  median':..      
+00013970: 636f 6d70 6f73 6974 6520 3d20 6c73 542e  composite = lsT.
+00013980: 6d65 6469 616e 2829 0d0a 2020 2020 656c  median()..    el
+00013990: 7365 3a0d 0a20 2020 2020 2063 6f6d 706f  se:..      compo
+000139a0: 7369 7465 203d 206d 6564 6f69 644d 6f73  site = medoidMos
+000139b0: 6169 634d 5344 286c 7354 2c5b 2767 7265  aicMSD(lsT,['gre
+000139c0: 656e 272c 2772 6564 272c 276e 6972 272c  en','red','nir',
+000139d0: 2773 7769 7231 272c 2773 7769 7232 275d  'swir1','swir2']
+000139e0: 290d 0a20 2020 2063 6f6d 706f 7369 7465  )..    composite
+000139f0: 203d 2063 6f6d 706f 7369 7465 2e61 6464   = composite.add
+00013a00: 4261 6e64 7328 636f 756e 7429 2e66 6c6f  Bands(count).flo
+00013a10: 6174 2829 0d0a 0d0a 2020 2020 7265 7475  at()....    retu
+00013a20: 726e 2063 6f6d 706f 7369 7465 2e73 6574  rn composite.set
+00013a30: 287b 2773 7973 7465 6d3a 7469 6d65 5f73  ({'system:time_s
+00013a40: 7461 7274 273a 6565 2e44 6174 652e 6672  tart':ee.Date.fr
+00013a50: 6f6d 594d 4428 7965 6172 2b20 7965 6172  omYMD(year+ year
+00013a60: 5769 7468 4d61 6a6f 7269 7479 2c36 2c31  WithMajority,6,1
+00013a70: 292e 6d69 6c6c 6973 2829 2c5c 0d0a 2020  ).millis(),\..  
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a90: 2020 2020 2020 2773 7461 7274 4461 7465        'startDate
+00013aa0: 273a 7374 6172 7444 6174 6554 2e6d 696c  ':startDateT.mil
+00013ab0: 6c69 7328 292c 5c0d 0a20 2020 2020 2020  lis(),\..       
+00013ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ad0: 2027 656e 6444 6174 6527 3a65 6e64 4461   'endDate':endDa
+00013ae0: 7465 542e 6d69 6c6c 6973 2829 2c5c 0d0a  teT.millis(),\..
 00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b00: 2027 7374 6172 744a 756c 6961 6e27 3a73   'startJulian':s
-00013b10: 7461 7274 4a75 6c69 616e 2c5c 0d0a 2020  tartJulian,\..  
-00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b30: 2020 2020 2020 2765 6e64 4a75 6c69 616e        'endJulian
-00013b40: 273a 656e 644a 756c 6961 6e2c 5c0d 0a20  ':endJulian,\.. 
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 2020 2020 2020 2027 7965 6172 4275 6666         'yearBuff
-00013b70: 6572 273a 7469 6d65 6275 6666 6572 2c5c  er':timebuffer,\
-00013b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013b90: 2020 2020 2020 2020 2020 2779 6561 7257            'yearW
-00013ba0: 6569 6768 7473 273a 2073 7472 2877 6569  eights': str(wei
-00013bb0: 6768 7473 292c 5c0d 0a20 2020 2020 2020  ghts),\..       
+00013b00: 2020 2020 2020 2020 2773 7461 7274 4a75          'startJu
+00013b10: 6c69 616e 273a 7374 6172 744a 756c 6961  lian':startJulia
+00013b20: 6e2c 5c0d 0a20 2020 2020 2020 2020 2020  n,\..           
+00013b30: 2020 2020 2020 2020 2020 2020 2027 656e               'en
+00013b40: 644a 756c 6961 6e27 3a65 6e64 4a75 6c69  dJulian':endJuli
+00013b50: 616e 2c5c 0d0a 2020 2020 2020 2020 2020  an,\..          
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2779                'y
+00013b70: 6561 7242 7566 6665 7227 3a74 696d 6562  earBuffer':timeb
+00013b80: 7566 6665 722c 5c0d 0a20 2020 2020 2020  uffer,\..       
+00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ba0: 2027 7965 6172 5765 6967 6874 7327 3a20   'yearWeights': 
+00013bb0: 7374 7228 7765 6967 6874 7329 2c5c 0d0a  str(weights),\..
 00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bd0: 2027 7972 4f72 6967 696e 616c 273a 7965   'yrOriginal':ye
-00013be0: 6172 2c5c 0d0a 2020 2020 2020 2020 2020  ar,\..          
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2779                'y
-00013c00: 7255 7365 6427 3a20 7965 6172 202b 2079  rUsed': year + y
-00013c10: 6561 7257 6974 684d 616a 6f72 6974 797d  earWithMajority}
-00013c20: 290d 0a0d 0a20 2023 4974 6572 6174 6520  )....  #Iterate 
-00013c30: 6163 726f 7373 2065 6163 6820 7965 6172  across each year
-00013c40: 0d0a 2020 7473 203d 205b 7965 6172 436f  ..  ts = [yearCo
-00013c50: 6d70 6f73 6974 6547 6574 7465 7228 7972  mpositeGetter(yr
-00013c60: 2920 666f 7220 7972 2069 6e20 6565 2e4c  ) for yr in ee.L
-00013c70: 6973 742e 7365 7175 656e 6365 2873 7461  ist.sequence(sta
-00013c80: 7274 5965 6172 2b74 696d 6562 7566 6665  rtYear+timebuffe
-00013c90: 722c 656e 6459 6561 722d 7469 6d65 6275  r,endYear-timebu
-00013ca0: 6666 6572 292e 6765 7449 6e66 6f28 295d  ffer).getInfo()]
-00013cb0: 0d0a 2020 7473 203d 2065 652e 496d 6167  ..  ts = ee.Imag
-00013cc0: 6543 6f6c 6c65 6374 696f 6e28 7473 292e  eCollection(ts).
-00013cd0: 7365 7428 6172 6773 290d 0a0d 0a20 2072  set(args)....  r
-00013ce0: 6574 7572 6e20 7473 0d0a 0d0a 2320 2f2f  eturn ts....# //
-00013cf0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+00013bd0: 2020 2020 2020 2020 2779 724f 7269 6769          'yrOrigi
+00013be0: 6e61 6c27 3a79 6561 722c 5c0d 0a20 2020  nal':year,\..   
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 2020 2027 7972 5573 6564 273a 2079       'yrUsed': y
+00013c10: 6561 7220 2b20 7965 6172 5769 7468 4d61  ear + yearWithMa
+00013c20: 6a6f 7269 7479 7d29 0d0a 0d0a 2020 2349  jority})....  #I
+00013c30: 7465 7261 7465 2061 6372 6f73 7320 6561  terate across ea
+00013c40: 6368 2079 6561 720d 0a20 2074 7320 3d20  ch year..  ts = 
+00013c50: 5b79 6561 7243 6f6d 706f 7369 7465 4765  [yearCompositeGe
+00013c60: 7474 6572 2879 7229 2066 6f72 2079 7220  tter(yr) for yr 
+00013c70: 696e 2065 652e 4c69 7374 2e73 6571 7565  in ee.List.seque
+00013c80: 6e63 6528 7374 6172 7459 6561 722b 7469  nce(startYear+ti
+00013c90: 6d65 6275 6666 6572 2c65 6e64 5965 6172  mebuffer,endYear
+00013ca0: 2d74 696d 6562 7566 6665 7229 2e67 6574  -timebuffer).get
+00013cb0: 496e 666f 2829 5d0d 0a20 2074 7320 3d20  Info()]..  ts = 
+00013cc0: 6565 2e49 6d61 6765 436f 6c6c 6563 7469  ee.ImageCollecti
+00013cd0: 6f6e 2874 7329 2e73 6574 2861 7267 7329  on(ts).set(args)
+00013ce0: 0d0a 0d0a 2020 7265 7475 726e 2074 730d  ....  return ts.
+00013cf0: 0a0d 0a23 202f 2f2f 2f2f 2f2f 2f2f 2f2f  ...# ///////////
 00013d00: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 00013d10: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 00013d20: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-00013d30: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 0d0a  //////////////..
-00013d40: 2320 4675 6e63 7469 6f6e 2074 6f20 6361  # Function to ca
-00013d50: 6c63 756c 6174 6520 696c 6c75 6d69 6e61  lculate illumina
-00013d60: 7469 6f6e 2063 6f6e 6469 7469 6f6e 2028  tion condition (
-00013d70: 4943 292e 2046 756e 6374 696f 6e20 6279  IC). Function by
-00013d80: 2050 6174 7269 636b 2042 7572 6e73 0d0a   Patrick Burns..
-00013d90: 2320 2870 6234 3633 406e 6175 2e65 6475  # (pb463@nau.edu
-00013da0: 2920 616e 6420 4d61 7474 204d 6163 616e  ) and Matt Macan
-00013db0: 6465 720d 0a23 2028 6d6d 6163 616e 6465  der..# (mmacande
-00013dc0: 7240 6162 7269 6e63 2e63 6f6d 290d 0a64  r@abrinc.com)..d
-00013dd0: 6566 2069 6c6c 756d 696e 6174 696f 6e43  ef illuminationC
-00013de0: 6f6e 6469 7469 6f6e 2869 6d67 293a 0d0a  ondition(img):..
-00013df0: 2020 2320 4578 7472 6163 7420 736f 6c61    # Extract sola
-00013e00: 7220 7a65 6e69 7468 2061 6e64 2061 7a69  r zenith and azi
-00013e10: 6d75 7468 2062 616e 6473 0d0a 2020 535a  muth bands..  SZ
-00013e20: 5f72 6164 203d 2069 6d67 2e73 656c 6563  _rad = img.selec
-00013e30: 7428 277a 656e 6974 6827 290d 0a20 2053  t('zenith')..  S
-00013e40: 415f 7261 6420 3d20 696d 672e 7365 6c65  A_rad = img.sele
-00013e50: 6374 2827 617a 696d 7574 6827 290d 0a0d  ct('azimuth')...
-00013e60: 0a20 2023 2043 7265 6174 2074 6572 7261  .  # Creat terra
-00013e70: 696e 206c 6179 6572 730d 0a20 2023 2064  in layers..  # d
-00013e80: 656d 203d 2065 652e 496d 6167 6528 2743  em = ee.Image('C
-00013e90: 4749 4152 2f53 5254 4d39 305f 5634 2729  GIAR/SRTM90_V4')
-00013ea0: 0d0a 2020 6465 6d20 3d20 6565 2e49 6d61  ..  dem = ee.Ima
-00013eb0: 6765 2827 5553 4753 2f4e 4544 2729 0d0a  ge('USGS/NED')..
-00013ec0: 2020 736c 7020 3d20 6565 2e54 6572 7261    slp = ee.Terra
-00013ed0: 696e 2e73 6c6f 7065 2864 656d 290d 0a20  in.slope(dem).. 
-00013ee0: 2073 6c70 5f72 6164 203d 2065 652e 5465   slp_rad = ee.Te
-00013ef0: 7272 6169 6e2e 736c 6f70 6528 6465 6d29  rrain.slope(dem)
-00013f00: 2e6d 756c 7469 706c 7928 6d61 7468 2e70  .multiply(math.p
-00013f10: 6929 2e64 6976 6964 6528 3138 3029 0d0a  i).divide(180)..
-00013f20: 2020 6173 705f 7261 6420 3d20 6565 2e54    asp_rad = ee.T
-00013f30: 6572 7261 696e 2e61 7370 6563 7428 6465  errain.aspect(de
-00013f40: 6d29 2e6d 756c 7469 706c 7928 6d61 7468  m).multiply(math
-00013f50: 2e70 6929 2e64 6976 6964 6528 3138 3029  .pi).divide(180)
-00013f60: 0d0a 0d0a 2020 2320 4361 6c63 756c 6174  ....  # Calculat
-00013f70: 6520 7468 6520 496c 6c75 6d69 6e61 7469  e the Illuminati
-00013f80: 6f6e 2043 6f6e 6469 7469 6f6e 2028 4943  on Condition (IC
-00013f90: 290d 0a20 2023 2073 6c6f 7065 2070 6172  )..  # slope par
-00013fa0: 7420 6f66 2074 6865 2069 6c6c 756d 696e  t of the illumin
-00013fb0: 6174 696f 6e20 636f 6e64 6974 696f 6e0d  ation condition.
-00013fc0: 0a20 2063 6f73 5a20 3d20 535a 5f72 6164  .  cosZ = SZ_rad
-00013fd0: 2e63 6f73 2829 0d0a 2020 636f 7353 203d  .cos()..  cosS =
-00013fe0: 2073 6c70 5f72 6164 2e63 6f73 2829 0d0a   slp_rad.cos()..
-00013ff0: 2020 736c 6f70 655f 696c 6c75 6d69 6e61    slope_illumina
-00014000: 7469 6f6e 203d 2063 6f73 532e 6578 7072  tion = cosS.expr
-00014010: 6573 7369 6f6e 2822 636f 735a 202a 2063  ession("cosZ * c
-00014020: 6f73 5322 2c0d 0a20 2020 2020 2020 2020  osS",..         
+00013d30: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+00013d40: 2f2f 2f2f 2f0d 0a23 2046 756e 6374 696f  /////..# Functio
+00013d50: 6e20 746f 2063 616c 6375 6c61 7465 2069  n to calculate i
+00013d60: 6c6c 756d 696e 6174 696f 6e20 636f 6e64  llumination cond
+00013d70: 6974 696f 6e20 2849 4329 2e20 4675 6e63  ition (IC). Func
+00013d80: 7469 6f6e 2062 7920 5061 7472 6963 6b20  tion by Patrick 
+00013d90: 4275 726e 730d 0a23 2028 7062 3436 3340  Burns..# (pb463@
+00013da0: 6e61 752e 6564 7529 2061 6e64 204d 6174  nau.edu) and Mat
+00013db0: 7420 4d61 6361 6e64 6572 0d0a 2320 286d  t Macander..# (m
+00013dc0: 6d61 6361 6e64 6572 4061 6272 696e 632e  macander@abrinc.
+00013dd0: 636f 6d29 0d0a 6465 6620 696c 6c75 6d69  com)..def illumi
+00013de0: 6e61 7469 6f6e 436f 6e64 6974 696f 6e28  nationCondition(
+00013df0: 696d 6729 3a0d 0a20 2023 2045 7874 7261  img):..  # Extra
+00013e00: 6374 2073 6f6c 6172 207a 656e 6974 6820  ct solar zenith 
+00013e10: 616e 6420 617a 696d 7574 6820 6261 6e64  and azimuth band
+00013e20: 730d 0a20 2053 5a5f 7261 6420 3d20 696d  s..  SZ_rad = im
+00013e30: 672e 7365 6c65 6374 2827 7a65 6e69 7468  g.select('zenith
+00013e40: 2729 0d0a 2020 5341 5f72 6164 203d 2069  ')..  SA_rad = i
+00013e50: 6d67 2e73 656c 6563 7428 2761 7a69 6d75  mg.select('azimu
+00013e60: 7468 2729 0d0a 0d0a 2020 2320 4372 6561  th')....  # Crea
+00013e70: 7420 7465 7272 6169 6e20 6c61 7965 7273  t terrain layers
+00013e80: 0d0a 2020 2320 6465 6d20 3d20 6565 2e49  ..  # dem = ee.I
+00013e90: 6d61 6765 2827 4347 4941 522f 5352 544d  mage('CGIAR/SRTM
+00013ea0: 3930 5f56 3427 290d 0a20 2064 656d 203d  90_V4')..  dem =
+00013eb0: 2065 652e 496d 6167 6528 2755 5347 532f   ee.Image('USGS/
+00013ec0: 4e45 4427 290d 0a20 2073 6c70 203d 2065  NED')..  slp = e
+00013ed0: 652e 5465 7272 6169 6e2e 736c 6f70 6528  e.Terrain.slope(
+00013ee0: 6465 6d29 0d0a 2020 736c 705f 7261 6420  dem)..  slp_rad 
+00013ef0: 3d20 6565 2e54 6572 7261 696e 2e73 6c6f  = ee.Terrain.slo
+00013f00: 7065 2864 656d 292e 6d75 6c74 6970 6c79  pe(dem).multiply
+00013f10: 286d 6174 682e 7069 292e 6469 7669 6465  (math.pi).divide
+00013f20: 2831 3830 290d 0a20 2061 7370 5f72 6164  (180)..  asp_rad
+00013f30: 203d 2065 652e 5465 7272 6169 6e2e 6173   = ee.Terrain.as
+00013f40: 7065 6374 2864 656d 292e 6d75 6c74 6970  pect(dem).multip
+00013f50: 6c79 286d 6174 682e 7069 292e 6469 7669  ly(math.pi).divi
+00013f60: 6465 2831 3830 290d 0a0d 0a20 2023 2043  de(180)....  # C
+00013f70: 616c 6375 6c61 7465 2074 6865 2049 6c6c  alculate the Ill
+00013f80: 756d 696e 6174 696f 6e20 436f 6e64 6974  umination Condit
+00013f90: 696f 6e20 2849 4329 0d0a 2020 2320 736c  ion (IC)..  # sl
+00013fa0: 6f70 6520 7061 7274 206f 6620 7468 6520  ope part of the 
+00013fb0: 696c 6c75 6d69 6e61 7469 6f6e 2063 6f6e  illumination con
+00013fc0: 6469 7469 6f6e 0d0a 2020 636f 735a 203d  dition..  cosZ =
+00013fd0: 2053 5a5f 7261 642e 636f 7328 290d 0a20   SZ_rad.cos().. 
+00013fe0: 2063 6f73 5320 3d20 736c 705f 7261 642e   cosS = slp_rad.
+00013ff0: 636f 7328 290d 0a20 2073 6c6f 7065 5f69  cos()..  slope_i
+00014000: 6c6c 756d 696e 6174 696f 6e20 3d20 636f  llumination = co
+00014010: 7353 2e65 7870 7265 7373 696f 6e28 2263  sS.expression("c
+00014020: 6f73 5a20 2a20 636f 7353 222c 0d0a 2020  osZ * cosS",..  
 00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014050: 207b 2763 6f73 5a27 3a20 636f 735a 2c0d   {'cosZ': cosZ,.
-00014060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014050: 2020 2020 2020 2020 7b27 636f 735a 273a          {'cosZ':
+00014060: 2063 6f73 5a2c 0d0a 2020 2020 2020 2020   cosZ,..        
 00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014080: 2020 2020 2020 2020 2020 2020 2763 6f73              'cos
-00014090: 5327 3a20 636f 7353 2e73 656c 6563 7428  S': cosS.select(
-000140a0: 2773 6c6f 7065 2729 7d29 0d0a 2020 2320  'slope')})..  # 
-000140b0: 6173 7065 6374 2070 6172 7420 6f66 2074  aspect part of t
-000140c0: 6865 2069 6c6c 756d 696e 6174 696f 6e20  he illumination 
-000140d0: 636f 6e64 6974 696f 6e0d 0a20 2073 696e  condition..  sin
-000140e0: 5a20 3d20 535a 5f72 6164 2e73 696e 2829  Z = SZ_rad.sin()
-000140f0: 0d0a 2020 7369 6e53 203d 2073 6c70 5f72  ..  sinS = slp_r
-00014100: 6164 2e73 696e 2829 0d0a 2020 636f 7341  ad.sin()..  cosA
-00014110: 7a69 4469 6666 203d 2028 5341 5f72 6164  ziDiff = (SA_rad
-00014120: 2e73 7562 7472 6163 7428 6173 705f 7261  .subtract(asp_ra
-00014130: 6429 292e 636f 7328 290d 0a20 2061 7370  d)).cos()..  asp
-00014140: 6563 745f 696c 6c75 6d69 6e61 7469 6f6e  ect_illumination
-00014150: 203d 2073 696e 5a2e 6578 7072 6573 7369   = sinZ.expressi
-00014160: 6f6e 2822 7369 6e5a 202a 2073 696e 5320  on("sinZ * sinS 
-00014170: 2a20 636f 7341 7a69 4469 6666 222c 0d0a  * cosAziDiff",..
-00014180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014090: 2020 2027 636f 7353 273a 2063 6f73 532e     'cosS': cosS.
+000140a0: 7365 6c65 6374 2827 736c 6f70 6527 297d  select('slope')}
+000140b0: 290d 0a20 2023 2061 7370 6563 7420 7061  )..  # aspect pa
+000140c0: 7274 206f 6620 7468 6520 696c 6c75 6d69  rt of the illumi
+000140d0: 6e61 7469 6f6e 2063 6f6e 6469 7469 6f6e  nation condition
+000140e0: 0d0a 2020 7369 6e5a 203d 2053 5a5f 7261  ..  sinZ = SZ_ra
+000140f0: 642e 7369 6e28 290d 0a20 2073 696e 5320  d.sin()..  sinS 
+00014100: 3d20 736c 705f 7261 642e 7369 6e28 290d  = slp_rad.sin().
+00014110: 0a20 2063 6f73 417a 6944 6966 6620 3d20  .  cosAziDiff = 
+00014120: 2853 415f 7261 642e 7375 6274 7261 6374  (SA_rad.subtract
+00014130: 2861 7370 5f72 6164 2929 2e63 6f73 2829  (asp_rad)).cos()
+00014140: 0d0a 2020 6173 7065 6374 5f69 6c6c 756d  ..  aspect_illum
+00014150: 696e 6174 696f 6e20 3d20 7369 6e5a 2e65  ination = sinZ.e
+00014160: 7870 7265 7373 696f 6e28 2273 696e 5a20  xpression("sinZ 
+00014170: 2a20 7369 6e53 202a 2063 6f73 417a 6944  * sinS * cosAziD
+00014180: 6966 6622 2c0d 0a20 2020 2020 2020 2020  iff",..         
 00014190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141a0: 2020 2020 2020 2020 2020 207b 2773 696e             {'sin
-000141b0: 5a27 3a20 7369 6e5a 2c0d 0a20 2020 2020  Z': sinZ,..     
-000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141b0: 2020 7b27 7369 6e5a 273a 2073 696e 5a2c    {'sinZ': sinZ,
+000141c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2020 2020 2020 2027 7369 6e53 273a 2073         'sinS': s
-000141f0: 696e 532c 0d0a 2020 2020 2020 2020 2020  inS,..          
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+000141f0: 696e 5327 3a20 7369 6e53 2c0d 0a20 2020  inS': sinS,..   
 00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014220: 2020 2763 6f73 417a 6944 6966 6627 3a20    'cosAziDiff': 
-00014230: 636f 7341 7a69 4469 6666 7d29 0d0a 2020  cosAziDiff})..  
-00014240: 2320 6675 6c6c 2069 6c6c 756d 696e 6174  # full illuminat
-00014250: 696f 6e20 636f 6e64 6974 696f 6e20 2849  ion condition (I
-00014260: 4329 0d0a 2020 6963 203d 2073 6c6f 7065  C)..  ic = slope
-00014270: 5f69 6c6c 756d 696e 6174 696f 6e2e 6164  _illumination.ad
-00014280: 6428 6173 7065 6374 5f69 6c6c 756d 696e  d(aspect_illumin
-00014290: 6174 696f 6e29 0d0a 0d0a 2020 2320 4164  ation)....  # Ad
-000142a0: 6420 4943 2074 6f20 6f72 6967 696e 616c  d IC to original
-000142b0: 2069 6d61 6765 0d0a 2020 7265 7475 726e   image..  return
-000142c0: 2069 6d67 2e61 6464 4261 6e64 7328 6963   img.addBands(ic
-000142d0: 2e72 656e 616d 6528 2749 4327 2929 5c0d  .rename('IC'))\.
-000142e0: 0a20 2020 2020 2020 2020 2020 202e 6164  .            .ad
-000142f0: 6442 616e 6473 2863 6f73 5a2e 7265 6e61  dBands(cosZ.rena
-00014300: 6d65 2827 636f 735a 2729 295c 0d0a 2020  me('cosZ'))\..  
-00014310: 2020 2020 2020 2020 2020 2e61 6464 4261            .addBa
-00014320: 6e64 7328 636f 7353 2e72 656e 616d 6528  nds(cosS.rename(
-00014330: 2763 6f73 5327 2929 5c0d 0a20 2020 2020  'cosS'))\..     
-00014340: 2020 2020 2020 202e 6164 6442 616e 6473         .addBands
-00014350: 2873 6c70 2e72 656e 616d 6528 2773 6c6f  (slp.rename('slo
-00014360: 7065 2729 290d 0a0d 0a23 2323 2323 2323  pe'))....#######
+00014220: 2020 2020 2020 2020 2027 636f 7341 7a69           'cosAzi
+00014230: 4469 6666 273a 2063 6f73 417a 6944 6966  Diff': cosAziDif
+00014240: 667d 290d 0a20 2023 2066 756c 6c20 696c  f})..  # full il
+00014250: 6c75 6d69 6e61 7469 6f6e 2063 6f6e 6469  lumination condi
+00014260: 7469 6f6e 2028 4943 290d 0a20 2069 6320  tion (IC)..  ic 
+00014270: 3d20 736c 6f70 655f 696c 6c75 6d69 6e61  = slope_illumina
+00014280: 7469 6f6e 2e61 6464 2861 7370 6563 745f  tion.add(aspect_
+00014290: 696c 6c75 6d69 6e61 7469 6f6e 290d 0a0d  illumination)...
+000142a0: 0a20 2023 2041 6464 2049 4320 746f 206f  .  # Add IC to o
+000142b0: 7269 6769 6e61 6c20 696d 6167 650d 0a20  riginal image.. 
+000142c0: 2072 6574 7572 6e20 696d 672e 6164 6442   return img.addB
+000142d0: 616e 6473 2869 632e 7265 6e61 6d65 2827  ands(ic.rename('
+000142e0: 4943 2729 295c 0d0a 2020 2020 2020 2020  IC'))\..        
+000142f0: 2020 2020 2e61 6464 4261 6e64 7328 636f      .addBands(co
+00014300: 735a 2e72 656e 616d 6528 2763 6f73 5a27  sZ.rename('cosZ'
+00014310: 2929 5c0d 0a20 2020 2020 2020 2020 2020  ))\..           
+00014320: 202e 6164 6442 616e 6473 2863 6f73 532e   .addBands(cosS.
+00014330: 7265 6e61 6d65 2827 636f 7353 2729 295c  rename('cosS'))\
+00014340: 0d0a 2020 2020 2020 2020 2020 2020 2e61  ..            .a
+00014350: 6464 4261 6e64 7328 736c 702e 7265 6e61  ddBands(slp.rena
+00014360: 6d65 2827 736c 6f70 6527 2929 0d0a 0d0a  me('slope'))....
 00014370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014390: 230d 0a23 2046 756e 6374 696f 6e20 746f  #..# Function to
-000143a0: 2061 7070 6c79 2074 6865 2053 756e 2d43   apply the Sun-C
-000143b0: 616e 6f70 792d 5365 6e73 6f72 202b 2043  anopy-Sensor + C
-000143c0: 2028 5343 5363 2920 636f 7272 6563 7469   (SCSc) correcti
-000143d0: 6f6e 206d 6574 686f 6420 746f 2065 6163  on method to eac
-000143e0: 680d 0a23 2069 6d61 6765 2e20 4675 6e63  h..# image. Func
-000143f0: 7469 6f6e 2062 7920 5061 7472 6963 6b20  tion by Patrick 
-00014400: 4275 726e 7320 2870 6234 3633 406e 6175  Burns (pb463@nau
-00014410: 2e65 6475 2920 616e 6420 4d61 7474 204d  .edu) and Matt M
-00014420: 6163 616e 6465 720d 0a23 2028 6d6d 6163  acander..# (mmac
-00014430: 616e 6465 7240 732e 636f 6d29 0d0a 6465  ander@s.com)..de
-00014440: 6620 2069 6c6c 756d 696e 6174 696f 6e43  f  illuminationC
-00014450: 6f72 7265 6374 696f 6e28 696d 672c 2073  orrection(img, s
-00014460: 6361 6c65 2c73 7475 6479 4172 6561 2c20  cale,studyArea, 
-00014470: 6261 6e64 4c69 7374 203d 205b 2762 6c75  bandList = ['blu
-00014480: 6527 2c20 2767 7265 656e 272c 2027 7265  e', 'green', 're
-00014490: 6427 2c20 276e 6972 272c 2027 7377 6972  d', 'nir', 'swir
-000144a0: 3127 2c20 2773 7769 7232 272c 2027 7465  1', 'swir2', 'te
-000144b0: 6d70 275d 293a 0d0a 0d0a 2020 7072 6f70  mp']):....  prop
-000144c0: 7320 3d20 696d 672e 746f 4469 6374 696f  s = img.toDictio
-000144d0: 6e61 7279 2829 0d0a 2020 7374 203d 2069  nary()..  st = i
-000144e0: 6d67 2e67 6574 2827 7379 7374 656d 3a74  mg.get('system:t
-000144f0: 696d 655f 7374 6172 7427 290d 0a20 2069  ime_start')..  i
-00014500: 6d67 5f70 6c75 735f 6963 203d 2069 6d67  mg_plus_ic = img
-00014510: 0d0a 2020 6d61 736b 3220 3d20 696d 675f  ..  mask2 = img_
-00014520: 706c 7573 5f69 632e 7365 6c65 6374 2827  plus_ic.select('
-00014530: 736c 6f70 6527 292e 6774 6528 3529 5c0d  slope').gte(5)\.
-00014540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014550: 2020 2020 202e 416e 6428 696d 675f 706c       .And(img_pl
-00014560: 7573 5f69 632e 7365 6c65 6374 2827 4943  us_ic.select('IC
-00014570: 2729 2e67 7465 2830 2929 5c0d 0a20 2020  ').gte(0))\..   
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 202e 416e 6428 696d 675f 706c 7573 5f69   .And(img_plus_i
-000145a0: 632e 7365 6c65 6374 2827 6e69 7227 292e  c.select('nir').
-000145b0: 6774 282d 302e 3129 290d 0a20 2069 6d67  gt(-0.1))..  img
-000145c0: 5f70 6c75 735f 6963 5f6d 6173 6b32 203d  _plus_ic_mask2 =
-000145d0: 2065 652e 496d 6167 6528 696d 675f 706c   ee.Image(img_pl
-000145e0: 7573 5f69 632e 7570 6461 7465 4d61 736b  us_ic.updateMask
-000145f0: 286d 6173 6b32 2929 0d0a 0d0a 2020 2320  (mask2))....  # 
-00014600: 5370 6563 6966 7920 4261 6e64 7320 746f  Specify Bands to
-00014610: 2074 6f70 6f67 7261 7068 6963 616c 6c79   topographically
-00014620: 2063 6f72 7265 6374 0d0a 2020 636f 6d70   correct..  comp
-00014630: 6f73 6974 6542 616e 6473 203d 2069 6d67  ositeBands = img
-00014640: 2e62 616e 644e 616d 6573 2829 0d0a 2020  .bandNames()..  
-00014650: 6e6f 6e43 6f72 7265 6374 4261 6e64 7320  nonCorrectBands 
-00014660: 3d20 696d 672e 7365 6c65 6374 2863 6f6d  = img.select(com
-00014670: 706f 7369 7465 4261 6e64 732e 7265 6d6f  positeBands.remo
-00014680: 7665 416c 6c28 6261 6e64 4c69 7374 2929  veAll(bandList))
-00014690: 0d0a 0d0a 2020 6465 6620 6170 706c 795f  ....  def apply_
-000146a0: 5343 5363 636f 7272 2862 616e 644c 6973  SCSccorr(bandLis
-000146b0: 7429 3a0d 0a20 2020 206d 6574 686f 6420  t):..    method 
-000146c0: 3d20 2753 4353 6327 0d0a 2020 2020 6f75  = 'SCSc'..    ou
-000146d0: 7420 3d20 696d 675f 706c 7573 5f69 635f  t = img_plus_ic_
-000146e0: 6d61 736b 322e 7365 6c65 6374 2827 4943  mask2.select('IC
-000146f0: 272c 2062 616e 644c 6973 7429 2e72 6564  ', bandList).red
-00014700: 7563 6552 6567 696f 6e28 2a2a 7b0d 0a20  uceRegion(**{.. 
-00014710: 2020 2020 2027 7265 6475 6365 7227 3a20       'reducer': 
-00014720: 6565 2e52 6564 7563 6572 2e6c 696e 6561  ee.Reducer.linea
-00014730: 7246 6974 2829 2c0d 0a20 2020 2020 2027  rFit(),..      '
-00014740: 6765 6f6d 6574 7279 273a 2073 7475 6479  geometry': study
-00014750: 4172 6561 2c0d 0a20 2020 2020 2027 7363  Area,..      'sc
-00014760: 616c 6527 3a20 7363 616c 652c 0d0a 2020  ale': scale,..  
-00014770: 2020 2020 276d 6178 5069 7865 6c73 273a      'maxPixels':
-00014780: 2031 6531 337d 290d 0a0d 0a20 2020 206f   1e13})....    o
-00014790: 7574 5f61 203d 2065 652e 4e75 6d62 6572  ut_a = ee.Number
-000147a0: 286f 7574 2e67 6574 2827 7363 616c 6527  (out.get('scale'
-000147b0: 2929 0d0a 2020 2020 6f75 745f 6220 3d20  ))..    out_b = 
-000147c0: 6565 2e4e 756d 6265 7228 6f75 742e 6765  ee.Number(out.ge
-000147d0: 7428 276f 6666 7365 7427 2929 0d0a 2020  t('offset'))..  
-000147e0: 2020 6f75 745f 6320 3d20 6f75 745f 622e    out_c = out_b.
-000147f0: 6469 7669 6465 286f 7574 5f61 290d 0a20  divide(out_a).. 
-00014800: 2020 2023 2041 7070 6c79 2074 6865 2053     # Apply the S
-00014810: 4353 6320 636f 7272 6563 7469 6f6e 0d0a  CSc correction..
-00014820: 2020 2020 5343 5363 5f6f 7574 7075 7420      SCSc_output 
-00014830: 3d20 696d 675f 706c 7573 5f69 635f 6d61  = img_plus_ic_ma
-00014840: 736b 322e 6578 7072 6573 7369 6f6e 285c  sk2.expression(\
-00014850: 0d0a 2020 2020 2020 2228 2869 6d61 6765  ..      "((image
-00014860: 202a 2028 636f 7342 202a 2063 6f73 5a20   * (cosB * cosZ 
-00014870: 2b20 6376 616c 7565 2929 202f 2028 6963  + cvalue)) / (ic
-00014880: 202b 2063 7661 6c75 6529 2922 2c20 7b5c   + cvalue))", {\
-00014890: 0d0a 2020 2020 2020 2769 6d61 6765 273a  ..      'image':
-000148a0: 2069 6d67 5f70 6c75 735f 6963 5f6d 6173   img_plus_ic_mas
-000148b0: 6b32 2e73 656c 6563 7428 6261 6e64 4c69  k2.select(bandLi
-000148c0: 7374 292c 0d0a 2020 2020 2020 2769 6327  st),..      'ic'
-000148d0: 3a20 696d 675f 706c 7573 5f69 635f 6d61  : img_plus_ic_ma
-000148e0: 736b 322e 7365 6c65 6374 2827 4943 2729  sk2.select('IC')
-000148f0: 2c0d 0a20 2020 2020 2027 636f 7342 273a  ,..      'cosB':
-00014900: 2069 6d67 5f70 6c75 735f 6963 5f6d 6173   img_plus_ic_mas
-00014910: 6b32 2e73 656c 6563 7428 2763 6f73 5327  k2.select('cosS'
-00014920: 292c 0d0a 2020 2020 2020 2763 6f73 5a27  ),..      'cosZ'
-00014930: 3a20 696d 675f 706c 7573 5f69 635f 6d61  : img_plus_ic_ma
-00014940: 736b 322e 7365 6c65 6374 2827 636f 735a  sk2.select('cosZ
-00014950: 2729 2c0d 0a20 2020 2020 2027 6376 616c  '),..      'cval
-00014960: 7565 273a 206f 7574 5f63 5c0d 0a20 2020  ue': out_c\..   
-00014970: 207d 290d 0a0d 0a20 2020 2072 6574 7572   })....    retur
-00014980: 6e20 5343 5363 5f6f 7574 7075 740d 0a0d  n SCSc_output...
-00014990: 0a20 2069 6d67 5f53 4353 6363 6f72 7220  .  img_SCSccorr 
-000149a0: 3d20 6565 2e49 6d61 6765 2862 616e 644c  = ee.Image(bandL
-000149b0: 6973 742e 6d61 7028 6170 706c 795f 5343  ist.map(apply_SC
-000149c0: 5363 636f 7272 2929 5c0d 0a20 2020 2020  Sccorr))\..     
-000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149e0: 202e 6164 6442 616e 6473 2869 6d67 5f70   .addBands(img_p
-000149f0: 6c75 735f 6963 2e73 656c 6563 7428 2749  lus_ic.select('I
-00014a00: 4327 2929 0d0a 2020 6261 6e64 4c69 7374  C'))..  bandList
-00014a10: 5f49 4320 3d20 6565 2e4c 6973 7428 5b62  _IC = ee.List([b
-00014a20: 616e 644c 6973 742c 2027 4943 275d 292e  andList, 'IC']).
-00014a30: 666c 6174 7465 6e28 290d 0a20 2069 6d67  flatten()..  img
-00014a40: 5f53 4353 6363 6f72 7220 3d20 696d 675f  _SCSccorr = img_
-00014a50: 5343 5363 636f 7272 2e75 6e6d 6173 6b28  SCSccorr.unmask(
-00014a60: 696d 675f 706c 7573 5f69 632e 7365 6c65  img_plus_ic.sele
-00014a70: 6374 2862 616e 644c 6973 745f 4943 2929  ct(bandList_IC))
-00014a80: 2e73 656c 6563 7428 6261 6e64 4c69 7374  .select(bandList
-00014a90: 290d 0a0d 0a20 2072 6574 7572 6e20 696d  )....  return im
-00014aa0: 675f 5343 5363 636f 7272 2e61 6464 4261  g_SCSccorr.addBa
-00014ab0: 6e64 7328 6e6f 6e43 6f72 7265 6374 4261  nds(nonCorrectBa
-00014ac0: 6e64 7329 5c0d 0a20 2020 2020 2020 2020  nds)\..         
-00014ad0: 2020 2020 2020 2020 2020 2020 202e 7365               .se
-00014ae0: 744d 756c 7469 2870 726f 7073 295c 0d0a  tMulti(props)\..
-00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b00: 2020 2020 2020 2e73 6574 2827 7379 7374        .set('syst
-00014b10: 656d 3a74 696d 655f 7374 6172 7427 2c73  em:time_start',s
-00014b20: 7429 0d0a 0d0a 2323 2323 2323 2323 2323  t)....##########
+00014390: 2323 2323 2323 2323 0d0a 2320 4675 6e63  ########..# Func
+000143a0: 7469 6f6e 2074 6f20 6170 706c 7920 7468  tion to apply th
+000143b0: 6520 5375 6e2d 4361 6e6f 7079 2d53 656e  e Sun-Canopy-Sen
+000143c0: 736f 7220 2b20 4320 2853 4353 6329 2063  sor + C (SCSc) c
+000143d0: 6f72 7265 6374 696f 6e20 6d65 7468 6f64  orrection method
+000143e0: 2074 6f20 6561 6368 0d0a 2320 696d 6167   to each..# imag
+000143f0: 652e 2046 756e 6374 696f 6e20 6279 2050  e. Function by P
+00014400: 6174 7269 636b 2042 7572 6e73 2028 7062  atrick Burns (pb
+00014410: 3436 3340 6e61 752e 6564 7529 2061 6e64  463@nau.edu) and
+00014420: 204d 6174 7420 4d61 6361 6e64 6572 0d0a   Matt Macander..
+00014430: 2320 286d 6d61 6361 6e64 6572 4073 2e63  # (mmacander@s.c
+00014440: 6f6d 290d 0a64 6566 2020 696c 6c75 6d69  om)..def  illumi
+00014450: 6e61 7469 6f6e 436f 7272 6563 7469 6f6e  nationCorrection
+00014460: 2869 6d67 2c20 7363 616c 652c 7374 7564  (img, scale,stud
+00014470: 7941 7265 612c 2062 616e 644c 6973 7420  yArea, bandList 
+00014480: 3d20 5b27 626c 7565 272c 2027 6772 6565  = ['blue', 'gree
+00014490: 6e27 2c20 2772 6564 272c 2027 6e69 7227  n', 'red', 'nir'
+000144a0: 2c20 2773 7769 7231 272c 2027 7377 6972  , 'swir1', 'swir
+000144b0: 3227 2c20 2774 656d 7027 5d29 3a0d 0a0d  2', 'temp']):...
+000144c0: 0a20 2070 726f 7073 203d 2069 6d67 2e74  .  props = img.t
+000144d0: 6f44 6963 7469 6f6e 6172 7928 290d 0a20  oDictionary().. 
+000144e0: 2073 7420 3d20 696d 672e 6765 7428 2773   st = img.get('s
+000144f0: 7973 7465 6d3a 7469 6d65 5f73 7461 7274  ystem:time_start
+00014500: 2729 0d0a 2020 696d 675f 706c 7573 5f69  ')..  img_plus_i
+00014510: 6320 3d20 696d 670d 0a20 206d 6173 6b32  c = img..  mask2
+00014520: 203d 2069 6d67 5f70 6c75 735f 6963 2e73   = img_plus_ic.s
+00014530: 656c 6563 7428 2773 6c6f 7065 2729 2e67  elect('slope').g
+00014540: 7465 2835 295c 0d0a 2020 2020 2020 2020  te(5)\..        
+00014550: 2020 2020 2020 2020 2020 2020 2e41 6e64              .And
+00014560: 2869 6d67 5f70 6c75 735f 6963 2e73 656c  (img_plus_ic.sel
+00014570: 6563 7428 2749 4327 292e 6774 6528 3029  ect('IC').gte(0)
+00014580: 295c 0d0a 2020 2020 2020 2020 2020 2020  )\..            
+00014590: 2020 2020 2020 2020 2e41 6e64 2869 6d67          .And(img
+000145a0: 5f70 6c75 735f 6963 2e73 656c 6563 7428  _plus_ic.select(
+000145b0: 276e 6972 2729 2e67 7428 2d30 2e31 2929  'nir').gt(-0.1))
+000145c0: 0d0a 2020 696d 675f 706c 7573 5f69 635f  ..  img_plus_ic_
+000145d0: 6d61 736b 3220 3d20 6565 2e49 6d61 6765  mask2 = ee.Image
+000145e0: 2869 6d67 5f70 6c75 735f 6963 2e75 7064  (img_plus_ic.upd
+000145f0: 6174 654d 6173 6b28 6d61 736b 3229 290d  ateMask(mask2)).
+00014600: 0a0d 0a20 2023 2053 7065 6369 6679 2042  ...  # Specify B
+00014610: 616e 6473 2074 6f20 746f 706f 6772 6170  ands to topograp
+00014620: 6869 6361 6c6c 7920 636f 7272 6563 740d  hically correct.
+00014630: 0a20 2063 6f6d 706f 7369 7465 4261 6e64  .  compositeBand
+00014640: 7320 3d20 696d 672e 6261 6e64 4e61 6d65  s = img.bandName
+00014650: 7328 290d 0a20 206e 6f6e 436f 7272 6563  s()..  nonCorrec
+00014660: 7442 616e 6473 203d 2069 6d67 2e73 656c  tBands = img.sel
+00014670: 6563 7428 636f 6d70 6f73 6974 6542 616e  ect(compositeBan
+00014680: 6473 2e72 656d 6f76 6541 6c6c 2862 616e  ds.removeAll(ban
+00014690: 644c 6973 7429 290d 0a0d 0a20 2064 6566  dList))....  def
+000146a0: 2061 7070 6c79 5f53 4353 6363 6f72 7228   apply_SCSccorr(
+000146b0: 6261 6e64 4c69 7374 293a 0d0a 2020 2020  bandList):..    
+000146c0: 6d65 7468 6f64 203d 2027 5343 5363 270d  method = 'SCSc'.
+000146d0: 0a20 2020 206f 7574 203d 2069 6d67 5f70  .    out = img_p
+000146e0: 6c75 735f 6963 5f6d 6173 6b32 2e73 656c  lus_ic_mask2.sel
+000146f0: 6563 7428 2749 4327 2c20 6261 6e64 4c69  ect('IC', bandLi
+00014700: 7374 292e 7265 6475 6365 5265 6769 6f6e  st).reduceRegion
+00014710: 282a 2a7b 0d0a 2020 2020 2020 2772 6564  (**{..      'red
+00014720: 7563 6572 273a 2065 652e 5265 6475 6365  ucer': ee.Reduce
+00014730: 722e 6c69 6e65 6172 4669 7428 292c 0d0a  r.linearFit(),..
+00014740: 2020 2020 2020 2767 656f 6d65 7472 7927        'geometry'
+00014750: 3a20 7374 7564 7941 7265 612c 0d0a 2020  : studyArea,..  
+00014760: 2020 2020 2773 6361 6c65 273a 2073 6361      'scale': sca
+00014770: 6c65 2c0d 0a20 2020 2020 2027 6d61 7850  le,..      'maxP
+00014780: 6978 656c 7327 3a20 3165 3133 7d29 0d0a  ixels': 1e13})..
+00014790: 0d0a 2020 2020 6f75 745f 6120 3d20 6565  ..    out_a = ee
+000147a0: 2e4e 756d 6265 7228 6f75 742e 6765 7428  .Number(out.get(
+000147b0: 2773 6361 6c65 2729 290d 0a20 2020 206f  'scale'))..    o
+000147c0: 7574 5f62 203d 2065 652e 4e75 6d62 6572  ut_b = ee.Number
+000147d0: 286f 7574 2e67 6574 2827 6f66 6673 6574  (out.get('offset
+000147e0: 2729 290d 0a20 2020 206f 7574 5f63 203d  '))..    out_c =
+000147f0: 206f 7574 5f62 2e64 6976 6964 6528 6f75   out_b.divide(ou
+00014800: 745f 6129 0d0a 2020 2020 2320 4170 706c  t_a)..    # Appl
+00014810: 7920 7468 6520 5343 5363 2063 6f72 7265  y the SCSc corre
+00014820: 6374 696f 6e0d 0a20 2020 2053 4353 635f  ction..    SCSc_
+00014830: 6f75 7470 7574 203d 2069 6d67 5f70 6c75  output = img_plu
+00014840: 735f 6963 5f6d 6173 6b32 2e65 7870 7265  s_ic_mask2.expre
+00014850: 7373 696f 6e28 5c0d 0a20 2020 2020 2022  ssion(\..      "
+00014860: 2828 696d 6167 6520 2a20 2863 6f73 4220  ((image * (cosB 
+00014870: 2a20 636f 735a 202b 2063 7661 6c75 6529  * cosZ + cvalue)
+00014880: 2920 2f20 2869 6320 2b20 6376 616c 7565  ) / (ic + cvalue
+00014890: 2929 222c 207b 5c0d 0a20 2020 2020 2027  ))", {\..      '
+000148a0: 696d 6167 6527 3a20 696d 675f 706c 7573  image': img_plus
+000148b0: 5f69 635f 6d61 736b 322e 7365 6c65 6374  _ic_mask2.select
+000148c0: 2862 616e 644c 6973 7429 2c0d 0a20 2020  (bandList),..   
+000148d0: 2020 2027 6963 273a 2069 6d67 5f70 6c75     'ic': img_plu
+000148e0: 735f 6963 5f6d 6173 6b32 2e73 656c 6563  s_ic_mask2.selec
+000148f0: 7428 2749 4327 292c 0d0a 2020 2020 2020  t('IC'),..      
+00014900: 2763 6f73 4227 3a20 696d 675f 706c 7573  'cosB': img_plus
+00014910: 5f69 635f 6d61 736b 322e 7365 6c65 6374  _ic_mask2.select
+00014920: 2827 636f 7353 2729 2c0d 0a20 2020 2020  ('cosS'),..     
+00014930: 2027 636f 735a 273a 2069 6d67 5f70 6c75   'cosZ': img_plu
+00014940: 735f 6963 5f6d 6173 6b32 2e73 656c 6563  s_ic_mask2.selec
+00014950: 7428 2763 6f73 5a27 292c 0d0a 2020 2020  t('cosZ'),..    
+00014960: 2020 2763 7661 6c75 6527 3a20 6f75 745f    'cvalue': out_
+00014970: 635c 0d0a 2020 2020 7d29 0d0a 0d0a 2020  c\..    })....  
+00014980: 2020 7265 7475 726e 2053 4353 635f 6f75    return SCSc_ou
+00014990: 7470 7574 0d0a 0d0a 2020 696d 675f 5343  tput....  img_SC
+000149a0: 5363 636f 7272 203d 2065 652e 496d 6167  Sccorr = ee.Imag
+000149b0: 6528 6261 6e64 4c69 7374 2e6d 6170 2861  e(bandList.map(a
+000149c0: 7070 6c79 5f53 4353 6363 6f72 7229 295c  pply_SCSccorr))\
+000149d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000149e0: 2020 2020 2020 2020 2e61 6464 4261 6e64          .addBand
+000149f0: 7328 696d 675f 706c 7573 5f69 632e 7365  s(img_plus_ic.se
+00014a00: 6c65 6374 2827 4943 2729 290d 0a20 2062  lect('IC'))..  b
+00014a10: 616e 644c 6973 745f 4943 203d 2065 652e  andList_IC = ee.
+00014a20: 4c69 7374 285b 6261 6e64 4c69 7374 2c20  List([bandList, 
+00014a30: 2749 4327 5d29 2e66 6c61 7474 656e 2829  'IC']).flatten()
+00014a40: 0d0a 2020 696d 675f 5343 5363 636f 7272  ..  img_SCSccorr
+00014a50: 203d 2069 6d67 5f53 4353 6363 6f72 722e   = img_SCSccorr.
+00014a60: 756e 6d61 736b 2869 6d67 5f70 6c75 735f  unmask(img_plus_
+00014a70: 6963 2e73 656c 6563 7428 6261 6e64 4c69  ic.select(bandLi
+00014a80: 7374 5f49 4329 292e 7365 6c65 6374 2862  st_IC)).select(b
+00014a90: 616e 644c 6973 7429 0d0a 0d0a 2020 7265  andList)....  re
+00014aa0: 7475 726e 2069 6d67 5f53 4353 6363 6f72  turn img_SCSccor
+00014ab0: 722e 6164 6442 616e 6473 286e 6f6e 436f  r.addBands(nonCo
+00014ac0: 7272 6563 7442 616e 6473 295c 0d0a 2020  rrectBands)\..  
+00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ae0: 2020 2020 2e73 6574 4d75 6c74 6928 7072      .setMulti(pr
+00014af0: 6f70 7329 5c0d 0a20 2020 2020 2020 2020  ops)\..         
+00014b00: 2020 2020 2020 2020 2020 2020 202e 7365               .se
+00014b10: 7428 2773 7973 7465 6d3a 7469 6d65 5f73  t('system:time_s
+00014b20: 7461 7274 272c 7374 290d 0a0d 0a23 2323  tart',st)....###
 00014b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014b60: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00014b70: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00014b60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014b70: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
 00014b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014bb0: 2323 2323 2323 2323 2323 0d0a 2341 2066  ##########..#A f
-00014bc0: 756e 6374 696f 6e20 746f 206d 6173 6b20  unction to mask 
-00014bd0: 6f75 7420 7069 7865 6c73 2074 6861 7420  out pixels that 
-00014be0: 6469 6420 6e6f 7420 6861 7665 206f 6273  did not have obs
-00014bf0: 6572 7661 7469 6f6e 7320 666f 7220 4d4f  ervations for MO
-00014c00: 4449 532e 0d0a 6465 6620 6d61 736b 456d  DIS...def maskEm
-00014c10: 7074 7950 6978 656c 7328 696d 6167 6529  ptyPixels(image)
-00014c20: 3a0d 0a20 2023 4669 6e64 2070 6978 656c  :..  #Find pixel
-00014c30: 7320 7468 6174 2068 6164 206f 6273 6572  s that had obser
-00014c40: 7661 7469 6f6e 732e 0d0a 2020 7769 7468  vations...  with
-00014c50: 4f62 7320 3d20 696d 6167 652e 7365 6c65  Obs = image.sele
-00014c60: 6374 2827 6e75 6d5f 6f62 7365 7276 6174  ct('num_observat
-00014c70: 696f 6e73 5f31 6b6d 2729 2e67 7428 3029  ions_1km').gt(0)
-00014c80: 0d0a 2020 7265 7475 726e 2069 6d61 6765  ..  return image
-00014c90: 2e6d 6173 6b28 696d 6167 652e 6d61 736b  .mask(image.mask
-00014ca0: 2829 2e41 6e64 2877 6974 684f 6273 2929  ().And(withObs))
-00014cb0: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
+00014bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014bc0: 230d 0a23 4120 6675 6e63 7469 6f6e 2074  #..#A function t
+00014bd0: 6f20 6d61 736b 206f 7574 2070 6978 656c  o mask out pixel
+00014be0: 7320 7468 6174 2064 6964 206e 6f74 2068  s that did not h
+00014bf0: 6176 6520 6f62 7365 7276 6174 696f 6e73  ave observations
+00014c00: 2066 6f72 204d 4f44 4953 2e0d 0a64 6566   for MODIS...def
+00014c10: 206d 6173 6b45 6d70 7479 5069 7865 6c73   maskEmptyPixels
+00014c20: 2869 6d61 6765 293a 0d0a 2020 2346 696e  (image):..  #Fin
+00014c30: 6420 7069 7865 6c73 2074 6861 7420 6861  d pixels that ha
+00014c40: 6420 6f62 7365 7276 6174 696f 6e73 2e0d  d observations..
+00014c50: 0a20 2077 6974 684f 6273 203d 2069 6d61  .  withObs = ima
+00014c60: 6765 2e73 656c 6563 7428 276e 756d 5f6f  ge.select('num_o
+00014c70: 6273 6572 7661 7469 6f6e 735f 316b 6d27  bservations_1km'
+00014c80: 292e 6774 2830 290d 0a20 2072 6574 7572  ).gt(0)..  retur
+00014c90: 6e20 696d 6167 652e 6d61 736b 2869 6d61  n image.mask(ima
+00014ca0: 6765 2e6d 6173 6b28 292e 416e 6428 7769  ge.mask().And(wi
+00014cb0: 7468 4f62 7329 290d 0a0d 0a23 2323 2323  thObs))....#####
 00014cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014cf0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-00014d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014d00: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
 00014d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014d40: 2323 2323 2323 2323 0d0a 2320 4120 6675  ########..# A fu
-00014d50: 6e63 7469 6f6e 2074 6861 7420 7265 7475  nction that retu
-00014d60: 726e 7320 616e 2069 6d61 6765 2063 6f6e  rns an image con
-00014d70: 7461 696e 696e 6720 6a75 7374 2074 6865  taining just the
-00014d80: 2073 7065 6369 6669 6564 2051 4120 6269   specified QA bi
-00014d90: 7473 2e0d 0a23 0d0a 2320 4172 6773 3a0d  ts...#..# Args:.
-00014da0: 0a23 2020 2069 6d61 6765 202d 2054 6865  .#   image - The
-00014db0: 2051 4120 496d 6167 6520 746f 2067 6574   QA Image to get
-00014dc0: 2062 6974 7320 6672 6f6d 2e0d 0a23 2020   bits from...#  
-00014dd0: 2073 7461 7274 202d 2054 6865 2066 6972   start - The fir
-00014de0: 7374 2062 6974 2070 6f73 6974 696f 6e2c  st bit position,
-00014df0: 2030 2d62 6173 6564 2e0d 0a23 2020 2065   0-based...#   e
-00014e00: 6e64 2020 202d 2054 6865 206c 6173 7420  nd   - The last 
-00014e10: 6269 7420 706f 7369 7469 6f6e 2c20 696e  bit position, in
-00014e20: 636c 7573 6976 652e 0d0a 2320 2020 6e61  clusive...#   na
-00014e30: 6d65 2020 2d20 4120 6e61 6d65 2066 6f72  me  - A name for
-00014e40: 2074 6865 206f 7574 7075 7420 696d 6167   the output imag
-00014e50: 652e 0d0a 0d0a 6465 6620 6765 7451 4142  e.....def getQAB
-00014e60: 6974 7328 696d 6167 652c 2073 7461 7274  its(image, start
-00014e70: 2c20 656e 642c 206e 6577 4e61 6d65 293a  , end, newName):
-00014e80: 0d0a 2020 2343 6f6d 7075 7465 2074 6865  ..  #Compute the
-00014e90: 2062 6974 7320 7765 206e 6565 6420 746f   bits we need to
-00014ea0: 2065 7874 7261 6374 2e0d 0a20 2070 6174   extract...  pat
-00014eb0: 7465 726e 203d 2030 0d0a 2020 666f 7220  tern = 0..  for 
-00014ec0: 6920 696e 2072 616e 6765 2873 7461 7274  i in range(start
-00014ed0: 2c65 6e64 2b31 293a 0d0a 2020 2020 7061  ,end+1):..    pa
-00014ee0: 7474 6572 6e20 2b3d 206d 6174 682e 706f  ttern += math.po
-00014ef0: 7728 322c 2069 290d 0a0d 0a20 2023 5265  w(2, i)....  #Re
-00014f00: 7475 726e 2061 2073 696e 676c 6520 6261  turn a single ba
-00014f10: 6e64 2069 6d61 6765 206f 6620 7468 6520  nd image of the 
-00014f20: 6578 7472 6163 7465 6420 5141 2062 6974  extracted QA bit
-00014f30: 732c 2067 6976 696e 6720 7468 6520 6261  s, giving the ba
-00014f40: 6e64 2061 206e 6577 206e 616d 652e 0d0a  nd a new name...
-00014f50: 2020 7265 7475 726e 2069 6d61 6765 2e73    return image.s
-00014f60: 656c 6563 7428 5b30 5d2c 205b 6e65 774e  elect([0], [newN
-00014f70: 616d 655d 292e 6269 7477 6973 6541 6e64  ame]).bitwiseAnd
-00014f80: 2870 6174 7465 726e 292e 7269 6768 7453  (pattern).rightS
-00014f90: 6869 6674 2873 7461 7274 290d 0a0d 0a23  hift(start)....#
-00014fa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014d40: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+00014d50: 0a23 2041 2066 756e 6374 696f 6e20 7468  .# A function th
+00014d60: 6174 2072 6574 7572 6e73 2061 6e20 696d  at returns an im
+00014d70: 6167 6520 636f 6e74 6169 6e69 6e67 206a  age containing j
+00014d80: 7573 7420 7468 6520 7370 6563 6966 6965  ust the specifie
+00014d90: 6420 5141 2062 6974 732e 0d0a 230d 0a23  d QA bits...#..#
+00014da0: 2041 7267 733a 0d0a 2320 2020 696d 6167   Args:..#   imag
+00014db0: 6520 2d20 5468 6520 5141 2049 6d61 6765  e - The QA Image
+00014dc0: 2074 6f20 6765 7420 6269 7473 2066 726f   to get bits fro
+00014dd0: 6d2e 0d0a 2320 2020 7374 6172 7420 2d20  m...#   start - 
+00014de0: 5468 6520 6669 7273 7420 6269 7420 706f  The first bit po
+00014df0: 7369 7469 6f6e 2c20 302d 6261 7365 642e  sition, 0-based.
+00014e00: 0d0a 2320 2020 656e 6420 2020 2d20 5468  ..#   end   - Th
+00014e10: 6520 6c61 7374 2062 6974 2070 6f73 6974  e last bit posit
+00014e20: 696f 6e2c 2069 6e63 6c75 7369 7665 2e0d  ion, inclusive..
+00014e30: 0a23 2020 206e 616d 6520 202d 2041 206e  .#   name  - A n
+00014e40: 616d 6520 666f 7220 7468 6520 6f75 7470  ame for the outp
+00014e50: 7574 2069 6d61 6765 2e0d 0a0d 0a64 6566  ut image.....def
+00014e60: 2067 6574 5141 4269 7473 2869 6d61 6765   getQABits(image
+00014e70: 2c20 7374 6172 742c 2065 6e64 2c20 6e65  , start, end, ne
+00014e80: 774e 616d 6529 3a0d 0a20 2023 436f 6d70  wName):..  #Comp
+00014e90: 7574 6520 7468 6520 6269 7473 2077 6520  ute the bits we 
+00014ea0: 6e65 6564 2074 6f20 6578 7472 6163 742e  need to extract.
+00014eb0: 0d0a 2020 7061 7474 6572 6e20 3d20 300d  ..  pattern = 0.
+00014ec0: 0a20 2066 6f72 2069 2069 6e20 7261 6e67  .  for i in rang
+00014ed0: 6528 7374 6172 742c 656e 642b 3129 3a0d  e(start,end+1):.
+00014ee0: 0a20 2020 2070 6174 7465 726e 202b 3d20  .    pattern += 
+00014ef0: 6d61 7468 2e70 6f77 2832 2c20 6929 0d0a  math.pow(2, i)..
+00014f00: 0d0a 2020 2352 6574 7572 6e20 6120 7369  ..  #Return a si
+00014f10: 6e67 6c65 2062 616e 6420 696d 6167 6520  ngle band image 
+00014f20: 6f66 2074 6865 2065 7874 7261 6374 6564  of the extracted
+00014f30: 2051 4120 6269 7473 2c20 6769 7669 6e67   QA bits, giving
+00014f40: 2074 6865 2062 616e 6420 6120 6e65 7720   the band a new 
+00014f50: 6e61 6d65 2e0d 0a20 2072 6574 7572 6e20  name...  return 
+00014f60: 696d 6167 652e 7365 6c65 6374 285b 305d  image.select([0]
+00014f70: 2c20 5b6e 6577 4e61 6d65 5d29 2e62 6974  , [newName]).bit
+00014f80: 7769 7365 416e 6428 7061 7474 6572 6e29  wiseAnd(pattern)
+00014f90: 2e72 6967 6874 5368 6966 7428 7374 6172  .rightShift(star
+00014fa0: 7429 0d0a 0d0a 2323 2323 2323 2323 2323  t)....##########
 00014fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00014fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00014fe0: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
-00014ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00014fe0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+00014ff0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
 00015000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015030: 2323 230d 0a23 4120 6675 6e63 7469 6f6e  ###..#A function
-00015040: 2074 6f20 6d61 736b 206f 7574 2063 6c6f   to mask out clo
-00015050: 7564 7920 7069 7865 6c73 2e0d 0a64 6566  udy pixels...def
-00015060: 206d 6173 6b43 6c6f 7564 7357 5141 2869   maskCloudsWQA(i
-00015070: 6d61 6765 293a 0d0a 2020 2353 656c 6563  mage):..  #Selec
-00015080: 7420 7468 6520 5141 2062 616e 642e 0d0a  t the QA band...
-00015090: 2020 5141 203d 2069 6d61 6765 2e73 656c    QA = image.sel
-000150a0: 6563 7428 2773 7461 7465 5f31 6b6d 2729  ect('state_1km')
-000150b0: 0d0a 2020 2347 6574 2074 6865 2069 6e74  ..  #Get the int
-000150c0: 6572 6e61 6c5f 636c 6f75 645f 616c 676f  ernal_cloud_algo
-000150d0: 7269 7468 6d5f 666c 6167 2062 6974 2e0d  rithm_flag bit..
-000150e0: 0a20 2069 6e74 6572 6e61 6c43 6c6f 7564  .  internalCloud
-000150f0: 203d 2067 6574 5141 4269 7473 2851 412c   = getQABits(QA,
-00015100: 2031 302c 2031 302c 2027 696e 7465 726e   10, 10, 'intern
-00015110: 616c 5f63 6c6f 7564 5f61 6c67 6f72 6974  al_cloud_algorit
-00015120: 686d 5f66 6c61 6727 290d 0a20 2023 5265  hm_flag')..  #Re
-00015130: 7475 726e 2061 6e20 696d 6167 6520 6d61  turn an image ma
-00015140: 736b 696e 6720 6f75 7420 636c 6f75 6479  sking out cloudy
-00015150: 2061 7265 6173 2e0d 0a20 2072 6574 7572   areas...  retur
-00015160: 6e20 696d 6167 652e 6d61 736b 2869 6d61  n image.mask(ima
-00015170: 6765 2e6d 6173 6b28 292e 416e 6428 696e  ge.mask().And(in
-00015180: 7465 726e 616c 436c 6f75 642e 6571 2830  ternalCloud.eq(0
-00015190: 2929 290d 0a0d 0a23 2323 2323 2323 2323  )))....#########
+00015030: 2323 2323 2323 2323 2323 0d0a 2341 2066  ##########..#A f
+00015040: 756e 6374 696f 6e20 746f 206d 6173 6b20  unction to mask 
+00015050: 6f75 7420 636c 6f75 6479 2070 6978 656c  out cloudy pixel
+00015060: 732e 0d0a 6465 6620 6d61 736b 436c 6f75  s...def maskClou
+00015070: 6473 5751 4128 696d 6167 6529 3a0d 0a20  dsWQA(image):.. 
+00015080: 2023 5365 6c65 6374 2074 6865 2051 4120   #Select the QA 
+00015090: 6261 6e64 2e0d 0a20 2051 4120 3d20 696d  band...  QA = im
+000150a0: 6167 652e 7365 6c65 6374 2827 7374 6174  age.select('stat
+000150b0: 655f 316b 6d27 290d 0a20 2023 4765 7420  e_1km')..  #Get 
+000150c0: 7468 6520 696e 7465 726e 616c 5f63 6c6f  the internal_clo
+000150d0: 7564 5f61 6c67 6f72 6974 686d 5f66 6c61  ud_algorithm_fla
+000150e0: 6720 6269 742e 0d0a 2020 696e 7465 726e  g bit...  intern
+000150f0: 616c 436c 6f75 6420 3d20 6765 7451 4142  alCloud = getQAB
+00015100: 6974 7328 5141 2c20 3130 2c20 3130 2c20  its(QA, 10, 10, 
+00015110: 2769 6e74 6572 6e61 6c5f 636c 6f75 645f  'internal_cloud_
+00015120: 616c 676f 7269 7468 6d5f 666c 6167 2729  algorithm_flag')
+00015130: 0d0a 2020 2352 6574 7572 6e20 616e 2069  ..  #Return an i
+00015140: 6d61 6765 206d 6173 6b69 6e67 206f 7574  mage masking out
+00015150: 2063 6c6f 7564 7920 6172 6561 732e 0d0a   cloudy areas...
+00015160: 2020 7265 7475 726e 2069 6d61 6765 2e6d    return image.m
+00015170: 6173 6b28 696d 6167 652e 6d61 736b 2829  ask(image.mask()
+00015180: 2e41 6e64 2869 6e74 6572 6e61 6c43 6c6f  .And(internalClo
+00015190: 7564 2e65 7128 3029 2929 0d0a 0d0a 2323  ud.eq(0)))....##
 000151a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000151b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000151c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000151d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000151e0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+000151e0: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
 000151f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015220: 2323 2323 2323 2323 2323 230d 0a23 536f  ###########..#So
-00015230: 7572 6365 3a20 636f 6465 2e65 6172 7468  urce: code.earth
-00015240: 656e 6769 6e65 2e67 6f6f 676c 652e 636f  engine.google.co
-00015250: 6d0d 0a23 436f 6d70 7574 6520 6120 636c  m..#Compute a cl
-00015260: 6f75 6420 7363 6f72 652e 2020 5468 6973  oud score.  This
-00015270: 2065 7870 6563 7473 2074 6865 2069 6e70   expects the inp
-00015280: 7574 2069 6d61 6765 2074 6f20 6861 7665  ut image to have
-00015290: 2074 6865 2063 6f6d 6d6f 6e0d 0a23 6261   the common..#ba
-000152a0: 6e64 206e 616d 6573 3a20 5b22 7265 6422  nd names: ["red"
-000152b0: 2c20 2262 6c75 6522 2c20 6574 635d 2c20  , "blue", etc], 
-000152c0: 736f 2069 7420 6361 6e20 776f 726b 2061  so it can work a
-000152d0: 6372 6f73 7320 7365 6e73 6f72 732e 0d0a  cross sensors...
-000152e0: 6465 6620 6d6f 6469 7343 6c6f 7564 5363  def modisCloudSc
-000152f0: 6f72 6528 696d 6729 3a0d 0a0d 0a20 2075  ore(img):....  u
-00015300: 7365 5465 6d70 496e 436c 6f75 644d 6173  seTempInCloudMas
-00015310: 6b20 3d20 5472 7565 0d0a 2020 2343 6f6d  k = True..  #Com
-00015320: 7075 7465 2073 6576 6572 616c 2069 6e64  pute several ind
-00015330: 6963 6174 6f72 7320 6f66 2063 6c6f 7564  icators of cloud
-00015340: 796e 6573 7320 616e 6420 7461 6b65 2074  yness and take t
-00015350: 6865 206d 696e 696d 756d 206f 6620 7468  he minimum of th
-00015360: 656d 2e0d 0a20 2073 636f 7265 203d 2065  em...  score = e
-00015370: 652e 496d 6167 6528 312e 3029 3b0d 0a0d  e.Image(1.0);...
-00015380: 0a20 2023 436c 6f75 6473 2061 7265 2072  .  #Clouds are r
-00015390: 6561 736f 6e61 626c 7920 6272 6967 6874  easonably bright
-000153a0: 2069 6e20 7468 6520 626c 7565 2062 616e   in the blue ban
-000153b0: 642e 0d0a 2020 2320 7363 6f72 6520 3d20  d...  # score = 
-000153c0: 7363 6f72 652e 6d69 6e28 7265 7363 616c  score.min(rescal
-000153d0: 6528 696d 672c 2027 696d 672e 626c 7565  e(img, 'img.blue
-000153e0: 272c 205b 302e 312c 2030 2e33 5d29 290d  ', [0.1, 0.3])).
-000153f0: 0a20 2023 436c 6f75 6473 2061 7265 2072  .  #Clouds are r
-00015400: 6561 736f 6e61 626c 7920 6272 6967 6874  easonably bright
-00015410: 2069 6e20 616c 6c20 7669 7369 626c 6520   in all visible 
-00015420: 6261 6e64 732e 0d0a 2020 7669 7a53 756d  bands...  vizSum
-00015430: 203d 2072 6573 6361 6c65 2869 6d67 2e73   = rescale(img.s
-00015440: 656c 6563 7428 5b27 7265 6427 2c27 6772  elect(['red','gr
-00015450: 6565 6e27 2c27 626c 7565 275d 292e 7265  een','blue']).re
-00015460: 6475 6365 2865 652e 5265 6475 6365 722e  duce(ee.Reducer.
-00015470: 7375 6d28 2929 2c20 5b30 2e32 2c20 302e  sum()), [0.2, 0.
-00015480: 385d 290d 0a20 2073 636f 7265 203d 2073  8])..  score = s
-00015490: 636f 7265 2e6d 696e 2876 697a 5375 6d29  core.min(vizSum)
-000154a0: 0d0a 0d0a 2020 2343 6c6f 7564 7320 6172  ....  #Clouds ar
-000154b0: 6520 7265 6173 6f6e 6162 6c79 2062 7269  e reasonably bri
-000154c0: 6768 7420 696e 2061 6c6c 2069 6e66 7261  ght in all infra
-000154d0: 7265 6420 6261 6e64 732e 0d0a 2020 2320  red bands...  # 
-000154e0: 6972 5375 6d20 3d72 6573 6361 6c65 2869  irSum =rescale(i
-000154f0: 6d67 2c20 2769 6d67 2e6e 6972 202b 2069  mg, 'img.nir + i
-00015500: 6d67 2e73 7769 7232 272c 205b 302e 332c  mg.swir2', [0.3,
-00015510: 2030 2e37 5d29 0d0a 2020 6972 5375 6d20   0.7])..  irSum 
-00015520: 3d72 6573 6361 6c65 2869 6d67 2e73 656c  =rescale(img.sel
-00015530: 6563 7428 5b27 6e69 7227 2c27 7377 6972  ect(['nir','swir
-00015540: 3127 2c27 7377 6972 3227 5d29 2e72 6564  1','swir2']).red
-00015550: 7563 6528 6565 2e52 6564 7563 6572 2e73  uce(ee.Reducer.s
-00015560: 756d 2829 292c 205b 302e 332c 2030 2e38  um()), [0.3, 0.8
-00015570: 5d29 0d0a 2020 7363 6f72 6520 3d20 7363  ])..  score = sc
-00015580: 6f72 652e 6d69 6e28 6972 5375 6d29 0d0a  ore.min(irSum)..
-00015590: 0d0a 2020 2348 6f77 6576 6572 2c20 636c  ..  #However, cl
-000155a0: 6f75 6473 2061 7265 206e 6f74 2073 6e6f  ouds are not sno
-000155b0: 772e 0d0a 2020 6e64 7369 203d 2069 6d67  w...  ndsi = img
-000155c0: 2e6e 6f72 6d61 6c69 7a65 6444 6966 6665  .normalizedDiffe
-000155d0: 7265 6e63 6528 5b27 6772 6565 6e27 2c20  rence(['green', 
-000155e0: 2773 7769 7232 275d 290d 0a20 2073 6e6f  'swir2'])..  sno
-000155f0: 7753 636f 7265 203d 2072 6573 6361 6c65  wScore = rescale
-00015600: 286e 6473 692c 2020 5b30 2e38 2c20 302e  (ndsi,  [0.8, 0.
-00015610: 365d 290d 0a20 2073 636f 7265 203d 7363  6])..  score =sc
-00015620: 6f72 652e 6d69 6e28 736e 6f77 5363 6f72  ore.min(snowScor
-00015630: 6529 0d0a 0d0a 2020 2346 6f72 204d 4f44  e)....  #For MOD
-00015640: 4953 2c20 7072 6f76 6964 6520 7468 6520  IS, provide the 
-00015650: 6f70 7469 6f6e 206f 6620 6e6f 7420 7573  option of not us
-00015660: 696e 6720 7468 6572 6d61 6c20 7369 6e63  ing thermal sinc
-00015670: 6520 6974 2069 6e74 726f 6475 6365 730d  e it introduces.
-00015680: 0a20 2023 6120 7072 6563 6f6d 7075 7465  .  #a precompute
-00015690: 6420 6d61 736b 2074 6861 7420 6d61 7920  d mask that may 
-000156a0: 6f72 206d 6179 206e 6f74 2062 6520 7761  or may not be wa
-000156b0: 6e74 6564 0d0a 2020 6966 2075 7365 5465  nted..  if useTe
-000156c0: 6d70 496e 436c 6f75 644d 6173 6b3a 0d0a  mpInCloudMask:..
-000156d0: 2020 2020 2020 2343 6c6f 7564 7320 6172        #Clouds ar
-000156e0: 6520 7265 6173 6f6e 6162 6c79 2063 6f6f  e reasonably coo
-000156f0: 6c20 696e 2074 656d 7065 7261 7475 7265  l in temperature
-00015700: 2e0d 0a20 2020 2020 2023 2074 656d 7053  ...      # tempS
-00015710: 636f 7265 203d 2072 6573 6361 6c65 2869  core = rescale(i
-00015720: 6d67 2c20 2769 6d67 2e74 656d 7027 2c20  mg, 'img.temp', 
-00015730: 5b33 3035 2c20 3330 305d 290d 0a20 2020  [305, 300])..   
-00015740: 2020 2023 204d 6170 2e61 6464 4c61 7965     # Map.addLaye
-00015750: 7228 7465 6d70 5363 6f72 652c 7b7d 2c27  r(tempScore,{},'
-00015760: 7465 6d70 7363 6f72 6527 290d 0a20 2020  tempscore')..   
-00015770: 2020 2023 7363 6f72 6520 3d20 7363 6f72     #score = scor
-00015780: 652e 6d69 6e28 7465 6d70 5363 6f72 6529  e.min(tempScore)
-00015790: 0d0a 2020 2020 2020 7363 6f72 6520 3d20  ..      score = 
-000157a0: 7363 6f72 652e 7768 6572 6528 696d 672e  score.where(img.
-000157b0: 7365 6c65 6374 285b 2774 656d 7027 5d29  select(['temp'])
-000157c0: 2e6d 6173 6b28 292e 4e6f 7428 292c 3129  .mask().Not(),1)
-000157d0: 0d0a 0d0a 2020 7363 6f72 6520 3d20 7363  ....  score = sc
-000157e0: 6f72 652e 6d75 6c74 6970 6c79 2831 3030  ore.multiply(100
-000157f0: 290d 0a20 2073 636f 7265 203d 2073 636f  )..  score = sco
-00015800: 7265 2e63 6c61 6d70 2830 2c31 3030 292e  re.clamp(0,100).
-00015810: 6279 7465 2829 0d0a 0d0a 2020 7265 7475  byte()....  retu
-00015820: 726e 2073 636f 7265 2e72 656e 616d 6528  rn score.rename(
-00015830: 5b27 636c 6f75 6453 636f 7265 275d 293b  ['cloudScore']);
-00015840: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
+00015220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015230: 2323 0d0a 2353 6f75 7263 653a 2063 6f64  ##..#Source: cod
+00015240: 652e 6561 7274 6865 6e67 696e 652e 676f  e.earthengine.go
+00015250: 6f67 6c65 2e63 6f6d 0d0a 2343 6f6d 7075  ogle.com..#Compu
+00015260: 7465 2061 2063 6c6f 7564 2073 636f 7265  te a cloud score
+00015270: 2e20 2054 6869 7320 6578 7065 6374 7320  .  This expects 
+00015280: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
+00015290: 746f 2068 6176 6520 7468 6520 636f 6d6d  to have the comm
+000152a0: 6f6e 0d0a 2362 616e 6420 6e61 6d65 733a  on..#band names:
+000152b0: 205b 2272 6564 222c 2022 626c 7565 222c   ["red", "blue",
+000152c0: 2065 7463 5d2c 2073 6f20 6974 2063 616e   etc], so it can
+000152d0: 2077 6f72 6b20 6163 726f 7373 2073 656e   work across sen
+000152e0: 736f 7273 2e0d 0a64 6566 206d 6f64 6973  sors...def modis
+000152f0: 436c 6f75 6453 636f 7265 2869 6d67 293a  CloudScore(img):
+00015300: 0d0a 0d0a 2020 7573 6554 656d 7049 6e43  ....  useTempInC
+00015310: 6c6f 7564 4d61 736b 203d 2054 7275 650d  loudMask = True.
+00015320: 0a20 2023 436f 6d70 7574 6520 7365 7665  .  #Compute seve
+00015330: 7261 6c20 696e 6469 6361 746f 7273 206f  ral indicators o
+00015340: 6620 636c 6f75 6479 6e65 7373 2061 6e64  f cloudyness and
+00015350: 2074 616b 6520 7468 6520 6d69 6e69 6d75   take the minimu
+00015360: 6d20 6f66 2074 6865 6d2e 0d0a 2020 7363  m of them...  sc
+00015370: 6f72 6520 3d20 6565 2e49 6d61 6765 2831  ore = ee.Image(1
+00015380: 2e30 293b 0d0a 0d0a 2020 2343 6c6f 7564  .0);....  #Cloud
+00015390: 7320 6172 6520 7265 6173 6f6e 6162 6c79  s are reasonably
+000153a0: 2062 7269 6768 7420 696e 2074 6865 2062   bright in the b
+000153b0: 6c75 6520 6261 6e64 2e0d 0a20 2023 2073  lue band...  # s
+000153c0: 636f 7265 203d 2073 636f 7265 2e6d 696e  core = score.min
+000153d0: 2872 6573 6361 6c65 2869 6d67 2c20 2769  (rescale(img, 'i
+000153e0: 6d67 2e62 6c75 6527 2c20 5b30 2e31 2c20  mg.blue', [0.1, 
+000153f0: 302e 335d 2929 0d0a 2020 2343 6c6f 7564  0.3]))..  #Cloud
+00015400: 7320 6172 6520 7265 6173 6f6e 6162 6c79  s are reasonably
+00015410: 2062 7269 6768 7420 696e 2061 6c6c 2076   bright in all v
+00015420: 6973 6962 6c65 2062 616e 6473 2e0d 0a20  isible bands... 
+00015430: 2076 697a 5375 6d20 3d20 7265 7363 616c   vizSum = rescal
+00015440: 6528 696d 672e 7365 6c65 6374 285b 2772  e(img.select(['r
+00015450: 6564 272c 2767 7265 656e 272c 2762 6c75  ed','green','blu
+00015460: 6527 5d29 2e72 6564 7563 6528 6565 2e52  e']).reduce(ee.R
+00015470: 6564 7563 6572 2e73 756d 2829 292c 205b  educer.sum()), [
+00015480: 302e 322c 2030 2e38 5d29 0d0a 2020 7363  0.2, 0.8])..  sc
+00015490: 6f72 6520 3d20 7363 6f72 652e 6d69 6e28  ore = score.min(
+000154a0: 7669 7a53 756d 290d 0a0d 0a20 2023 436c  vizSum)....  #Cl
+000154b0: 6f75 6473 2061 7265 2072 6561 736f 6e61  ouds are reasona
+000154c0: 626c 7920 6272 6967 6874 2069 6e20 616c  bly bright in al
+000154d0: 6c20 696e 6672 6172 6564 2062 616e 6473  l infrared bands
+000154e0: 2e0d 0a20 2023 2069 7253 756d 203d 7265  ...  # irSum =re
+000154f0: 7363 616c 6528 696d 672c 2027 696d 672e  scale(img, 'img.
+00015500: 6e69 7220 2b20 696d 672e 7377 6972 3227  nir + img.swir2'
+00015510: 2c20 5b30 2e33 2c20 302e 375d 290d 0a20  , [0.3, 0.7]).. 
+00015520: 2069 7253 756d 203d 7265 7363 616c 6528   irSum =rescale(
+00015530: 696d 672e 7365 6c65 6374 285b 276e 6972  img.select(['nir
+00015540: 272c 2773 7769 7231 272c 2773 7769 7232  ','swir1','swir2
+00015550: 275d 292e 7265 6475 6365 2865 652e 5265  ']).reduce(ee.Re
+00015560: 6475 6365 722e 7375 6d28 2929 2c20 5b30  ducer.sum()), [0
+00015570: 2e33 2c20 302e 385d 290d 0a20 2073 636f  .3, 0.8])..  sco
+00015580: 7265 203d 2073 636f 7265 2e6d 696e 2869  re = score.min(i
+00015590: 7253 756d 290d 0a0d 0a20 2023 486f 7765  rSum)....  #Howe
+000155a0: 7665 722c 2063 6c6f 7564 7320 6172 6520  ver, clouds are 
+000155b0: 6e6f 7420 736e 6f77 2e0d 0a20 206e 6473  not snow...  nds
+000155c0: 6920 3d20 696d 672e 6e6f 726d 616c 697a  i = img.normaliz
+000155d0: 6564 4469 6666 6572 656e 6365 285b 2767  edDifference(['g
+000155e0: 7265 656e 272c 2027 7377 6972 3227 5d29  reen', 'swir2'])
+000155f0: 0d0a 2020 736e 6f77 5363 6f72 6520 3d20  ..  snowScore = 
+00015600: 7265 7363 616c 6528 6e64 7369 2c20 205b  rescale(ndsi,  [
+00015610: 302e 382c 2030 2e36 5d29 0d0a 2020 7363  0.8, 0.6])..  sc
+00015620: 6f72 6520 3d73 636f 7265 2e6d 696e 2873  ore =score.min(s
+00015630: 6e6f 7753 636f 7265 290d 0a0d 0a20 2023  nowScore)....  #
+00015640: 466f 7220 4d4f 4449 532c 2070 726f 7669  For MODIS, provi
+00015650: 6465 2074 6865 206f 7074 696f 6e20 6f66  de the option of
+00015660: 206e 6f74 2075 7369 6e67 2074 6865 726d   not using therm
+00015670: 616c 2073 696e 6365 2069 7420 696e 7472  al since it intr
+00015680: 6f64 7563 6573 0d0a 2020 2361 2070 7265  oduces..  #a pre
+00015690: 636f 6d70 7574 6564 206d 6173 6b20 7468  computed mask th
+000156a0: 6174 206d 6179 206f 7220 6d61 7920 6e6f  at may or may no
+000156b0: 7420 6265 2077 616e 7465 640d 0a20 2069  t be wanted..  i
+000156c0: 6620 7573 6554 656d 7049 6e43 6c6f 7564  f useTempInCloud
+000156d0: 4d61 736b 3a0d 0a20 2020 2020 2023 436c  Mask:..      #Cl
+000156e0: 6f75 6473 2061 7265 2072 6561 736f 6e61  ouds are reasona
+000156f0: 626c 7920 636f 6f6c 2069 6e20 7465 6d70  bly cool in temp
+00015700: 6572 6174 7572 652e 0d0a 2020 2020 2020  erature...      
+00015710: 2320 7465 6d70 5363 6f72 6520 3d20 7265  # tempScore = re
+00015720: 7363 616c 6528 696d 672c 2027 696d 672e  scale(img, 'img.
+00015730: 7465 6d70 272c 205b 3330 352c 2033 3030  temp', [305, 300
+00015740: 5d29 0d0a 2020 2020 2020 2320 4d61 702e  ])..      # Map.
+00015750: 6164 644c 6179 6572 2874 656d 7053 636f  addLayer(tempSco
+00015760: 7265 2c7b 7d2c 2774 656d 7073 636f 7265  re,{},'tempscore
+00015770: 2729 0d0a 2020 2020 2020 2373 636f 7265  ')..      #score
+00015780: 203d 2073 636f 7265 2e6d 696e 2874 656d   = score.min(tem
+00015790: 7053 636f 7265 290d 0a20 2020 2020 2073  pScore)..      s
+000157a0: 636f 7265 203d 2073 636f 7265 2e77 6865  core = score.whe
+000157b0: 7265 2869 6d67 2e73 656c 6563 7428 5b27  re(img.select(['
+000157c0: 7465 6d70 275d 292e 6d61 736b 2829 2e4e  temp']).mask().N
+000157d0: 6f74 2829 2c31 290d 0a0d 0a20 2073 636f  ot(),1)....  sco
+000157e0: 7265 203d 2073 636f 7265 2e6d 756c 7469  re = score.multi
+000157f0: 706c 7928 3130 3029 0d0a 2020 7363 6f72  ply(100)..  scor
+00015800: 6520 3d20 7363 6f72 652e 636c 616d 7028  e = score.clamp(
+00015810: 302c 3130 3029 2e62 7974 6528 290d 0a0d  0,100).byte()...
+00015820: 0a20 2072 6574 7572 6e20 7363 6f72 652e  .  return score.
+00015830: 7265 6e61 6d65 285b 2763 6c6f 7564 5363  rename(['cloudSc
+00015840: 6f72 6527 5d29 3b0d 0a0d 0a23 2323 2323  ore']);....#####
 00015850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015880: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-00015890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015890: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
 000158a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000158b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000158c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000158d0: 2323 2323 2323 2323 0d0a 2343 6c6f 7564  ########..#Cloud
-000158e0: 206d 6173 6b69 6e67 2061 6c67 6f72 6974   masking algorit
-000158f0: 686d 2066 6f72 2053 656e 7469 6e65 6c32  hm for Sentinel2
-00015900: 0d0a 2342 7569 6c74 206f 6e20 6964 6561  ..#Built on idea
-00015910: 7320 6672 6f6d 204c 616e 6473 6174 2063  s from Landsat c
-00015920: 6c6f 7564 5363 6f72 6520 616c 676f 7269  loudScore algori
-00015930: 7468 6d0d 0a23 4375 7272 656e 746c 7920  thm..#Currently 
-00015940: 696e 2062 6574 6120 616e 6420 6d61 7920  in beta and may 
-00015950: 6e65 6564 2074 7765 616b 696e 6720 666f  need tweaking fo
-00015960: 7220 696e 6469 7669 6475 616c 2073 7475  r individual stu
-00015970: 6479 2061 7265 6173 0d0a 6465 6620 7365  dy areas..def se
-00015980: 6e74 696e 656c 3243 6c6f 7564 5363 6f72  ntinel2CloudScor
-00015990: 6528 696d 6729 3a0d 0a20 2023 436f 6d70  e(img):..  #Comp
-000159a0: 7574 6520 7365 7665 7261 6c20 696e 6469  ute several indi
-000159b0: 6361 746f 7273 206f 6620 636c 6f75 6479  cators of cloudy
-000159c0: 6e65 7373 2061 6e64 2074 616b 6520 7468  ness and take th
-000159d0: 6520 6d69 6e69 6d75 6d20 6f66 2074 6865  e minimum of the
-000159e0: 6d2e 0d0a 2020 7363 6f72 6520 3d20 6565  m...  score = ee
-000159f0: 2e49 6d61 6765 2831 290d 0a20 2062 6c75  .Image(1)..  blu
-00015a00: 6543 6972 7275 7353 636f 7265 203d 2065  eCirrusScore = e
-00015a10: 652e 496d 6167 6528 3029 0d0a 0d0a 2020  e.Image(0)....  
-00015a20: 2343 6c6f 7564 7320 6172 6520 7265 6173  #Clouds are reas
-00015a30: 6f6e 6162 6c79 2062 7269 6768 7420 696e  onably bright in
-00015a40: 2074 6865 2062 6c75 6520 6f72 2063 6972   the blue or cir
-00015a50: 7275 7320 6261 6e64 732e 0d0a 2020 2355  rus bands...  #U
-00015a60: 7365 202e 6d61 7820 6173 2061 2070 7365  se .max as a pse
-00015a70: 7564 6f20 4f52 2063 6f6e 6469 7469 6f6e  udo OR condition
-00015a80: 616c 0d0a 2020 626c 7565 4369 7272 7573  al..  blueCirrus
-00015a90: 5363 6f72 6520 3d20 626c 7565 4369 7272  Score = blueCirr
-00015aa0: 7573 5363 6f72 652e 6d61 7828 7265 7363  usScore.max(resc
-00015ab0: 616c 6528 696d 672e 7365 6c65 6374 285b  ale(img.select([
-00015ac0: 2762 6c75 6527 5d29 2c20 5b30 2e31 2c20  'blue']), [0.1, 
-00015ad0: 302e 355d 2929 0d0a 2020 626c 7565 4369  0.5]))..  blueCi
-00015ae0: 7272 7573 5363 6f72 6520 3d20 626c 7565  rrusScore = blue
-00015af0: 4369 7272 7573 5363 6f72 652e 6d61 7828  CirrusScore.max(
-00015b00: 7265 7363 616c 6528 696d 672e 7365 6c65  rescale(img.sele
-00015b10: 6374 285b 2763 6227 5d29 2c20 5b30 2e31  ct(['cb']), [0.1
-00015b20: 2c20 302e 355d 2929 0d0a 2020 2320 626c  , 0.5]))..  # bl
-00015b30: 7565 4369 7272 7573 5363 6f72 6520 3d20  ueCirrusScore = 
-00015b40: 626c 7565 4369 7272 7573 5363 6f72 652e  blueCirrusScore.
-00015b50: 6d61 7828 7265 7363 616c 6528 696d 672c  max(rescale(img,
-00015b60: 2027 696d 672e 6369 7272 7573 272c 205b   'img.cirrus', [
-00015b70: 302e 312c 2030 2e33 5d29 290d 0a0d 0a20  0.1, 0.3])).... 
-00015b80: 2023 7265 5375 6d20 3d20 7265 7363 616c   #reSum = rescal
-00015b90: 6528 696d 672c 2728 696d 672e 7265 312b  e(img,'(img.re1+
-00015ba0: 696d 672e 7265 322b 696d 672e 7265 3329  img.re2+img.re3)
-00015bb0: 2f33 272c 5b30 2e35 2c20 302e 375d 290d  /3',[0.5, 0.7]).
-00015bc0: 0a0d 0a20 2073 636f 7265 203d 2073 636f  ...  score = sco
-00015bd0: 7265 2e6d 696e 2862 6c75 6543 6972 7275  re.min(blueCirru
-00015be0: 7353 636f 7265 290d 0a0d 0a20 2023 436c  sScore)....  #Cl
-00015bf0: 6f75 6473 2061 7265 2072 6561 736f 6e61  ouds are reasona
-00015c00: 626c 7920 6272 6967 6874 2069 6e20 616c  bly bright in al
-00015c10: 6c20 7669 7369 626c 6520 6261 6e64 732e  l visible bands.
-00015c20: 0d0a 2020 7363 6f72 6520 3d20 7363 6f72  ..  score = scor
-00015c30: 652e 6d69 6e28 7265 7363 616c 6528 696d  e.min(rescale(im
-00015c40: 672e 7365 6c65 6374 285b 2772 6564 272c  g.select(['red',
-00015c50: 2767 7265 656e 272c 2762 6c75 6527 5d29  'green','blue'])
-00015c60: 2e72 6564 7563 6528 6565 2e52 6564 7563  .reduce(ee.Reduc
-00015c70: 6572 2e73 756d 2829 292c 205b 302e 322c  er.sum()), [0.2,
-00015c80: 2030 2e38 5d29 290d 0a0d 0a20 2023 436c   0.8]))....  #Cl
-00015c90: 6f75 6473 2061 7265 2072 6561 736f 6e61  ouds are reasona
-00015ca0: 626c 7920 6272 6967 6874 2069 6e20 616c  bly bright in al
-00015cb0: 6c20 696e 6672 6172 6564 2062 616e 6473  l infrared bands
-00015cc0: 2e0d 0a20 2073 636f 7265 203d 2073 636f  ...  score = sco
-00015cd0: 7265 2e6d 696e 2872 6573 6361 6c65 2869  re.min(rescale(i
-00015ce0: 6d67 2e73 656c 6563 7428 5b27 6e69 7227  mg.select(['nir'
-00015cf0: 2c27 7377 6972 3127 2c27 7377 6972 3227  ,'swir1','swir2'
-00015d00: 5d29 2e72 6564 7563 6528 6565 2e52 6564  ]).reduce(ee.Red
-00015d10: 7563 6572 2e73 756d 2829 292c 205b 302e  ucer.sum()), [0.
-00015d20: 332c 2030 2e38 5d29 290d 0a0d 0a20 2023  3, 0.8]))....  #
-00015d30: 486f 7765 7665 722c 2063 6c6f 7564 7320  However, clouds 
-00015d40: 6172 6520 6e6f 7420 736e 6f77 2e0d 0a20  are not snow... 
-00015d50: 206e 6473 6920 3d20 2069 6d67 2e6e 6f72   ndsi =  img.nor
-00015d60: 6d61 6c69 7a65 6444 6966 6665 7265 6e63  malizedDifferenc
-00015d70: 6528 5b27 6772 6565 6e27 2c20 2773 7769  e(['green', 'swi
-00015d80: 7231 275d 290d 0a20 2073 636f 7265 3d73  r1'])..  score=s
-00015d90: 636f 7265 2e6d 696e 2872 6573 6361 6c65  core.min(rescale
-00015da0: 286e 6473 692c 205b 302e 382c 2030 2e36  (ndsi, [0.8, 0.6
-00015db0: 5d29 290d 0a0d 0a20 2073 636f 7265 203d  ]))....  score =
-00015dc0: 2073 636f 7265 2e6d 756c 7469 706c 7928   score.multiply(
-00015dd0: 3130 3029 2e62 7974 6528 292e 636c 616d  100).byte().clam
-00015de0: 7028 302c 3130 3029 2e72 656e 616d 6528  p(0,100).rename(
-00015df0: 5b27 636c 6f75 6453 636f 7265 275d 290d  ['cloudScore']).
-00015e00: 0a20 2072 6574 7572 6e20 7363 6f72 650d  .  return score.
-00015e10: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+000158d0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+000158e0: 0a23 436c 6f75 6420 6d61 736b 696e 6720  .#Cloud masking 
+000158f0: 616c 676f 7269 7468 6d20 666f 7220 5365  algorithm for Se
+00015900: 6e74 696e 656c 320d 0a23 4275 696c 7420  ntinel2..#Built 
+00015910: 6f6e 2069 6465 6173 2066 726f 6d20 4c61  on ideas from La
+00015920: 6e64 7361 7420 636c 6f75 6453 636f 7265  ndsat cloudScore
+00015930: 2061 6c67 6f72 6974 686d 0d0a 2343 7572   algorithm..#Cur
+00015940: 7265 6e74 6c79 2069 6e20 6265 7461 2061  rently in beta a
+00015950: 6e64 206d 6179 206e 6565 6420 7477 6561  nd may need twea
+00015960: 6b69 6e67 2066 6f72 2069 6e64 6976 6964  king for individ
+00015970: 7561 6c20 7374 7564 7920 6172 6561 730d  ual study areas.
+00015980: 0a64 6566 2073 656e 7469 6e65 6c32 436c  .def sentinel2Cl
+00015990: 6f75 6453 636f 7265 2869 6d67 293a 0d0a  oudScore(img):..
+000159a0: 2020 2343 6f6d 7075 7465 2073 6576 6572    #Compute sever
+000159b0: 616c 2069 6e64 6963 6174 6f72 7320 6f66  al indicators of
+000159c0: 2063 6c6f 7564 796e 6573 7320 616e 6420   cloudyness and 
+000159d0: 7461 6b65 2074 6865 206d 696e 696d 756d  take the minimum
+000159e0: 206f 6620 7468 656d 2e0d 0a20 2073 636f   of them...  sco
+000159f0: 7265 203d 2065 652e 496d 6167 6528 3129  re = ee.Image(1)
+00015a00: 0d0a 2020 626c 7565 4369 7272 7573 5363  ..  blueCirrusSc
+00015a10: 6f72 6520 3d20 6565 2e49 6d61 6765 2830  ore = ee.Image(0
+00015a20: 290d 0a0d 0a20 2023 436c 6f75 6473 2061  )....  #Clouds a
+00015a30: 7265 2072 6561 736f 6e61 626c 7920 6272  re reasonably br
+00015a40: 6967 6874 2069 6e20 7468 6520 626c 7565  ight in the blue
+00015a50: 206f 7220 6369 7272 7573 2062 616e 6473   or cirrus bands
+00015a60: 2e0d 0a20 2023 5573 6520 2e6d 6178 2061  ...  #Use .max a
+00015a70: 7320 6120 7073 6575 646f 204f 5220 636f  s a pseudo OR co
+00015a80: 6e64 6974 696f 6e61 6c0d 0a20 2062 6c75  nditional..  blu
+00015a90: 6543 6972 7275 7353 636f 7265 203d 2062  eCirrusScore = b
+00015aa0: 6c75 6543 6972 7275 7353 636f 7265 2e6d  lueCirrusScore.m
+00015ab0: 6178 2872 6573 6361 6c65 2869 6d67 2e73  ax(rescale(img.s
+00015ac0: 656c 6563 7428 5b27 626c 7565 275d 292c  elect(['blue']),
+00015ad0: 205b 302e 312c 2030 2e35 5d29 290d 0a20   [0.1, 0.5])).. 
+00015ae0: 2062 6c75 6543 6972 7275 7353 636f 7265   blueCirrusScore
+00015af0: 203d 2062 6c75 6543 6972 7275 7353 636f   = blueCirrusSco
+00015b00: 7265 2e6d 6178 2872 6573 6361 6c65 2869  re.max(rescale(i
+00015b10: 6d67 2e73 656c 6563 7428 5b27 6362 275d  mg.select(['cb']
+00015b20: 292c 205b 302e 312c 2030 2e35 5d29 290d  ), [0.1, 0.5])).
+00015b30: 0a20 2023 2062 6c75 6543 6972 7275 7353  .  # blueCirrusS
+00015b40: 636f 7265 203d 2062 6c75 6543 6972 7275  core = blueCirru
+00015b50: 7353 636f 7265 2e6d 6178 2872 6573 6361  sScore.max(resca
+00015b60: 6c65 2869 6d67 2c20 2769 6d67 2e63 6972  le(img, 'img.cir
+00015b70: 7275 7327 2c20 5b30 2e31 2c20 302e 335d  rus', [0.1, 0.3]
+00015b80: 2929 0d0a 0d0a 2020 2372 6553 756d 203d  ))....  #reSum =
+00015b90: 2072 6573 6361 6c65 2869 6d67 2c27 2869   rescale(img,'(i
+00015ba0: 6d67 2e72 6531 2b69 6d67 2e72 6532 2b69  mg.re1+img.re2+i
+00015bb0: 6d67 2e72 6533 292f 3327 2c5b 302e 352c  mg.re3)/3',[0.5,
+00015bc0: 2030 2e37 5d29 0d0a 0d0a 2020 7363 6f72   0.7])....  scor
+00015bd0: 6520 3d20 7363 6f72 652e 6d69 6e28 626c  e = score.min(bl
+00015be0: 7565 4369 7272 7573 5363 6f72 6529 0d0a  ueCirrusScore)..
+00015bf0: 0d0a 2020 2343 6c6f 7564 7320 6172 6520  ..  #Clouds are 
+00015c00: 7265 6173 6f6e 6162 6c79 2062 7269 6768  reasonably brigh
+00015c10: 7420 696e 2061 6c6c 2076 6973 6962 6c65  t in all visible
+00015c20: 2062 616e 6473 2e0d 0a20 2073 636f 7265   bands...  score
+00015c30: 203d 2073 636f 7265 2e6d 696e 2872 6573   = score.min(res
+00015c40: 6361 6c65 2869 6d67 2e73 656c 6563 7428  cale(img.select(
+00015c50: 5b27 7265 6427 2c27 6772 6565 6e27 2c27  ['red','green','
+00015c60: 626c 7565 275d 292e 7265 6475 6365 2865  blue']).reduce(e
+00015c70: 652e 5265 6475 6365 722e 7375 6d28 2929  e.Reducer.sum())
+00015c80: 2c20 5b30 2e32 2c20 302e 385d 2929 0d0a  , [0.2, 0.8]))..
+00015c90: 0d0a 2020 2343 6c6f 7564 7320 6172 6520  ..  #Clouds are 
+00015ca0: 7265 6173 6f6e 6162 6c79 2062 7269 6768  reasonably brigh
+00015cb0: 7420 696e 2061 6c6c 2069 6e66 7261 7265  t in all infrare
+00015cc0: 6420 6261 6e64 732e 0d0a 2020 7363 6f72  d bands...  scor
+00015cd0: 6520 3d20 7363 6f72 652e 6d69 6e28 7265  e = score.min(re
+00015ce0: 7363 616c 6528 696d 672e 7365 6c65 6374  scale(img.select
+00015cf0: 285b 276e 6972 272c 2773 7769 7231 272c  (['nir','swir1',
+00015d00: 2773 7769 7232 275d 292e 7265 6475 6365  'swir2']).reduce
+00015d10: 2865 652e 5265 6475 6365 722e 7375 6d28  (ee.Reducer.sum(
+00015d20: 2929 2c20 5b30 2e33 2c20 302e 385d 2929  )), [0.3, 0.8]))
+00015d30: 0d0a 0d0a 2020 2348 6f77 6576 6572 2c20  ....  #However, 
+00015d40: 636c 6f75 6473 2061 7265 206e 6f74 2073  clouds are not s
+00015d50: 6e6f 772e 0d0a 2020 6e64 7369 203d 2020  now...  ndsi =  
+00015d60: 696d 672e 6e6f 726d 616c 697a 6564 4469  img.normalizedDi
+00015d70: 6666 6572 656e 6365 285b 2767 7265 656e  fference(['green
+00015d80: 272c 2027 7377 6972 3127 5d29 0d0a 2020  ', 'swir1'])..  
+00015d90: 7363 6f72 653d 7363 6f72 652e 6d69 6e28  score=score.min(
+00015da0: 7265 7363 616c 6528 6e64 7369 2c20 5b30  rescale(ndsi, [0
+00015db0: 2e38 2c20 302e 365d 2929 0d0a 0d0a 2020  .8, 0.6]))....  
+00015dc0: 7363 6f72 6520 3d20 7363 6f72 652e 6d75  score = score.mu
+00015dd0: 6c74 6970 6c79 2831 3030 292e 6279 7465  ltiply(100).byte
+00015de0: 2829 2e63 6c61 6d70 2830 2c31 3030 292e  ().clamp(0,100).
+00015df0: 7265 6e61 6d65 285b 2763 6c6f 7564 5363  rename(['cloudSc
+00015e00: 6f72 6527 5d29 0d0a 2020 7265 7475 726e  ore'])..  return
+00015e10: 2073 636f 7265 0d0a 2323 2323 2323 2323   score..########
 00015e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015e30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015e40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015e50: 2323 2323 2323 2323 2323 0d0a 2341 6461  ##########..#Ada
-00015e60: 7074 6564 2066 726f 6d3a 2068 7474 7073  pted from: https
-00015e70: 3a2f 2f65 6172 7468 2e65 7361 2e69 6e74  ://earth.esa.int
-00015e80: 2f64 6f63 756d 656e 7473 2f31 3031 3734  /documents/10174
-00015e90: 2f33 3136 3630 3038 2f45 5341 5f54 7261  /3166008/ESA_Tra
-00015ea0: 696e 696e 675f 5669 6c6e 6975 735f 3037  ining_Vilnius_07
-00015eb0: 3037 3230 3137 5f53 4152 5f4f 7074 6963  072017_SAR_Optic
-00015ec0: 616c 5f53 6e6f 775f 4963 655f 4578 6572  al_Snow_Ice_Exer
-00015ed0: 6369 7365 732e 7064 660d 0a64 6566 2073  cises.pdf..def s
-00015ee0: 656e 7469 6e65 6c32 536e 6f77 4d61 736b  entinel2SnowMask
-00015ef0: 2869 6d67 2c64 696c 6174 6550 6978 656c  (img,dilatePixel
-00015f00: 7320 3d20 332e 3529 3a0d 0a20 206e 6473  s = 3.5):..  nds
-00015f10: 6920 3d20 2069 6d67 2e6e 6f72 6d61 6c69  i =  img.normali
-00015f20: 7a65 6444 6966 6665 7265 6e63 6528 5b27  zedDifference(['
-00015f30: 6772 6565 6e27 2c20 2773 7769 7231 275d  green', 'swir1']
-00015f40: 290d 0a0d 0a20 2023 4946 204e 4453 4920  )....  #IF NDSI 
-00015f50: 3e20 302e 3430 2041 4e44 20cf 8128 4e49  > 0.40 AND ..(NI
-00015f60: 5229 203e 2030 2e31 3120 5448 454e 2073  R) > 0.11 THEN s
-00015f70: 6e6f 7720 696e 206f 7065 6e20 6c61 6e64  now in open land
-00015f80: 0d0a 2020 2349 4620 302e 3120 3c20 4e44  ..  #IF 0.1 < ND
-00015f90: 5349 203c 2030 2e34 2054 4845 4e20 736e  SI < 0.4 THEN sn
-00015fa0: 6f77 2069 6e20 666f 7265 7374 0d0a 2020  ow in forest..  
-00015fb0: 736e 6f77 4f70 656e 4c61 6e64 203d 206e  snowOpenLand = n
-00015fc0: 6473 692e 6774 2830 2e34 292e 416e 6428  dsi.gt(0.4).And(
-00015fd0: 696d 672e 7365 6c65 6374 285b 276e 6972  img.select(['nir
-00015fe0: 275d 292e 6774 2830 2e31 3129 290d 0a20  ']).gt(0.11)).. 
-00015ff0: 2073 6e6f 7746 6f72 6573 7420 3d20 6e64   snowForest = nd
-00016000: 7369 2e67 7428 302e 3129 2e41 6e64 286e  si.gt(0.1).And(n
-00016010: 6473 692e 6c74 2830 2e34 2929 0d0a 0d0a  dsi.lt(0.4))....
-00016020: 2020 2320 4d61 702e 6164 644c 6179 6572    # Map.addLayer
-00016030: 2873 6e6f 774f 7065 6e4c 616e 642e 7365  (snowOpenLand.se
-00016040: 6c66 4d61 736b 2829 2c7b 276d 696e 273a  lfMask(),{'min':
-00016050: 312c 276d 6178 273a 312c 2770 616c 6574  1,'max':1,'palet
-00016060: 7465 273a 2738 3846 277d 2c27 536e 6f77  te':'88F'},'Snow
-00016070: 204f 7065 6e20 4c61 6e64 2729 0d0a 2020   Open Land')..  
-00016080: 2320 4d61 702e 6164 644c 6179 6572 2873  # Map.addLayer(s
-00016090: 6e6f 7746 6f72 6573 742e 7365 6c66 4d61  nowForest.selfMa
-000160a0: 736b 2829 2c7b 276d 696e 273a 312c 276d  sk(),{'min':1,'m
-000160b0: 6178 273a 312c 2770 616c 6574 7465 273a  ax':1,'palette':
-000160c0: 2730 3046 277d 2c27 536e 6f77 2046 6f72  '00F'},'Snow For
-000160d0: 6573 7427 290d 0a20 2023 4672 6163 7469  est')..  #Fracti
-000160e0: 6f6e 616c 2073 6e6f 7720 636f 7665 7220  onal snow cover 
-000160f0: 2846 5343 2c20 3020 2520 2d20 3130 3025  (FSC, 0 % - 100%
-00016100: 2073 6e6f 7729 2063 616e 2062 6520 6465   snow) can be de
-00016110: 7465 6374 6564 2062 7920 7468 6520 6170  tected by the ap
-00016120: 7072 6f61 6368 206f 6620 5361 6c6f 6d6f  proach of Salomo
-00016130: 6e73 6f6e 0d0a 2020 2361 6e64 2041 7070  nson..  #and App
-00016140: 656c 2028 3230 3034 2c20 3230 3036 292c  el (2004, 2006),
-00016150: 2077 6869 6368 2077 6173 206f 7269 6769   which was origi
-00016160: 6e61 6c6c 7920 6465 7665 6c6f 7065 6420  nally developed 
-00016170: 666f 7220 4d4f 4449 5320 6461 7461 3a0d  for MODIS data:.
-00016180: 0a20 2023 4653 4320 3d20 e280 9330 2e30  .  #FSC = ...0.0
-00016190: 3120 2b20 312e 3435 202a 204e 4453 490d  1 + 1.45 * NDSI.
-000161a0: 0a20 2066 7363 203d 206e 6473 692e 6d75  .  fsc = ndsi.mu
-000161b0: 6c74 6970 6c79 2831 2e34 3529 2e73 7562  ltiply(1.45).sub
-000161c0: 7472 6163 7428 302e 3031 290d 0a20 2023  tract(0.01)..  #
-000161d0: 204d 6170 2e61 6464 4c61 7965 7228 6673   Map.addLayer(fs
-000161e0: 632c 7b27 6d69 6e27 3a30 2c27 6d61 7827  c,{'min':0,'max'
-000161f0: 3a31 2c27 7061 6c65 7474 6527 3a27 3038  :1,'palette':'08
-00016200: 302c 3030 3827 7d2c 2746 7261 6374 696f  0,008'},'Fractio
-00016210: 6e61 6c20 536e 6f77 2043 6f76 6572 2729  nal Snow Cover')
-00016220: 0d0a 2020 736e 6f77 4d61 736b 203d 2028  ..  snowMask = (
-00016230: 2873 6e6f 774f 7065 6e4c 616e 642e 4f72  (snowOpenLand.Or
-00016240: 2873 6e6f 7746 6f72 6573 7429 292e 4e6f  (snowForest)).No
-00016250: 7428 2929 2e66 6f63 616c 5f6d 696e 2864  t()).focal_min(d
-00016260: 696c 6174 6550 6978 656c 7329 0d0a 2020  ilatePixels)..  
-00016270: 7265 7475 726e 2069 6d67 2e75 7064 6174  return img.updat
-00016280: 654d 6173 6b28 736e 6f77 4d61 736b 290d  eMask(snowMask).
-00016290: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00015e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015e60: 230d 0a23 4164 6170 7465 6420 6672 6f6d  #..#Adapted from
+00015e70: 3a20 6874 7470 733a 2f2f 6561 7274 682e  : https://earth.
+00015e80: 6573 612e 696e 742f 646f 6375 6d65 6e74  esa.int/document
+00015e90: 732f 3130 3137 342f 3331 3636 3030 382f  s/10174/3166008/
+00015ea0: 4553 415f 5472 6169 6e69 6e67 5f56 696c  ESA_Training_Vil
+00015eb0: 6e69 7573 5f30 3730 3732 3031 375f 5341  nius_07072017_SA
+00015ec0: 525f 4f70 7469 6361 6c5f 536e 6f77 5f49  R_Optical_Snow_I
+00015ed0: 6365 5f45 7865 7263 6973 6573 2e70 6466  ce_Exercises.pdf
+00015ee0: 0d0a 6465 6620 7365 6e74 696e 656c 3253  ..def sentinel2S
+00015ef0: 6e6f 774d 6173 6b28 696d 672c 6469 6c61  nowMask(img,dila
+00015f00: 7465 5069 7865 6c73 203d 2033 2e35 293a  tePixels = 3.5):
+00015f10: 0d0a 2020 6e64 7369 203d 2020 696d 672e  ..  ndsi =  img.
+00015f20: 6e6f 726d 616c 697a 6564 4469 6666 6572  normalizedDiffer
+00015f30: 656e 6365 285b 2767 7265 656e 272c 2027  ence(['green', '
+00015f40: 7377 6972 3127 5d29 0d0a 0d0a 2020 2349  swir1'])....  #I
+00015f50: 4620 4e44 5349 203e 2030 2e34 3020 414e  F NDSI > 0.40 AN
+00015f60: 4420 cf81 284e 4952 2920 3e20 302e 3131  D ..(NIR) > 0.11
+00015f70: 2054 4845 4e20 736e 6f77 2069 6e20 6f70   THEN snow in op
+00015f80: 656e 206c 616e 640d 0a20 2023 4946 2030  en land..  #IF 0
+00015f90: 2e31 203c 204e 4453 4920 3c20 302e 3420  .1 < NDSI < 0.4 
+00015fa0: 5448 454e 2073 6e6f 7720 696e 2066 6f72  THEN snow in for
+00015fb0: 6573 740d 0a20 2073 6e6f 774f 7065 6e4c  est..  snowOpenL
+00015fc0: 616e 6420 3d20 6e64 7369 2e67 7428 302e  and = ndsi.gt(0.
+00015fd0: 3429 2e41 6e64 2869 6d67 2e73 656c 6563  4).And(img.selec
+00015fe0: 7428 5b27 6e69 7227 5d29 2e67 7428 302e  t(['nir']).gt(0.
+00015ff0: 3131 2929 0d0a 2020 736e 6f77 466f 7265  11))..  snowFore
+00016000: 7374 203d 206e 6473 692e 6774 2830 2e31  st = ndsi.gt(0.1
+00016010: 292e 416e 6428 6e64 7369 2e6c 7428 302e  ).And(ndsi.lt(0.
+00016020: 3429 290d 0a0d 0a20 2023 204d 6170 2e61  4))....  # Map.a
+00016030: 6464 4c61 7965 7228 736e 6f77 4f70 656e  ddLayer(snowOpen
+00016040: 4c61 6e64 2e73 656c 664d 6173 6b28 292c  Land.selfMask(),
+00016050: 7b27 6d69 6e27 3a31 2c27 6d61 7827 3a31  {'min':1,'max':1
+00016060: 2c27 7061 6c65 7474 6527 3a27 3838 4627  ,'palette':'88F'
+00016070: 7d2c 2753 6e6f 7720 4f70 656e 204c 616e  },'Snow Open Lan
+00016080: 6427 290d 0a20 2023 204d 6170 2e61 6464  d')..  # Map.add
+00016090: 4c61 7965 7228 736e 6f77 466f 7265 7374  Layer(snowForest
+000160a0: 2e73 656c 664d 6173 6b28 292c 7b27 6d69  .selfMask(),{'mi
+000160b0: 6e27 3a31 2c27 6d61 7827 3a31 2c27 7061  n':1,'max':1,'pa
+000160c0: 6c65 7474 6527 3a27 3030 4627 7d2c 2753  lette':'00F'},'S
+000160d0: 6e6f 7720 466f 7265 7374 2729 0d0a 2020  now Forest')..  
+000160e0: 2346 7261 6374 696f 6e61 6c20 736e 6f77  #Fractional snow
+000160f0: 2063 6f76 6572 2028 4653 432c 2030 2025   cover (FSC, 0 %
+00016100: 202d 2031 3030 2520 736e 6f77 2920 6361   - 100% snow) ca
+00016110: 6e20 6265 2064 6574 6563 7465 6420 6279  n be detected by
+00016120: 2074 6865 2061 7070 726f 6163 6820 6f66   the approach of
+00016130: 2053 616c 6f6d 6f6e 736f 6e0d 0a20 2023   Salomonson..  #
+00016140: 616e 6420 4170 7065 6c20 2832 3030 342c  and Appel (2004,
+00016150: 2032 3030 3629 2c20 7768 6963 6820 7761   2006), which wa
+00016160: 7320 6f72 6967 696e 616c 6c79 2064 6576  s originally dev
+00016170: 656c 6f70 6564 2066 6f72 204d 4f44 4953  eloped for MODIS
+00016180: 2064 6174 613a 0d0a 2020 2346 5343 203d   data:..  #FSC =
+00016190: 20e2 8093 302e 3031 202b 2031 2e34 3520   ...0.01 + 1.45 
+000161a0: 2a20 4e44 5349 0d0a 2020 6673 6320 3d20  * NDSI..  fsc = 
+000161b0: 6e64 7369 2e6d 756c 7469 706c 7928 312e  ndsi.multiply(1.
+000161c0: 3435 292e 7375 6274 7261 6374 2830 2e30  45).subtract(0.0
+000161d0: 3129 0d0a 2020 2320 4d61 702e 6164 644c  1)..  # Map.addL
+000161e0: 6179 6572 2866 7363 2c7b 276d 696e 273a  ayer(fsc,{'min':
+000161f0: 302c 276d 6178 273a 312c 2770 616c 6574  0,'max':1,'palet
+00016200: 7465 273a 2730 3830 2c30 3038 277d 2c27  te':'080,008'},'
+00016210: 4672 6163 7469 6f6e 616c 2053 6e6f 7720  Fractional Snow 
+00016220: 436f 7665 7227 290d 0a20 2073 6e6f 774d  Cover')..  snowM
+00016230: 6173 6b20 3d20 2828 736e 6f77 4f70 656e  ask = ((snowOpen
+00016240: 4c61 6e64 2e4f 7228 736e 6f77 466f 7265  Land.Or(snowFore
+00016250: 7374 2929 2e4e 6f74 2829 292e 666f 6361  st)).Not()).foca
+00016260: 6c5f 6d69 6e28 6469 6c61 7465 5069 7865  l_min(dilatePixe
+00016270: 6c73 290d 0a20 2072 6574 7572 6e20 696d  ls)..  return im
+00016280: 672e 7570 6461 7465 4d61 736b 2873 6e6f  g.updateMask(sno
+00016290: 774d 6173 6b29 0d0a 2323 2323 2323 2323  wMask)..########
 000162a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000162b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000162c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000162d0: 2323 2323 2323 2323 2323 0d0a 2323 2323  ##########..####
-000162e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000162d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000162e0: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
 000162f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016320: 2323 2323 230d 0a23 4d4f 4449 5320 7072  #####..#MODIS pr
-00016330: 6f63 6573 7369 6e67 0d0a 2323 2323 2323  ocessing..######
-00016340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016320: 2323 2323 2323 2323 2323 2323 0d0a 234d  ############..#M
+00016330: 4f44 4953 2070 726f 6365 7373 696e 670d  ODIS processing.
+00016340: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
 00016350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016380: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
+00016380: 2323 2323 2323 2323 2323 0d0a 2323 2323  ##########..####
 00016390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000163a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000163b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000163c0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-000163d0: 2353 6f6d 6520 676c 6f62 616c 7320 746f  #Some globals to
-000163e0: 2064 6561 6c20 7769 7468 206d 756c 7469   deal with multi
-000163f0: 2d73 7065 6374 7261 6c20 4d4f 4449 530d  -spectral MODIS.
-00016400: 0a23 2077 5465 6d70 5365 6c65 6374 4f72  .# wTempSelectOr
-00016410: 6465 7220 3d20 5b32 2c33 2c30 2c31 2c34  der = [2,3,0,1,4
-00016420: 2c36 2c35 5d23 4261 6e64 206f 7264 6572  ,6,5]#Band order
-00016430: 2074 6f20 7365 6c65 6374 2074 6f20 6265   to select to be
-00016440: 204c 616e 6473 6174 2035 2d6c 696b 6520   Landsat 5-like 
-00016450: 6966 2074 6865 726d 616c 2069 7320 696e  if thermal is in
-00016460: 636c 7564 6564 0d0a 2320 7754 656d 7053  cluded..# wTempS
-00016470: 7464 4e61 6d65 7320 3d20 5b27 626c 7565  tdNames = ['blue
-00016480: 272c 2027 6772 6565 6e27 2c20 2772 6564  ', 'green', 'red
-00016490: 272c 2027 6e69 7227 2c20 2773 7769 7231  ', 'nir', 'swir1
-000164a0: 272c 2774 656d 7027 2c27 7377 6972 3227  ','temp','swir2'
-000164b0: 5d0d 0a0d 0a23 2077 6f54 656d 7053 656c  ]....# woTempSel
-000164c0: 6563 744f 7264 6572 203d 205b 322c 332c  ectOrder = [2,3,
-000164d0: 302c 312c 342c 355d 2342 616e 6420 6f72  0,1,4,5]#Band or
-000164e0: 6465 7220 746f 2073 656c 6563 7420 746f  der to select to
-000164f0: 2062 6520 4c61 6e64 7361 7420 352d 6c69   be Landsat 5-li
-00016500: 6b65 2069 6620 7468 6572 6d61 6c20 6973  ke if thermal is
-00016510: 2065 7863 6c75 6465 640d 0a23 2077 6f54   excluded..# woT
-00016520: 656d 7053 7464 4e61 6d65 7320 3d20 5b27  empStdNames = ['
-00016530: 626c 7565 272c 2027 6772 6565 6e27 2c20  blue', 'green', 
-00016540: 2772 6564 272c 2027 6e69 7227 2c20 2773  'red', 'nir', 's
-00016550: 7769 7231 272c 2773 7769 7232 275d 0d0a  wir1','swir2']..
-00016560: 6d6f 6469 7332 3530 5365 6c65 6374 4261  modis250SelectBa
-00016570: 6e64 7320 3d20 5b27 7375 725f 7265 666c  nds = ['sur_refl
-00016580: 5f62 3031 272c 2773 7572 5f72 6566 6c5f  _b01','sur_refl_
-00016590: 6230 3227 5d0d 0a6d 6f64 6973 3235 3042  b02']..modis250B
-000165a0: 616e 644e 616d 6573 203d 205b 2772 6564  andNames = ['red
-000165b0: 272c 276e 6972 275d 0d0a 0d0a 6d6f 6469  ','nir']....modi
-000165c0: 7335 3030 5365 6c65 6374 4261 6e64 7320  s500SelectBands 
-000165d0: 3d20 5b27 7375 725f 7265 666c 5f62 3033  = ['sur_refl_b03
-000165e0: 272c 2773 7572 5f72 6566 6c5f 6230 3427  ','sur_refl_b04'
-000165f0: 2c27 7375 725f 7265 666c 5f62 3036 272c  ,'sur_refl_b06',
-00016600: 2773 7572 5f72 6566 6c5f 6230 3727 5d0d  'sur_refl_b07'].
-00016610: 0a6d 6f64 6973 3530 3042 616e 644e 616d  .modis500BandNam
-00016620: 6573 203d 205b 2762 6c75 6527 2c27 6772  es = ['blue','gr
-00016630: 6565 6e27 2c27 7377 6972 3127 2c27 7377  een','swir1','sw
-00016640: 6972 3227 5d0d 0a0d 0a63 6f6d 6269 6e65  ir2']....combine
-00016650: 644d 6f64 6973 4261 6e64 4e61 6d65 7320  dModisBandNames 
-00016660: 3d20 5b27 7265 6427 2c27 6e69 7227 2c27  = ['red','nir','
-00016670: 626c 7565 272c 2767 7265 656e 272c 2773  blue','green','s
-00016680: 7769 7231 272c 2773 7769 7232 275d 0d0a  wir1','swir2']..
-00016690: 0d0a 6461 696c 7956 6965 7741 6e67 6c65  ..dailyViewAngle
-000166a0: 4261 6e64 4e61 6d65 7320 3d20 5b27 5365  BandNames = ['Se
-000166b0: 6e73 6f72 5a65 6e69 7468 272c 2753 656e  nsorZenith','Sen
-000166c0: 736f 7241 7a69 6d75 7468 272c 2753 6f6c  sorAzimuth','Sol
-000166d0: 6172 5a65 6e69 7468 272c 2753 6f6c 6172  arZenith','Solar
-000166e0: 417a 696d 7574 6827 5d0d 0a63 6f6d 706f  Azimuth']..compo
-000166f0: 7369 7465 5669 6577 416e 676c 6542 616e  siteViewAngleBan
-00016700: 644e 616d 6573 203d 205b 2753 6f6c 6172  dNames = ['Solar
-00016710: 5a65 6e69 7468 272c 2027 5669 6577 5a65  Zenith', 'ViewZe
-00016720: 6e69 7468 272c 2027 5265 6c61 7469 7665  nith', 'Relative
-00016730: 417a 696d 7574 6827 5d0d 0a23 4469 6374  Azimuth']..#Dict
-00016740: 696f 6e61 7279 206f 6620 4d4f 4449 5320  ionary of MODIS 
-00016750: 636f 6c6c 6563 7469 6f6e 730d 0a6d 6f64  collections..mod
-00016760: 6973 4344 6963 7420 3d20 7b5c 0d0a 2020  isCDict = {\..  
-00016770: 2765 6967 6874 4461 794e 4456 4941 2720  'eightDayNDVIA' 
-00016780: 3a20 274d 4f44 4953 2f30 3631 2f4d 5944  : 'MODIS/061/MYD
-00016790: 3133 5131 272c 5c0d 0a20 2027 6569 6768  13Q1',\..  'eigh
-000167a0: 7444 6179 4e44 5649 5427 203a 2027 4d4f  tDayNDVIT' : 'MO
-000167b0: 4449 532f 3036 312f 4d4f 4431 3351 3127  DIS/061/MOD13Q1'
-000167c0: 2c5c 0d0a 2020 2765 6967 6874 4461 7953  ,\..  'eightDayS
-000167d0: 5232 3530 4127 203a 2027 4d4f 4449 532f  R250A' : 'MODIS/
-000167e0: 3036 312f 4d59 4430 3951 3127 2c5c 0d0a  061/MYD09Q1',\..
-000167f0: 2020 2765 6967 6874 4461 7953 5232 3530    'eightDaySR250
-00016800: 5427 203a 2027 4d4f 4449 532f 3036 312f  T' : 'MODIS/061/
-00016810: 4d4f 4430 3951 3127 2c5c 0d0a 2020 2765  MOD09Q1',\..  'e
-00016820: 6967 6874 4461 7953 5235 3030 4127 203a  ightDaySR500A' :
-00016830: 2027 4d4f 4449 532f 3036 312f 4d59 4430   'MODIS/061/MYD0
-00016840: 3941 3127 2c5c 0d0a 2020 2765 6967 6874  9A1',\..  'eight
-00016850: 4461 7953 5235 3030 5427 203a 2027 4d4f  DaySR500T' : 'MO
-00016860: 4449 532f 3036 312f 4d4f 4430 3941 3127  DIS/061/MOD09A1'
-00016870: 2c5c 0d0a 2020 2765 6967 6874 4461 794c  ,\..  'eightDayL
-00016880: 5354 3130 3030 4127 203a 2027 4d4f 4449  ST1000A' : 'MODI
-00016890: 532f 3036 312f 4d59 4431 3141 3227 2c5c  S/061/MYD11A2',\
-000168a0: 0d0a 2020 2765 6967 6874 4461 794c 5354  ..  'eightDayLST
-000168b0: 3130 3030 5427 203a 2027 4d4f 4449 532f  1000T' : 'MODIS/
-000168c0: 3036 312f 4d4f 4431 3141 3227 2c5c 0d0a  061/MOD11A2',\..
-000168d0: 2020 2764 6169 6c79 5352 3235 3041 2720    'dailySR250A' 
-000168e0: 3a20 274d 4f44 4953 2f30 3631 2f4d 5944  : 'MODIS/061/MYD
-000168f0: 3039 4751 272c 5c0d 0a20 2027 6461 696c  09GQ',\..  'dail
-00016900: 7953 5232 3530 5427 203a 2027 4d4f 4449  ySR250T' : 'MODI
-00016910: 532f 3036 312f 4d4f 4430 3947 5127 2c5c  S/061/MOD09GQ',\
-00016920: 0d0a 2020 2764 6169 6c79 5352 3530 3041  ..  'dailySR500A
-00016930: 2720 3a20 274d 4f44 4953 2f30 3631 2f4d  ' : 'MODIS/061/M
-00016940: 5944 3039 4741 272c 5c0d 0a20 2027 6461  YD09GA',\..  'da
-00016950: 696c 7953 5235 3030 5427 203a 2027 4d4f  ilySR500T' : 'MO
-00016960: 4449 532f 3036 312f 4d4f 4430 3947 4127  DIS/061/MOD09GA'
-00016970: 2c5c 0d0a 2020 2764 6169 6c79 4c53 5431  ,\..  'dailyLST1
-00016980: 3030 3041 2720 3a20 274d 4f44 4953 2f30  000A' : 'MODIS/0
-00016990: 3631 2f4d 5944 3131 4131 272c 5c0d 0a20  61/MYD11A1',\.. 
-000169a0: 2027 6461 696c 794c 5354 3130 3030 5427   'dailyLST1000T'
-000169b0: 203a 2027 4d4f 4449 532f 3036 312f 4d4f   : 'MODIS/061/MO
-000169c0: 4431 3141 3127 5c0d 0a7d 0d0a 6d75 6c74  D11A1'\..}..mult
-000169d0: 4d6f 6469 7344 6963 7420 3d20 7b5c 0d0a  ModisDict = {\..
-000169e0: 2020 2020 2774 656d 704e 6f41 6e67 6c65      'tempNoAngle
-000169f0: 4461 696c 7927 3a20 5b65 652e 496d 6167  Daily': [ee.Imag
-00016a00: 6528 5b30 2e30 3030 312c 302e 3030 3031  e([0.0001,0.0001
+000163c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000163d0: 2323 2323 230d 0a23 536f 6d65 2067 6c6f  #####..#Some glo
+000163e0: 6261 6c73 2074 6f20 6465 616c 2077 6974  bals to deal wit
+000163f0: 6820 6d75 6c74 692d 7370 6563 7472 616c  h multi-spectral
+00016400: 204d 4f44 4953 0d0a 2320 7754 656d 7053   MODIS..# wTempS
+00016410: 656c 6563 744f 7264 6572 203d 205b 322c  electOrder = [2,
+00016420: 332c 302c 312c 342c 362c 355d 2342 616e  3,0,1,4,6,5]#Ban
+00016430: 6420 6f72 6465 7220 746f 2073 656c 6563  d order to selec
+00016440: 7420 746f 2062 6520 4c61 6e64 7361 7420  t to be Landsat 
+00016450: 352d 6c69 6b65 2069 6620 7468 6572 6d61  5-like if therma
+00016460: 6c20 6973 2069 6e63 6c75 6465 640d 0a23  l is included..#
+00016470: 2077 5465 6d70 5374 644e 616d 6573 203d   wTempStdNames =
+00016480: 205b 2762 6c75 6527 2c20 2767 7265 656e   ['blue', 'green
+00016490: 272c 2027 7265 6427 2c20 276e 6972 272c  ', 'red', 'nir',
+000164a0: 2027 7377 6972 3127 2c27 7465 6d70 272c   'swir1','temp',
+000164b0: 2773 7769 7232 275d 0d0a 0d0a 2320 776f  'swir2']....# wo
+000164c0: 5465 6d70 5365 6c65 6374 4f72 6465 7220  TempSelectOrder 
+000164d0: 3d20 5b32 2c33 2c30 2c31 2c34 2c35 5d23  = [2,3,0,1,4,5]#
+000164e0: 4261 6e64 206f 7264 6572 2074 6f20 7365  Band order to se
+000164f0: 6c65 6374 2074 6f20 6265 204c 616e 6473  lect to be Lands
+00016500: 6174 2035 2d6c 696b 6520 6966 2074 6865  at 5-like if the
+00016510: 726d 616c 2069 7320 6578 636c 7564 6564  rmal is excluded
+00016520: 0d0a 2320 776f 5465 6d70 5374 644e 616d  ..# woTempStdNam
+00016530: 6573 203d 205b 2762 6c75 6527 2c20 2767  es = ['blue', 'g
+00016540: 7265 656e 272c 2027 7265 6427 2c20 276e  reen', 'red', 'n
+00016550: 6972 272c 2027 7377 6972 3127 2c27 7377  ir', 'swir1','sw
+00016560: 6972 3227 5d0d 0a6d 6f64 6973 3235 3053  ir2']..modis250S
+00016570: 656c 6563 7442 616e 6473 203d 205b 2773  electBands = ['s
+00016580: 7572 5f72 6566 6c5f 6230 3127 2c27 7375  ur_refl_b01','su
+00016590: 725f 7265 666c 5f62 3032 275d 0d0a 6d6f  r_refl_b02']..mo
+000165a0: 6469 7332 3530 4261 6e64 4e61 6d65 7320  dis250BandNames 
+000165b0: 3d20 5b27 7265 6427 2c27 6e69 7227 5d0d  = ['red','nir'].
+000165c0: 0a0d 0a6d 6f64 6973 3530 3053 656c 6563  ...modis500Selec
+000165d0: 7442 616e 6473 203d 205b 2773 7572 5f72  tBands = ['sur_r
+000165e0: 6566 6c5f 6230 3327 2c27 7375 725f 7265  efl_b03','sur_re
+000165f0: 666c 5f62 3034 272c 2773 7572 5f72 6566  fl_b04','sur_ref
+00016600: 6c5f 6230 3627 2c27 7375 725f 7265 666c  l_b06','sur_refl
+00016610: 5f62 3037 275d 0d0a 6d6f 6469 7335 3030  _b07']..modis500
+00016620: 4261 6e64 4e61 6d65 7320 3d20 5b27 626c  BandNames = ['bl
+00016630: 7565 272c 2767 7265 656e 272c 2773 7769  ue','green','swi
+00016640: 7231 272c 2773 7769 7232 275d 0d0a 0d0a  r1','swir2']....
+00016650: 636f 6d62 696e 6564 4d6f 6469 7342 616e  combinedModisBan
+00016660: 644e 616d 6573 203d 205b 2772 6564 272c  dNames = ['red',
+00016670: 276e 6972 272c 2762 6c75 6527 2c27 6772  'nir','blue','gr
+00016680: 6565 6e27 2c27 7377 6972 3127 2c27 7377  een','swir1','sw
+00016690: 6972 3227 5d0d 0a0d 0a64 6169 6c79 5669  ir2']....dailyVi
+000166a0: 6577 416e 676c 6542 616e 644e 616d 6573  ewAngleBandNames
+000166b0: 203d 205b 2753 656e 736f 725a 656e 6974   = ['SensorZenit
+000166c0: 6827 2c27 5365 6e73 6f72 417a 696d 7574  h','SensorAzimut
+000166d0: 6827 2c27 536f 6c61 725a 656e 6974 6827  h','SolarZenith'
+000166e0: 2c27 536f 6c61 7241 7a69 6d75 7468 275d  ,'SolarAzimuth']
+000166f0: 0d0a 636f 6d70 6f73 6974 6556 6965 7741  ..compositeViewA
+00016700: 6e67 6c65 4261 6e64 4e61 6d65 7320 3d20  ngleBandNames = 
+00016710: 5b27 536f 6c61 725a 656e 6974 6827 2c20  ['SolarZenith', 
+00016720: 2756 6965 775a 656e 6974 6827 2c20 2752  'ViewZenith', 'R
+00016730: 656c 6174 6976 6541 7a69 6d75 7468 275d  elativeAzimuth']
+00016740: 0d0a 2344 6963 7469 6f6e 6172 7920 6f66  ..#Dictionary of
+00016750: 204d 4f44 4953 2063 6f6c 6c65 6374 696f   MODIS collectio
+00016760: 6e73 0d0a 6d6f 6469 7343 4469 6374 203d  ns..modisCDict =
+00016770: 207b 5c0d 0a20 2027 6569 6768 7444 6179   {\..  'eightDay
+00016780: 4e44 5649 4127 203a 2027 4d4f 4449 532f  NDVIA' : 'MODIS/
+00016790: 3036 312f 4d59 4431 3351 3127 2c5c 0d0a  061/MYD13Q1',\..
+000167a0: 2020 2765 6967 6874 4461 794e 4456 4954    'eightDayNDVIT
+000167b0: 2720 3a20 274d 4f44 4953 2f30 3631 2f4d  ' : 'MODIS/061/M
+000167c0: 4f44 3133 5131 272c 5c0d 0a20 2027 6569  OD13Q1',\..  'ei
+000167d0: 6768 7444 6179 5352 3235 3041 2720 3a20  ghtDaySR250A' : 
+000167e0: 274d 4f44 4953 2f30 3631 2f4d 5944 3039  'MODIS/061/MYD09
+000167f0: 5131 272c 5c0d 0a20 2027 6569 6768 7444  Q1',\..  'eightD
+00016800: 6179 5352 3235 3054 2720 3a20 274d 4f44  aySR250T' : 'MOD
+00016810: 4953 2f30 3631 2f4d 4f44 3039 5131 272c  IS/061/MOD09Q1',
+00016820: 5c0d 0a20 2027 6569 6768 7444 6179 5352  \..  'eightDaySR
+00016830: 3530 3041 2720 3a20 274d 4f44 4953 2f30  500A' : 'MODIS/0
+00016840: 3631 2f4d 5944 3039 4131 272c 5c0d 0a20  61/MYD09A1',\.. 
+00016850: 2027 6569 6768 7444 6179 5352 3530 3054   'eightDaySR500T
+00016860: 2720 3a20 274d 4f44 4953 2f30 3631 2f4d  ' : 'MODIS/061/M
+00016870: 4f44 3039 4131 272c 5c0d 0a20 2027 6569  OD09A1',\..  'ei
+00016880: 6768 7444 6179 4c53 5431 3030 3041 2720  ghtDayLST1000A' 
+00016890: 3a20 274d 4f44 4953 2f30 3631 2f4d 5944  : 'MODIS/061/MYD
+000168a0: 3131 4132 272c 5c0d 0a20 2027 6569 6768  11A2',\..  'eigh
+000168b0: 7444 6179 4c53 5431 3030 3054 2720 3a20  tDayLST1000T' : 
+000168c0: 274d 4f44 4953 2f30 3631 2f4d 4f44 3131  'MODIS/061/MOD11
+000168d0: 4132 272c 5c0d 0a20 2027 6461 696c 7953  A2',\..  'dailyS
+000168e0: 5232 3530 4127 203a 2027 4d4f 4449 532f  R250A' : 'MODIS/
+000168f0: 3036 312f 4d59 4430 3947 5127 2c5c 0d0a  061/MYD09GQ',\..
+00016900: 2020 2764 6169 6c79 5352 3235 3054 2720    'dailySR250T' 
+00016910: 3a20 274d 4f44 4953 2f30 3631 2f4d 4f44  : 'MODIS/061/MOD
+00016920: 3039 4751 272c 5c0d 0a20 2027 6461 696c  09GQ',\..  'dail
+00016930: 7953 5235 3030 4127 203a 2027 4d4f 4449  ySR500A' : 'MODI
+00016940: 532f 3036 312f 4d59 4430 3947 4127 2c5c  S/061/MYD09GA',\
+00016950: 0d0a 2020 2764 6169 6c79 5352 3530 3054  ..  'dailySR500T
+00016960: 2720 3a20 274d 4f44 4953 2f30 3631 2f4d  ' : 'MODIS/061/M
+00016970: 4f44 3039 4741 272c 5c0d 0a20 2027 6461  OD09GA',\..  'da
+00016980: 696c 794c 5354 3130 3030 4127 203a 2027  ilyLST1000A' : '
+00016990: 4d4f 4449 532f 3036 312f 4d59 4431 3141  MODIS/061/MYD11A
+000169a0: 3127 2c5c 0d0a 2020 2764 6169 6c79 4c53  1',\..  'dailyLS
+000169b0: 5431 3030 3054 2720 3a20 274d 4f44 4953  T1000T' : 'MODIS
+000169c0: 2f30 3631 2f4d 4f44 3131 4131 275c 0d0a  /061/MOD11A1'\..
+000169d0: 7d0d 0a6d 756c 744d 6f64 6973 4469 6374  }..multModisDict
+000169e0: 203d 207b 5c0d 0a20 2020 2027 7465 6d70   = {\..    'temp
+000169f0: 4e6f 416e 676c 6544 6169 6c79 273a 205b  NoAngleDaily': [
+00016a00: 6565 2e49 6d61 6765 285b 302e 3030 3031  ee.Image([0.0001
 00016a10: 2c30 2e30 3030 312c 302e 3030 3031 2c30  ,0.0001,0.0001,0
 00016a20: 2e30 3030 312c 302e 3030 3031 2c30 2e30  .0001,0.0001,0.0
-00016a30: 322c 312c 315d 292c 5c0d 0a20 2020 2020  2,1,1]),\..     
-00016a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a50: 2020 205b 2762 6c75 6527 2c27 6772 6565     ['blue','gree
-00016a60: 6e27 2c27 7265 6427 2c27 6e69 7227 2c27  n','red','nir','
-00016a70: 7377 6972 3127 2c27 7465 6d70 272c 2773  swir1','temp','s
-00016a80: 7769 7232 272c 2745 6d69 735f 3331 272c  wir2','Emis_31',
-00016a90: 2745 6d69 735f 3332 275d 5d2c 5c0d 0a20  'Emis_32']],\.. 
-00016aa0: 2020 2027 7465 6d70 4e6f 416e 676c 6543     'tempNoAngleC
-00016ab0: 6f6d 706f 7369 7465 273a 205b 6565 2e49  omposite': [ee.I
-00016ac0: 6d61 6765 285b 302e 3030 3031 2c30 2e30  mage([0.0001,0.0
+00016a30: 3030 312c 302e 3032 2c31 2c31 5d29 2c5c  001,0.02,1,1]),\
+00016a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a50: 2020 2020 2020 2020 2020 5b27 626c 7565            ['blue
+00016a60: 272c 2767 7265 656e 272c 2772 6564 272c  ','green','red',
+00016a70: 276e 6972 272c 2773 7769 7231 272c 2774  'nir','swir1','t
+00016a80: 656d 7027 2c27 7377 6972 3227 2c27 456d  emp','swir2','Em
+00016a90: 6973 5f33 3127 2c27 456d 6973 5f33 3227  is_31','Emis_32'
+00016aa0: 5d5d 2c5c 0d0a 2020 2020 2774 656d 704e  ]],\..    'tempN
+00016ab0: 6f41 6e67 6c65 436f 6d70 6f73 6974 6527  oAngleComposite'
+00016ac0: 3a20 5b65 652e 496d 6167 6528 5b30 2e30  : [ee.Image([0.0
 00016ad0: 3030 312c 302e 3030 3031 2c30 2e30 3030  001,0.0001,0.000
 00016ae0: 312c 302e 3030 3031 2c30 2e30 3030 312c  1,0.0001,0.0001,
-00016af0: 302e 3032 2c31 2c31 5d29 2c5c 0d0a 2020  0.02,1,1]),\..  
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 2020 2020 5b27 626c 7565 272c 2767        ['blue','g
-00016b20: 7265 656e 272c 2772 6564 272c 276e 6972  reen','red','nir
-00016b30: 272c 2773 7769 7231 272c 2774 656d 7027  ','swir1','temp'
-00016b40: 2c27 7377 6972 3227 2c27 456d 6973 5f33  ,'swir2','Emis_3
-00016b50: 3127 2c27 456d 6973 5f33 3227 5d5d 2c5c  1','Emis_32']],\
-00016b60: 0d0a 2020 2020 2774 656d 7041 6e67 6c65  ..    'tempAngle
-00016b70: 4461 696c 7927 3a20 5b65 652e 496d 6167  Daily': [ee.Imag
-00016b80: 6528 5b30 2e30 3030 312c 302e 3030 3031  e([0.0001,0.0001
+00016af0: 302e 3030 3031 2c30 2e30 322c 312c 315d  0.0001,0.02,1,1]
+00016b00: 292c 5c0d 0a20 2020 2020 2020 2020 2020  ),\..           
+00016b10: 2020 2020 2020 2020 2020 2020 205b 2762               ['b
+00016b20: 6c75 6527 2c27 6772 6565 6e27 2c27 7265  lue','green','re
+00016b30: 6427 2c27 6e69 7227 2c27 7377 6972 3127  d','nir','swir1'
+00016b40: 2c27 7465 6d70 272c 2773 7769 7232 272c  ,'temp','swir2',
+00016b50: 2745 6d69 735f 3331 272c 2745 6d69 735f  'Emis_31','Emis_
+00016b60: 3332 275d 5d2c 5c0d 0a20 2020 2027 7465  32']],\..    'te
+00016b70: 6d70 416e 676c 6544 6169 6c79 273a 205b  mpAngleDaily': [
+00016b80: 6565 2e49 6d61 6765 285b 302e 3030 3031  ee.Image([0.0001
 00016b90: 2c30 2e30 3030 312c 302e 3030 3031 2c30  ,0.0001,0.0001,0
-00016ba0: 2e30 3030 312c 302e 3030 3031 2c31 2c31  .0001,0.0001,1,1
-00016bb0: 2c31 2c31 2c30 2e30 322c 312c 315d 292c  ,1,1,0.02,1,1]),
-00016bc0: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-00016bd0: 2020 2020 2020 2020 205b 2762 6c75 6527           ['blue'
-00016be0: 2c27 6772 6565 6e27 2c27 7265 6427 2c27  ,'green','red','
-00016bf0: 6e69 7227 2c27 7377 6972 3127 2c27 7465  nir','swir1','te
-00016c00: 6d70 272c 2773 7769 7232 272c 2753 656e  mp','swir2','Sen
-00016c10: 736f 725a 656e 6974 6827 2c27 5365 6e73  sorZenith','Sens
-00016c20: 6f72 417a 696d 7574 6827 2c27 536f 6c61  orAzimuth','Sola
-00016c30: 725a 656e 6974 6827 2c27 536f 6c61 7241  rZenith','SolarA
-00016c40: 7a69 6d75 7468 272c 2745 6d69 735f 3331  zimuth','Emis_31
-00016c50: 272c 2745 6d69 735f 3332 275d 5d2c 5c0d  ','Emis_32']],\.
-00016c60: 0a20 2020 2027 7465 6d70 416e 676c 6543  .    'tempAngleC
-00016c70: 6f6d 706f 7369 7465 273a 205b 6565 2e49  omposite': [ee.I
-00016c80: 6d61 6765 285b 302e 3030 3031 2c30 2e30  mage([0.0001,0.0
+00016ba0: 2e30 3030 312c 302e 3030 3031 2c30 2e30  .0001,0.0001,0.0
+00016bb0: 3030 312c 312c 312c 312c 312c 302e 3032  001,1,1,1,1,0.02
+00016bc0: 2c31 2c31 5d29 2c5c 0d0a 2020 2020 2020  ,1,1]),\..      
+00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016be0: 5b27 626c 7565 272c 2767 7265 656e 272c  ['blue','green',
+00016bf0: 2772 6564 272c 276e 6972 272c 2773 7769  'red','nir','swi
+00016c00: 7231 272c 2774 656d 7027 2c27 7377 6972  r1','temp','swir
+00016c10: 3227 2c27 5365 6e73 6f72 5a65 6e69 7468  2','SensorZenith
+00016c20: 272c 2753 656e 736f 7241 7a69 6d75 7468  ','SensorAzimuth
+00016c30: 272c 2753 6f6c 6172 5a65 6e69 7468 272c  ','SolarZenith',
+00016c40: 2753 6f6c 6172 417a 696d 7574 6827 2c27  'SolarAzimuth','
+00016c50: 456d 6973 5f33 3127 2c27 456d 6973 5f33  Emis_31','Emis_3
+00016c60: 3227 5d5d 2c5c 0d0a 2020 2020 2774 656d  2']],\..    'tem
+00016c70: 7041 6e67 6c65 436f 6d70 6f73 6974 6527  pAngleComposite'
+00016c80: 3a20 5b65 652e 496d 6167 6528 5b30 2e30  : [ee.Image([0.0
 00016c90: 3030 312c 302e 3030 3031 2c30 2e30 3030  001,0.0001,0.000
 00016ca0: 312c 302e 3030 3031 2c30 2e30 3030 312c  1,0.0001,0.0001,
-00016cb0: 312c 312c 312c 302e 3032 2c31 2c31 5d29  1,1,1,0.02,1,1])
-00016cc0: 2c5c 0d0a 2020 2020 2020 2020 2020 2020  ,\..            
-00016cd0: 2020 2020 2020 2020 2020 5b27 626c 7565            ['blue
-00016ce0: 272c 2767 7265 656e 272c 2772 6564 272c  ','green','red',
-00016cf0: 276e 6972 272c 2773 7769 7231 272c 2774  'nir','swir1','t
-00016d00: 656d 7027 2c27 7377 6972 3227 2c27 536f  emp','swir2','So
-00016d10: 6c61 725a 656e 6974 6827 2c20 2756 6965  larZenith', 'Vie
-00016d20: 775a 656e 6974 6827 2c20 2752 656c 6174  wZenith', 'Relat
-00016d30: 6976 6541 7a69 6d75 7468 272c 2745 6d69  iveAzimuth','Emi
-00016d40: 735f 3331 272c 2745 6d69 735f 3332 275d  s_31','Emis_32']
-00016d50: 5d2c 5c0d 0a20 2020 2027 6e6f 5465 6d70  ],\..    'noTemp
-00016d60: 4e6f 416e 676c 6544 6169 6c79 273a 205b  NoAngleDaily': [
-00016d70: 6565 2e49 6d61 6765 285b 302e 3030 3031  ee.Image([0.0001
-00016d80: 2c30 2e30 3030 312c 302e 3030 3031 2c30  ,0.0001,0.0001,0
+00016cb0: 302e 3030 3031 2c31 2c31 2c31 2c30 2e30  0.0001,1,1,1,0.0
+00016cc0: 322c 312c 315d 292c 5c0d 0a20 2020 2020  2,1,1]),\..     
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ce0: 205b 2762 6c75 6527 2c27 6772 6565 6e27   ['blue','green'
+00016cf0: 2c27 7265 6427 2c27 6e69 7227 2c27 7377  ,'red','nir','sw
+00016d00: 6972 3127 2c27 7465 6d70 272c 2773 7769  ir1','temp','swi
+00016d10: 7232 272c 2753 6f6c 6172 5a65 6e69 7468  r2','SolarZenith
+00016d20: 272c 2027 5669 6577 5a65 6e69 7468 272c  ', 'ViewZenith',
+00016d30: 2027 5265 6c61 7469 7665 417a 696d 7574   'RelativeAzimut
+00016d40: 6827 2c27 456d 6973 5f33 3127 2c27 456d  h','Emis_31','Em
+00016d50: 6973 5f33 3227 5d5d 2c5c 0d0a 2020 2020  is_32']],\..    
+00016d60: 276e 6f54 656d 704e 6f41 6e67 6c65 4461  'noTempNoAngleDa
+00016d70: 696c 7927 3a20 5b65 652e 496d 6167 6528  ily': [ee.Image(
+00016d80: 5b30 2e30 3030 312c 302e 3030 3031 2c30  [0.0001,0.0001,0
 00016d90: 2e30 3030 312c 302e 3030 3031 2c30 2e30  .0001,0.0001,0.0
-00016da0: 3030 315d 292c 5c0d 0a20 2020 2020 2020  001]),\..       
-00016db0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00016dc0: 2762 6c75 6527 2c27 6772 6565 6e27 2c27  'blue','green','
-00016dd0: 7265 6427 2c27 6e69 7227 2c27 7377 6972  red','nir','swir
-00016de0: 3127 2c27 7377 6972 3227 5d5d 2c5c 0d0a  1','swir2']],\..
-00016df0: 2020 2020 276e 6f54 656d 704e 6f41 6e67      'noTempNoAng
-00016e00: 6c65 436f 6d70 6f73 6974 6527 3a20 5b65  leComposite': [e
-00016e10: 652e 496d 6167 6528 5b30 2e30 3030 312c  e.Image([0.0001,
+00016da0: 3030 312c 302e 3030 3031 5d29 2c5c 0d0a  001,0.0001]),\..
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dc0: 2020 2020 2020 5b27 626c 7565 272c 2767        ['blue','g
+00016dd0: 7265 656e 272c 2772 6564 272c 276e 6972  reen','red','nir
+00016de0: 272c 2773 7769 7231 272c 2773 7769 7232  ','swir1','swir2
+00016df0: 275d 5d2c 5c0d 0a20 2020 2027 6e6f 5465  ']],\..    'noTe
+00016e00: 6d70 4e6f 416e 676c 6543 6f6d 706f 7369  mpNoAngleComposi
+00016e10: 7465 273a 205b 6565 2e49 6d61 6765 285b  te': [ee.Image([
 00016e20: 302e 3030 3031 2c30 2e30 3030 312c 302e  0.0001,0.0001,0.
 00016e30: 3030 3031 2c30 2e30 3030 312c 302e 3030  0001,0.0001,0.00
-00016e40: 3031 5d29 2c5c 0d0a 2020 2020 2020 2020  01]),\..        
-00016e50: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00016e60: 626c 7565 272c 2767 7265 656e 272c 2772  blue','green','r
-00016e70: 6564 272c 276e 6972 272c 2773 7769 7231  ed','nir','swir1
-00016e80: 272c 2773 7769 7232 275d 5d2c 5c0d 0a20  ','swir2']],\.. 
-00016e90: 2020 2027 6e6f 5465 6d70 416e 676c 6544     'noTempAngleD
-00016ea0: 6169 6c79 273a 205b 6565 2e49 6d61 6765  aily': [ee.Image
-00016eb0: 285b 302e 3030 3031 2c30 2e30 3030 312c  ([0.0001,0.0001,
+00016e40: 3031 2c30 2e30 3030 315d 292c 5c0d 0a20  01,0.0001]),\.. 
+00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e60: 2020 2020 205b 2762 6c75 6527 2c27 6772       ['blue','gr
+00016e70: 6565 6e27 2c27 7265 6427 2c27 6e69 7227  een','red','nir'
+00016e80: 2c27 7377 6972 3127 2c27 7377 6972 3227  ,'swir1','swir2'
+00016e90: 5d5d 2c5c 0d0a 2020 2020 276e 6f54 656d  ]],\..    'noTem
+00016ea0: 7041 6e67 6c65 4461 696c 7927 3a20 5b65  pAngleDaily': [e
+00016eb0: 652e 496d 6167 6528 5b30 2e30 3030 312c  e.Image([0.0001,
 00016ec0: 302e 3030 3031 2c30 2e30 3030 312c 302e  0.0001,0.0001,0.
-00016ed0: 3030 3031 2c30 2e30 3030 312c 312c 312c  0001,0.0001,1,1,
-00016ee0: 312c 315d 292c 5c0d 0a20 2020 2020 2020  1,1]),\..       
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00016f00: 2762 6c75 6527 2c27 6772 6565 6e27 2c27  'blue','green','
-00016f10: 7265 6427 2c27 6e69 7227 2c27 7377 6972  red','nir','swir
-00016f20: 3127 2c27 7377 6972 3227 2c27 5365 6e73  1','swir2','Sens
-00016f30: 6f72 5a65 6e69 7468 272c 2753 656e 736f  orZenith','Senso
-00016f40: 7241 7a69 6d75 7468 272c 2753 6f6c 6172  rAzimuth','Solar
-00016f50: 5a65 6e69 7468 272c 2753 6f6c 6172 417a  Zenith','SolarAz
-00016f60: 696d 7574 6827 5d5d 2c5c 0d0a 2020 2020  imuth']],\..    
-00016f70: 276e 6f54 656d 7041 6e67 6c65 436f 6d70  'noTempAngleComp
-00016f80: 6f73 6974 6527 3a20 5b65 652e 496d 6167  osite': [ee.Imag
-00016f90: 6528 5b30 2e30 3030 312c 302e 3030 3031  e([0.0001,0.0001
+00016ed0: 3030 3031 2c30 2e30 3030 312c 302e 3030  0001,0.0001,0.00
+00016ee0: 3031 2c31 2c31 2c31 2c31 5d29 2c5c 0d0a  01,1,1,1,1]),\..
+00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f00: 2020 2020 2020 5b27 626c 7565 272c 2767        ['blue','g
+00016f10: 7265 656e 272c 2772 6564 272c 276e 6972  reen','red','nir
+00016f20: 272c 2773 7769 7231 272c 2773 7769 7232  ','swir1','swir2
+00016f30: 272c 2753 656e 736f 725a 656e 6974 6827  ','SensorZenith'
+00016f40: 2c27 5365 6e73 6f72 417a 696d 7574 6827  ,'SensorAzimuth'
+00016f50: 2c27 536f 6c61 725a 656e 6974 6827 2c27  ,'SolarZenith','
+00016f60: 536f 6c61 7241 7a69 6d75 7468 275d 5d2c  SolarAzimuth']],
+00016f70: 5c0d 0a20 2020 2027 6e6f 5465 6d70 416e  \..    'noTempAn
+00016f80: 676c 6543 6f6d 706f 7369 7465 273a 205b  gleComposite': [
+00016f90: 6565 2e49 6d61 6765 285b 302e 3030 3031  ee.Image([0.0001
 00016fa0: 2c30 2e30 3030 312c 302e 3030 3031 2c30  ,0.0001,0.0001,0
-00016fb0: 2e30 3030 312c 302e 3030 3031 2c31 2c31  .0001,0.0001,1,1
-00016fc0: 2c31 5d29 2c5c 0d0a 2020 2020 2020 2020  ,1]),\..        
-00016fd0: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00016fe0: 626c 7565 272c 2767 7265 656e 272c 2772  blue','green','r
-00016ff0: 6564 272c 276e 6972 272c 2773 7769 7231  ed','nir','swir1
-00017000: 272c 2773 7769 7232 272c 2753 6f6c 6172  ','swir2','Solar
-00017010: 5a65 6e69 7468 272c 2027 5669 6577 5a65  Zenith', 'ViewZe
-00017020: 6e69 7468 272c 2027 5265 6c61 7469 7665  nith', 'Relative
-00017030: 417a 696d 7574 6827 5d5d 5c0d 0a20 207d  Azimuth']]\..  }
-00017040: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
+00016fb0: 2e30 3030 312c 302e 3030 3031 2c30 2e30  .0001,0.0001,0.0
+00016fc0: 3030 312c 312c 312c 315d 292c 5c0d 0a20  001,1,1,1]),\.. 
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fe0: 2020 2020 205b 2762 6c75 6527 2c27 6772       ['blue','gr
+00016ff0: 6565 6e27 2c27 7265 6427 2c27 6e69 7227  een','red','nir'
+00017000: 2c27 7377 6972 3127 2c27 7377 6972 3227  ,'swir1','swir2'
+00017010: 2c27 536f 6c61 725a 656e 6974 6827 2c20  ,'SolarZenith', 
+00017020: 2756 6965 775a 656e 6974 6827 2c20 2752  'ViewZenith', 'R
+00017030: 656c 6174 6976 6541 7a69 6d75 7468 275d  elativeAzimuth']
+00017040: 5d5c 0d0a 2020 7d0d 0a0d 0a23 2323 2323  ]\..  }....#####
 00017050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00017060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00017070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00017080: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-00017090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00017080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00017090: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
 000170a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000170b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000170c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000170d0: 2323 2323 2323 2323 0d0a 2348 656c 7065  ########..#Helpe
-000170e0: 7220 6675 6e63 7469 6f6e 2074 6f20 6a6f  r function to jo
-000170f0: 696e 2074 776f 2063 6f6c 6c65 6374 696f  in two collectio
-00017100: 6e73 2d20 536f 7572 6365 3a20 636f 6465  ns- Source: code
-00017110: 2e65 6172 7468 656e 6769 6e65 2e67 6f6f  .earthengine.goo
-00017120: 676c 652e 636f 6d0d 0a64 6566 206a 6f69  gle.com..def joi
-00017130: 6e43 6f6c 6c65 6374 696f 6e73 2863 312c  nCollections(c1,
-00017140: 2063 322c 206d 6173 6b41 6e79 4e75 6c6c   c2, maskAnyNull
-00017150: 5661 6c75 6573 203d 2054 7275 652c 206a  Values = True, j
-00017160: 6f69 6e50 726f 7065 7274 7920 3d20 2773  oinProperty = 's
-00017170: 7973 7465 6d3a 7469 6d65 5f73 7461 7274  ystem:time_start
-00017180: 272c 6a6f 696e 5072 6f70 6572 7479 5365  ',joinPropertySe
-00017190: 636f 6e64 6172 793d 4e6f 6e65 293a 0d0a  condary=None):..
-000171a0: 2020 0d0a 2020 6966 206a 6f69 6e50 726f    ..  if joinPro
-000171b0: 7065 7274 7953 6563 6f6e 6461 7279 3d3d  pertySecondary==
-000171c0: 4e6f 6e65 3a6a 6f69 6e50 726f 7065 7274  None:joinPropert
-000171d0: 7953 6563 6f6e 6461 7279 3d6a 6f69 6e50  ySecondary=joinP
-000171e0: 726f 7065 7274 790d 0a20 200d 0a20 2064  roperty..  ..  d
-000171f0: 6566 204d 6572 6765 4261 6e64 7328 656c  ef MergeBands(el
-00017200: 656d 656e 7429 3a0d 0a20 2020 2023 4120  ement):..    #A 
-00017210: 6675 6e63 7469 6f6e 2074 6f20 6d65 7267  function to merg
-00017220: 6520 7468 6520 6261 6e64 7320 746f 6765  e the bands toge
-00017230: 7468 6572 2e0d 0a20 2020 2023 4166 7465  ther...    #Afte
-00017240: 7220 6120 6a6f 696e 2c20 7265 7375 6c74  r a join, result
-00017250: 7320 6172 6520 696e 2027 7072 696d 6172  s are in 'primar
-00017260: 7927 2061 6e64 2027 7365 636f 6e64 6172  y' and 'secondar
-00017270: 7927 2070 726f 7065 7274 6965 732e 0d0a  y' properties...
-00017280: 2020 2020 7265 7475 726e 2065 652e 496d      return ee.Im
-00017290: 6167 652e 6361 7428 656c 656d 656e 742e  age.cat(element.
-000172a0: 6765 7428 2770 7269 6d61 7279 2729 2c20  get('primary'), 
-000172b0: 656c 656d 656e 742e 6765 7428 2773 6563  element.get('sec
-000172c0: 6f6e 6461 7279 2729 290d 0a0d 0a0d 0a20  ondary'))...... 
-000172d0: 206a 6f69 6e20 3d20 6565 2e4a 6f69 6e2e   join = ee.Join.
-000172e0: 696e 6e65 7228 290d 0a20 206a 6f69 6e46  inner()..  joinF
-000172f0: 696c 7465 7220 3d20 6565 2e46 696c 7465  ilter = ee.Filte
-00017300: 722e 6571 7561 6c73 286a 6f69 6e50 726f  r.equals(joinPro
-00017310: 7065 7274 792c 204e 6f6e 652c 206a 6f69  perty, None, joi
-00017320: 6e50 726f 7065 7274 7953 6563 6f6e 6461  nPropertySeconda
-00017330: 7279 290d 0a20 206a 6f69 6e65 6420 3d20  ry)..  joined = 
-00017340: 6565 2e49 6d61 6765 436f 6c6c 6563 7469  ee.ImageCollecti
-00017350: 6f6e 286a 6f69 6e2e 6170 706c 7928 6331  on(join.apply(c1
-00017360: 2c20 6332 2c20 6a6f 696e 4669 6c74 6572  , c2, joinFilter
-00017370: 2929 0d0a 0d0a 2020 6a6f 696e 6564 203d  ))....  joined =
-00017380: 2065 652e 496d 6167 6543 6f6c 6c65 6374   ee.ImageCollect
-00017390: 696f 6e28 6a6f 696e 6564 2e6d 6170 284d  ion(joined.map(M
-000173a0: 6572 6765 4261 6e64 7329 290d 0a20 2069  ergeBands))..  i
-000173b0: 6620 6d61 736b 416e 794e 756c 6c56 616c  f maskAnyNullVal
-000173c0: 7565 733a 0d0a 2020 2020 6465 6620 6e75  ues:..    def nu
-000173d0: 6c6c 6572 2869 6d67 293a 0d0a 2020 2020  ller(img):..    
-000173e0: 2020 7265 7475 726e 2069 6d67 2e6d 6173    return img.mas
-000173f0: 6b28 696d 672e 6d61 736b 2829 2e41 6e64  k(img.mask().And
-00017400: 2869 6d67 2e72 6564 7563 6528 6565 2e52  (img.reduce(ee.R
-00017410: 6564 7563 6572 2e6d 696e 2829 292e 6e65  educer.min()).ne
-00017420: 7128 3029 2929 0d0a 2020 2020 6a6f 696e  q(0)))..    join
-00017430: 6564 203d 206a 6f69 6e65 642e 6d61 7028  ed = joined.map(
-00017440: 6e75 6c6c 6572 293b 0d0a 0d0a 2020 7265  nuller);....  re
-00017450: 7475 726e 206a 6f69 6e65 643b 0d0a 0d0a  turn joined;....
-00017460: 6465 6620 736d 6172 744a 6f69 6e28 7072  def smartJoin(pr
-00017470: 696d 6172 792c 7365 636f 6e64 6172 792c  imary,secondary,
-00017480: 686f 7572 4469 6666 293a 0d0a 2020 6d69  hourDiff):..  mi
-00017490: 6c6c 6973 203d 2068 6f75 7244 6966 6620  llis = hourDiff 
-000174a0: 2a20 3630 202a 2036 3020 2a20 3130 3030  * 60 * 60 * 1000
-000174b0: 0d0a 0d0a 2020 2343 7265 6174 6520 6120  ....  #Create a 
-000174c0: 7469 6d65 2066 696c 7465 7220 746f 2064  time filter to d
-000174d0: 6566 696e 6520 6120 6d61 7463 6820 6173  efine a match as
-000174e0: 206f 7665 726c 6170 7069 6e67 2074 696d   overlapping tim
-000174f0: 6573 7461 6d70 732e 0d0a 2020 6d61 7844  estamps...  maxD
-00017500: 6966 6646 696c 7465 7220 3d20 6565 2e46  iffFilter = ee.F
-00017510: 696c 7465 722e 6d61 7844 6966 6665 7265  ilter.maxDiffere
-00017520: 6e63 6528 7b5c 0d0a 2020 2020 2764 6966  nce({\..    'dif
-00017530: 6665 7265 6e63 6527 3a20 6d69 6c6c 6973  ference': millis
-00017540: 2c5c 0d0a 2020 2020 276c 6566 7446 6965  ,\..    'leftFie
-00017550: 6c64 273a 2027 7379 7374 656d 3a74 696d  ld': 'system:tim
-00017560: 655f 7374 6172 7427 2c5c 0d0a 2020 2020  e_start',\..    
-00017570: 2772 6967 6874 4669 656c 6427 3a20 2773  'rightField': 's
-00017580: 7973 7465 6d3a 7469 6d65 5f73 7461 7274  ystem:time_start
-00017590: 275c 0d0a 2020 7d29 0d0a 2020 2344 6566  '\..  })..  #Def
-000175a0: 696e 6520 7468 6520 6a6f 696e 2e0d 0a20  ine the join... 
-000175b0: 2073 6176 6542 6573 744a 6f69 6e20 3d20   saveBestJoin = 
-000175c0: 6565 2e4a 6f69 6e2e 7361 7665 4265 7374  ee.Join.saveBest
-000175d0: 287b 5c0d 0a20 2020 2027 6d61 7463 684b  ({\..    'matchK
-000175e0: 6579 273a 2027 6265 7374 496d 6167 6527  ey': 'bestImage'
-000175f0: 2c5c 0d0a 2020 2020 276d 6561 7375 7265  ,\..    'measure
-00017600: 4b65 7927 3a20 2774 696d 6544 6966 6627  Key': 'timeDiff'
-00017610: 5c0d 0a20 207d 290d 0a20 2064 6566 204d  \..  })..  def M
-00017620: 6572 6765 4261 6e64 7328 656c 656d 656e  ergeBands(elemen
-00017630: 7429 3a0d 0a20 2020 2023 4120 6675 6e63  t):..    #A func
-00017640: 7469 6f6e 2074 6f20 6d65 7267 6520 7468  tion to merge th
-00017650: 6520 6261 6e64 7320 746f 6765 7468 6572  e bands together
-00017660: 2e0d 0a20 2020 2023 4166 7465 7220 6120  ...    #After a 
-00017670: 6a6f 696e 2c20 7265 7375 6c74 7320 6172  join, results ar
-00017680: 6520 696e 2027 7072 696d 6172 7927 2061  e in 'primary' a
-00017690: 6e64 2027 7365 636f 6e64 6172 7927 2070  nd 'secondary' p
-000176a0: 726f 7065 7274 6965 732e 0d0a 2020 2020  roperties...    
-000176b0: 7265 7475 726e 2065 652e 496d 6167 652e  return ee.Image.
-000176c0: 6361 7428 656c 656d 656e 742c 2065 6c65  cat(element, ele
-000176d0: 6d65 6e74 2e67 6574 2827 6265 7374 496d  ment.get('bestIm
-000176e0: 6167 6527 2929 0d0a 0d0a 2020 2341 7070  age'))....  #App
-000176f0: 6c79 2074 6865 206a 6f69 6e2e 0d0a 2020  ly the join...  
-00017700: 6a6f 696e 6564 203d 2073 6176 6542 6573  joined = saveBes
-00017710: 744a 6f69 6e2e 6170 706c 7928 7072 696d  tJoin.apply(prim
-00017720: 6172 792c 2073 6563 6f6e 6461 7279 2c20  ary, secondary, 
-00017730: 6d61 7844 6966 6646 696c 7465 7229 0d0a  maxDiffFilter)..
-00017740: 2020 6a6f 696e 6564 203d 206a 6f69 6e65    joined = joine
-00017750: 642e 6d61 7028 4d65 7267 6542 616e 6473  d.map(MergeBands
-00017760: 290d 0a20 2072 6574 7572 6e20 6a6f 696e  )..  return join
-00017770: 6564 0d0a 2323 2323 2323 2323 2323 2323  ed..############
+000170d0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+000170e0: 0a23 4865 6c70 6572 2066 756e 6374 696f  .#Helper functio
+000170f0: 6e20 746f 206a 6f69 6e20 7477 6f20 636f  n to join two co
+00017100: 6c6c 6563 7469 6f6e 732d 2053 6f75 7263  llections- Sourc
+00017110: 653a 2063 6f64 652e 6561 7274 6865 6e67  e: code.eartheng
+00017120: 696e 652e 676f 6f67 6c65 2e63 6f6d 0d0a  ine.google.com..
+00017130: 6465 6620 6a6f 696e 436f 6c6c 6563 7469  def joinCollecti
+00017140: 6f6e 7328 6331 2c20 6332 2c20 6d61 736b  ons(c1, c2, mask
+00017150: 416e 794e 756c 6c56 616c 7565 7320 3d20  AnyNullValues = 
+00017160: 5472 7565 2c20 6a6f 696e 5072 6f70 6572  True, joinProper
+00017170: 7479 203d 2027 7379 7374 656d 3a74 696d  ty = 'system:tim
+00017180: 655f 7374 6172 7427 2c6a 6f69 6e50 726f  e_start',joinPro
+00017190: 7065 7274 7953 6563 6f6e 6461 7279 3d4e  pertySecondary=N
+000171a0: 6f6e 6529 3a0d 0a20 200d 0a20 2069 6620  one):..  ..  if 
+000171b0: 6a6f 696e 5072 6f70 6572 7479 5365 636f  joinPropertySeco
+000171c0: 6e64 6172 793d 3d4e 6f6e 653a 6a6f 696e  ndary==None:join
+000171d0: 5072 6f70 6572 7479 5365 636f 6e64 6172  PropertySecondar
+000171e0: 793d 6a6f 696e 5072 6f70 6572 7479 0d0a  y=joinProperty..
+000171f0: 2020 0d0a 2020 6465 6620 4d65 7267 6542    ..  def MergeB
+00017200: 616e 6473 2865 6c65 6d65 6e74 293a 0d0a  ands(element):..
+00017210: 2020 2020 2341 2066 756e 6374 696f 6e20      #A function 
+00017220: 746f 206d 6572 6765 2074 6865 2062 616e  to merge the ban
+00017230: 6473 2074 6f67 6574 6865 722e 0d0a 2020  ds together...  
+00017240: 2020 2341 6674 6572 2061 206a 6f69 6e2c    #After a join,
+00017250: 2072 6573 756c 7473 2061 7265 2069 6e20   results are in 
+00017260: 2770 7269 6d61 7279 2720 616e 6420 2773  'primary' and 's
+00017270: 6563 6f6e 6461 7279 2720 7072 6f70 6572  econdary' proper
+00017280: 7469 6573 2e0d 0a20 2020 2072 6574 7572  ties...    retur
+00017290: 6e20 6565 2e49 6d61 6765 2e63 6174 2865  n ee.Image.cat(e
+000172a0: 6c65 6d65 6e74 2e67 6574 2827 7072 696d  lement.get('prim
+000172b0: 6172 7927 292c 2065 6c65 6d65 6e74 2e67  ary'), element.g
+000172c0: 6574 2827 7365 636f 6e64 6172 7927 2929  et('secondary'))
+000172d0: 0d0a 0d0a 0d0a 2020 6a6f 696e 203d 2065  ......  join = e
+000172e0: 652e 4a6f 696e 2e69 6e6e 6572 2829 0d0a  e.Join.inner()..
+000172f0: 2020 6a6f 696e 4669 6c74 6572 203d 2065    joinFilter = e
+00017300: 652e 4669 6c74 6572 2e65 7175 616c 7328  e.Filter.equals(
+00017310: 6a6f 696e 5072 6f70 6572 7479 2c20 4e6f  joinProperty, No
+00017320: 6e65 2c20 6a6f 696e 5072 6f70 6572 7479  ne, joinProperty
+00017330: 5365 636f 6e64 6172 7929 0d0a 2020 6a6f  Secondary)..  jo
+00017340: 696e 6564 203d 2065 652e 496d 6167 6543  ined = ee.ImageC
+00017350: 6f6c 6c65 6374 696f 6e28 6a6f 696e 2e61  ollection(join.a
+00017360: 7070 6c79 2863 312c 2063 322c 206a 6f69  pply(c1, c2, joi
+00017370: 6e46 696c 7465 7229 290d 0a0d 0a20 206a  nFilter))....  j
+00017380: 6f69 6e65 6420 3d20 6565 2e49 6d61 6765  oined = ee.Image
+00017390: 436f 6c6c 6563 7469 6f6e 286a 6f69 6e65  Collection(joine
+000173a0: 642e 6d61 7028 4d65 7267 6542 616e 6473  d.map(MergeBands
+000173b0: 2929 0d0a 2020 6966 206d 6173 6b41 6e79  ))..  if maskAny
+000173c0: 4e75 6c6c 5661 6c75 6573 3a0d 0a20 2020  NullValues:..   
+000173d0: 2064 6566 206e 756c 6c65 7228 696d 6729   def nuller(img)
+000173e0: 3a0d 0a20 2020 2020 2072 6574 7572 6e20  :..      return 
+000173f0: 696d 672e 6d61 736b 2869 6d67 2e6d 6173  img.mask(img.mas
+00017400: 6b28 292e 416e 6428 696d 672e 7265 6475  k().And(img.redu
+00017410: 6365 2865 652e 5265 6475 6365 722e 6d69  ce(ee.Reducer.mi
+00017420: 6e28 2929 2e6e 6571 2830 2929 290d 0a20  n()).neq(0))).. 
+00017430: 2020 206a 6f69 6e65 6420 3d20 6a6f 696e     joined = join
+00017440: 6564 2e6d 6170 286e 756c 6c65 7229 3b0d  ed.map(nuller);.
+00017450: 0a0d 0a20 2072 6574 7572 6e20 6a6f 696e  ...  return join
+00017460: 6564 3b0d 0a0d 0a64 6566 2073 6d61 7274  ed;....def smart
+00017470: 4a6f 696e 2870 7269 6d61 7279 2c73 6563  Join(primary,sec
+00017480: 6f6e 6461 7279 2c68 6f75 7244 6966 6629  ondary,hourDiff)
+00017490: 3a0d 0a20 206d 696c 6c69 7320 3d20 686f  :..  millis = ho
+000174a0: 7572 4469 6666 202a 2036 3020 2a20 3630  urDiff * 60 * 60
+000174b0: 202a 2031 3030 300d 0a0d 0a20 2023 4372   * 1000....  #Cr
+000174c0: 6561 7465 2061 2074 696d 6520 6669 6c74  eate a time filt
+000174d0: 6572 2074 6f20 6465 6669 6e65 2061 206d  er to define a m
+000174e0: 6174 6368 2061 7320 6f76 6572 6c61 7070  atch as overlapp
+000174f0: 696e 6720 7469 6d65 7374 616d 7073 2e0d  ing timestamps..
+00017500: 0a20 206d 6178 4469 6666 4669 6c74 6572  .  maxDiffFilter
+00017510: 203d 2065 652e 4669 6c74 6572 2e6d 6178   = ee.Filter.max
+00017520: 4469 6666 6572 656e 6365 287b 5c0d 0a20  Difference({\.. 
+00017530: 2020 2027 6469 6666 6572 656e 6365 273a     'difference':
+00017540: 206d 696c 6c69 732c 5c0d 0a20 2020 2027   millis,\..    '
+00017550: 6c65 6674 4669 656c 6427 3a20 2773 7973  leftField': 'sys
+00017560: 7465 6d3a 7469 6d65 5f73 7461 7274 272c  tem:time_start',
+00017570: 5c0d 0a20 2020 2027 7269 6768 7446 6965  \..    'rightFie
+00017580: 6c64 273a 2027 7379 7374 656d 3a74 696d  ld': 'system:tim
+00017590: 655f 7374 6172 7427 5c0d 0a20 207d 290d  e_start'\..  }).
+000175a0: 0a20 2023 4465 6669 6e65 2074 6865 206a  .  #Define the j
+000175b0: 6f69 6e2e 0d0a 2020 7361 7665 4265 7374  oin...  saveBest
+000175c0: 4a6f 696e 203d 2065 652e 4a6f 696e 2e73  Join = ee.Join.s
+000175d0: 6176 6542 6573 7428 7b5c 0d0a 2020 2020  aveBest({\..    
+000175e0: 276d 6174 6368 4b65 7927 3a20 2762 6573  'matchKey': 'bes
+000175f0: 7449 6d61 6765 272c 5c0d 0a20 2020 2027  tImage',\..    '
+00017600: 6d65 6173 7572 654b 6579 273a 2027 7469  measureKey': 'ti
+00017610: 6d65 4469 6666 275c 0d0a 2020 7d29 0d0a  meDiff'\..  })..
+00017620: 2020 6465 6620 4d65 7267 6542 616e 6473    def MergeBands
+00017630: 2865 6c65 6d65 6e74 293a 0d0a 2020 2020  (element):..    
+00017640: 2341 2066 756e 6374 696f 6e20 746f 206d  #A function to m
+00017650: 6572 6765 2074 6865 2062 616e 6473 2074  erge the bands t
+00017660: 6f67 6574 6865 722e 0d0a 2020 2020 2341  ogether...    #A
+00017670: 6674 6572 2061 206a 6f69 6e2c 2072 6573  fter a join, res
+00017680: 756c 7473 2061 7265 2069 6e20 2770 7269  ults are in 'pri
+00017690: 6d61 7279 2720 616e 6420 2773 6563 6f6e  mary' and 'secon
+000176a0: 6461 7279 2720 7072 6f70 6572 7469 6573  dary' properties
+000176b0: 2e0d 0a20 2020 2072 6574 7572 6e20 6565  ...    return ee
+000176c0: 2e49 6d61 6765 2e63 6174 2865 6c65 6d65  .Image.cat(eleme
+000176d0: 6e74 2c20 656c 656d 656e 742e 6765 7428  nt, element.get(
+000176e0: 2762 6573 7449 6d61 6765 2729 290d 0a0d  'bestImage'))...
+000176f0: 0a20 2023 4170 706c 7920 7468 6520 6a6f  .  #Apply the jo
+00017700: 696e 2e0d 0a20 206a 6f69 6e65 6420 3d20  in...  joined = 
+00017710: 7361 7665 4265 7374 4a6f 696e 2e61 7070  saveBestJoin.app
+00017720: 6c79 2870 7269 6d61 7279 2c20 7365 636f  ly(primary, seco
+00017730: 6e64 6172 792c 206d 6178 4469 6666 4669  ndary, maxDiffFi
+00017740: 6c74 6572 290d 0a20 206a 6f69 6e65 6420  lter)..  joined 
+00017750: 3d20 6a6f 696e 6564 2e6d 6170 284d 6572  = joined.map(Mer
+00017760: 6765 4261 6e64 7329 0d0a 2020 7265 7475  geBands)..  retu
+00017770: 726e 206a 6f69 6e65 640d 0a23 2323 2323  rn joined..#####
 00017780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00017790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000177a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000177b0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-000177c0: 4a6f 696e 2063 6f6c 6c65 6374 696f 6e73  Join collections
-000177d0: 2062 7920 7370 6163 6520 2869 6e74 6572   by space (inter
-000177e0: 7365 6374 696f 6e29 2061 6e64 2074 696d  section) and tim
-000177f0: 6520 2873 7065 6369 6669 6564 2062 7920  e (specified by 
-00017800: 7573 6572 290d 0a64 6566 2073 7061 7469  user)..def spati
-00017810: 6f54 656d 706f 7261 6c4a 6f69 6e28 7072  oTemporalJoin(pr
-00017820: 696d 6172 792c 2073 6563 6f6e 6461 7279  imary, secondary
-00017830: 2c20 686f 7572 4469 6666 203d 2032 342c  , hourDiff = 24,
-00017840: 206f 7574 4b65 7920 3d20 2773 6563 6f6e   outKey = 'secon
-00017850: 6461 7279 2729 3a0d 0a20 2074 696d 6520  dary'):..  time 
-00017860: 3d20 686f 7572 4469 6666 2a20 3630 202a  = hourDiff* 60 *
-00017870: 2036 3020 2a20 3130 3030 0d0a 0d0a 2020   60 * 1000....  
-00017880: 6f75 7442 6e73 203d 2065 652e 496d 6167  outBns = ee.Imag
-00017890: 6528 7365 636f 6e64 6172 792e 6669 7273  e(secondary.firs
-000178a0: 7428 2929 2e62 616e 644e 616d 6573 2829  t()).bandNames()
-000178b0: 2e6d 6170 286c 616d 6264 6120 626e 3a20  .map(lambda bn: 
-000178c0: 6565 2e53 7472 696e 6728 626e 292e 6361  ee.String(bn).ca
-000178d0: 7428 275f 2729 2e63 6174 286f 7574 4b65  t('_').cat(outKe
-000178e0: 7929 290d 0a20 2023 4465 6669 6e65 2061  y))..  #Define a
-000178f0: 2073 7061 7469 616c 2066 696c 7465 7220   spatial filter 
-00017900: 6173 2067 656f 6d65 7472 6965 7320 7468  as geometries th
-00017910: 6174 2069 6e74 6572 7365 6374 2e0d 0a20  at intersect... 
-00017920: 2073 7061 7469 6f54 656d 706f 7261 6c46   spatioTemporalF
-00017930: 696c 7465 7220 3d20 6565 2e46 696c 7465  ilter = ee.Filte
-00017940: 722e 416e 6428 5c0d 0a20 2020 2065 652e  r.And(\..    ee.
-00017950: 4669 6c74 6572 2e6d 6178 4469 6666 6572  Filter.maxDiffer
-00017960: 656e 6365 287b 5c0d 0a20 2020 2020 2027  ence({\..      '
-00017970: 6469 6666 6572 656e 6365 273a 2074 696d  difference': tim
-00017980: 652c 5c0d 0a20 2020 2020 2027 6c65 6674  e,\..      'left
-00017990: 4669 656c 6427 3a20 2773 7973 7465 6d3a  Field': 'system:
-000179a0: 7469 6d65 5f73 7461 7274 272c 5c0d 0a20  time_start',\.. 
-000179b0: 2020 2020 2027 7269 6768 7446 6965 6c64       'rightField
-000179c0: 273a 2027 7379 7374 656d 3a74 696d 655f  ': 'system:time_
-000179d0: 7374 6172 7427 5c0d 0a20 2020 207d 292c  start'\..    }),
-000179e0: 5c0d 0a20 2020 2065 652e 4669 6c74 6572  \..    ee.Filter
-000179f0: 2e69 6e74 6572 7365 6374 7328 7b5c 0d0a  .intersects({\..
-00017a00: 2020 2020 276c 6566 7446 6965 6c64 273a      'leftField':
-00017a10: 2027 2e67 656f 272c 5c0d 0a20 2020 2027   '.geo',\..    '
-00017a20: 7269 6768 7446 6965 6c64 273a 2027 2e67  rightField': '.g
-00017a30: 656f 272c 5c0d 0a20 2020 2027 6d61 7845  eo',\..    'maxE
-00017a40: 7272 6f72 273a 2031 305c 0d0a 2020 7d29  rror': 10\..  })
-00017a50: 5c0d 0a20 2029 0d0a 2020 2344 6566 696e  \..  )..  #Defin
-00017a60: 6520 6120 7361 7665 2061 6c6c 206a 6f69  e a save all joi
-00017a70: 6e2e 0d0a 2020 7361 7665 4265 7374 4a6f  n...  saveBestJo
-00017a80: 696e 203d 2065 652e 4a6f 696e 2e73 6176  in = ee.Join.sav
-00017a90: 6542 6573 7428 7b5c 0d0a 2020 2020 276d  eBest({\..    'm
-00017aa0: 6174 6368 4b65 7927 3a20 6f75 744b 6579  atchKey': outKey
-00017ab0: 2c5c 0d0a 2020 2020 276d 6561 7375 7265  ,\..    'measure
-00017ac0: 4b65 7927 3a20 2774 696d 6544 6966 6627  Key': 'timeDiff'
-00017ad0: 5c0d 0a20 207d 290d 0a0d 0a20 2023 4170  \..  })....  #Ap
-00017ae0: 706c 7920 7468 6520 6a6f 696e 2e0d 0a20  ply the join... 
-00017af0: 206a 6f69 6e65 6420 3d20 7361 7665 4265   joined = saveBe
-00017b00: 7374 4a6f 696e 2e61 7070 6c79 2870 7269  stJoin.apply(pri
-00017b10: 6d61 7279 2c20 7365 636f 6e64 6172 792c  mary, secondary,
-00017b20: 2073 7061 7469 6f54 656d 706f 7261 6c46   spatioTemporalF
-00017b30: 696c 7465 7229 0d0a 2020 6465 6620 4d65  ilter)..  def Me
-00017b40: 7267 6542 616e 6473 2865 6c65 6d65 6e74  rgeBands(element
-00017b50: 293a 0d0a 2020 2020 2341 2066 756e 6374  ):..    #A funct
-00017b60: 696f 6e20 746f 206d 6572 6765 2074 6865  ion to merge the
-00017b70: 2062 616e 6473 2074 6f67 6574 6865 722e   bands together.
-00017b80: 0d0a 2020 2020 2341 6674 6572 2061 206a  ..    #After a j
-00017b90: 6f69 6e2c 2072 6573 756c 7473 2061 7265  oin, results are
-00017ba0: 2069 6e20 2770 7269 6d61 7279 2720 616e   in 'primary' an
-00017bb0: 6420 2773 6563 6f6e 6461 7279 2720 7072  d 'secondary' pr
-00017bc0: 6f70 6572 7469 6573 2e0d 0a20 2020 2072  operties...    r
-00017bd0: 6574 7572 6e20 6565 2e49 6d61 6765 2e63  eturn ee.Image.c
-00017be0: 6174 2865 6c65 6d65 6e74 2c20 6565 2e49  at(element, ee.I
-00017bf0: 6d61 6765 2865 6c65 6d65 6e74 2e67 6574  mage(element.get
-00017c00: 286f 7574 4b65 7929 292e 7265 6e61 6d65  (outKey)).rename
-00017c10: 286f 7574 426e 7329 290d 0a0d 0a20 206a  (outBns))....  j
-00017c20: 6f69 6e65 6420 3d20 6a6f 696e 6564 2e6d  oined = joined.m
-00017c30: 6170 284d 6572 6765 4261 6e64 7329 0d0a  ap(MergeBands)..
-00017c40: 2020 7265 7475 726e 206a 6f69 6e65 640d    return joined.
-00017c50: 0a0d 0a23 2053 696d 706c 6520 696e 6e65  ...# Simple inne
-00017c60: 7220 6a6f 696e 2066 756e 6374 696f 6e20  r join function 
-00017c70: 666f 7220 6665 6174 7572 6543 6f6c 6c65  for featureColle
-00017c80: 6374 696f 6e73 0d0a 2320 4d61 7463 6865  ctions..# Matche
-00017c90: 7320 6665 6174 7572 6573 2062 6173 6564  s features based
-00017ca0: 206f 6e20 616e 2065 7861 6374 206d 6174   on an exact mat
-00017cb0: 6368 206f 6620 7468 6520 6669 656c 644e  ch of the fieldN
-00017cc0: 616d 6520 7061 7261 6d65 7465 720d 0a23  ame parameter..#
-00017cd0: 2041 6e20 6f70 7469 6f6e 616c 2064 6966   An optional dif
-00017ce0: 6665 7265 6e74 2066 6965 6c64 206e 616d  ferent field nam
-00017cf0: 6520 6361 6e20 6265 2070 726f 7669 6465  e can be provide
-00017d00: 6420 666f 7220 7468 6520 7365 636f 6e64  d for the second
-00017d10: 2066 6561 7475 7265 436f 6c6c 6563 7469   featureCollecti
-00017d20: 6f6e 0d0a 2320 5265 7461 696e 7320 7468  on..# Retains th
-00017d30: 6520 6765 6f6d 6574 7279 206f 6620 7468  e geometry of th
-00017d40: 6520 7072 696d 6172 792c 2062 7574 2063  e primary, but c
-00017d50: 6f70 6965 7320 7468 6520 7072 6f70 6572  opies the proper
-00017d60: 7469 6573 206f 6620 7468 6520 7365 636f  ties of the seco
-00017d70: 6e64 6172 7920 636f 6c6c 6563 7469 6f6e  ndary collection
-00017d80: 0d0a 6465 6620 6a6f 696e 4665 6174 7572  ..def joinFeatur
-00017d90: 6543 6f6c 6c65 6374 696f 6e73 2870 7269  eCollections(pri
-00017da0: 6d61 7279 2c73 6563 6f6e 6461 7279 2c66  mary,secondary,f
-00017db0: 6965 6c64 4e61 6d65 2c66 6965 6c64 4e61  ieldName,fieldNa
-00017dc0: 6d65 5365 636f 6e64 6172 793d 4e6f 6e65  meSecondary=None
-00017dd0: 293a 0d0a 2020 6966 2066 6965 6c64 4e61  ):..  if fieldNa
-00017de0: 6d65 5365 636f 6e64 6172 793d 3d4e 6f6e  meSecondary==Non
-00017df0: 653a 6669 656c 644e 616d 6553 6563 6f6e  e:fieldNameSecon
-00017e00: 6461 7279 3d66 6965 6c64 4e61 6d65 0d0a  dary=fieldName..
-00017e10: 2020 2320 5573 6520 616e 2065 7175 616c    # Use an equal
-00017e20: 7320 6669 6c74 6572 2074 6f20 7370 6563  s filter to spec
-00017e30: 6966 7920 686f 7720 7468 6520 636f 6c6c  ify how the coll
-00017e40: 6563 7469 6f6e 7320 6d61 7463 682e 0d0a  ections match...
-00017e50: 2020 6620 3d20 6565 2e46 696c 7465 722e    f = ee.Filter.
-00017e60: 6571 7561 6c73 2866 6965 6c64 4e61 6d65  equals(fieldName
-00017e70: 2c4e 6f6e 652c 6669 656c 644e 616d 6553  ,None,fieldNameS
-00017e80: 6563 6f6e 6461 7279 290d 0a0d 0a0d 0a20  econdary)...... 
-00017e90: 2023 2044 6566 696e 6520 7468 6520 6a6f   # Define the jo
-00017ea0: 696e 2e0d 0a20 2069 6e6e 6572 4a6f 696e  in...  innerJoin
-00017eb0: 203d 2065 652e 4a6f 696e 2e69 6e6e 6572   = ee.Join.inner
-00017ec0: 2827 7072 696d 6172 7927 2c20 2773 6563  ('primary', 'sec
-00017ed0: 6f6e 6461 7279 2729 0d0a 0d0a 2020 2320  ondary')....  # 
-00017ee0: 4170 706c 7920 7468 6520 6a6f 696e 2e0d  Apply the join..
-00017ef0: 0a20 206a 6f69 6e65 6420 3d20 696e 6e65  .  joined = inne
-00017f00: 724a 6f69 6e2e 6170 706c 7928 7072 696d  rJoin.apply(prim
-00017f10: 6172 792c 2073 6563 6f6e 6461 7279 2c20  ary, secondary, 
-00017f20: 6629 0d0a 2020 6a6f 696e 6564 203d 206a  f)..  joined = j
-00017f30: 6f69 6e65 642e 6d61 7028 6c61 6d62 6461  oined.map(lambda
-00017f40: 2066 3a20 6565 2e46 6561 7475 7265 2866   f: ee.Feature(f
-00017f50: 2e67 6574 2827 7072 696d 6172 7927 2929  .get('primary'))
-00017f60: 2e63 6f70 7950 726f 7065 7274 6965 7328  .copyProperties(
-00017f70: 6565 2e46 6561 7475 7265 2866 2e67 6574  ee.Feature(f.get
-00017f80: 2827 7365 636f 6e64 6172 7927 2929 2929  ('secondary'))))
-00017f90: 0d0a 0d0a 2020 7265 7475 726e 206a 6f69  ....  return joi
-00017fa0: 6e65 640d 0a23 2323 2323 2323 2323 2323  ned..###########
+000177b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000177c0: 2323 2323 0d0a 234a 6f69 6e20 636f 6c6c  ####..#Join coll
+000177d0: 6563 7469 6f6e 7320 6279 2073 7061 6365  ections by space
+000177e0: 2028 696e 7465 7273 6563 7469 6f6e 2920   (intersection) 
+000177f0: 616e 6420 7469 6d65 2028 7370 6563 6966  and time (specif
+00017800: 6965 6420 6279 2075 7365 7229 0d0a 6465  ied by user)..de
+00017810: 6620 7370 6174 696f 5465 6d70 6f72 616c  f spatioTemporal
+00017820: 4a6f 696e 2870 7269 6d61 7279 2c20 7365  Join(primary, se
+00017830: 636f 6e64 6172 792c 2068 6f75 7244 6966  condary, hourDif
+00017840: 6620 3d20 3234 2c20 6f75 744b 6579 203d  f = 24, outKey =
+00017850: 2027 7365 636f 6e64 6172 7927 293a 0d0a   'secondary'):..
+00017860: 2020 7469 6d65 203d 2068 6f75 7244 6966    time = hourDif
+00017870: 662a 2036 3020 2a20 3630 202a 2031 3030  f* 60 * 60 * 100
+00017880: 300d 0a0d 0a20 206f 7574 426e 7320 3d20  0....  outBns = 
+00017890: 6565 2e49 6d61 6765 2873 6563 6f6e 6461  ee.Image(seconda
+000178a0: 7279 2e66 6972 7374 2829 292e 6261 6e64  ry.first()).band
+000178b0: 4e61 6d65 7328 292e 6d61 7028 6c61 6d62  Names().map(lamb
+000178c0: 6461 2062 6e3a 2065 652e 5374 7269 6e67  da bn: ee.String
+000178d0: 2862 6e29 2e63 6174 2827 5f27 292e 6361  (bn).cat('_').ca
+000178e0: 7428 6f75 744b 6579 2929 0d0a 2020 2344  t(outKey))..  #D
+000178f0: 6566 696e 6520 6120 7370 6174 6961 6c20  efine a spatial 
+00017900: 6669 6c74 6572 2061 7320 6765 6f6d 6574  filter as geomet
+00017910: 7269 6573 2074 6861 7420 696e 7465 7273  ries that inters
+00017920: 6563 742e 0d0a 2020 7370 6174 696f 5465  ect...  spatioTe
+00017930: 6d70 6f72 616c 4669 6c74 6572 203d 2065  mporalFilter = e
+00017940: 652e 4669 6c74 6572 2e41 6e64 285c 0d0a  e.Filter.And(\..
+00017950: 2020 2020 6565 2e46 696c 7465 722e 6d61      ee.Filter.ma
+00017960: 7844 6966 6665 7265 6e63 6528 7b5c 0d0a  xDifference({\..
+00017970: 2020 2020 2020 2764 6966 6665 7265 6e63        'differenc
+00017980: 6527 3a20 7469 6d65 2c5c 0d0a 2020 2020  e': time,\..    
+00017990: 2020 276c 6566 7446 6965 6c64 273a 2027    'leftField': '
+000179a0: 7379 7374 656d 3a74 696d 655f 7374 6172  system:time_star
+000179b0: 7427 2c5c 0d0a 2020 2020 2020 2772 6967  t',\..      'rig
+000179c0: 6874 4669 656c 6427 3a20 2773 7973 7465  htField': 'syste
+000179d0: 6d3a 7469 6d65 5f73 7461 7274 275c 0d0a  m:time_start'\..
+000179e0: 2020 2020 7d29 2c5c 0d0a 2020 2020 6565      }),\..    ee
+000179f0: 2e46 696c 7465 722e 696e 7465 7273 6563  .Filter.intersec
+00017a00: 7473 287b 5c0d 0a20 2020 2027 6c65 6674  ts({\..    'left
+00017a10: 4669 656c 6427 3a20 272e 6765 6f27 2c5c  Field': '.geo',\
+00017a20: 0d0a 2020 2020 2772 6967 6874 4669 656c  ..    'rightFiel
+00017a30: 6427 3a20 272e 6765 6f27 2c5c 0d0a 2020  d': '.geo',\..  
+00017a40: 2020 276d 6178 4572 726f 7227 3a20 3130    'maxError': 10
+00017a50: 5c0d 0a20 207d 295c 0d0a 2020 290d 0a20  \..  })\..  ).. 
+00017a60: 2023 4465 6669 6e65 2061 2073 6176 6520   #Define a save 
+00017a70: 616c 6c20 6a6f 696e 2e0d 0a20 2073 6176  all join...  sav
+00017a80: 6542 6573 744a 6f69 6e20 3d20 6565 2e4a  eBestJoin = ee.J
+00017a90: 6f69 6e2e 7361 7665 4265 7374 287b 5c0d  oin.saveBest({\.
+00017aa0: 0a20 2020 2027 6d61 7463 684b 6579 273a  .    'matchKey':
+00017ab0: 206f 7574 4b65 792c 5c0d 0a20 2020 2027   outKey,\..    '
+00017ac0: 6d65 6173 7572 654b 6579 273a 2027 7469  measureKey': 'ti
+00017ad0: 6d65 4469 6666 275c 0d0a 2020 7d29 0d0a  meDiff'\..  })..
+00017ae0: 0d0a 2020 2341 7070 6c79 2074 6865 206a  ..  #Apply the j
+00017af0: 6f69 6e2e 0d0a 2020 6a6f 696e 6564 203d  oin...  joined =
+00017b00: 2073 6176 6542 6573 744a 6f69 6e2e 6170   saveBestJoin.ap
+00017b10: 706c 7928 7072 696d 6172 792c 2073 6563  ply(primary, sec
+00017b20: 6f6e 6461 7279 2c20 7370 6174 696f 5465  ondary, spatioTe
+00017b30: 6d70 6f72 616c 4669 6c74 6572 290d 0a20  mporalFilter).. 
+00017b40: 2064 6566 204d 6572 6765 4261 6e64 7328   def MergeBands(
+00017b50: 656c 656d 656e 7429 3a0d 0a20 2020 2023  element):..    #
+00017b60: 4120 6675 6e63 7469 6f6e 2074 6f20 6d65  A function to me
+00017b70: 7267 6520 7468 6520 6261 6e64 7320 746f  rge the bands to
+00017b80: 6765 7468 6572 2e0d 0a20 2020 2023 4166  gether...    #Af
+00017b90: 7465 7220 6120 6a6f 696e 2c20 7265 7375  ter a join, resu
+00017ba0: 6c74 7320 6172 6520 696e 2027 7072 696d  lts are in 'prim
+00017bb0: 6172 7927 2061 6e64 2027 7365 636f 6e64  ary' and 'second
+00017bc0: 6172 7927 2070 726f 7065 7274 6965 732e  ary' properties.
+00017bd0: 0d0a 2020 2020 7265 7475 726e 2065 652e  ..    return ee.
+00017be0: 496d 6167 652e 6361 7428 656c 656d 656e  Image.cat(elemen
+00017bf0: 742c 2065 652e 496d 6167 6528 656c 656d  t, ee.Image(elem
+00017c00: 656e 742e 6765 7428 6f75 744b 6579 2929  ent.get(outKey))
+00017c10: 2e72 656e 616d 6528 6f75 7442 6e73 2929  .rename(outBns))
+00017c20: 0d0a 0d0a 2020 6a6f 696e 6564 203d 206a  ....  joined = j
+00017c30: 6f69 6e65 642e 6d61 7028 4d65 7267 6542  oined.map(MergeB
+00017c40: 616e 6473 290d 0a20 2072 6574 7572 6e20  ands)..  return 
+00017c50: 6a6f 696e 6564 0d0a 0d0a 2320 5369 6d70  joined....# Simp
+00017c60: 6c65 2069 6e6e 6572 206a 6f69 6e20 6675  le inner join fu
+00017c70: 6e63 7469 6f6e 2066 6f72 2066 6561 7475  nction for featu
+00017c80: 7265 436f 6c6c 6563 7469 6f6e 730d 0a23  reCollections..#
+00017c90: 204d 6174 6368 6573 2066 6561 7475 7265   Matches feature
+00017ca0: 7320 6261 7365 6420 6f6e 2061 6e20 6578  s based on an ex
+00017cb0: 6163 7420 6d61 7463 6820 6f66 2074 6865  act match of the
+00017cc0: 2066 6965 6c64 4e61 6d65 2070 6172 616d   fieldName param
+00017cd0: 6574 6572 0d0a 2320 416e 206f 7074 696f  eter..# An optio
+00017ce0: 6e61 6c20 6469 6666 6572 656e 7420 6669  nal different fi
+00017cf0: 656c 6420 6e61 6d65 2063 616e 2062 6520  eld name can be 
+00017d00: 7072 6f76 6964 6564 2066 6f72 2074 6865  provided for the
+00017d10: 2073 6563 6f6e 6420 6665 6174 7572 6543   second featureC
+00017d20: 6f6c 6c65 6374 696f 6e0d 0a23 2052 6574  ollection..# Ret
+00017d30: 6169 6e73 2074 6865 2067 656f 6d65 7472  ains the geometr
+00017d40: 7920 6f66 2074 6865 2070 7269 6d61 7279  y of the primary
+00017d50: 2c20 6275 7420 636f 7069 6573 2074 6865  , but copies the
+00017d60: 2070 726f 7065 7274 6965 7320 6f66 2074   properties of t
+00017d70: 6865 2073 6563 6f6e 6461 7279 2063 6f6c  he secondary col
+00017d80: 6c65 6374 696f 6e0d 0a64 6566 206a 6f69  lection..def joi
+00017d90: 6e46 6561 7475 7265 436f 6c6c 6563 7469  nFeatureCollecti
+00017da0: 6f6e 7328 7072 696d 6172 792c 7365 636f  ons(primary,seco
+00017db0: 6e64 6172 792c 6669 656c 644e 616d 652c  ndary,fieldName,
+00017dc0: 6669 656c 644e 616d 6553 6563 6f6e 6461  fieldNameSeconda
+00017dd0: 7279 3d4e 6f6e 6529 3a0d 0a20 2069 6620  ry=None):..  if 
+00017de0: 6669 656c 644e 616d 6553 6563 6f6e 6461  fieldNameSeconda
+00017df0: 7279 3d3d 4e6f 6e65 3a66 6965 6c64 4e61  ry==None:fieldNa
+00017e00: 6d65 5365 636f 6e64 6172 793d 6669 656c  meSecondary=fiel
+00017e10: 644e 616d 650d 0a20 2023 2055 7365 2061  dName..  # Use a
+00017e20: 6e20 6571 7561 6c73 2066 696c 7465 7220  n equals filter 
+00017e30: 746f 2073 7065 6369 6679 2068 6f77 2074  to specify how t
+00017e40: 6865 2063 6f6c 6c65 6374 696f 6e73 206d  he collections m
+00017e50: 6174 6368 2e0d 0a20 2066 203d 2065 652e  atch...  f = ee.
+00017e60: 4669 6c74 6572 2e65 7175 616c 7328 6669  Filter.equals(fi
+00017e70: 656c 644e 616d 652c 4e6f 6e65 2c66 6965  eldName,None,fie
+00017e80: 6c64 4e61 6d65 5365 636f 6e64 6172 7929  ldNameSecondary)
+00017e90: 0d0a 0d0a 0d0a 2020 2320 4465 6669 6e65  ......  # Define
+00017ea0: 2074 6865 206a 6f69 6e2e 0d0a 2020 696e   the join...  in
+00017eb0: 6e65 724a 6f69 6e20 3d20 6565 2e4a 6f69  nerJoin = ee.Joi
+00017ec0: 6e2e 696e 6e65 7228 2770 7269 6d61 7279  n.inner('primary
+00017ed0: 272c 2027 7365 636f 6e64 6172 7927 290d  ', 'secondary').
+00017ee0: 0a0d 0a20 2023 2041 7070 6c79 2074 6865  ...  # Apply the
+00017ef0: 206a 6f69 6e2e 0d0a 2020 6a6f 696e 6564   join...  joined
+00017f00: 203d 2069 6e6e 6572 4a6f 696e 2e61 7070   = innerJoin.app
+00017f10: 6c79 2870 7269 6d61 7279 2c20 7365 636f  ly(primary, seco
+00017f20: 6e64 6172 792c 2066 290d 0a20 206a 6f69  ndary, f)..  joi
+00017f30: 6e65 6420 3d20 6a6f 696e 6564 2e6d 6170  ned = joined.map
+00017f40: 286c 616d 6264 6120 663a 2065 652e 4665  (lambda f: ee.Fe
+00017f50: 6174 7572 6528 662e 6765 7428 2770 7269  ature(f.get('pri
+00017f60: 6d61 7279 2729 292e 636f 7079 5072 6f70  mary')).copyProp
+00017f70: 6572 7469 6573 2865 652e 4665 6174 7572  erties(ee.Featur
+00017f80: 6528 662e 6765 7428 2773 6563 6f6e 6461  e(f.get('seconda
+00017f90: 7279 2729 2929 290d 0a0d 0a20 2072 6574  ry'))))....  ret
+00017fa0: 7572 6e20 6a6f 696e 6564 0d0a 2323 2323  urn joined..####
 00017fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00017fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00017fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00017fe0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00017ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00017fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00017ff0: 2323 2323 230d 0a23 2323 2323 2323 2323  #####..#########
 00018000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018030: 2323 2323 2323 2323 230d 0a23 4d65 7468  #########..#Meth
-00018040: 6f64 2066 6f72 2072 656d 6f76 696e 6720  od for removing 
-00018050: 7370 696b 6573 2069 6e20 7469 6d65 2073  spikes in time s
-00018060: 6572 6965 730d 0a64 6566 2064 6573 7069  eries..def despi
-00018070: 6b65 436f 6c6c 6563 7469 6f6e 2863 2c20  keCollection(c, 
-00018080: 6162 736f 6c75 7465 5370 696b 652c 2062  absoluteSpike, b
-00018090: 616e 644e 6f29 3a0d 0a20 2063 203d 2063  andNo):..  c = c
-000180a0: 2e74 6f4c 6973 7428 3130 3030 302c 3029  .toList(10000,0)
-000180b0: 0d0a 0d0a 2020 2347 6574 2062 6f6f 6b20  ....  #Get book 
-000180c0: 656e 6473 2066 6f72 2061 6464 696e 6720  ends for adding 
-000180d0: 6261 636b 2061 7420 7468 6520 656e 640d  back at the end.
-000180e0: 0a20 2066 6972 7374 203d 2063 2e73 6c69  .  first = c.sli
-000180f0: 6365 2830 2c31 290d 0a20 206c 6173 7420  ce(0,1)..  last 
-00018100: 3d20 632e 736c 6963 6528 2d31 2c4e 6f6e  = c.slice(-1,Non
-00018110: 6529 0d0a 0d0a 2020 2353 6c69 6365 2074  e)....  #Slice t
-00018120: 6865 206c 6566 742c 2063 656e 7465 722c  he left, center,
-00018130: 2061 6e64 2072 6967 6874 2066 6f72 2074   and right for t
-00018140: 6865 206d 6f76 696e 6720 7769 6e64 6f77  he moving window
-00018150: 0d0a 2020 6c65 6674 203d 2063 2e73 6c69  ..  left = c.sli
-00018160: 6365 2830 2c2d 3229 0d0a 2020 6365 6e74  ce(0,-2)..  cent
-00018170: 6572 203d 2063 2e73 6c69 6365 2831 2c2d  er = c.slice(1,-
-00018180: 3129 0d0a 2020 7269 6768 7420 3d20 632e  1)..  right = c.
-00018190: 736c 6963 6528 322c 4e6f 6e65 290d 0a0d  slice(2,None)...
-000181a0: 0a20 2023 4669 6e64 2068 6f77 206d 616e  .  #Find how man
-000181b0: 7920 696d 6167 6573 2074 6865 7265 2061  y images there a
-000181c0: 7265 2074 6f20 636f 6d70 6172 650d 0a20  re to compare.. 
-000181d0: 2073 6571 203d 2065 652e 4c69 7374 2e73   seq = ee.List.s
-000181e0: 6571 7565 6e63 6528 302c 6c65 6674 2e6c  equence(0,left.l
-000181f0: 656e 6774 6828 292e 7375 6274 7261 6374  ength().subtract
-00018200: 2831 2929 0d0a 0d0a 2020 2343 6f6d 7061  (1))....  #Compa
-00018210: 7265 2074 6865 2063 656e 7465 7220 746f  re the center to
-00018220: 2074 6865 206c 6566 7420 616e 6420 7269   the left and ri
-00018230: 6768 7420 696d 6167 6573 0d0a 2020 6465  ght images..  de
-00018240: 6620 636f 6d70 6172 6528 6929 3a0d 0a20  f compare(i):.. 
-00018250: 2020 206c 7420 3d20 6565 2e49 6d61 6765     lt = ee.Image
-00018260: 286c 6566 742e 6765 7428 6929 290d 0a20  (left.get(i)).. 
-00018270: 2020 2072 7420 3d20 6565 2e49 6d61 6765     rt = ee.Image
-00018280: 2872 6967 6874 2e67 6574 2869 2929 0d0a  (right.get(i))..
-00018290: 0d0a 2020 2020 6374 203d 2065 652e 496d  ..    ct = ee.Im
-000182a0: 6167 6528 6365 6e74 6572 2e67 6574 2869  age(center.get(i
-000182b0: 2929 3b0d 0a20 2020 2074 696d 655f 7374  ));..    time_st
-000182c0: 6172 7420 3d20 6374 2e67 6574 2827 7379  art = ct.get('sy
-000182d0: 7374 656d 3a74 696d 655f 7374 6172 7427  stem:time_start'
-000182e0: 290d 0a20 2020 2074 696d 655f 656e 6420  )..    time_end 
-000182f0: 3d20 6374 2e67 6574 2827 7379 7374 656d  = ct.get('system
-00018300: 3a74 696d 655f 656e 6427 290d 0a20 2020  :time_end')..   
-00018310: 2073 6920 3d20 6374 2e67 6574 2827 7379   si = ct.get('sy
-00018320: 7374 656d 3a69 6e64 6578 2729 0d0a 0d0a  stem:index')....
-00018330: 0d0a 0d0a 2020 2020 6469 6666 3120 3d20  ....    diff1 = 
-00018340: 6374 2e73 656c 6563 7428 5b62 616e 644e  ct.select([bandN
-00018350: 6f5d 292e 6164 6428 3129 2e73 7562 7472  o]).add(1).subtr
-00018360: 6163 7428 6c74 2e73 656c 6563 7428 5b62  act(lt.select([b
-00018370: 616e 644e 6f5d 292e 6164 6428 3129 290d  andNo]).add(1)).
-00018380: 0a20 2020 2064 6966 6632 203d 2063 742e  .    diff2 = ct.
-00018390: 7365 6c65 6374 285b 6261 6e64 4e6f 5d29  select([bandNo])
-000183a0: 2e61 6464 2831 292e 7375 6274 7261 6374  .add(1).subtract
-000183b0: 2872 742e 7365 6c65 6374 285b 6261 6e64  (rt.select([band
-000183c0: 4e6f 5d29 2e61 6464 2831 2929 0d0a 0d0a  No]).add(1))....
-000183d0: 2020 2020 6869 6768 5370 696b 6520 3d20      highSpike = 
-000183e0: 6469 6666 312e 6774 2861 6273 6f6c 7574  diff1.gt(absolut
-000183f0: 6553 7069 6b65 292e 416e 6428 6469 6666  eSpike).And(diff
-00018400: 322e 6774 2861 6273 6f6c 7574 6553 7069  2.gt(absoluteSpi
-00018410: 6b65 2929 0d0a 2020 2020 6c6f 7753 7069  ke))..    lowSpi
-00018420: 6b65 203d 2064 6966 6631 2e6c 7428 2d20  ke = diff1.lt(- 
-00018430: 6162 736f 6c75 7465 5370 696b 6529 2e41  absoluteSpike).A
-00018440: 6e64 2864 6966 6632 2e6c 7428 2d20 6162  nd(diff2.lt(- ab
-00018450: 736f 6c75 7465 5370 696b 6529 290d 0a20  soluteSpike)).. 
-00018460: 2020 2042 696e 6172 7953 7069 6b65 203d     BinarySpike =
-00018470: 2068 6967 6853 7069 6b65 2e4f 7228 6c6f   highSpike.Or(lo
-00018480: 7753 7069 6b65 290d 0a0d 0a20 2020 206f  wSpike)....    o
-00018490: 7269 6769 6e61 6c4d 6173 6b20 3d20 6374  riginalMask = ct
-000184a0: 2e6d 6173 6b28 290d 0a20 2020 2063 7420  .mask()..    ct 
-000184b0: 3d20 6374 2e6d 6173 6b28 4269 6e61 7279  = ct.mask(Binary
-000184c0: 5370 696b 652e 6571 2830 2929 0d0a 0d0a  Spike.eq(0))....
-000184d0: 2020 2020 646f 4e6f 744d 6173 6b20 3d20      doNotMask = 
-000184e0: 6c74 2e6d 6173 6b28 292e 4e6f 7428 292e  lt.mask().Not().
-000184f0: 4f72 2872 742e 6d61 736b 2829 2e4e 6f74  Or(rt.mask().Not
-00018500: 2829 290d 0a20 2020 206c 724d 6561 6e20  ())..    lrMean 
-00018510: 3d20 6c74 2e61 6464 2872 7429 0d0a 2020  = lt.add(rt)..  
-00018520: 2020 6c72 4d65 616e 203d 206c 724d 6561    lrMean = lrMea
-00018530: 6e2e 6469 7669 6465 2832 290d 0a20 2020  n.divide(2)..   
-00018540: 2023 6f75 7420 3d20 6374 2e6d 6173 6b28   #out = ct.mask(
-00018550: 646f 4e6f 744d 6173 6b2e 4e6f 7428 292e  doNotMask.Not().
-00018560: 416e 6428 6374 2e6d 6173 6b28 2929 290d  And(ct.mask())).
-00018570: 0a20 2020 206f 7574 203d 2063 742e 7768  .    out = ct.wh
-00018580: 6572 6528 4269 6e61 7279 5370 696b 652e  ere(BinarySpike.
-00018590: 6571 2831 292e 416e 6428 646f 4e6f 744d  eq(1).And(doNotM
-000185a0: 6173 6b2e 4e6f 7428 2929 2c6c 724d 6561  ask.Not()),lrMea
-000185b0: 6e29 0d0a 2020 2020 7265 7475 726e 206f  n)..    return o
-000185c0: 7574 2e73 6574 2827 7379 7374 656d 3a69  ut.set('system:i
-000185d0: 6e64 6578 272c 7369 292e 7365 7428 2773  ndex',si).set('s
-000185e0: 7973 7465 6d3a 7469 6d65 5f73 7461 7274  ystem:time_start
-000185f0: 272c 2074 696d 655f 7374 6172 7429 2e73  ', time_start).s
-00018600: 6574 2827 7379 7374 656d 3a74 696d 655f  et('system:time_
-00018610: 656e 6427 2c20 7469 6d65 5f65 6e64 290d  end', time_end).
-00018620: 0a0d 0a0d 0a20 206f 7574 436f 6c6c 6563  .....  outCollec
-00018630: 7469 6f6e 203d 2073 6571 2e6d 6170 2863  tion = seq.map(c
-00018640: 6f6d 7061 7265 290d 0a0d 0a20 2023 4164  ompare)....  #Ad
-00018650: 6420 7468 6520 626f 6f6b 656e 6473 2062  d the bookends b
-00018660: 6163 6b20 6f6e 0d0a 2020 6f75 7443 6f6c  ack on..  outCol
-00018670: 6c65 6374 696f 6e20 3d20 2065 652e 4c69  lection =  ee.Li
-00018680: 7374 285b 6669 7273 742c 6f75 7443 6f6c  st([first,outCol
-00018690: 6c65 6374 696f 6e2c 6c61 7374 5d29 2e66  lection,last]).f
-000186a0: 6c61 7474 656e 2829 0d0a 2020 7265 7475  latten()..  retu
-000186b0: 726e 2065 652e 496d 6167 6543 6f6c 6c65  rn ee.ImageColle
-000186c0: 6374 696f 6e2e 6672 6f6d 496d 6167 6573  ction.fromImages
-000186d0: 286f 7574 436f 6c6c 6563 7469 6f6e 290d  (outCollection).
-000186e0: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00018030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018040: 0d0a 234d 6574 686f 6420 666f 7220 7265  ..#Method for re
+00018050: 6d6f 7669 6e67 2073 7069 6b65 7320 696e  moving spikes in
+00018060: 2074 696d 6520 7365 7269 6573 0d0a 6465   time series..de
+00018070: 6620 6465 7370 696b 6543 6f6c 6c65 6374  f despikeCollect
+00018080: 696f 6e28 632c 2061 6273 6f6c 7574 6553  ion(c, absoluteS
+00018090: 7069 6b65 2c20 6261 6e64 4e6f 293a 0d0a  pike, bandNo):..
+000180a0: 2020 6320 3d20 632e 746f 4c69 7374 2831    c = c.toList(1
+000180b0: 3030 3030 2c30 290d 0a0d 0a20 2023 4765  0000,0)....  #Ge
+000180c0: 7420 626f 6f6b 2065 6e64 7320 666f 7220  t book ends for 
+000180d0: 6164 6469 6e67 2062 6163 6b20 6174 2074  adding back at t
+000180e0: 6865 2065 6e64 0d0a 2020 6669 7273 7420  he end..  first 
+000180f0: 3d20 632e 736c 6963 6528 302c 3129 0d0a  = c.slice(0,1)..
+00018100: 2020 6c61 7374 203d 2063 2e73 6c69 6365    last = c.slice
+00018110: 282d 312c 4e6f 6e65 290d 0a0d 0a20 2023  (-1,None)....  #
+00018120: 536c 6963 6520 7468 6520 6c65 6674 2c20  Slice the left, 
+00018130: 6365 6e74 6572 2c20 616e 6420 7269 6768  center, and righ
+00018140: 7420 666f 7220 7468 6520 6d6f 7669 6e67  t for the moving
+00018150: 2077 696e 646f 770d 0a20 206c 6566 7420   window..  left 
+00018160: 3d20 632e 736c 6963 6528 302c 2d32 290d  = c.slice(0,-2).
+00018170: 0a20 2063 656e 7465 7220 3d20 632e 736c  .  center = c.sl
+00018180: 6963 6528 312c 2d31 290d 0a20 2072 6967  ice(1,-1)..  rig
+00018190: 6874 203d 2063 2e73 6c69 6365 2832 2c4e  ht = c.slice(2,N
+000181a0: 6f6e 6529 0d0a 0d0a 2020 2346 696e 6420  one)....  #Find 
+000181b0: 686f 7720 6d61 6e79 2069 6d61 6765 7320  how many images 
+000181c0: 7468 6572 6520 6172 6520 746f 2063 6f6d  there are to com
+000181d0: 7061 7265 0d0a 2020 7365 7120 3d20 6565  pare..  seq = ee
+000181e0: 2e4c 6973 742e 7365 7175 656e 6365 2830  .List.sequence(0
+000181f0: 2c6c 6566 742e 6c65 6e67 7468 2829 2e73  ,left.length().s
+00018200: 7562 7472 6163 7428 3129 290d 0a0d 0a20  ubtract(1)).... 
+00018210: 2023 436f 6d70 6172 6520 7468 6520 6365   #Compare the ce
+00018220: 6e74 6572 2074 6f20 7468 6520 6c65 6674  nter to the left
+00018230: 2061 6e64 2072 6967 6874 2069 6d61 6765   and right image
+00018240: 730d 0a20 2064 6566 2063 6f6d 7061 7265  s..  def compare
+00018250: 2869 293a 0d0a 2020 2020 6c74 203d 2065  (i):..    lt = e
+00018260: 652e 496d 6167 6528 6c65 6674 2e67 6574  e.Image(left.get
+00018270: 2869 2929 0d0a 2020 2020 7274 203d 2065  (i))..    rt = e
+00018280: 652e 496d 6167 6528 7269 6768 742e 6765  e.Image(right.ge
+00018290: 7428 6929 290d 0a0d 0a20 2020 2063 7420  t(i))....    ct 
+000182a0: 3d20 6565 2e49 6d61 6765 2863 656e 7465  = ee.Image(cente
+000182b0: 722e 6765 7428 6929 293b 0d0a 2020 2020  r.get(i));..    
+000182c0: 7469 6d65 5f73 7461 7274 203d 2063 742e  time_start = ct.
+000182d0: 6765 7428 2773 7973 7465 6d3a 7469 6d65  get('system:time
+000182e0: 5f73 7461 7274 2729 0d0a 2020 2020 7469  _start')..    ti
+000182f0: 6d65 5f65 6e64 203d 2063 742e 6765 7428  me_end = ct.get(
+00018300: 2773 7973 7465 6d3a 7469 6d65 5f65 6e64  'system:time_end
+00018310: 2729 0d0a 2020 2020 7369 203d 2063 742e  ')..    si = ct.
+00018320: 6765 7428 2773 7973 7465 6d3a 696e 6465  get('system:inde
+00018330: 7827 290d 0a0d 0a0d 0a0d 0a20 2020 2064  x')........    d
+00018340: 6966 6631 203d 2063 742e 7365 6c65 6374  iff1 = ct.select
+00018350: 285b 6261 6e64 4e6f 5d29 2e61 6464 2831  ([bandNo]).add(1
+00018360: 292e 7375 6274 7261 6374 286c 742e 7365  ).subtract(lt.se
+00018370: 6c65 6374 285b 6261 6e64 4e6f 5d29 2e61  lect([bandNo]).a
+00018380: 6464 2831 2929 0d0a 2020 2020 6469 6666  dd(1))..    diff
+00018390: 3220 3d20 6374 2e73 656c 6563 7428 5b62  2 = ct.select([b
+000183a0: 616e 644e 6f5d 292e 6164 6428 3129 2e73  andNo]).add(1).s
+000183b0: 7562 7472 6163 7428 7274 2e73 656c 6563  ubtract(rt.selec
+000183c0: 7428 5b62 616e 644e 6f5d 292e 6164 6428  t([bandNo]).add(
+000183d0: 3129 290d 0a0d 0a20 2020 2068 6967 6853  1))....    highS
+000183e0: 7069 6b65 203d 2064 6966 6631 2e67 7428  pike = diff1.gt(
+000183f0: 6162 736f 6c75 7465 5370 696b 6529 2e41  absoluteSpike).A
+00018400: 6e64 2864 6966 6632 2e67 7428 6162 736f  nd(diff2.gt(abso
+00018410: 6c75 7465 5370 696b 6529 290d 0a20 2020  luteSpike))..   
+00018420: 206c 6f77 5370 696b 6520 3d20 6469 6666   lowSpike = diff
+00018430: 312e 6c74 282d 2061 6273 6f6c 7574 6553  1.lt(- absoluteS
+00018440: 7069 6b65 292e 416e 6428 6469 6666 322e  pike).And(diff2.
+00018450: 6c74 282d 2061 6273 6f6c 7574 6553 7069  lt(- absoluteSpi
+00018460: 6b65 2929 0d0a 2020 2020 4269 6e61 7279  ke))..    Binary
+00018470: 5370 696b 6520 3d20 6869 6768 5370 696b  Spike = highSpik
+00018480: 652e 4f72 286c 6f77 5370 696b 6529 0d0a  e.Or(lowSpike)..
+00018490: 0d0a 2020 2020 6f72 6967 696e 616c 4d61  ..    originalMa
+000184a0: 736b 203d 2063 742e 6d61 736b 2829 0d0a  sk = ct.mask()..
+000184b0: 2020 2020 6374 203d 2063 742e 6d61 736b      ct = ct.mask
+000184c0: 2842 696e 6172 7953 7069 6b65 2e65 7128  (BinarySpike.eq(
+000184d0: 3029 290d 0a0d 0a20 2020 2064 6f4e 6f74  0))....    doNot
+000184e0: 4d61 736b 203d 206c 742e 6d61 736b 2829  Mask = lt.mask()
+000184f0: 2e4e 6f74 2829 2e4f 7228 7274 2e6d 6173  .Not().Or(rt.mas
+00018500: 6b28 292e 4e6f 7428 2929 0d0a 2020 2020  k().Not())..    
+00018510: 6c72 4d65 616e 203d 206c 742e 6164 6428  lrMean = lt.add(
+00018520: 7274 290d 0a20 2020 206c 724d 6561 6e20  rt)..    lrMean 
+00018530: 3d20 6c72 4d65 616e 2e64 6976 6964 6528  = lrMean.divide(
+00018540: 3229 0d0a 2020 2020 236f 7574 203d 2063  2)..    #out = c
+00018550: 742e 6d61 736b 2864 6f4e 6f74 4d61 736b  t.mask(doNotMask
+00018560: 2e4e 6f74 2829 2e41 6e64 2863 742e 6d61  .Not().And(ct.ma
+00018570: 736b 2829 2929 0d0a 2020 2020 6f75 7420  sk()))..    out 
+00018580: 3d20 6374 2e77 6865 7265 2842 696e 6172  = ct.where(Binar
+00018590: 7953 7069 6b65 2e65 7128 3129 2e41 6e64  ySpike.eq(1).And
+000185a0: 2864 6f4e 6f74 4d61 736b 2e4e 6f74 2829  (doNotMask.Not()
+000185b0: 292c 6c72 4d65 616e 290d 0a20 2020 2072  ),lrMean)..    r
+000185c0: 6574 7572 6e20 6f75 742e 7365 7428 2773  eturn out.set('s
+000185d0: 7973 7465 6d3a 696e 6465 7827 2c73 6929  ystem:index',si)
+000185e0: 2e73 6574 2827 7379 7374 656d 3a74 696d  .set('system:tim
+000185f0: 655f 7374 6172 7427 2c20 7469 6d65 5f73  e_start', time_s
+00018600: 7461 7274 292e 7365 7428 2773 7973 7465  tart).set('syste
+00018610: 6d3a 7469 6d65 5f65 6e64 272c 2074 696d  m:time_end', tim
+00018620: 655f 656e 6429 0d0a 0d0a 0d0a 2020 6f75  e_end)......  ou
+00018630: 7443 6f6c 6c65 6374 696f 6e20 3d20 7365  tCollection = se
+00018640: 712e 6d61 7028 636f 6d70 6172 6529 0d0a  q.map(compare)..
+00018650: 0d0a 2020 2341 6464 2074 6865 2062 6f6f  ..  #Add the boo
+00018660: 6b65 6e64 7320 6261 636b 206f 6e0d 0a20  kends back on.. 
+00018670: 206f 7574 436f 6c6c 6563 7469 6f6e 203d   outCollection =
+00018680: 2020 6565 2e4c 6973 7428 5b66 6972 7374    ee.List([first
+00018690: 2c6f 7574 436f 6c6c 6563 7469 6f6e 2c6c  ,outCollection,l
+000186a0: 6173 745d 292e 666c 6174 7465 6e28 290d  ast]).flatten().
+000186b0: 0a20 2072 6574 7572 6e20 6565 2e49 6d61  .  return ee.Ima
+000186c0: 6765 436f 6c6c 6563 7469 6f6e 2e66 726f  geCollection.fro
+000186d0: 6d49 6d61 6765 7328 6f75 7443 6f6c 6c65  mImages(outColle
+000186e0: 6374 696f 6e29 0d0a 0d0a 2323 2323 2323  ction)....######
 000186f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018720: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
-00018730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018730: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
 00018740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018770: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
-00018780: 6f6e 2074 6f20 6765 7420 4d4f 4449 5320  on to get MODIS 
-00018790: 6461 7461 2066 726f 6d20 7661 7269 6f75  data from variou
-000187a0: 7320 636f 6c6c 6563 7469 6f6e 730d 0a23  s collections..#
-000187b0: 5769 6c6c 2070 756c 6c20 6672 6f6d 2064  Will pull from d
-000187c0: 6169 6c79 206f 7220 382d 6461 7920 636f  aily or 8-day co
-000187d0: 6d70 6f73 6974 6520 636f 6c6c 6563 7469  mposite collecti
-000187e0: 6f6e 7320 6261 7365 6420 6f6e 2074 6865  ons based on the
-000187f0: 2062 6f6f 6c65 616e 2076 6172 6961 626c   boolean variabl
-00018800: 6520 2264 6169 6c79 220d 0a64 6566 2067  e "daily"..def g
-00018810: 6574 4d6f 6469 7344 6174 6128 7374 6172  etModisData(star
-00018820: 7459 6561 722c 656e 6459 6561 722c 7374  tYear,endYear,st
-00018830: 6172 744a 756c 6961 6e2c 656e 644a 756c  artJulian,endJul
-00018840: 6961 6e2c 6461 696c 7920 3d20 4661 6c73  ian,daily = Fals
-00018850: 652c 6d61 736b 5751 4120 3d20 4661 6c73  e,maskWQA = Fals
-00018860: 652c 7a65 6e69 7468 5468 7265 7368 203d  e,zenithThresh =
-00018870: 2039 302c 7573 6554 656d 7049 6e43 6c6f   90,useTempInClo
-00018880: 7564 4d61 736b 203d 2054 7275 652c 6164  udMask = True,ad
-00018890: 644c 6f6f 6b41 6e67 6c65 4261 6e64 7320  dLookAngleBands 
-000188a0: 3d20 4661 6c73 652c 7265 7361 6d70 6c65  = False,resample
-000188b0: 4d65 7468 6f64 203d 2027 6e65 6172 2729  Method = 'near')
-000188c0: 3a0d 0a0d 0a20 2023 4669 6e64 2077 6869  :....  #Find whi
-000188d0: 6368 2063 6f6c 6c65 6374 696f 6e73 2074  ch collections t
-000188e0: 6f20 7075 6c6c 2066 726f 6d20 6261 7365  o pull from base
-000188f0: 6420 6f6e 2064 6169 6c79 206f 7220 382d  d on daily or 8-
-00018900: 6461 790d 0a20 2069 6620 6461 696c 7920  day..  if daily 
-00018910: 3d3d 2046 616c 7365 3a0d 0a20 2020 2061  == False:..    a
-00018920: 3235 3043 203d 206d 6f64 6973 4344 6963  250C = modisCDic
-00018930: 745b 2765 6967 6874 4461 7953 5232 3530  t['eightDaySR250
-00018940: 4127 5d0d 0a20 2020 2074 3235 3043 203d  A']..    t250C =
-00018950: 206d 6f64 6973 4344 6963 745b 2765 6967   modisCDict['eig
-00018960: 6874 4461 7953 5232 3530 5427 5d0d 0a20  htDaySR250T'].. 
-00018970: 2020 2061 3530 3043 203d 206d 6f64 6973     a500C = modis
-00018980: 4344 6963 745b 2765 6967 6874 4461 7953  CDict['eightDayS
-00018990: 5235 3030 4127 5d0d 0a20 2020 2074 3530  R500A']..    t50
-000189a0: 3043 203d 206d 6f64 6973 4344 6963 745b  0C = modisCDict[
-000189b0: 2765 6967 6874 4461 7953 5235 3030 5427  'eightDaySR500T'
-000189c0: 5d0d 0a20 2020 2061 3130 3030 4320 3d20  ]..    a1000C = 
-000189d0: 6d6f 6469 7343 4469 6374 5b27 6569 6768  modisCDict['eigh
-000189e0: 7444 6179 4c53 5431 3030 3041 275d 0d0a  tDayLST1000A']..
-000189f0: 2020 2020 7431 3030 3043 203d 206d 6f64      t1000C = mod
-00018a00: 6973 4344 6963 745b 2765 6967 6874 4461  isCDict['eightDa
-00018a10: 794c 5354 3130 3030 5427 5d0d 0a20 2020  yLST1000T']..   
-00018a20: 2076 6965 7741 6e67 6c65 4261 6e64 4e61   viewAngleBandNa
-00018a30: 6d65 7320 3d20 636f 6d70 6f73 6974 6556  mes = compositeV
-00018a40: 6965 7741 6e67 6c65 4261 6e64 4e61 6d65  iewAngleBandName
-00018a50: 733b 0d0a 2020 656c 7365 3a0d 0a20 2020  s;..  else:..   
-00018a60: 2061 3235 3043 203d 206d 6f64 6973 4344   a250C = modisCD
-00018a70: 6963 745b 2764 6169 6c79 5352 3235 3041  ict['dailySR250A
-00018a80: 275d 0d0a 2020 2020 7432 3530 4320 3d20  ']..    t250C = 
-00018a90: 6d6f 6469 7343 4469 6374 5b27 6461 696c  modisCDict['dail
-00018aa0: 7953 5232 3530 5427 5d0d 0a20 2020 2061  ySR250T']..    a
-00018ab0: 3530 3043 203d 206d 6f64 6973 4344 6963  500C = modisCDic
-00018ac0: 745b 2764 6169 6c79 5352 3530 3041 275d  t['dailySR500A']
-00018ad0: 0d0a 2020 2020 7435 3030 4320 3d20 6d6f  ..    t500C = mo
-00018ae0: 6469 7343 4469 6374 5b27 6461 696c 7953  disCDict['dailyS
-00018af0: 5235 3030 5427 5d0d 0a20 2020 2061 3130  R500T']..    a10
-00018b00: 3030 4320 3d20 6d6f 6469 7343 4469 6374  00C = modisCDict
-00018b10: 5b27 6461 696c 794c 5354 3130 3030 4127  ['dailyLST1000A'
-00018b20: 5d0d 0a20 2020 2074 3130 3030 4320 3d20  ]..    t1000C = 
-00018b30: 6d6f 6469 7343 4469 6374 5b27 6461 696c  modisCDict['dail
-00018b40: 794c 5354 3130 3030 5427 5d0d 0a20 2020  yLST1000T']..   
-00018b50: 2076 6965 7741 6e67 6c65 4261 6e64 4e61   viewAngleBandNa
-00018b60: 6d65 7320 3d20 6461 696c 7956 6965 7741  mes = dailyViewA
-00018b70: 6e67 6c65 4261 6e64 4e61 6d65 733b 0d0a  ngleBandNames;..
-00018b80: 0d0a 2020 2350 756c 6c20 696d 6167 6573  ..  #Pull images
-00018b90: 2066 726f 6d20 6561 6368 206f 6620 7468   from each of th
-00018ba0: 6520 636f 6c6c 6563 7469 6f6e 730d 0a20  e collections.. 
-00018bb0: 2061 3235 3020 3d20 6565 2e49 6d61 6765   a250 = ee.Image
-00018bc0: 436f 6c6c 6563 7469 6f6e 2861 3235 3043  Collection(a250C
-00018bd0: 295c 0d0a 2020 2020 2e66 696c 7465 7228  )\..    .filter(
-00018be0: 6565 2e46 696c 7465 722e 6361 6c65 6e64  ee.Filter.calend
-00018bf0: 6172 5261 6e67 6528 7374 6172 7459 6561  arRange(startYea
-00018c00: 722c 656e 6459 6561 722c 2779 6561 7227  r,endYear,'year'
-00018c10: 2929 5c0d 0a20 2020 202e 6669 6c74 6572  ))\..    .filter
-00018c20: 2865 652e 4669 6c74 6572 2e63 616c 656e  (ee.Filter.calen
-00018c30: 6461 7252 616e 6765 2873 7461 7274 4a75  darRange(startJu
-00018c40: 6c69 616e 2c65 6e64 4a75 6c69 616e 2929  lian,endJulian))
-00018c50: 5c0d 0a20 2020 202e 7365 6c65 6374 286d  \..    .select(m
-00018c60: 6f64 6973 3235 3053 656c 6563 7442 616e  odis250SelectBan
-00018c70: 6473 2c6d 6f64 6973 3235 3042 616e 644e  ds,modis250BandN
-00018c80: 616d 6573 290d 0a0d 0a0d 0a20 2074 3235  ames)......  t25
-00018c90: 3020 3d20 6565 2e49 6d61 6765 436f 6c6c  0 = ee.ImageColl
-00018ca0: 6563 7469 6f6e 2874 3235 3043 295c 0d0a  ection(t250C)\..
-00018cb0: 2020 2e66 696c 7465 7228 6565 2e46 696c    .filter(ee.Fil
-00018cc0: 7465 722e 6361 6c65 6e64 6172 5261 6e67  ter.calendarRang
-00018cd0: 6528 7374 6172 7459 6561 722c 656e 6459  e(startYear,endY
-00018ce0: 6561 722c 2779 6561 7227 2929 5c0d 0a20  ear,'year'))\.. 
-00018cf0: 202e 6669 6c74 6572 2865 652e 4669 6c74   .filter(ee.Filt
-00018d00: 6572 2e63 616c 656e 6461 7252 616e 6765  er.calendarRange
-00018d10: 2873 7461 7274 4a75 6c69 616e 2c65 6e64  (startJulian,end
-00018d20: 4a75 6c69 616e 2929 5c0d 0a20 202e 7365  Julian))\..  .se
-00018d30: 6c65 6374 286d 6f64 6973 3235 3053 656c  lect(modis250Sel
-00018d40: 6563 7442 616e 6473 2c6d 6f64 6973 3235  ectBands,modis25
-00018d50: 3042 616e 644e 616d 6573 290d 0a0d 0a0d  0BandNames).....
-00018d60: 0a20 2064 6566 2067 6574 3530 3028 6329  .  def get500(c)
-00018d70: 3a0d 0a20 2020 2069 6d61 6765 7320 3d20  :..    images = 
-00018d80: 6565 2e49 6d61 6765 436f 6c6c 6563 7469  ee.ImageCollecti
-00018d90: 6f6e 2863 295c 0d0a 2020 2020 2020 2020  on(c)\..        
-00018da0: 2020 2e66 696c 7465 7228 6565 2e46 696c    .filter(ee.Fil
-00018db0: 7465 722e 6361 6c65 6e64 6172 5261 6e67  ter.calendarRang
-00018dc0: 6528 7374 6172 7459 6561 722c 656e 6459  e(startYear,endY
-00018dd0: 6561 722c 2779 6561 7227 2929 5c0d 0a20  ear,'year'))\.. 
-00018de0: 2020 2020 2020 2020 202e 6669 6c74 6572           .filter
-00018df0: 2865 652e 4669 6c74 6572 2e63 616c 656e  (ee.Filter.calen
-00018e00: 6461 7252 616e 6765 2873 7461 7274 4a75  darRange(startJu
-00018e10: 6c69 616e 2c65 6e64 4a75 6c69 616e 2929  lian,endJulian))
-00018e20: 0d0a 2020 2020 6465 6620 6170 706c 795a  ..    def applyZ
-00018e30: 656e 6974 6828 696d 6729 3a0d 0a20 2020  enith(img):..   
-00018e40: 2020 2069 6d67 203d 2069 6d67 2e6d 6173     img = img.mas
-00018e50: 6b28 696d 672e 6d61 736b 2829 2e41 6e64  k(img.mask().And
-00018e60: 2869 6d67 2e73 656c 6563 7428 5b27 5365  (img.select(['Se
-00018e70: 6e73 6f72 5a65 6e69 7468 275d 292e 6c74  nsorZenith']).lt
-00018e80: 287a 656e 6974 6854 6872 6573 682a 3130  (zenithThresh*10
-00018e90: 3029 2929 0d0a 2020 2020 2020 6966 206d  0)))..      if m
-00018ea0: 6173 6b57 5141 3a69 6d67 203d 206d 6173  askWQA:img = mas
-00018eb0: 6b43 6c6f 7564 7357 5141 2869 6d67 290d  kCloudsWQA(img).
-00018ec0: 0a20 2020 2020 2072 6574 7572 6e20 696d  .      return im
-00018ed0: 670d 0a20 2020 2023 4d61 736b 2070 6978  g..    #Mask pix
-00018ee0: 656c 7320 6162 6f76 6520 6120 6365 7274  els above a cert
-00018ef0: 6169 6e20 7a65 6e69 7468 0d0a 2020 2020  ain zenith..    
-00018f00: 6966 2064 6169 6c79 3a0d 0a20 2020 2020  if daily:..     
-00018f10: 2069 6620 6d61 736b 5751 413a 7072 696e   if maskWQA:prin
-00018f20: 7428 274d 6173 6b69 6e67 2077 6974 6820  t('Masking with 
-00018f30: 5141 2062 616e 643a 272c 6329 0d0a 2020  QA band:',c)..  
-00018f40: 2020 2020 696d 6167 6573 203d 2069 6d61      images = ima
-00018f50: 6765 732e 6d61 7028 6170 706c 795a 656e  ges.map(applyZen
-00018f60: 6974 6829 0d0a 0d0a 2020 2020 6966 2061  ith)....    if a
-00018f70: 6464 4c6f 6f6b 416e 676c 6542 616e 6473  ddLookAngleBands
-00018f80: 3a0d 0a20 2020 2020 2069 6d61 6765 7320  :..      images 
-00018f90: 3d20 696d 6167 6573 2e73 656c 6563 7428  = images.select(
-00018fa0: 6565 2e4c 6973 7428 6d6f 6469 7335 3030  ee.List(modis500
-00018fb0: 5365 6c65 6374 4261 6e64 7329 2e63 6174  SelectBands).cat
-00018fc0: 2876 6965 7741 6e67 6c65 4261 6e64 4e61  (viewAngleBandNa
-00018fd0: 6d65 7329 2c65 652e 4c69 7374 286d 6f64  mes),ee.List(mod
-00018fe0: 6973 3530 3042 616e 644e 616d 6573 292e  is500BandNames).
-00018ff0: 6361 7428 7669 6577 416e 676c 6542 616e  cat(viewAngleBan
-00019000: 644e 616d 6573 2929 3b0d 0a20 2020 2065  dNames));..    e
-00019010: 6c73 653a 0d0a 2020 2020 2020 696d 6167  lse:..      imag
-00019020: 6573 203d 2069 6d61 6765 732e 7365 6c65  es = images.sele
-00019030: 6374 286d 6f64 6973 3530 3053 656c 6563  ct(modis500Selec
-00019040: 7442 616e 6473 2c6d 6f64 6973 3530 3042  tBands,modis500B
-00019050: 616e 644e 616d 6573 290d 0a0d 0a20 2020  andNames)....   
-00019060: 2072 6574 7572 6e20 696d 6167 6573 0d0a   return images..
-00019070: 0d0a 0d0a 2020 6135 3030 203d 2067 6574  ....  a500 = get
-00019080: 3530 3028 6135 3030 4329 0d0a 2020 7435  500(a500C)..  t5
-00019090: 3030 203d 2067 6574 3530 3028 7435 3030  00 = get500(t500
-000190a0: 4329 0d0a 0d0a 0d0a 2020 2349 6620 7468  C)......  #If th
-000190b0: 6572 6d61 6c20 636f 6c6c 6563 7469 6f6e  ermal collection
-000190c0: 2069 7320 7761 6e74 6564 2c20 7075 6c6c   is wanted, pull
-000190d0: 2069 7420 6173 2077 656c 6c0d 0a20 2069   it as well..  i
-000190e0: 6620 7573 6554 656d 7049 6e43 6c6f 7564  f useTempInCloud
-000190f0: 4d61 736b 3a0d 0a20 2020 2074 3130 3030  Mask:..    t1000
-00019100: 203d 2065 652e 496d 6167 6543 6f6c 6c65   = ee.ImageColle
-00019110: 6374 696f 6e28 7431 3030 3043 295c 0d0a  ction(t1000C)\..
-00019120: 2020 2020 2020 2020 2020 2020 2e66 696c              .fil
-00019130: 7465 7228 6565 2e46 696c 7465 722e 6361  ter(ee.Filter.ca
-00019140: 6c65 6e64 6172 5261 6e67 6528 7374 6172  lendarRange(star
-00019150: 7459 6561 722c 656e 6459 6561 722c 2779  tYear,endYear,'y
-00019160: 6561 7227 2929 5c0d 0a20 2020 2020 2020  ear'))\..       
-00019170: 2020 2020 202e 6669 6c74 6572 2865 652e       .filter(ee.
-00019180: 4669 6c74 6572 2e63 616c 656e 6461 7252  Filter.calendarR
-00019190: 616e 6765 2873 7461 7274 4a75 6c69 616e  ange(startJulian
-000191a0: 2c65 6e64 4a75 6c69 616e 2929 5c0d 0a20  ,endJulian))\.. 
-000191b0: 2020 2020 2020 2020 2020 202e 7365 6c65             .sele
-000191c0: 6374 285b 302c 382c 395d 2c5b 2774 656d  ct([0,8,9],['tem
-000191d0: 7027 2c27 456d 6973 5f33 3127 2c27 456d  p','Emis_31','Em
-000191e0: 6973 5f33 3227 5d29 3b0d 0a0d 0a20 2020  is_32']);....   
-000191f0: 2061 3130 3030 203d 2065 652e 496d 6167   a1000 = ee.Imag
-00019200: 6543 6f6c 6c65 6374 696f 6e28 6131 3030  eCollection(a100
-00019210: 3043 295c 0d0a 2020 2020 2020 2020 2020  0C)\..          
-00019220: 2020 2e66 696c 7465 7228 6565 2e46 696c    .filter(ee.Fil
-00019230: 7465 722e 6361 6c65 6e64 6172 5261 6e67  ter.calendarRang
-00019240: 6528 7374 6172 7459 6561 722c 656e 6459  e(startYear,endY
-00019250: 6561 722c 2779 6561 7227 2929 5c0d 0a20  ear,'year'))\.. 
-00019260: 2020 2020 2020 2020 2020 202e 6669 6c74             .filt
-00019270: 6572 2865 652e 4669 6c74 6572 2e63 616c  er(ee.Filter.cal
-00019280: 656e 6461 7252 616e 6765 2873 7461 7274  endarRange(start
-00019290: 4a75 6c69 616e 2c65 6e64 4a75 6c69 616e  Julian,endJulian
-000192a0: 2929 5c0d 0a20 2020 2020 2020 2020 2020  ))\..           
-000192b0: 202e 7365 6c65 6374 285b 302c 382c 395d   .select([0,8,9]
-000192c0: 2c5b 2774 656d 7027 2c27 456d 6973 5f33  ,['temp','Emis_3
-000192d0: 3127 2c27 456d 6973 5f33 3227 5d29 3b0d  1','Emis_32']);.
-000192e0: 0a0d 0a0d 0a20 2023 4e6f 7720 616c 6c20  .....  #Now all 
-000192f0: 636f 6c6c 6563 7469 6f6e 7320 6172 6520  collections are 
-00019300: 7075 6c6c 6564 2c20 7374 6172 7420 6a6f  pulled, start jo
-00019310: 696e 696e 6720 7468 656d 0d0a 2020 2346  ining them..  #F
-00019320: 6972 7374 206a 6f69 6e20 7468 6520 3235  irst join the 25
-00019330: 3020 616e 6420 3530 3020 6d20 4171 7561  0 and 500 m Aqua
-00019340: 0d0a 2020 6120 3d20 6a6f 696e 436f 6c6c  ..  a = joinColl
-00019350: 6563 7469 6f6e 7328 6132 3530 2c61 3530  ections(a250,a50
-00019360: 302c 4661 6c73 6529 0d0a 0d0a 2020 2354  0,False)....  #T
-00019370: 6865 6e20 5465 7272 610d 0a20 2074 203d  hen Terra..  t =
-00019380: 206a 6f69 6e43 6f6c 6c65 6374 696f 6e73   joinCollections
-00019390: 2874 3235 302c 7435 3030 2c46 616c 7365  (t250,t500,False
-000193a0: 290d 0a0d 0a20 2023 4966 2074 656d 7020  )....  #If temp 
-000193b0: 7761 7320 7075 6c6c 6564 2c20 6a6f 696e  was pulled, join
-000193c0: 2074 6861 7420 696e 2061 7320 7765 6c6c   that in as well
-000193d0: 0d0a 2020 2341 6c73 6f20 7365 6c65 6374  ..  #Also select
-000193e0: 2074 6865 2062 616e 6473 2069 6e20 616e   the bands in an
-000193f0: 204c 352d 6c69 6b65 206f 7264 6572 2061   L5-like order a
-00019400: 6e64 2067 6976 6520 6465 7363 7269 7074  nd give descript
-00019410: 6976 6520 6e61 6d65 730d 0a20 2069 6620  ive names..  if 
-00019420: 7573 6554 656d 7049 6e43 6c6f 7564 4d61  useTempInCloudMa
-00019430: 736b 3a0d 0a20 2020 2061 203d 206a 6f69  sk:..    a = joi
-00019440: 6e43 6f6c 6c65 6374 696f 6e73 2861 2c61  nCollections(a,a
-00019450: 3130 3030 2c46 616c 7365 290d 0a20 2020  1000,False)..   
-00019460: 2074 203d 206a 6f69 6e43 6f6c 6c65 6374   t = joinCollect
-00019470: 696f 6e73 2874 2c74 3130 3030 2c46 616c  ions(t,t1000,Fal
-00019480: 7365 290d 0a0d 0a0d 0a20 2023 2020 2074  se)......  #   t
-00019490: 5365 6c65 6374 4f72 6465 7220 3d20 7754  SelectOrder = wT
-000194a0: 656d 7053 656c 6563 744f 7264 6572 0d0a  empSelectOrder..
-000194b0: 2020 2320 2020 7453 7464 4e61 6d65 7320    #   tStdNames 
-000194c0: 3d20 7754 656d 7053 7464 4e61 6d65 730d  = wTempStdNames.
-000194d0: 0a0d 0a20 2023 2023 4966 206e 6f20 7468  ...  # #If no th
-000194e0: 6572 6d61 6c20 7761 7320 7075 6c6c 6564  ermal was pulled
-000194f0: 2c20 6c65 6176 6520 7468 6174 206f 7574  , leave that out
-00019500: 0d0a 2020 2320 656c 7365 3a0d 0a20 2023  ..  # else:..  #
-00019510: 2020 2074 5365 6c65 6374 4f72 6465 7220     tSelectOrder 
-00019520: 3d20 776f 5465 6d70 5365 6c65 6374 4f72  = woTempSelectOr
-00019530: 6465 720d 0a20 2023 2020 2074 5374 644e  der..  #   tStdN
-00019540: 616d 6573 203d 2077 6f54 656d 7053 7464  ames = woTempStd
-00019550: 4e61 6d65 730d 0a0d 0a20 2061 203d 2061  Names....  a = a
-00019560: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
-00019570: 696d 672e 7365 7428 7b27 706c 6174 666f  img.set({'platfo
-00019580: 726d 273a 2761 7175 6127 7d29 293b 0d0a  rm':'aqua'}));..
-00019590: 2020 7420 3d20 742e 6d61 7028 6c61 6d62    t = t.map(lamb
-000195a0: 6461 2069 6d67 3a69 6d67 2e73 6574 287b  da img:img.set({
-000195b0: 2770 6c61 7466 6f72 6d27 3a27 7465 7272  'platform':'terr
-000195c0: 6127 7d29 293b 0d0a 0d0a 0d0a 2020 6966  a'}));......  if
-000195d0: 2864 6169 6c79 293a 6461 696c 7950 6965  (daily):dailyPie
-000195e0: 6365 203d 2027 4461 696c 7927 0d0a 2020  ce = 'Daily'..  
-000195f0: 656c 7365 3a64 6169 6c79 5069 6563 6520  else:dailyPiece 
-00019600: 3d20 2743 6f6d 706f 7369 7465 270d 0a0d  = 'Composite'...
-00019610: 0a20 2069 6628 7573 6554 656d 7049 6e43  .  if(useTempInC
-00019620: 6c6f 7564 4d61 736b 293a 7465 6d70 5069  loudMask):tempPi
-00019630: 6563 6520 3d20 2774 656d 7027 0d0a 2020  ece = 'temp'..  
-00019640: 656c 7365 3a74 656d 7050 6965 6365 203d  else:tempPiece =
-00019650: 2027 6e6f 5465 6d70 270d 0a20 2069 6620   'noTemp'..  if 
-00019660: 6164 644c 6f6f 6b41 6e67 6c65 4261 6e64  addLookAngleBand
-00019670: 733a 616e 676c 6550 6965 6365 203d 2027  s:anglePiece = '
-00019680: 416e 676c 6527 0d0a 2020 656c 7365 3a61  Angle'..  else:a
-00019690: 6e67 6c65 5069 6563 6520 3d20 274e 6f41  nglePiece = 'NoA
-000196a0: 6e67 6c65 270d 0a20 206d 756c 744b 6579  ngle'..  multKey
-000196b0: 203d 2074 656d 7050 6965 6365 2b61 6e67   = tempPiece+ang
-000196c0: 6c65 5069 6563 652b 6461 696c 7950 6965  lePiece+dailyPie
-000196d0: 6365 0d0a 0d0a 2020 6d75 6c74 203d 206d  ce....  mult = m
-000196e0: 756c 744d 6f64 6973 4469 6374 5b6d 756c  ultModisDict[mul
-000196f0: 744b 6579 5d0d 0a20 206d 756c 7449 6d61  tKey]..  multIma
-00019700: 6765 203d 206d 756c 745b 305d 0d0a 2020  ge = mult[0]..  
-00019710: 6d75 6c74 4e61 6d65 7320 3d20 6d75 6c74  multNames = mult
-00019720: 5b31 5d0d 0a0d 0a20 2023 4a6f 696e 2054  [1]....  #Join T
-00019730: 6572 7261 2061 6e64 2041 7175 610d 0a20  erra and Aqua.. 
-00019740: 206a 6f69 6e65 6420 3d20 6565 2e49 6d61   joined = ee.Ima
-00019750: 6765 436f 6c6c 6563 7469 6f6e 2861 2e6d  geCollection(a.m
-00019760: 6572 6765 2874 2929 232e 7365 6c65 6374  erge(t))#.select
-00019770: 2874 5365 6c65 6374 4f72 6465 722c 7453  (tSelectOrder,tS
-00019780: 7464 4e61 6d65 7329 0d0a 0d0a 2020 6465  tdNames)....  de
-00019790: 6620 6d75 6c74 6970 6c79 496d 6728 696d  f multiplyImg(im
-000197a0: 6729 3a0d 0a20 2020 2072 6574 7572 6e20  g):..    return 
-000197b0: 696d 672e 6d75 6c74 6970 6c79 286d 756c  img.multiply(mul
-000197c0: 7449 6d61 6765 292e 666c 6f61 7428 292e  tImage).float().
-000197d0: 7365 6c65 6374 286d 756c 744e 616d 6573  select(multNames
-000197e0: 295c 0d0a 2020 2020 2020 2020 2e63 6f70  )\..        .cop
-000197f0: 7950 726f 7065 7274 6965 7328 696d 672c  yProperties(img,
-00019800: 5b27 7379 7374 656d 3a74 696d 655f 7374  ['system:time_st
-00019810: 6172 7427 2c27 7379 7374 656d 3a74 696d  art','system:tim
-00019820: 655f 656e 6427 2c27 7379 7374 656d 3a69  e_end','system:i
-00019830: 6e64 6578 275d 295c 0d0a 2020 2020 2020  ndex'])\..      
-00019840: 2020 2e63 6f70 7950 726f 7065 7274 6965    .copyPropertie
-00019850: 7328 696d 6729 0d0a 2020 6465 6620 7365  s(img)..  def se
-00019860: 7452 6573 616d 706c 6528 696d 6729 3a0d  tResample(img):.
-00019870: 0a20 2020 2072 6574 7572 6e20 696d 672e  .    return img.
-00019880: 7265 7361 6d70 6c65 2872 6573 616d 706c  resample(resampl
-00019890: 654d 6574 686f 6429 0d0a 0d0a 2020 6a6f  eMethod)....  jo
-000198a0: 696e 6564 203d 206a 6f69 6e65 642e 6d61  ined = joined.ma
-000198b0: 7028 6d75 6c74 6970 6c79 496d 6729 0d0a  p(multiplyImg)..
-000198c0: 2020 6966 2020 7265 7361 6d70 6c65 4d65    if  resampleMe
-000198d0: 7468 6f64 2069 6e20 5b27 6269 6c69 6e65  thod in ['biline
-000198e0: 6172 272c 2762 6963 7562 6963 275d 3a0d  ar','bicubic']:.
-000198f0: 0a20 2020 2070 7269 6e74 2827 5365 7474  .    print('Sett
-00019900: 696e 6720 7265 7361 6d70 6c65 206d 6574  ing resample met
-00019910: 686f 6420 746f 2027 2c72 6573 616d 706c  hod to ',resampl
-00019920: 654d 6574 686f 6429 0d0a 2020 2020 6a6f  eMethod)..    jo
-00019930: 696e 6564 203d 206a 6f69 6e65 642e 6d61  ined = joined.ma
-00019940: 7028 7365 7452 6573 616d 706c 6529 0d0a  p(setResample)..
-00019950: 2020 7265 7475 726e 206a 6f69 6e65 640d    return joined.
-00019960: 0a0d 0a0d 0a23 4675 6e63 7469 6f6e 2074  .....#Function t
-00019970: 6f20 6765 7420 636c 6f75 642c 2063 6c6f  o get cloud, clo
-00019980: 7564 2073 6861 646f 7720 6275 7374 6564  ud shadow busted
-00019990: 206d 6f64 6973 2069 6d61 6765 730d 0a23   modis images..#
-000199a0: 5461 6b65 7320 6361 7265 206f 6620 6d61  Takes care of ma
-000199b0: 7463 6869 6e67 2064 6966 6665 7265 6e74  tching different
-000199c0: 206d 6f64 6973 2063 6f6c 6c65 6374 696f   modis collectio
-000199d0: 6e73 2061 7320 7765 6c6c 0d0a 6465 6620  ns as well..def 
-000199e0: 6765 7450 726f 6365 7373 6564 4d6f 6469  getProcessedModi
-000199f0: 7328 7374 6172 7459 6561 722c 0d0a 2020  s(startYear,..  
-00019a00: 2020 2020 2020 2020 2020 656e 6459 6561            endYea
-00019a10: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00019a20: 7374 6172 744a 756c 6961 6e2c 0d0a 2020  startJulian,..  
-00019a30: 2020 2020 2020 2020 2020 656e 644a 756c            endJul
-00019a40: 6961 6e2c 0d0a 2020 2020 2020 2020 2020  ian,..          
-00019a50: 2020 7a65 6e69 7468 5468 7265 7368 203d    zenithThresh =
-00019a60: 2039 302c 0d0a 2020 2020 2020 2020 2020   90,..          
-00019a70: 2020 6164 644c 6f6f 6b41 6e67 6c65 4261    addLookAngleBa
-00019a80: 6e64 7320 3d20 5472 7565 2c0d 0a20 2020  nds = True,..   
-00019a90: 2020 2020 2020 2020 2061 7070 6c79 436c           applyCl
-00019aa0: 6f75 6453 636f 7265 203d 2054 7275 652c  oudScore = True,
-00019ab0: 0d0a 2020 2020 2020 2020 2020 2020 6170  ..            ap
-00019ac0: 706c 7954 444f 4d20 3d20 5472 7565 2c0d  plyTDOM = True,.
-00019ad0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00019ae0: 5465 6d70 496e 436c 6f75 644d 6173 6b20  TempInCloudMask 
-00019af0: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
-00019b00: 2020 2020 2063 6c6f 7564 5363 6f72 6554       cloudScoreT
-00019b10: 6872 6573 6820 3d20 3230 2c0d 0a20 2020  hresh = 20,..   
-00019b20: 2020 2020 2020 2020 2070 6572 666f 726d           perform
-00019b30: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-00019b40: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-00019b50: 2020 2020 2020 636c 6f75 6453 636f 7265        cloudScore
-00019b60: 5063 746c 203d 2031 302c 0d0a 2020 2020  Pctl = 10,..    
-00019b70: 2020 2020 2020 2020 7a53 636f 7265 5468          zScoreTh
-00019b80: 7265 7368 203d 202d 312c 0d0a 2020 2020  resh = -1,..    
-00019b90: 2020 2020 2020 2020 7368 6164 6f77 5375          shadowSu
-00019ba0: 6d54 6872 6573 6820 3d20 302e 3335 2c0d  mThresh = 0.35,.
-00019bb0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00019bc0: 7472 6163 7450 6978 656c 7320 3d20 302c  tractPixels = 0,
-00019bd0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-00019be0: 6c61 7465 5069 7865 6c73 203d 2032 2e35  latePixels = 2.5
-00019bf0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00019c00: 6861 646f 7753 756d 4261 6e64 7320 3d20  hadowSumBands = 
-00019c10: 5b27 6e69 7227 2c27 7377 6972 3227 5d2c  ['nir','swir2'],
-00019c20: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00019c30: 7361 6d70 6c65 4d65 7468 6f64 203d 2027  sampleMethod = '
-00019c40: 6269 6375 6269 6327 2c0d 0a20 2020 2020  bicubic',..     
-00019c50: 2020 2020 2020 2070 7265 436f 6d70 7574         preComput
-00019c60: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
-00019c70: 6574 203d 204e 6f6e 652c 0d0a 2020 2020  et = None,..    
-00019c80: 2020 2020 2020 2020 7072 6543 6f6d 7075          preCompu
-00019c90: 7465 6454 444f 4d49 524d 6561 6e20 3d20  tedTDOMIRMean = 
-00019ca0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-00019cb0: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
-00019cc0: 4f4d 4952 5374 6444 6576 203d 204e 6f6e  OMIRStdDev = Non
-00019cd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00019ce0: 6164 6454 6f4d 6170 203d 2046 616c 7365  addToMap = False
-00019cf0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00019d00: 7273 203d 2027 4550 5347 3a34 3332 3627  rs = 'EPSG:4326'
-00019d10: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00019d20: 6361 6c65 203d 2032 3530 2c0d 0a20 2020  cale = 250,..   
-00019d30: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00019d40: 726d 203d 204e 6f6e 6529 3a0d 0a0d 0a20  rm = None):.... 
-00019d50: 2061 7267 7320 3d20 666f 726d 6174 4172   args = formatAr
-00019d60: 6773 286c 6f63 616c 7328 2929 0d0a 2020  gs(locals())..  
-00019d70: 6966 2027 6172 6773 2720 696e 2061 7267  if 'args' in arg
-00019d80: 732e 6b65 7973 2829 3a0d 0a20 2020 2064  s.keys():..    d
-00019d90: 656c 2061 7267 735b 2761 7267 7327 5d0d  el args['args'].
-00019da0: 0a0d 0a20 2023 4765 7420 6a6f 696e 6564  ...  #Get joined
-00019db0: 206d 6f64 6973 2063 6f6c 6c65 6374 696f   modis collectio
-00019dc0: 6e0d 0a20 206d 6f64 6973 496d 6167 6573  n..  modisImages
-00019dd0: 203d 2067 6574 4d6f 6469 7344 6174 6128   = getModisData(
-00019de0: 7374 6172 7459 6561 722c 656e 6459 6561  startYear,endYea
-00019df0: 722c 7374 6172 744a 756c 6961 6e2c 656e  r,startJulian,en
-00019e00: 644a 756c 6961 6e2c 0d0a 2020 2020 6461  dJulian,..    da
-00019e10: 696c 7920 3d20 5472 7565 2c0d 0a20 2020  ily = True,..   
-00019e20: 206d 6173 6b57 5141 203d 2046 616c 7365   maskWQA = False
-00019e30: 2c0d 0a20 2020 207a 656e 6974 6854 6872  ,..    zenithThr
-00019e40: 6573 6820 3d20 7a65 6e69 7468 5468 7265  esh = zenithThre
-00019e50: 7368 2c0d 0a20 2020 2075 7365 5465 6d70  sh,..    useTemp
-00019e60: 496e 436c 6f75 644d 6173 6b20 3d20 7573  InCloudMask = us
-00019e70: 6554 656d 7049 6e43 6c6f 7564 4d61 736b  eTempInCloudMask
-00019e80: 2c0d 0a20 2020 2061 6464 4c6f 6f6b 416e  ,..    addLookAn
-00019e90: 676c 6542 616e 6473 203d 2061 6464 4c6f  gleBands = addLo
-00019ea0: 6f6b 416e 676c 6542 616e 6473 2c0d 0a20  okAngleBands,.. 
-00019eb0: 2020 2072 6573 616d 706c 654d 6574 686f     resampleMetho
-00019ec0: 6420 3d20 2072 6573 616d 706c 654d 6574  d =  resampleMet
-00019ed0: 686f 6429 0d0a 0d0a 2020 6966 2061 6464  hod)....  if add
-00019ee0: 546f 4d61 703a 0d0a 2020 2020 4d61 702e  ToMap:..    Map.
-00019ef0: 6164 644c 6179 6572 286d 6f64 6973 496d  addLayer(modisIm
-00019f00: 6167 6573 2e6d 6564 6961 6e28 292e 7265  ages.median().re
-00019f10: 7072 6f6a 6563 7428 6372 732c 7472 616e  project(crs,tran
-00019f20: 7366 6f72 6d2c 7363 616c 6529 2c76 697a  sform,scale),viz
-00019f30: 5061 7261 6d73 4661 6c73 652c 2752 6177  ParamsFalse,'Raw
-00019f40: 204d 6564 6961 6e27 290d 0a0d 0a0d 0a20   Median')...... 
-00019f50: 2069 6620 6170 706c 7943 6c6f 7564 5363   if applyCloudSc
-00019f60: 6f72 653a 0d0a 2020 2020 7072 696e 7428  ore:..    print(
-00019f70: 2741 7070 6c79 696e 6720 636c 6f75 6453  'Applying cloudS
-00019f80: 636f 7265 2729 0d0a 2020 2020 6d6f 6469  core')..    modi
-00019f90: 7349 6d61 6765 7320 3d20 6170 706c 7943  sImages = applyC
-00019fa0: 6c6f 7564 5363 6f72 6541 6c67 6f72 6974  loudScoreAlgorit
-00019fb0: 686d 286d 6f64 6973 496d 6167 6573 2c6d  hm(modisImages,m
-00019fc0: 6f64 6973 436c 6f75 6453 636f 7265 2c63  odisCloudScore,c
-00019fd0: 6c6f 7564 5363 6f72 6554 6872 6573 682c  loudScoreThresh,
-00019fe0: 636c 6f75 6453 636f 7265 5063 746c 2c63  cloudScorePctl,c
-00019ff0: 6f6e 7472 6163 7450 6978 656c 732c 6469  ontractPixels,di
-0001a000: 6c61 7465 5069 7865 6c73 2c70 6572 666f  latePixels,perfo
-0001a010: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
-0001a020: 6574 2c70 7265 436f 6d70 7574 6564 436c  et,preComputedCl
-0001a030: 6f75 6453 636f 7265 4f66 6673 6574 290d  oudScoreOffset).
-0001a040: 0a0d 0a20 2020 2069 6620 6164 6454 6f4d  ...    if addToM
-0001a050: 6170 3a0d 0a20 2020 2020 204d 6170 2e61  ap:..      Map.a
-0001a060: 6464 4c61 7965 7228 6d6f 6469 7349 6d61  ddLayer(modisIma
-0001a070: 6765 732e 6d65 6469 616e 2829 2e72 6570  ges.median().rep
-0001a080: 726f 6a65 6374 2863 7273 2c74 7261 6e73  roject(crs,trans
-0001a090: 666f 726d 2c73 6361 6c65 292c 7669 7a50  form,scale),vizP
-0001a0a0: 6172 616d 7346 616c 7365 2c27 436c 6f75  aramsFalse,'Clou
-0001a0b0: 6420 4d61 736b 6564 204d 6564 6961 6e27  d Masked Median'
-0001a0c0: 2c46 616c 7365 290d 0a20 2020 2020 204d  ,False)..      M
-0001a0d0: 6170 2e61 6464 4c61 7965 7228 6d6f 6469  ap.addLayer(modi
-0001a0e0: 7349 6d61 6765 732e 6d69 6e28 292e 7265  sImages.min().re
-0001a0f0: 7072 6f6a 6563 7428 6372 732c 7472 616e  project(crs,tran
-0001a100: 7366 6f72 6d2c 7363 616c 6529 2c76 697a  sform,scale),viz
-0001a110: 5061 7261 6d73 4661 6c73 652c 2743 6c6f  ParamsFalse,'Clo
-0001a120: 7564 204d 6173 6b65 6420 4d69 6e27 2c46  ud Masked Min',F
-0001a130: 616c 7365 290d 0a0d 0a20 2069 6620 6170  alse)....  if ap
-0001a140: 706c 7954 444f 4d3a 0d0a 2020 2020 7072  plyTDOM:..    pr
-0001a150: 696e 7428 2741 7070 6c79 696e 6720 5444  int('Applying TD
-0001a160: 4f4d 2729 0d0a 2020 2020 2346 696e 6420  OM')..    #Find 
-0001a170: 616e 6420 6d61 736b 206f 7574 2064 6172  and mask out dar
-0001a180: 6b20 6f75 746c 6965 7273 0d0a 2020 2020  k outliers..    
-0001a190: 6d6f 6469 7349 6d61 6765 7320 3d20 7369  modisImages = si
-0001a1a0: 6d70 6c65 5444 4f4d 3228 6d6f 6469 7349  mpleTDOM2(modisI
-0001a1b0: 6d61 6765 732c 7a53 636f 7265 5468 7265  mages,zScoreThre
-0001a1c0: 7368 2c73 6861 646f 7753 756d 5468 7265  sh,shadowSumThre
-0001a1d0: 7368 2c63 6f6e 7472 6163 7450 6978 656c  sh,contractPixel
-0001a1e0: 732c 6469 6c61 7465 5069 7865 6c73 2c73  s,dilatePixels,s
-0001a1f0: 6861 646f 7753 756d 4261 6e64 732c 7072  hadowSumBands,pr
-0001a200: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
-0001a210: 6561 6e2c 7072 6543 6f6d 7075 7465 6454  ean,preComputedT
-0001a220: 444f 4d49 5253 7464 4465 7629 0d0a 0d0a  DOMIRStdDev)....
-0001a230: 2020 2020 6966 2061 6464 546f 4d61 703a      if addToMap:
-0001a240: 0d0a 2020 2020 2020 4d61 702e 6164 644c  ..      Map.addL
-0001a250: 6179 6572 286d 6f64 6973 496d 6167 6573  ayer(modisImages
-0001a260: 2e6d 6564 6961 6e28 292e 7265 7072 6f6a  .median().reproj
-0001a270: 6563 7428 6372 732c 7472 616e 7366 6f72  ect(crs,transfor
-0001a280: 6d2c 7363 616c 6529 2c76 697a 5061 7261  m,scale),vizPara
-0001a290: 6d73 4661 6c73 652c 2743 6c6f 7564 2f43  msFalse,'Cloud/C
-0001a2a0: 6c6f 7564 2053 6861 646f 7720 4d61 736b  loud Shadow Mask
-0001a2b0: 6564 204d 6564 6961 6e27 2c46 616c 7365  ed Median',False
-0001a2c0: 290d 0a20 2020 2020 204d 6170 2e61 6464  )..      Map.add
-0001a2d0: 4c61 7965 7228 6d6f 6469 7349 6d61 6765  Layer(modisImage
-0001a2e0: 732e 6d69 6e28 292e 7265 7072 6f6a 6563  s.min().reprojec
-0001a2f0: 7428 6372 732c 7472 616e 7366 6f72 6d2c  t(crs,transform,
-0001a300: 7363 616c 6529 2c76 697a 5061 7261 6d73  scale),vizParams
-0001a310: 4661 6c73 652c 2743 6c6f 7564 2f43 6c6f  False,'Cloud/Clo
-0001a320: 7564 2053 6861 646f 7720 4d61 736b 6564  ud Shadow Masked
-0001a330: 204d 696e 272c 4661 6c73 6529 0d0a 0d0a   Min',False)....
-0001a340: 2020 6d6f 6469 7349 6d61 6765 7320 3d20    modisImages = 
-0001a350: 6d6f 6469 7349 6d61 6765 732e 6d61 7028  modisImages.map(
-0001a360: 7369 6d70 6c65 4164 6449 6e64 6963 6573  simpleAddIndices
-0001a370: 290d 0a20 206d 6f64 6973 496d 6167 6573  )..  modisImages
-0001a380: 203d 206d 6f64 6973 496d 6167 6573 2e6d   = modisImages.m
-0001a390: 6170 286c 616d 6264 6120 696d 673a 2069  ap(lambda img: i
-0001a3a0: 6d67 2e66 6c6f 6174 2829 290d 0a20 2072  mg.float())..  r
-0001a3b0: 6574 7572 6e20 6d6f 6469 7349 6d61 6765  eturn modisImage
-0001a3c0: 732e 7365 7428 6172 6773 290d 0a23 2323  s.set(args)..###
-0001a3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018770: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00018780: 2346 756e 6374 696f 6e20 746f 2067 6574  #Function to get
+00018790: 204d 4f44 4953 2064 6174 6120 6672 6f6d   MODIS data from
+000187a0: 2076 6172 696f 7573 2063 6f6c 6c65 6374   various collect
+000187b0: 696f 6e73 0d0a 2357 696c 6c20 7075 6c6c  ions..#Will pull
+000187c0: 2066 726f 6d20 6461 696c 7920 6f72 2038   from daily or 8
+000187d0: 2d64 6179 2063 6f6d 706f 7369 7465 2063  -day composite c
+000187e0: 6f6c 6c65 6374 696f 6e73 2062 6173 6564  ollections based
+000187f0: 206f 6e20 7468 6520 626f 6f6c 6561 6e20   on the boolean 
+00018800: 7661 7269 6162 6c65 2022 6461 696c 7922  variable "daily"
+00018810: 0d0a 6465 6620 6765 744d 6f64 6973 4461  ..def getModisDa
+00018820: 7461 2873 7461 7274 5965 6172 2c65 6e64  ta(startYear,end
+00018830: 5965 6172 2c73 7461 7274 4a75 6c69 616e  Year,startJulian
+00018840: 2c65 6e64 4a75 6c69 616e 2c64 6169 6c79  ,endJulian,daily
+00018850: 203d 2046 616c 7365 2c6d 6173 6b57 5141   = False,maskWQA
+00018860: 203d 2046 616c 7365 2c7a 656e 6974 6854   = False,zenithT
+00018870: 6872 6573 6820 3d20 3930 2c75 7365 5465  hresh = 90,useTe
+00018880: 6d70 496e 436c 6f75 644d 6173 6b20 3d20  mpInCloudMask = 
+00018890: 5472 7565 2c61 6464 4c6f 6f6b 416e 676c  True,addLookAngl
+000188a0: 6542 616e 6473 203d 2046 616c 7365 2c72  eBands = False,r
+000188b0: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+000188c0: 276e 6561 7227 293a 0d0a 0d0a 2020 2346  'near'):....  #F
+000188d0: 696e 6420 7768 6963 6820 636f 6c6c 6563  ind which collec
+000188e0: 7469 6f6e 7320 746f 2070 756c 6c20 6672  tions to pull fr
+000188f0: 6f6d 2062 6173 6564 206f 6e20 6461 696c  om based on dail
+00018900: 7920 6f72 2038 2d64 6179 0d0a 2020 6966  y or 8-day..  if
+00018910: 2064 6169 6c79 203d 3d20 4661 6c73 653a   daily == False:
+00018920: 0d0a 2020 2020 6132 3530 4320 3d20 6d6f  ..    a250C = mo
+00018930: 6469 7343 4469 6374 5b27 6569 6768 7444  disCDict['eightD
+00018940: 6179 5352 3235 3041 275d 0d0a 2020 2020  aySR250A']..    
+00018950: 7432 3530 4320 3d20 6d6f 6469 7343 4469  t250C = modisCDi
+00018960: 6374 5b27 6569 6768 7444 6179 5352 3235  ct['eightDaySR25
+00018970: 3054 275d 0d0a 2020 2020 6135 3030 4320  0T']..    a500C 
+00018980: 3d20 6d6f 6469 7343 4469 6374 5b27 6569  = modisCDict['ei
+00018990: 6768 7444 6179 5352 3530 3041 275d 0d0a  ghtDaySR500A']..
+000189a0: 2020 2020 7435 3030 4320 3d20 6d6f 6469      t500C = modi
+000189b0: 7343 4469 6374 5b27 6569 6768 7444 6179  sCDict['eightDay
+000189c0: 5352 3530 3054 275d 0d0a 2020 2020 6131  SR500T']..    a1
+000189d0: 3030 3043 203d 206d 6f64 6973 4344 6963  000C = modisCDic
+000189e0: 745b 2765 6967 6874 4461 794c 5354 3130  t['eightDayLST10
+000189f0: 3030 4127 5d0d 0a20 2020 2074 3130 3030  00A']..    t1000
+00018a00: 4320 3d20 6d6f 6469 7343 4469 6374 5b27  C = modisCDict['
+00018a10: 6569 6768 7444 6179 4c53 5431 3030 3054  eightDayLST1000T
+00018a20: 275d 0d0a 2020 2020 7669 6577 416e 676c  ']..    viewAngl
+00018a30: 6542 616e 644e 616d 6573 203d 2063 6f6d  eBandNames = com
+00018a40: 706f 7369 7465 5669 6577 416e 676c 6542  positeViewAngleB
+00018a50: 616e 644e 616d 6573 3b0d 0a20 2065 6c73  andNames;..  els
+00018a60: 653a 0d0a 2020 2020 6132 3530 4320 3d20  e:..    a250C = 
+00018a70: 6d6f 6469 7343 4469 6374 5b27 6461 696c  modisCDict['dail
+00018a80: 7953 5232 3530 4127 5d0d 0a20 2020 2074  ySR250A']..    t
+00018a90: 3235 3043 203d 206d 6f64 6973 4344 6963  250C = modisCDic
+00018aa0: 745b 2764 6169 6c79 5352 3235 3054 275d  t['dailySR250T']
+00018ab0: 0d0a 2020 2020 6135 3030 4320 3d20 6d6f  ..    a500C = mo
+00018ac0: 6469 7343 4469 6374 5b27 6461 696c 7953  disCDict['dailyS
+00018ad0: 5235 3030 4127 5d0d 0a20 2020 2074 3530  R500A']..    t50
+00018ae0: 3043 203d 206d 6f64 6973 4344 6963 745b  0C = modisCDict[
+00018af0: 2764 6169 6c79 5352 3530 3054 275d 0d0a  'dailySR500T']..
+00018b00: 2020 2020 6131 3030 3043 203d 206d 6f64      a1000C = mod
+00018b10: 6973 4344 6963 745b 2764 6169 6c79 4c53  isCDict['dailyLS
+00018b20: 5431 3030 3041 275d 0d0a 2020 2020 7431  T1000A']..    t1
+00018b30: 3030 3043 203d 206d 6f64 6973 4344 6963  000C = modisCDic
+00018b40: 745b 2764 6169 6c79 4c53 5431 3030 3054  t['dailyLST1000T
+00018b50: 275d 0d0a 2020 2020 7669 6577 416e 676c  ']..    viewAngl
+00018b60: 6542 616e 644e 616d 6573 203d 2064 6169  eBandNames = dai
+00018b70: 6c79 5669 6577 416e 676c 6542 616e 644e  lyViewAngleBandN
+00018b80: 616d 6573 3b0d 0a0d 0a20 2023 5075 6c6c  ames;....  #Pull
+00018b90: 2069 6d61 6765 7320 6672 6f6d 2065 6163   images from eac
+00018ba0: 6820 6f66 2074 6865 2063 6f6c 6c65 6374  h of the collect
+00018bb0: 696f 6e73 0d0a 2020 6132 3530 203d 2065  ions..  a250 = e
+00018bc0: 652e 496d 6167 6543 6f6c 6c65 6374 696f  e.ImageCollectio
+00018bd0: 6e28 6132 3530 4329 5c0d 0a20 2020 202e  n(a250C)\..    .
+00018be0: 6669 6c74 6572 2865 652e 4669 6c74 6572  filter(ee.Filter
+00018bf0: 2e63 616c 656e 6461 7252 616e 6765 2873  .calendarRange(s
+00018c00: 7461 7274 5965 6172 2c65 6e64 5965 6172  tartYear,endYear
+00018c10: 2c27 7965 6172 2729 295c 0d0a 2020 2020  ,'year'))\..    
+00018c20: 2e66 696c 7465 7228 6565 2e46 696c 7465  .filter(ee.Filte
+00018c30: 722e 6361 6c65 6e64 6172 5261 6e67 6528  r.calendarRange(
+00018c40: 7374 6172 744a 756c 6961 6e2c 656e 644a  startJulian,endJ
+00018c50: 756c 6961 6e29 295c 0d0a 2020 2020 2e73  ulian))\..    .s
+00018c60: 656c 6563 7428 6d6f 6469 7332 3530 5365  elect(modis250Se
+00018c70: 6c65 6374 4261 6e64 732c 6d6f 6469 7332  lectBands,modis2
+00018c80: 3530 4261 6e64 4e61 6d65 7329 0d0a 0d0a  50BandNames)....
+00018c90: 0d0a 2020 7432 3530 203d 2065 652e 496d  ..  t250 = ee.Im
+00018ca0: 6167 6543 6f6c 6c65 6374 696f 6e28 7432  ageCollection(t2
+00018cb0: 3530 4329 5c0d 0a20 202e 6669 6c74 6572  50C)\..  .filter
+00018cc0: 2865 652e 4669 6c74 6572 2e63 616c 656e  (ee.Filter.calen
+00018cd0: 6461 7252 616e 6765 2873 7461 7274 5965  darRange(startYe
+00018ce0: 6172 2c65 6e64 5965 6172 2c27 7965 6172  ar,endYear,'year
+00018cf0: 2729 295c 0d0a 2020 2e66 696c 7465 7228  '))\..  .filter(
+00018d00: 6565 2e46 696c 7465 722e 6361 6c65 6e64  ee.Filter.calend
+00018d10: 6172 5261 6e67 6528 7374 6172 744a 756c  arRange(startJul
+00018d20: 6961 6e2c 656e 644a 756c 6961 6e29 295c  ian,endJulian))\
+00018d30: 0d0a 2020 2e73 656c 6563 7428 6d6f 6469  ..  .select(modi
+00018d40: 7332 3530 5365 6c65 6374 4261 6e64 732c  s250SelectBands,
+00018d50: 6d6f 6469 7332 3530 4261 6e64 4e61 6d65  modis250BandName
+00018d60: 7329 0d0a 0d0a 0d0a 2020 6465 6620 6765  s)......  def ge
+00018d70: 7435 3030 2863 293a 0d0a 2020 2020 696d  t500(c):..    im
+00018d80: 6167 6573 203d 2065 652e 496d 6167 6543  ages = ee.ImageC
+00018d90: 6f6c 6c65 6374 696f 6e28 6329 5c0d 0a20  ollection(c)\.. 
+00018da0: 2020 2020 2020 2020 202e 6669 6c74 6572           .filter
+00018db0: 2865 652e 4669 6c74 6572 2e63 616c 656e  (ee.Filter.calen
+00018dc0: 6461 7252 616e 6765 2873 7461 7274 5965  darRange(startYe
+00018dd0: 6172 2c65 6e64 5965 6172 2c27 7965 6172  ar,endYear,'year
+00018de0: 2729 295c 0d0a 2020 2020 2020 2020 2020  '))\..          
+00018df0: 2e66 696c 7465 7228 6565 2e46 696c 7465  .filter(ee.Filte
+00018e00: 722e 6361 6c65 6e64 6172 5261 6e67 6528  r.calendarRange(
+00018e10: 7374 6172 744a 756c 6961 6e2c 656e 644a  startJulian,endJ
+00018e20: 756c 6961 6e29 290d 0a20 2020 2064 6566  ulian))..    def
+00018e30: 2061 7070 6c79 5a65 6e69 7468 2869 6d67   applyZenith(img
+00018e40: 293a 0d0a 2020 2020 2020 696d 6720 3d20  ):..      img = 
+00018e50: 696d 672e 6d61 736b 2869 6d67 2e6d 6173  img.mask(img.mas
+00018e60: 6b28 292e 416e 6428 696d 672e 7365 6c65  k().And(img.sele
+00018e70: 6374 285b 2753 656e 736f 725a 656e 6974  ct(['SensorZenit
+00018e80: 6827 5d29 2e6c 7428 7a65 6e69 7468 5468  h']).lt(zenithTh
+00018e90: 7265 7368 2a31 3030 2929 290d 0a20 2020  resh*100)))..   
+00018ea0: 2020 2069 6620 6d61 736b 5751 413a 696d     if maskWQA:im
+00018eb0: 6720 3d20 6d61 736b 436c 6f75 6473 5751  g = maskCloudsWQ
+00018ec0: 4128 696d 6729 0d0a 2020 2020 2020 7265  A(img)..      re
+00018ed0: 7475 726e 2069 6d67 0d0a 2020 2020 234d  turn img..    #M
+00018ee0: 6173 6b20 7069 7865 6c73 2061 626f 7665  ask pixels above
+00018ef0: 2061 2063 6572 7461 696e 207a 656e 6974   a certain zenit
+00018f00: 680d 0a20 2020 2069 6620 6461 696c 793a  h..    if daily:
+00018f10: 0d0a 2020 2020 2020 6966 206d 6173 6b57  ..      if maskW
+00018f20: 5141 3a70 7269 6e74 2827 4d61 736b 696e  QA:print('Maskin
+00018f30: 6720 7769 7468 2051 4120 6261 6e64 3a27  g with QA band:'
+00018f40: 2c63 290d 0a20 2020 2020 2069 6d61 6765  ,c)..      image
+00018f50: 7320 3d20 696d 6167 6573 2e6d 6170 2861  s = images.map(a
+00018f60: 7070 6c79 5a65 6e69 7468 290d 0a0d 0a20  pplyZenith).... 
+00018f70: 2020 2069 6620 6164 644c 6f6f 6b41 6e67     if addLookAng
+00018f80: 6c65 4261 6e64 733a 0d0a 2020 2020 2020  leBands:..      
+00018f90: 696d 6167 6573 203d 2069 6d61 6765 732e  images = images.
+00018fa0: 7365 6c65 6374 2865 652e 4c69 7374 286d  select(ee.List(m
+00018fb0: 6f64 6973 3530 3053 656c 6563 7442 616e  odis500SelectBan
+00018fc0: 6473 292e 6361 7428 7669 6577 416e 676c  ds).cat(viewAngl
+00018fd0: 6542 616e 644e 616d 6573 292c 6565 2e4c  eBandNames),ee.L
+00018fe0: 6973 7428 6d6f 6469 7335 3030 4261 6e64  ist(modis500Band
+00018ff0: 4e61 6d65 7329 2e63 6174 2876 6965 7741  Names).cat(viewA
+00019000: 6e67 6c65 4261 6e64 4e61 6d65 7329 293b  ngleBandNames));
+00019010: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00019020: 2020 2069 6d61 6765 7320 3d20 696d 6167     images = imag
+00019030: 6573 2e73 656c 6563 7428 6d6f 6469 7335  es.select(modis5
+00019040: 3030 5365 6c65 6374 4261 6e64 732c 6d6f  00SelectBands,mo
+00019050: 6469 7335 3030 4261 6e64 4e61 6d65 7329  dis500BandNames)
+00019060: 0d0a 0d0a 2020 2020 7265 7475 726e 2069  ....    return i
+00019070: 6d61 6765 730d 0a0d 0a0d 0a20 2061 3530  mages......  a50
+00019080: 3020 3d20 6765 7435 3030 2861 3530 3043  0 = get500(a500C
+00019090: 290d 0a20 2074 3530 3020 3d20 6765 7435  )..  t500 = get5
+000190a0: 3030 2874 3530 3043 290d 0a0d 0a0d 0a20  00(t500C)...... 
+000190b0: 2023 4966 2074 6865 726d 616c 2063 6f6c   #If thermal col
+000190c0: 6c65 6374 696f 6e20 6973 2077 616e 7465  lection is wante
+000190d0: 642c 2070 756c 6c20 6974 2061 7320 7765  d, pull it as we
+000190e0: 6c6c 0d0a 2020 6966 2075 7365 5465 6d70  ll..  if useTemp
+000190f0: 496e 436c 6f75 644d 6173 6b3a 0d0a 2020  InCloudMask:..  
+00019100: 2020 7431 3030 3020 3d20 6565 2e49 6d61    t1000 = ee.Ima
+00019110: 6765 436f 6c6c 6563 7469 6f6e 2874 3130  geCollection(t10
+00019120: 3030 4329 5c0d 0a20 2020 2020 2020 2020  00C)\..         
+00019130: 2020 202e 6669 6c74 6572 2865 652e 4669     .filter(ee.Fi
+00019140: 6c74 6572 2e63 616c 656e 6461 7252 616e  lter.calendarRan
+00019150: 6765 2873 7461 7274 5965 6172 2c65 6e64  ge(startYear,end
+00019160: 5965 6172 2c27 7965 6172 2729 295c 0d0a  Year,'year'))\..
+00019170: 2020 2020 2020 2020 2020 2020 2e66 696c              .fil
+00019180: 7465 7228 6565 2e46 696c 7465 722e 6361  ter(ee.Filter.ca
+00019190: 6c65 6e64 6172 5261 6e67 6528 7374 6172  lendarRange(star
+000191a0: 744a 756c 6961 6e2c 656e 644a 756c 6961  tJulian,endJulia
+000191b0: 6e29 295c 0d0a 2020 2020 2020 2020 2020  n))\..          
+000191c0: 2020 2e73 656c 6563 7428 5b30 2c38 2c39    .select([0,8,9
+000191d0: 5d2c 5b27 7465 6d70 272c 2745 6d69 735f  ],['temp','Emis_
+000191e0: 3331 272c 2745 6d69 735f 3332 275d 293b  31','Emis_32']);
+000191f0: 0d0a 0d0a 2020 2020 6131 3030 3020 3d20  ....    a1000 = 
+00019200: 6565 2e49 6d61 6765 436f 6c6c 6563 7469  ee.ImageCollecti
+00019210: 6f6e 2861 3130 3030 4329 5c0d 0a20 2020  on(a1000C)\..   
+00019220: 2020 2020 2020 2020 202e 6669 6c74 6572           .filter
+00019230: 2865 652e 4669 6c74 6572 2e63 616c 656e  (ee.Filter.calen
+00019240: 6461 7252 616e 6765 2873 7461 7274 5965  darRange(startYe
+00019250: 6172 2c65 6e64 5965 6172 2c27 7965 6172  ar,endYear,'year
+00019260: 2729 295c 0d0a 2020 2020 2020 2020 2020  '))\..          
+00019270: 2020 2e66 696c 7465 7228 6565 2e46 696c    .filter(ee.Fil
+00019280: 7465 722e 6361 6c65 6e64 6172 5261 6e67  ter.calendarRang
+00019290: 6528 7374 6172 744a 756c 6961 6e2c 656e  e(startJulian,en
+000192a0: 644a 756c 6961 6e29 295c 0d0a 2020 2020  dJulian))\..    
+000192b0: 2020 2020 2020 2020 2e73 656c 6563 7428          .select(
+000192c0: 5b30 2c38 2c39 5d2c 5b27 7465 6d70 272c  [0,8,9],['temp',
+000192d0: 2745 6d69 735f 3331 272c 2745 6d69 735f  'Emis_31','Emis_
+000192e0: 3332 275d 293b 0d0a 0d0a 0d0a 2020 234e  32']);......  #N
+000192f0: 6f77 2061 6c6c 2063 6f6c 6c65 6374 696f  ow all collectio
+00019300: 6e73 2061 7265 2070 756c 6c65 642c 2073  ns are pulled, s
+00019310: 7461 7274 206a 6f69 6e69 6e67 2074 6865  tart joining the
+00019320: 6d0d 0a20 2023 4669 7273 7420 6a6f 696e  m..  #First join
+00019330: 2074 6865 2032 3530 2061 6e64 2035 3030   the 250 and 500
+00019340: 206d 2041 7175 610d 0a20 2061 203d 206a   m Aqua..  a = j
+00019350: 6f69 6e43 6f6c 6c65 6374 696f 6e73 2861  oinCollections(a
+00019360: 3235 302c 6135 3030 2c46 616c 7365 290d  250,a500,False).
+00019370: 0a0d 0a20 2023 5468 656e 2054 6572 7261  ...  #Then Terra
+00019380: 0d0a 2020 7420 3d20 6a6f 696e 436f 6c6c  ..  t = joinColl
+00019390: 6563 7469 6f6e 7328 7432 3530 2c74 3530  ections(t250,t50
+000193a0: 302c 4661 6c73 6529 0d0a 0d0a 2020 2349  0,False)....  #I
+000193b0: 6620 7465 6d70 2077 6173 2070 756c 6c65  f temp was pulle
+000193c0: 642c 206a 6f69 6e20 7468 6174 2069 6e20  d, join that in 
+000193d0: 6173 2077 656c 6c0d 0a20 2023 416c 736f  as well..  #Also
+000193e0: 2073 656c 6563 7420 7468 6520 6261 6e64   select the band
+000193f0: 7320 696e 2061 6e20 4c35 2d6c 696b 6520  s in an L5-like 
+00019400: 6f72 6465 7220 616e 6420 6769 7665 2064  order and give d
+00019410: 6573 6372 6970 7469 7665 206e 616d 6573  escriptive names
+00019420: 0d0a 2020 6966 2075 7365 5465 6d70 496e  ..  if useTempIn
+00019430: 436c 6f75 644d 6173 6b3a 0d0a 2020 2020  CloudMask:..    
+00019440: 6120 3d20 6a6f 696e 436f 6c6c 6563 7469  a = joinCollecti
+00019450: 6f6e 7328 612c 6131 3030 302c 4661 6c73  ons(a,a1000,Fals
+00019460: 6529 0d0a 2020 2020 7420 3d20 6a6f 696e  e)..    t = join
+00019470: 436f 6c6c 6563 7469 6f6e 7328 742c 7431  Collections(t,t1
+00019480: 3030 302c 4661 6c73 6529 0d0a 0d0a 0d0a  000,False)......
+00019490: 2020 2320 2020 7453 656c 6563 744f 7264    #   tSelectOrd
+000194a0: 6572 203d 2077 5465 6d70 5365 6c65 6374  er = wTempSelect
+000194b0: 4f72 6465 720d 0a20 2023 2020 2074 5374  Order..  #   tSt
+000194c0: 644e 616d 6573 203d 2077 5465 6d70 5374  dNames = wTempSt
+000194d0: 644e 616d 6573 0d0a 0d0a 2020 2320 2349  dNames....  # #I
+000194e0: 6620 6e6f 2074 6865 726d 616c 2077 6173  f no thermal was
+000194f0: 2070 756c 6c65 642c 206c 6561 7665 2074   pulled, leave t
+00019500: 6861 7420 6f75 740d 0a20 2023 2065 6c73  hat out..  # els
+00019510: 653a 0d0a 2020 2320 2020 7453 656c 6563  e:..  #   tSelec
+00019520: 744f 7264 6572 203d 2077 6f54 656d 7053  tOrder = woTempS
+00019530: 656c 6563 744f 7264 6572 0d0a 2020 2320  electOrder..  # 
+00019540: 2020 7453 7464 4e61 6d65 7320 3d20 776f    tStdNames = wo
+00019550: 5465 6d70 5374 644e 616d 6573 0d0a 0d0a  TempStdNames....
+00019560: 2020 6120 3d20 612e 6d61 7028 6c61 6d62    a = a.map(lamb
+00019570: 6461 2069 6d67 3a69 6d67 2e73 6574 287b  da img:img.set({
+00019580: 2770 6c61 7466 6f72 6d27 3a27 6171 7561  'platform':'aqua
+00019590: 277d 2929 3b0d 0a20 2074 203d 2074 2e6d  '}));..  t = t.m
+000195a0: 6170 286c 616d 6264 6120 696d 673a 696d  ap(lambda img:im
+000195b0: 672e 7365 7428 7b27 706c 6174 666f 726d  g.set({'platform
+000195c0: 273a 2774 6572 7261 277d 2929 3b0d 0a0d  ':'terra'}));...
+000195d0: 0a0d 0a20 2069 6628 6461 696c 7929 3a64  ...  if(daily):d
+000195e0: 6169 6c79 5069 6563 6520 3d20 2744 6169  ailyPiece = 'Dai
+000195f0: 6c79 270d 0a20 2065 6c73 653a 6461 696c  ly'..  else:dail
+00019600: 7950 6965 6365 203d 2027 436f 6d70 6f73  yPiece = 'Compos
+00019610: 6974 6527 0d0a 0d0a 2020 6966 2875 7365  ite'....  if(use
+00019620: 5465 6d70 496e 436c 6f75 644d 6173 6b29  TempInCloudMask)
+00019630: 3a74 656d 7050 6965 6365 203d 2027 7465  :tempPiece = 'te
+00019640: 6d70 270d 0a20 2065 6c73 653a 7465 6d70  mp'..  else:temp
+00019650: 5069 6563 6520 3d20 276e 6f54 656d 7027  Piece = 'noTemp'
+00019660: 0d0a 2020 6966 2061 6464 4c6f 6f6b 416e  ..  if addLookAn
+00019670: 676c 6542 616e 6473 3a61 6e67 6c65 5069  gleBands:anglePi
+00019680: 6563 6520 3d20 2741 6e67 6c65 270d 0a20  ece = 'Angle'.. 
+00019690: 2065 6c73 653a 616e 676c 6550 6965 6365   else:anglePiece
+000196a0: 203d 2027 4e6f 416e 676c 6527 0d0a 2020   = 'NoAngle'..  
+000196b0: 6d75 6c74 4b65 7920 3d20 7465 6d70 5069  multKey = tempPi
+000196c0: 6563 652b 616e 676c 6550 6965 6365 2b64  ece+anglePiece+d
+000196d0: 6169 6c79 5069 6563 650d 0a0d 0a20 206d  ailyPiece....  m
+000196e0: 756c 7420 3d20 6d75 6c74 4d6f 6469 7344  ult = multModisD
+000196f0: 6963 745b 6d75 6c74 4b65 795d 0d0a 2020  ict[multKey]..  
+00019700: 6d75 6c74 496d 6167 6520 3d20 6d75 6c74  multImage = mult
+00019710: 5b30 5d0d 0a20 206d 756c 744e 616d 6573  [0]..  multNames
+00019720: 203d 206d 756c 745b 315d 0d0a 0d0a 2020   = mult[1]....  
+00019730: 234a 6f69 6e20 5465 7272 6120 616e 6420  #Join Terra and 
+00019740: 4171 7561 0d0a 2020 6a6f 696e 6564 203d  Aqua..  joined =
+00019750: 2065 652e 496d 6167 6543 6f6c 6c65 6374   ee.ImageCollect
+00019760: 696f 6e28 612e 6d65 7267 6528 7429 2923  ion(a.merge(t))#
+00019770: 2e73 656c 6563 7428 7453 656c 6563 744f  .select(tSelectO
+00019780: 7264 6572 2c74 5374 644e 616d 6573 290d  rder,tStdNames).
+00019790: 0a0d 0a20 2064 6566 206d 756c 7469 706c  ...  def multipl
+000197a0: 7949 6d67 2869 6d67 293a 0d0a 2020 2020  yImg(img):..    
+000197b0: 7265 7475 726e 2069 6d67 2e6d 756c 7469  return img.multi
+000197c0: 706c 7928 6d75 6c74 496d 6167 6529 2e66  ply(multImage).f
+000197d0: 6c6f 6174 2829 2e73 656c 6563 7428 6d75  loat().select(mu
+000197e0: 6c74 4e61 6d65 7329 5c0d 0a20 2020 2020  ltNames)\..     
+000197f0: 2020 202e 636f 7079 5072 6f70 6572 7469     .copyProperti
+00019800: 6573 2869 6d67 2c5b 2773 7973 7465 6d3a  es(img,['system:
+00019810: 7469 6d65 5f73 7461 7274 272c 2773 7973  time_start','sys
+00019820: 7465 6d3a 7469 6d65 5f65 6e64 272c 2773  tem:time_end','s
+00019830: 7973 7465 6d3a 696e 6465 7827 5d29 5c0d  ystem:index'])\.
+00019840: 0a20 2020 2020 2020 202e 636f 7079 5072  .        .copyPr
+00019850: 6f70 6572 7469 6573 2869 6d67 290d 0a20  operties(img).. 
+00019860: 2064 6566 2073 6574 5265 7361 6d70 6c65   def setResample
+00019870: 2869 6d67 293a 0d0a 2020 2020 7265 7475  (img):..    retu
+00019880: 726e 2069 6d67 2e72 6573 616d 706c 6528  rn img.resample(
+00019890: 7265 7361 6d70 6c65 4d65 7468 6f64 290d  resampleMethod).
+000198a0: 0a0d 0a20 206a 6f69 6e65 6420 3d20 6a6f  ...  joined = jo
+000198b0: 696e 6564 2e6d 6170 286d 756c 7469 706c  ined.map(multipl
+000198c0: 7949 6d67 290d 0a20 2069 6620 2072 6573  yImg)..  if  res
+000198d0: 616d 706c 654d 6574 686f 6420 696e 205b  ampleMethod in [
+000198e0: 2762 696c 696e 6561 7227 2c27 6269 6375  'bilinear','bicu
+000198f0: 6269 6327 5d3a 0d0a 2020 2020 7072 696e  bic']:..    prin
+00019900: 7428 2753 6574 7469 6e67 2072 6573 616d  t('Setting resam
+00019910: 706c 6520 6d65 7468 6f64 2074 6f20 272c  ple method to ',
+00019920: 7265 7361 6d70 6c65 4d65 7468 6f64 290d  resampleMethod).
+00019930: 0a20 2020 206a 6f69 6e65 6420 3d20 6a6f  .    joined = jo
+00019940: 696e 6564 2e6d 6170 2873 6574 5265 7361  ined.map(setResa
+00019950: 6d70 6c65 290d 0a20 2072 6574 7572 6e20  mple)..  return 
+00019960: 6a6f 696e 6564 0d0a 0d0a 0d0a 2346 756e  joined......#Fun
+00019970: 6374 696f 6e20 746f 2067 6574 2063 6c6f  ction to get clo
+00019980: 7564 2c20 636c 6f75 6420 7368 6164 6f77  ud, cloud shadow
+00019990: 2062 7573 7465 6420 6d6f 6469 7320 696d   busted modis im
+000199a0: 6167 6573 0d0a 2354 616b 6573 2063 6172  ages..#Takes car
+000199b0: 6520 6f66 206d 6174 6368 696e 6720 6469  e of matching di
+000199c0: 6666 6572 656e 7420 6d6f 6469 7320 636f  fferent modis co
+000199d0: 6c6c 6563 7469 6f6e 7320 6173 2077 656c  llections as wel
+000199e0: 6c0d 0a64 6566 2067 6574 5072 6f63 6573  l..def getProces
+000199f0: 7365 644d 6f64 6973 2873 7461 7274 5965  sedModis(startYe
+00019a00: 6172 2c0d 0a20 2020 2020 2020 2020 2020  ar,..           
+00019a10: 2065 6e64 5965 6172 2c0d 0a20 2020 2020   endYear,..     
+00019a20: 2020 2020 2020 2073 7461 7274 4a75 6c69         startJuli
+00019a30: 616e 2c0d 0a20 2020 2020 2020 2020 2020  an,..           
+00019a40: 2065 6e64 4a75 6c69 616e 2c0d 0a20 2020   endJulian,..   
+00019a50: 2020 2020 2020 2020 207a 656e 6974 6854           zenithT
+00019a60: 6872 6573 6820 3d20 3930 2c0d 0a20 2020  hresh = 90,..   
+00019a70: 2020 2020 2020 2020 2061 6464 4c6f 6f6b           addLook
+00019a80: 416e 676c 6542 616e 6473 203d 2054 7275  AngleBands = Tru
+00019a90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00019aa0: 6170 706c 7943 6c6f 7564 5363 6f72 6520  applyCloudScore 
+00019ab0: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+00019ac0: 2020 2020 2061 7070 6c79 5444 4f4d 203d       applyTDOM =
+00019ad0: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+00019ae0: 2020 2020 7573 6554 656d 7049 6e43 6c6f      useTempInClo
+00019af0: 7564 4d61 736b 203d 2054 7275 652c 0d0a  udMask = True,..
+00019b00: 2020 2020 2020 2020 2020 2020 636c 6f75              clou
+00019b10: 6453 636f 7265 5468 7265 7368 203d 2032  dScoreThresh = 2
+00019b20: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00019b30: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
+00019b40: 654f 6666 7365 7420 3d20 5472 7565 2c0d  eOffset = True,.
+00019b50: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+00019b60: 7564 5363 6f72 6550 6374 6c20 3d20 3130  udScorePctl = 10
+00019b70: 2c0d 0a20 2020 2020 2020 2020 2020 207a  ,..            z
+00019b80: 5363 6f72 6554 6872 6573 6820 3d20 2d31  ScoreThresh = -1
+00019b90: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00019ba0: 6861 646f 7753 756d 5468 7265 7368 203d  hadowSumThresh =
+00019bb0: 2030 2e33 352c 0d0a 2020 2020 2020 2020   0.35,..        
+00019bc0: 2020 2020 636f 6e74 7261 6374 5069 7865      contractPixe
+00019bd0: 6c73 203d 2030 2c0d 0a20 2020 2020 2020  ls = 0,..       
+00019be0: 2020 2020 2064 696c 6174 6550 6978 656c       dilatePixel
+00019bf0: 7320 3d20 322e 352c 0d0a 2020 2020 2020  s = 2.5,..      
+00019c00: 2020 2020 2020 7368 6164 6f77 5375 6d42        shadowSumB
+00019c10: 616e 6473 203d 205b 276e 6972 272c 2773  ands = ['nir','s
+00019c20: 7769 7232 275d 2c0d 0a20 2020 2020 2020  wir2'],..       
+00019c30: 2020 2020 2072 6573 616d 706c 654d 6574       resampleMet
+00019c40: 686f 6420 3d20 2762 6963 7562 6963 272c  hod = 'bicubic',
+00019c50: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00019c60: 6543 6f6d 7075 7465 6443 6c6f 7564 5363  eComputedCloudSc
+00019c70: 6f72 654f 6666 7365 7420 3d20 4e6f 6e65  oreOffset = None
+00019c80: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00019c90: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
+00019ca0: 4d65 616e 203d 204e 6f6e 652c 0d0a 2020  Mean = None,..  
+00019cb0: 2020 2020 2020 2020 2020 7072 6543 6f6d            preCom
+00019cc0: 7075 7465 6454 444f 4d49 5253 7464 4465  putedTDOMIRStdDe
+00019cd0: 7620 3d20 4e6f 6e65 2c0d 0a20 2020 2020  v = None,..     
+00019ce0: 2020 2020 2020 2061 6464 546f 4d61 7020         addToMap 
+00019cf0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00019d00: 2020 2020 2020 6372 7320 3d20 2745 5053        crs = 'EPS
+00019d10: 473a 3433 3236 272c 0d0a 2020 2020 2020  G:4326',..      
+00019d20: 2020 2020 2020 7363 616c 6520 3d20 3235        scale = 25
+00019d30: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00019d40: 7472 616e 7366 6f72 6d20 3d20 4e6f 6e65  transform = None
+00019d50: 293a 0d0a 0d0a 2020 6172 6773 203d 2066  ):....  args = f
+00019d60: 6f72 6d61 7441 7267 7328 6c6f 6361 6c73  ormatArgs(locals
+00019d70: 2829 290d 0a20 2069 6620 2761 7267 7327  ())..  if 'args'
+00019d80: 2069 6e20 6172 6773 2e6b 6579 7328 293a   in args.keys():
+00019d90: 0d0a 2020 2020 6465 6c20 6172 6773 5b27  ..    del args['
+00019da0: 6172 6773 275d 0d0a 0d0a 2020 2347 6574  args']....  #Get
+00019db0: 206a 6f69 6e65 6420 6d6f 6469 7320 636f   joined modis co
+00019dc0: 6c6c 6563 7469 6f6e 0d0a 2020 6d6f 6469  llection..  modi
+00019dd0: 7349 6d61 6765 7320 3d20 6765 744d 6f64  sImages = getMod
+00019de0: 6973 4461 7461 2873 7461 7274 5965 6172  isData(startYear
+00019df0: 2c65 6e64 5965 6172 2c73 7461 7274 4a75  ,endYear,startJu
+00019e00: 6c69 616e 2c65 6e64 4a75 6c69 616e 2c0d  lian,endJulian,.
+00019e10: 0a20 2020 2064 6169 6c79 203d 2054 7275  .    daily = Tru
+00019e20: 652c 0d0a 2020 2020 6d61 736b 5751 4120  e,..    maskWQA 
+00019e30: 3d20 4661 6c73 652c 0d0a 2020 2020 7a65  = False,..    ze
+00019e40: 6e69 7468 5468 7265 7368 203d 207a 656e  nithThresh = zen
+00019e50: 6974 6854 6872 6573 682c 0d0a 2020 2020  ithThresh,..    
+00019e60: 7573 6554 656d 7049 6e43 6c6f 7564 4d61  useTempInCloudMa
+00019e70: 736b 203d 2075 7365 5465 6d70 496e 436c  sk = useTempInCl
+00019e80: 6f75 644d 6173 6b2c 0d0a 2020 2020 6164  oudMask,..    ad
+00019e90: 644c 6f6f 6b41 6e67 6c65 4261 6e64 7320  dLookAngleBands 
+00019ea0: 3d20 6164 644c 6f6f 6b41 6e67 6c65 4261  = addLookAngleBa
+00019eb0: 6e64 732c 0d0a 2020 2020 7265 7361 6d70  nds,..    resamp
+00019ec0: 6c65 4d65 7468 6f64 203d 2020 7265 7361  leMethod =  resa
+00019ed0: 6d70 6c65 4d65 7468 6f64 290d 0a0d 0a20  mpleMethod).... 
+00019ee0: 2069 6620 6164 6454 6f4d 6170 3a0d 0a20   if addToMap:.. 
+00019ef0: 2020 204d 6170 2e61 6464 4c61 7965 7228     Map.addLayer(
+00019f00: 6d6f 6469 7349 6d61 6765 732e 6d65 6469  modisImages.medi
+00019f10: 616e 2829 2e72 6570 726f 6a65 6374 2863  an().reproject(c
+00019f20: 7273 2c74 7261 6e73 666f 726d 2c73 6361  rs,transform,sca
+00019f30: 6c65 292c 7669 7a50 6172 616d 7346 616c  le),vizParamsFal
+00019f40: 7365 2c27 5261 7720 4d65 6469 616e 2729  se,'Raw Median')
+00019f50: 0d0a 0d0a 0d0a 2020 6966 2061 7070 6c79  ......  if apply
+00019f60: 436c 6f75 6453 636f 7265 3a0d 0a20 2020  CloudScore:..   
+00019f70: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
+00019f80: 2063 6c6f 7564 5363 6f72 6527 290d 0a20   cloudScore').. 
+00019f90: 2020 206d 6f64 6973 496d 6167 6573 203d     modisImages =
+00019fa0: 2061 7070 6c79 436c 6f75 6453 636f 7265   applyCloudScore
+00019fb0: 416c 676f 7269 7468 6d28 6d6f 6469 7349  Algorithm(modisI
+00019fc0: 6d61 6765 732c 6d6f 6469 7343 6c6f 7564  mages,modisCloud
+00019fd0: 5363 6f72 652c 636c 6f75 6453 636f 7265  Score,cloudScore
+00019fe0: 5468 7265 7368 2c63 6c6f 7564 5363 6f72  Thresh,cloudScor
+00019ff0: 6550 6374 6c2c 636f 6e74 7261 6374 5069  ePctl,contractPi
+0001a000: 7865 6c73 2c64 696c 6174 6550 6978 656c  xels,dilatePixel
+0001a010: 732c 7065 7266 6f72 6d43 6c6f 7564 5363  s,performCloudSc
+0001a020: 6f72 654f 6666 7365 742c 7072 6543 6f6d  oreOffset,preCom
+0001a030: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
+0001a040: 6666 7365 7429 0d0a 0d0a 2020 2020 6966  ffset)....    if
+0001a050: 2061 6464 546f 4d61 703a 0d0a 2020 2020   addToMap:..    
+0001a060: 2020 4d61 702e 6164 644c 6179 6572 286d    Map.addLayer(m
+0001a070: 6f64 6973 496d 6167 6573 2e6d 6564 6961  odisImages.media
+0001a080: 6e28 292e 7265 7072 6f6a 6563 7428 6372  n().reproject(cr
+0001a090: 732c 7472 616e 7366 6f72 6d2c 7363 616c  s,transform,scal
+0001a0a0: 6529 2c76 697a 5061 7261 6d73 4661 6c73  e),vizParamsFals
+0001a0b0: 652c 2743 6c6f 7564 204d 6173 6b65 6420  e,'Cloud Masked 
+0001a0c0: 4d65 6469 616e 272c 4661 6c73 6529 0d0a  Median',False)..
+0001a0d0: 2020 2020 2020 4d61 702e 6164 644c 6179        Map.addLay
+0001a0e0: 6572 286d 6f64 6973 496d 6167 6573 2e6d  er(modisImages.m
+0001a0f0: 696e 2829 2e72 6570 726f 6a65 6374 2863  in().reproject(c
+0001a100: 7273 2c74 7261 6e73 666f 726d 2c73 6361  rs,transform,sca
+0001a110: 6c65 292c 7669 7a50 6172 616d 7346 616c  le),vizParamsFal
+0001a120: 7365 2c27 436c 6f75 6420 4d61 736b 6564  se,'Cloud Masked
+0001a130: 204d 696e 272c 4661 6c73 6529 0d0a 0d0a   Min',False)....
+0001a140: 2020 6966 2061 7070 6c79 5444 4f4d 3a0d    if applyTDOM:.
+0001a150: 0a20 2020 2070 7269 6e74 2827 4170 706c  .    print('Appl
+0001a160: 7969 6e67 2054 444f 4d27 290d 0a20 2020  ying TDOM')..   
+0001a170: 2023 4669 6e64 2061 6e64 206d 6173 6b20   #Find and mask 
+0001a180: 6f75 7420 6461 726b 206f 7574 6c69 6572  out dark outlier
+0001a190: 730d 0a20 2020 206d 6f64 6973 496d 6167  s..    modisImag
+0001a1a0: 6573 203d 2073 696d 706c 6554 444f 4d32  es = simpleTDOM2
+0001a1b0: 286d 6f64 6973 496d 6167 6573 2c7a 5363  (modisImages,zSc
+0001a1c0: 6f72 6554 6872 6573 682c 7368 6164 6f77  oreThresh,shadow
+0001a1d0: 5375 6d54 6872 6573 682c 636f 6e74 7261  SumThresh,contra
+0001a1e0: 6374 5069 7865 6c73 2c64 696c 6174 6550  ctPixels,dilateP
+0001a1f0: 6978 656c 732c 7368 6164 6f77 5375 6d42  ixels,shadowSumB
+0001a200: 616e 6473 2c70 7265 436f 6d70 7574 6564  ands,preComputed
+0001a210: 5444 4f4d 4952 4d65 616e 2c70 7265 436f  TDOMIRMean,preCo
+0001a220: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
+0001a230: 6576 290d 0a0d 0a20 2020 2069 6620 6164  ev)....    if ad
+0001a240: 6454 6f4d 6170 3a0d 0a20 2020 2020 204d  dToMap:..      M
+0001a250: 6170 2e61 6464 4c61 7965 7228 6d6f 6469  ap.addLayer(modi
+0001a260: 7349 6d61 6765 732e 6d65 6469 616e 2829  sImages.median()
+0001a270: 2e72 6570 726f 6a65 6374 2863 7273 2c74  .reproject(crs,t
+0001a280: 7261 6e73 666f 726d 2c73 6361 6c65 292c  ransform,scale),
+0001a290: 7669 7a50 6172 616d 7346 616c 7365 2c27  vizParamsFalse,'
+0001a2a0: 436c 6f75 642f 436c 6f75 6420 5368 6164  Cloud/Cloud Shad
+0001a2b0: 6f77 204d 6173 6b65 6420 4d65 6469 616e  ow Masked Median
+0001a2c0: 272c 4661 6c73 6529 0d0a 2020 2020 2020  ',False)..      
+0001a2d0: 4d61 702e 6164 644c 6179 6572 286d 6f64  Map.addLayer(mod
+0001a2e0: 6973 496d 6167 6573 2e6d 696e 2829 2e72  isImages.min().r
+0001a2f0: 6570 726f 6a65 6374 2863 7273 2c74 7261  eproject(crs,tra
+0001a300: 6e73 666f 726d 2c73 6361 6c65 292c 7669  nsform,scale),vi
+0001a310: 7a50 6172 616d 7346 616c 7365 2c27 436c  zParamsFalse,'Cl
+0001a320: 6f75 642f 436c 6f75 6420 5368 6164 6f77  oud/Cloud Shadow
+0001a330: 204d 6173 6b65 6420 4d69 6e27 2c46 616c   Masked Min',Fal
+0001a340: 7365 290d 0a0d 0a20 206d 6f64 6973 496d  se)....  modisIm
+0001a350: 6167 6573 203d 206d 6f64 6973 496d 6167  ages = modisImag
+0001a360: 6573 2e6d 6170 2873 696d 706c 6541 6464  es.map(simpleAdd
+0001a370: 496e 6469 6365 7329 0d0a 2020 6d6f 6469  Indices)..  modi
+0001a380: 7349 6d61 6765 7320 3d20 6d6f 6469 7349  sImages = modisI
+0001a390: 6d61 6765 732e 6d61 7028 6c61 6d62 6461  mages.map(lambda
+0001a3a0: 2069 6d67 3a20 696d 672e 666c 6f61 7428   img: img.float(
+0001a3b0: 2929 0d0a 2020 7265 7475 726e 206d 6f64  ))..  return mod
+0001a3c0: 6973 496d 6167 6573 2e73 6574 2861 7267  isImages.set(arg
+0001a3d0: 7329 0d0a 2323 2323 2323 2323 2323 2323  s)..############
 0001a3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001a3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001a400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a410: 2323 2323 2323 0d0a 2346 756e 6374 696f  ######..#Functio
-0001a420: 6e20 746f 2074 616b 6520 696d 6167 6573  n to take images
-0001a430: 2061 6e64 2063 7265 6174 6520 6120 6d65   and create a me
-0001a440: 6469 616e 2063 6f6d 706f 7369 7465 2065  dian composite e
-0001a450: 7665 7279 206e 2064 6179 730d 0a64 6566  very n days..def
-0001a460: 206e 4461 7943 6f6d 706f 7369 7465 7328   nDayComposites(
-0001a470: 696d 6167 6573 2c73 7461 7274 5965 6172  images,startYear
-0001a480: 2c65 6e64 5965 6172 2c73 7461 7274 4a75  ,endYear,startJu
-0001a490: 6c69 616e 2c65 6e64 4a75 6c69 616e 2c63  lian,endJulian,c
-0001a4a0: 6f6d 706f 7369 7465 5065 7269 6f64 293a  ompositePeriod):
-0001a4b0: 0d0a 0d0a 2020 2363 7265 6174 6520 6475  ....  #create du
-0001a4c0: 6d6d 7920 696d 6167 6520 666f 7220 7769  mmy image for wi
-0001a4d0: 7468 206e 6f20 7661 6c75 6573 0d0a 2020  th no values..  
-0001a4e0: 6475 6d6d 7949 6d61 6765 203d 2065 652e  dummyImage = ee.
-0001a4f0: 496d 6167 6528 696d 6167 6573 2e66 6972  Image(images.fir
-0001a500: 7374 2829 290d 0a0d 0a20 2023 636f 6e76  st())....  #conv
-0001a510: 6572 7420 746f 2063 6f6d 706f 7369 7465  ert to composite
-0001a520: 7320 6173 2064 6566 696e 6564 2061 626f  s as defined abo
-0001a530: 7665 0d0a 2020 6465 6620 6765 7459 7249  ve..  def getYrI
-0001a540: 6d61 6765 7328 7972 293a 0d0a 2020 2020  mages(yr):..    
-0001a550: 2374 616b 6520 7468 6520 7965 6172 206f  #take the year o
-0001a560: 6620 7468 6520 696d 6167 650d 0a20 2020  f the image..   
-0001a570: 2079 7220 3d20 6565 2e4e 756d 6265 7228   yr = ee.Number(
-0001a580: 7972 292e 696e 7431 3628 290d 0a20 2020  yr).int16()..   
-0001a590: 2023 6669 6c74 6572 206f 7574 2069 6d61   #filter out ima
-0001a5a0: 6765 7320 666f 7220 7468 6520 7965 6172  ges for the year
-0001a5b0: 0d0a 2020 2020 7972 496d 6167 6573 203d  ..    yrImages =
-0001a5c0: 2069 6d61 6765 732e 6669 6c74 6572 2865   images.filter(e
-0001a5d0: 652e 4669 6c74 6572 2e63 616c 656e 6461  e.Filter.calenda
-0001a5e0: 7252 616e 6765 2879 722c 7972 2c27 7965  rRange(yr,yr,'ye
-0001a5f0: 6172 2729 290d 0a0d 0a20 2020 2023 7573  ar'))....    #us
-0001a600: 6520 6475 6d6d 7920 696d 6167 6520 746f  e dummy image to
-0001a610: 2066 696c 6c20 696e 2067 6170 7320 666f   fill in gaps fo
-0001a620: 7220 4745 4520 7072 6f63 6573 7369 6e67  r GEE processing
-0001a630: 0d0a 2020 2020 7972 496d 6167 6573 203d  ..    yrImages =
-0001a640: 2066 696c 6c45 6d70 7479 436f 6c6c 6563   fillEmptyCollec
-0001a650: 7469 6f6e 7328 7972 496d 6167 6573 2c64  tions(yrImages,d
-0001a660: 756d 6d79 496d 6167 6529 0d0a 2020 2020  ummyImage)..    
-0001a670: 7265 7475 726e 2079 7249 6d61 6765 730d  return yrImages.
-0001a680: 0a0d 0a20 2023 4765 7420 696d 6167 6573  ...  #Get images
-0001a690: 2066 6f72 2061 2073 7065 6369 6669 6564   for a specified
-0001a6a0: 2073 7461 7274 2064 6179 0d0a 2020 6465   start day..  de
-0001a6b0: 6620 6765 744a 6449 6d61 6765 7328 7972  f getJdImages(yr
-0001a6c0: 2c79 7249 6d61 6765 732c 7374 6172 7429  ,yrImages,start)
-0001a6d0: 3a0d 0a20 2020 2079 7220 3d20 6565 2e4e  :..    yr = ee.N
-0001a6e0: 756d 6265 7228 7972 292e 696e 7431 3628  umber(yr).int16(
-0001a6f0: 290d 0a20 2020 2073 7461 7274 203d 2065  )..    start = e
-0001a700: 652e 4e75 6d62 6572 2873 7461 7274 292e  e.Number(start).
-0001a710: 696e 7431 3628 290d 0a20 2020 2064 6174  int16()..    dat
-0001a720: 6520 3d20 6565 2e44 6174 652e 6672 6f6d  e = ee.Date.from
-0001a730: 594d 4428 7972 2c31 2c31 292e 6164 7661  YMD(yr,1,1).adva
-0001a740: 6e63 6528 7374 6172 742e 7375 6274 7261  nce(start.subtra
-0001a750: 6374 2831 292c 2764 6179 2729 0d0a 2020  ct(1),'day')..  
-0001a760: 2020 696e 6465 7820 3d20 6461 7465 2e66    index = date.f
-0001a770: 6f72 6d61 7428 2779 7979 792d 4d4d 2d64  ormat('yyyy-MM-d
-0001a780: 6427 290d 0a20 2020 2065 6e64 203d 2073  d')..    end = s
-0001a790: 7461 7274 2e61 6464 2863 6f6d 706f 7369  tart.add(composi
-0001a7a0: 7465 5065 7269 6f64 2d31 292e 696e 7431  tePeriod-1).int1
-0001a7b0: 3628 290d 0a20 2020 206a 6449 6d61 6765  6()..    jdImage
-0001a7c0: 7320 3d20 7972 496d 6167 6573 2e66 696c  s = yrImages.fil
-0001a7d0: 7465 7228 6565 2e46 696c 7465 722e 6361  ter(ee.Filter.ca
-0001a7e0: 6c65 6e64 6172 5261 6e67 6528 7374 6172  lendarRange(star
-0001a7f0: 742c 656e 6429 290d 0a20 2020 206a 6449  t,end))..    jdI
-0001a800: 6d61 6765 7320 3d20 6669 6c6c 456d 7074  mages = fillEmpt
-0001a810: 7943 6f6c 6c65 6374 696f 6e73 286a 6449  yCollections(jdI
-0001a820: 6d61 6765 732c 6475 6d6d 7949 6d61 6765  mages,dummyImage
-0001a830: 290d 0a20 2020 2063 6f6d 706f 7369 7465  )..    composite
-0001a840: 203d 206a 6449 6d61 6765 732e 6d65 6469   = jdImages.medi
-0001a850: 616e 2829 0d0a 2020 2020 7265 7475 726e  an()..    return
-0001a860: 2063 6f6d 706f 7369 7465 2e73 6574 287b   composite.set({
-0001a870: 2773 7973 7465 6d3a 696e 6465 7827 3a69  'system:index':i
-0001a880: 6e64 6578 2c27 7379 7374 656d 3a74 696d  ndex,'system:tim
-0001a890: 655f 7374 6172 7427 3a64 6174 652e 6d69  e_start':date.mi
-0001a8a0: 6c6c 6973 2829 7d29 0d0a 0d0a 2020 2353  llis()})....  #S
-0001a8b0: 6574 2075 7020 7772 6170 7065 7273 0d0a  et up wrappers..
-0001a8c0: 2020 6465 6620 6a64 5772 6170 7065 7228    def jdWrapper(
-0001a8d0: 7972 2c79 7249 6d61 6765 7329 3a0d 0a20  yr,yrImages):.. 
-0001a8e0: 2020 2072 6574 7572 6e20 6565 2e46 6561     return ee.Fea
-0001a8f0: 7475 7265 436f 6c6c 6563 7469 6f6e 2865  tureCollection(e
-0001a900: 652e 4c69 7374 2e73 6571 7565 6e63 6528  e.List.sequence(
-0001a910: 7374 6172 744a 756c 6961 6e2c 656e 644a  startJulian,endJ
-0001a920: 756c 6961 6e2c 636f 6d70 6f73 6974 6550  ulian,compositeP
-0001a930: 6572 696f 6429 2e6d 6170 286c 616d 6264  eriod).map(lambd
-0001a940: 6120 7374 6172 743a 2067 6574 4a64 496d  a start: getJdIm
-0001a950: 6167 6573 2879 722c 7972 496d 6167 6573  ages(yr,yrImages
-0001a960: 2c73 7461 7274 2929 290d 0a20 2064 6566  ,start)))..  def
-0001a970: 2079 7257 7261 7070 6572 2879 7229 3a0d   yrWrapper(yr):.
-0001a980: 0a20 2020 2079 7249 6d61 6765 7320 3d20  .    yrImages = 
-0001a990: 6765 7459 7249 6d61 6765 7328 7972 290d  getYrImages(yr).
-0001a9a0: 0a20 2020 2072 6574 7572 6e20 6a64 5772  .    return jdWr
-0001a9b0: 6170 7065 7228 7972 2c79 7249 6d61 6765  apper(yr,yrImage
-0001a9c0: 7329 0d0a 0d0a 2020 636f 6d70 6f73 6974  s)....  composit
-0001a9d0: 6573 203d 2065 652e 4665 6174 7572 6543  es = ee.FeatureC
-0001a9e0: 6f6c 6c65 6374 696f 6e28 6565 2e4c 6973  ollection(ee.Lis
-0001a9f0: 742e 7365 7175 656e 6365 2873 7461 7274  t.sequence(start
-0001aa00: 5965 6172 2c65 6e64 5965 6172 292e 6d61  Year,endYear).ma
-0001aa10: 7028 6c61 6d62 6461 2079 723a 7972 5772  p(lambda yr:yrWr
-0001aa20: 6170 7065 7228 7972 2929 290d 0a20 2023  apper(yr)))..  #
-0001aa30: 7265 7475 726e 2074 6865 2063 6f6d 706f  return the compo
-0001aa40: 7369 7465 7320 6173 2061 6e20 696d 6167  sites as an imag
-0001aa50: 6520 636f 6c6c 6563 7469 6f6e 0d0a 2020  e collection..  
-0001aa60: 636f 6d70 6f73 6974 6573 203d 2065 652e  composites = ee.
-0001aa70: 496d 6167 6543 6f6c 6c65 6374 696f 6e28  ImageCollection(
-0001aa80: 636f 6d70 6f73 6974 6573 2e66 6c61 7474  composites.flatt
-0001aa90: 656e 2829 293b 0d0a 0d0a 2020 7265 7475  en());....  retu
-0001aaa0: 726e 2063 6f6d 706f 7369 7465 730d 0a23  rn composites..#
-0001aab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a410: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+0001a420: 4675 6e63 7469 6f6e 2074 6f20 7461 6b65  Function to take
+0001a430: 2069 6d61 6765 7320 616e 6420 6372 6561   images and crea
+0001a440: 7465 2061 206d 6564 6961 6e20 636f 6d70  te a median comp
+0001a450: 6f73 6974 6520 6576 6572 7920 6e20 6461  osite every n da
+0001a460: 7973 0d0a 6465 6620 6e44 6179 436f 6d70  ys..def nDayComp
+0001a470: 6f73 6974 6573 2869 6d61 6765 732c 7374  osites(images,st
+0001a480: 6172 7459 6561 722c 656e 6459 6561 722c  artYear,endYear,
+0001a490: 7374 6172 744a 756c 6961 6e2c 656e 644a  startJulian,endJ
+0001a4a0: 756c 6961 6e2c 636f 6d70 6f73 6974 6550  ulian,compositeP
+0001a4b0: 6572 696f 6429 3a0d 0a0d 0a20 2023 6372  eriod):....  #cr
+0001a4c0: 6561 7465 2064 756d 6d79 2069 6d61 6765  eate dummy image
+0001a4d0: 2066 6f72 2077 6974 6820 6e6f 2076 616c   for with no val
+0001a4e0: 7565 730d 0a20 2064 756d 6d79 496d 6167  ues..  dummyImag
+0001a4f0: 6520 3d20 6565 2e49 6d61 6765 2869 6d61  e = ee.Image(ima
+0001a500: 6765 732e 6669 7273 7428 2929 0d0a 0d0a  ges.first())....
+0001a510: 2020 2363 6f6e 7665 7274 2074 6f20 636f    #convert to co
+0001a520: 6d70 6f73 6974 6573 2061 7320 6465 6669  mposites as defi
+0001a530: 6e65 6420 6162 6f76 650d 0a20 2064 6566  ned above..  def
+0001a540: 2067 6574 5972 496d 6167 6573 2879 7229   getYrImages(yr)
+0001a550: 3a0d 0a20 2020 2023 7461 6b65 2074 6865  :..    #take the
+0001a560: 2079 6561 7220 6f66 2074 6865 2069 6d61   year of the ima
+0001a570: 6765 0d0a 2020 2020 7972 203d 2065 652e  ge..    yr = ee.
+0001a580: 4e75 6d62 6572 2879 7229 2e69 6e74 3136  Number(yr).int16
+0001a590: 2829 0d0a 2020 2020 2366 696c 7465 7220  ()..    #filter 
+0001a5a0: 6f75 7420 696d 6167 6573 2066 6f72 2074  out images for t
+0001a5b0: 6865 2079 6561 720d 0a20 2020 2079 7249  he year..    yrI
+0001a5c0: 6d61 6765 7320 3d20 696d 6167 6573 2e66  mages = images.f
+0001a5d0: 696c 7465 7228 6565 2e46 696c 7465 722e  ilter(ee.Filter.
+0001a5e0: 6361 6c65 6e64 6172 5261 6e67 6528 7972  calendarRange(yr
+0001a5f0: 2c79 722c 2779 6561 7227 2929 0d0a 0d0a  ,yr,'year'))....
+0001a600: 2020 2020 2375 7365 2064 756d 6d79 2069      #use dummy i
+0001a610: 6d61 6765 2074 6f20 6669 6c6c 2069 6e20  mage to fill in 
+0001a620: 6761 7073 2066 6f72 2047 4545 2070 726f  gaps for GEE pro
+0001a630: 6365 7373 696e 670d 0a20 2020 2079 7249  cessing..    yrI
+0001a640: 6d61 6765 7320 3d20 6669 6c6c 456d 7074  mages = fillEmpt
+0001a650: 7943 6f6c 6c65 6374 696f 6e73 2879 7249  yCollections(yrI
+0001a660: 6d61 6765 732c 6475 6d6d 7949 6d61 6765  mages,dummyImage
+0001a670: 290d 0a20 2020 2072 6574 7572 6e20 7972  )..    return yr
+0001a680: 496d 6167 6573 0d0a 0d0a 2020 2347 6574  Images....  #Get
+0001a690: 2069 6d61 6765 7320 666f 7220 6120 7370   images for a sp
+0001a6a0: 6563 6966 6965 6420 7374 6172 7420 6461  ecified start da
+0001a6b0: 790d 0a20 2064 6566 2067 6574 4a64 496d  y..  def getJdIm
+0001a6c0: 6167 6573 2879 722c 7972 496d 6167 6573  ages(yr,yrImages
+0001a6d0: 2c73 7461 7274 293a 0d0a 2020 2020 7972  ,start):..    yr
+0001a6e0: 203d 2065 652e 4e75 6d62 6572 2879 7229   = ee.Number(yr)
+0001a6f0: 2e69 6e74 3136 2829 0d0a 2020 2020 7374  .int16()..    st
+0001a700: 6172 7420 3d20 6565 2e4e 756d 6265 7228  art = ee.Number(
+0001a710: 7374 6172 7429 2e69 6e74 3136 2829 0d0a  start).int16()..
+0001a720: 2020 2020 6461 7465 203d 2065 652e 4461      date = ee.Da
+0001a730: 7465 2e66 726f 6d59 4d44 2879 722c 312c  te.fromYMD(yr,1,
+0001a740: 3129 2e61 6476 616e 6365 2873 7461 7274  1).advance(start
+0001a750: 2e73 7562 7472 6163 7428 3129 2c27 6461  .subtract(1),'da
+0001a760: 7927 290d 0a20 2020 2069 6e64 6578 203d  y')..    index =
+0001a770: 2064 6174 652e 666f 726d 6174 2827 7979   date.format('yy
+0001a780: 7979 2d4d 4d2d 6464 2729 0d0a 2020 2020  yy-MM-dd')..    
+0001a790: 656e 6420 3d20 7374 6172 742e 6164 6428  end = start.add(
+0001a7a0: 636f 6d70 6f73 6974 6550 6572 696f 642d  compositePeriod-
+0001a7b0: 3129 2e69 6e74 3136 2829 0d0a 2020 2020  1).int16()..    
+0001a7c0: 6a64 496d 6167 6573 203d 2079 7249 6d61  jdImages = yrIma
+0001a7d0: 6765 732e 6669 6c74 6572 2865 652e 4669  ges.filter(ee.Fi
+0001a7e0: 6c74 6572 2e63 616c 656e 6461 7252 616e  lter.calendarRan
+0001a7f0: 6765 2873 7461 7274 2c65 6e64 2929 0d0a  ge(start,end))..
+0001a800: 2020 2020 6a64 496d 6167 6573 203d 2066      jdImages = f
+0001a810: 696c 6c45 6d70 7479 436f 6c6c 6563 7469  illEmptyCollecti
+0001a820: 6f6e 7328 6a64 496d 6167 6573 2c64 756d  ons(jdImages,dum
+0001a830: 6d79 496d 6167 6529 0d0a 2020 2020 636f  myImage)..    co
+0001a840: 6d70 6f73 6974 6520 3d20 6a64 496d 6167  mposite = jdImag
+0001a850: 6573 2e6d 6564 6961 6e28 290d 0a20 2020  es.median()..   
+0001a860: 2072 6574 7572 6e20 636f 6d70 6f73 6974   return composit
+0001a870: 652e 7365 7428 7b27 7379 7374 656d 3a69  e.set({'system:i
+0001a880: 6e64 6578 273a 696e 6465 782c 2773 7973  ndex':index,'sys
+0001a890: 7465 6d3a 7469 6d65 5f73 7461 7274 273a  tem:time_start':
+0001a8a0: 6461 7465 2e6d 696c 6c69 7328 297d 290d  date.millis()}).
+0001a8b0: 0a0d 0a20 2023 5365 7420 7570 2077 7261  ...  #Set up wra
+0001a8c0: 7070 6572 730d 0a20 2064 6566 206a 6457  ppers..  def jdW
+0001a8d0: 7261 7070 6572 2879 722c 7972 496d 6167  rapper(yr,yrImag
+0001a8e0: 6573 293a 0d0a 2020 2020 7265 7475 726e  es):..    return
+0001a8f0: 2065 652e 4665 6174 7572 6543 6f6c 6c65   ee.FeatureColle
+0001a900: 6374 696f 6e28 6565 2e4c 6973 742e 7365  ction(ee.List.se
+0001a910: 7175 656e 6365 2873 7461 7274 4a75 6c69  quence(startJuli
+0001a920: 616e 2c65 6e64 4a75 6c69 616e 2c63 6f6d  an,endJulian,com
+0001a930: 706f 7369 7465 5065 7269 6f64 292e 6d61  positePeriod).ma
+0001a940: 7028 6c61 6d62 6461 2073 7461 7274 3a20  p(lambda start: 
+0001a950: 6765 744a 6449 6d61 6765 7328 7972 2c79  getJdImages(yr,y
+0001a960: 7249 6d61 6765 732c 7374 6172 7429 2929  rImages,start)))
+0001a970: 0d0a 2020 6465 6620 7972 5772 6170 7065  ..  def yrWrappe
+0001a980: 7228 7972 293a 0d0a 2020 2020 7972 496d  r(yr):..    yrIm
+0001a990: 6167 6573 203d 2067 6574 5972 496d 6167  ages = getYrImag
+0001a9a0: 6573 2879 7229 0d0a 2020 2020 7265 7475  es(yr)..    retu
+0001a9b0: 726e 206a 6457 7261 7070 6572 2879 722c  rn jdWrapper(yr,
+0001a9c0: 7972 496d 6167 6573 290d 0a0d 0a20 2063  yrImages)....  c
+0001a9d0: 6f6d 706f 7369 7465 7320 3d20 6565 2e46  omposites = ee.F
+0001a9e0: 6561 7475 7265 436f 6c6c 6563 7469 6f6e  eatureCollection
+0001a9f0: 2865 652e 4c69 7374 2e73 6571 7565 6e63  (ee.List.sequenc
+0001aa00: 6528 7374 6172 7459 6561 722c 656e 6459  e(startYear,endY
+0001aa10: 6561 7229 2e6d 6170 286c 616d 6264 6120  ear).map(lambda 
+0001aa20: 7972 3a79 7257 7261 7070 6572 2879 7229  yr:yrWrapper(yr)
+0001aa30: 2929 0d0a 2020 2372 6574 7572 6e20 7468  ))..  #return th
+0001aa40: 6520 636f 6d70 6f73 6974 6573 2061 7320  e composites as 
+0001aa50: 616e 2069 6d61 6765 2063 6f6c 6c65 6374  an image collect
+0001aa60: 696f 6e0d 0a20 2063 6f6d 706f 7369 7465  ion..  composite
+0001aa70: 7320 3d20 6565 2e49 6d61 6765 436f 6c6c  s = ee.ImageColl
+0001aa80: 6563 7469 6f6e 2863 6f6d 706f 7369 7465  ection(composite
+0001aa90: 732e 666c 6174 7465 6e28 2929 3b0d 0a0d  s.flatten());...
+0001aaa0: 0a20 2072 6574 7572 6e20 636f 6d70 6f73  .  return compos
+0001aab0: 6974 6573 0d0a 2323 2323 2323 2323 2323  ites..##########
 0001aac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001aad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aae0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-0001aaf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001aae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001aaf0: 2323 2323 230d 0a23 2323 2323 2323 2323  #####..#########
 0001ab00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001ab10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001ab20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ab30: 2323 2323 2323 2323 230d 0a64 6566 2065  #########..def e
-0001ab40: 7870 6f72 7443 6f6c 6c65 6374 696f 6e28  xportCollection(
-0001ab50: 6578 706f 7274 5061 7468 526f 6f74 2c6f  exportPathRoot,o
-0001ab60: 7574 7075 744e 616d 652c 7374 7564 7941  utputName,studyA
-0001ab70: 7265 612c 2063 7273 2c74 7261 6e73 666f  rea, crs,transfo
-0001ab80: 726d 2c73 6361 6c65 2c63 6f6c 6c65 6374  rm,scale,collect
-0001ab90: 696f 6e2c 7374 6172 7459 6561 722c 656e  ion,startYear,en
-0001aba0: 6459 6561 722c 7374 6172 744a 756c 6961  dYear,startJulia
-0001abb0: 6e2c 656e 644a 756c 6961 6e2c 636f 6d70  n,endJulian,comp
-0001abc0: 6f73 6974 696e 6752 6564 7563 6572 2c74  ositingReducer,t
-0001abd0: 696d 6562 7566 6665 722c 6578 706f 7274  imebuffer,export
-0001abe0: 4261 6e64 732c 6f76 6572 7772 6974 653d  Bands,overwrite=
-0001abf0: 4661 6c73 6529 3a0d 0a0d 0a20 2023 5461  False):....  #Ta
-0001ac00: 6b65 2063 6172 6520 6f66 2064 6174 6520  ke care of date 
-0001ac10: 7772 6170 7069 6e67 0d0a 2020 6461 7465  wrapping..  date
-0001ac20: 5772 6170 7069 6e67 203d 2077 7261 7044  Wrapping = wrapD
-0001ac30: 6174 6573 2873 7461 7274 4a75 6c69 616e  ates(startJulian
-0001ac40: 2c65 6e64 4a75 6c69 616e 290d 0a20 2077  ,endJulian)..  w
-0001ac50: 7261 704f 6666 7365 7420 3d20 6461 7465  rapOffset = date
-0001ac60: 5772 6170 7069 6e67 5b30 5d0d 0a20 2079  Wrapping[0]..  y
-0001ac70: 6561 7257 6974 684d 616a 6f72 6974 7920  earWithMajority 
-0001ac80: 3d20 6461 7465 5772 6170 7069 6e67 5b31  = dateWrapping[1
-0001ac90: 5d0d 0a0d 0a20 2023 436c 6561 6e20 7570  ]....  #Clean up
-0001aca0: 206f 7574 7075 7420 6e61 6d65 0d0a 2020   output name..  
-0001acb0: 6f75 7470 7574 4e61 6d65 203d 206f 7574  outputName = out
-0001acc0: 7075 744e 616d 652e 7265 706c 6163 6528  putName.replace(
-0001acd0: 272f 5c73 2b2f 6727 2c27 2d27 290d 0a20  '/\s+/g','-').. 
-0001ace0: 206f 7574 7075 744e 616d 6520 3d20 6f75   outputName = ou
-0001acf0: 7470 7574 4e61 6d65 2e72 6570 6c61 6365  tputName.replace
-0001ad00: 2827 2f5c 2f2f 6727 2c27 2d27 290d 0a0d  ('/\//g','-')...
-0001ad10: 0a20 2023 5365 6c65 6374 2062 616e 6473  .  #Select bands
-0001ad20: 2066 6f72 2065 7870 6f72 740d 0a20 2063   for export..  c
-0001ad30: 6f6c 6c65 6374 696f 6e20 3d20 636f 6c6c  ollection = coll
-0001ad40: 6563 7469 6f6e 2e73 656c 6563 7428 6578  ection.select(ex
-0001ad50: 706f 7274 4261 6e64 7329 0d0a 0d0a 2020  portBands)....  
-0001ad60: 2349 7465 7261 7465 2061 6372 6f73 7320  #Iterate across 
-0001ad70: 6561 6368 2079 6561 7220 616e 6420 6578  each year and ex
-0001ad80: 706f 7274 2069 6d61 6765 0d0a 2020 666f  port image..  fo
-0001ad90: 7220 7965 6172 2069 6e20 6565 2e4c 6973  r year in ee.Lis
-0001ada0: 742e 7365 7175 656e 6365 2873 7461 7274  t.sequence(start
-0001adb0: 5965 6172 2b74 696d 6562 7566 6665 722c  Year+timebuffer,
-0001adc0: 656e 6459 6561 722d 7469 6d65 6275 6666  endYear-timebuff
-0001add0: 6572 292e 6765 7449 6e66 6f28 293a 0d0a  er).getInfo():..
-0001ade0: 2020 2020 7072 696e 7428 2745 7870 6f72      print('Expor
-0001adf0: 7469 6e67 3a27 2c79 6561 7229 0d0a 2020  ting:',year)..  
-0001ae00: 2020 2353 6574 2075 7020 6461 7465 730d    #Set up dates.
-0001ae10: 0a20 2020 2073 7461 7274 5965 6172 5420  .    startYearT 
-0001ae20: 3d20 7965 6172 2d74 696d 6562 7566 6665  = year-timebuffe
-0001ae30: 720d 0a20 2020 2065 6e64 5965 6172 5420  r..    endYearT 
-0001ae40: 3d20 7965 6172 2b74 696d 6562 7566 6665  = year+timebuffe
-0001ae50: 722b 7965 6172 5769 7468 4d61 6a6f 7269  r+yearWithMajori
-0001ae60: 7479 0d0a 0d0a 2020 2020 2347 6574 2079  ty....    #Get y
-0001ae70: 6561 726c 7920 636f 6d70 6f73 6974 650d  early composite.
-0001ae80: 0a20 2020 2063 6f6d 706f 7369 7465 203d  .    composite =
-0001ae90: 2063 6f6c 6c65 6374 696f 6e2e 6669 6c74   collection.filt
-0001aea0: 6572 2865 652e 4669 6c74 6572 2e63 616c  er(ee.Filter.cal
-0001aeb0: 656e 6461 7252 616e 6765 2879 6561 722b  endarRange(year+
-0001aec0: 7965 6172 5769 7468 4d61 6a6f 7269 7479  yearWithMajority
-0001aed0: 2c79 6561 722b 7965 6172 5769 7468 4d61  ,year+yearWithMa
-0001aee0: 6a6f 7269 7479 2c27 7965 6172 2729 290d  jority,'year')).
-0001aef0: 0a20 2020 2063 6f6d 706f 7369 7465 203d  .    composite =
-0001af00: 2065 652e 496d 6167 6528 636f 6d70 6f73   ee.Image(compos
-0001af10: 6974 652e 6669 7273 7428 2929 2e63 6c69  ite.first()).cli
-0001af20: 7028 7374 7564 7941 7265 6129 0d0a 0d0a  p(studyArea)....
-0001af30: 2020 2020 2341 6464 206d 6574 6164 6174      #Add metadat
-0001af40: 612c 2063 6173 7420 746f 2069 6e74 6567  a, cast to integ
-0001af50: 6572 2c20 616e 6420 6578 706f 7274 2063  er, and export c
-0001af60: 6f6d 706f 7369 7465 0d0a 2020 2020 636f  omposite..    co
-0001af70: 6d70 6f73 6974 6520 3d20 636f 6d70 6f73  mposite = compos
-0001af80: 6974 652e 7365 7428 7b5c 0d0a 2020 2020  ite.set({\..    
-0001af90: 2020 2773 7973 7465 6d3a 7469 6d65 5f73    'system:time_s
-0001afa0: 7461 7274 273a 2065 652e 4461 7465 2e66  tart': ee.Date.f
-0001afb0: 726f 6d59 4d44 2879 6561 722b 7965 6172  romYMD(year+year
-0001afc0: 5769 7468 4d61 6a6f 7269 7479 2c36 2c31  WithMajority,6,1
-0001afd0: 292e 6d69 6c6c 6973 2829 2c5c 0d0a 2020  ).millis(),\..  
-0001afe0: 2020 2020 2779 6561 7242 7566 6665 7227      'yearBuffer'
-0001aff0: 3a74 696d 6562 7566 6665 725c 0d0a 2020  :timebuffer\..  
-0001b000: 2020 7d29 0d0a 0d0a 2020 2020 2345 7870    })....    #Exp
-0001b010: 6f72 7420 7468 6520 636f 6d70 6f73 6974  ort the composit
-0001b020: 650d 0a20 2020 2023 5365 7420 7570 2065  e..    #Set up e
-0001b030: 7870 6f72 7420 6e61 6d65 2061 6e64 2070  xport name and p
-0001b040: 6174 680d 0a20 2020 2065 7870 6f72 744e  ath..    exportN
-0001b050: 616d 6520 3d20 6f75 7470 7574 4e61 6d65  ame = outputName
-0001b060: 2020 2b27 5f27 2020 2b20 7374 7228 696e    +'_'  + str(in
-0001b070: 7428 7374 6172 7459 6561 7254 2929 202b  t(startYearT)) +
-0001b080: 2027 5f27 202b 2073 7472 2869 6e74 2865   '_' + str(int(e
-0001b090: 6e64 5965 6172 5429 292b 275f 2720 2b20  ndYearT))+'_' + 
-0001b0a0: 7374 7228 696e 7428 7374 6172 744a 756c  str(int(startJul
-0001b0b0: 6961 6e29 2920 2b20 275f 2720 2b20 7374  ian)) + '_' + st
-0001b0c0: 7228 696e 7428 656e 644a 756c 6961 6e29  r(int(endJulian)
-0001b0d0: 290d 0a0d 0a20 2020 2065 7870 6f72 7450  )....    exportP
-0001b0e0: 6174 6820 3d20 6578 706f 7274 5061 7468  ath = exportPath
-0001b0f0: 526f 6f74 202b 2027 2f27 202b 2065 7870  Root + '/' + exp
-0001b100: 6f72 744e 616d 650d 0a0d 0a20 2020 2065  ortName....    e
-0001b110: 7870 6f72 7454 6f41 7373 6574 5772 6170  xportToAssetWrap
-0001b120: 7065 7228 636f 6d70 6f73 6974 652c 6578  per(composite,ex
-0001b130: 706f 7274 4e61 6d65 2c65 7870 6f72 7450  portName,exportP
-0001b140: 6174 682c 276d 6561 6e27 2c73 7475 6479  ath,'mean',study
-0001b150: 4172 6561 2c73 6361 6c65 2c63 7273 2c74  Area,scale,crs,t
-0001b160: 7261 6e73 666f 726d 2c6f 7665 7277 7269  ransform,overwri
-0001b170: 7465 293b 0d0a 0d0a 2323 2323 2323 2323  te);....########
+0001ab30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ab40: 0d0a 6465 6620 6578 706f 7274 436f 6c6c  ..def exportColl
+0001ab50: 6563 7469 6f6e 2865 7870 6f72 7450 6174  ection(exportPat
+0001ab60: 6852 6f6f 742c 6f75 7470 7574 4e61 6d65  hRoot,outputName
+0001ab70: 2c73 7475 6479 4172 6561 2c20 6372 732c  ,studyArea, crs,
+0001ab80: 7472 616e 7366 6f72 6d2c 7363 616c 652c  transform,scale,
+0001ab90: 636f 6c6c 6563 7469 6f6e 2c73 7461 7274  collection,start
+0001aba0: 5965 6172 2c65 6e64 5965 6172 2c73 7461  Year,endYear,sta
+0001abb0: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
+0001abc0: 616e 2c63 6f6d 706f 7369 7469 6e67 5265  an,compositingRe
+0001abd0: 6475 6365 722c 7469 6d65 6275 6666 6572  ducer,timebuffer
+0001abe0: 2c65 7870 6f72 7442 616e 6473 2c6f 7665  ,exportBands,ove
+0001abf0: 7277 7269 7465 3d46 616c 7365 293a 0d0a  rwrite=False):..
+0001ac00: 0d0a 2020 2354 616b 6520 6361 7265 206f  ..  #Take care o
+0001ac10: 6620 6461 7465 2077 7261 7070 696e 670d  f date wrapping.
+0001ac20: 0a20 2064 6174 6557 7261 7070 696e 6720  .  dateWrapping 
+0001ac30: 3d20 7772 6170 4461 7465 7328 7374 6172  = wrapDates(star
+0001ac40: 744a 756c 6961 6e2c 656e 644a 756c 6961  tJulian,endJulia
+0001ac50: 6e29 0d0a 2020 7772 6170 4f66 6673 6574  n)..  wrapOffset
+0001ac60: 203d 2064 6174 6557 7261 7070 696e 675b   = dateWrapping[
+0001ac70: 305d 0d0a 2020 7965 6172 5769 7468 4d61  0]..  yearWithMa
+0001ac80: 6a6f 7269 7479 203d 2064 6174 6557 7261  jority = dateWra
+0001ac90: 7070 696e 675b 315d 0d0a 0d0a 2020 2343  pping[1]....  #C
+0001aca0: 6c65 616e 2075 7020 6f75 7470 7574 206e  lean up output n
+0001acb0: 616d 650d 0a20 206f 7574 7075 744e 616d  ame..  outputNam
+0001acc0: 6520 3d20 6f75 7470 7574 4e61 6d65 2e72  e = outputName.r
+0001acd0: 6570 6c61 6365 2827 2f5c 732b 2f67 272c  eplace('/\s+/g',
+0001ace0: 272d 2729 0d0a 2020 6f75 7470 7574 4e61  '-')..  outputNa
+0001acf0: 6d65 203d 206f 7574 7075 744e 616d 652e  me = outputName.
+0001ad00: 7265 706c 6163 6528 272f 5c2f 2f67 272c  replace('/\//g',
+0001ad10: 272d 2729 0d0a 0d0a 2020 2353 656c 6563  '-')....  #Selec
+0001ad20: 7420 6261 6e64 7320 666f 7220 6578 706f  t bands for expo
+0001ad30: 7274 0d0a 2020 636f 6c6c 6563 7469 6f6e  rt..  collection
+0001ad40: 203d 2063 6f6c 6c65 6374 696f 6e2e 7365   = collection.se
+0001ad50: 6c65 6374 2865 7870 6f72 7442 616e 6473  lect(exportBands
+0001ad60: 290d 0a0d 0a20 2023 4974 6572 6174 6520  )....  #Iterate 
+0001ad70: 6163 726f 7373 2065 6163 6820 7965 6172  across each year
+0001ad80: 2061 6e64 2065 7870 6f72 7420 696d 6167   and export imag
+0001ad90: 650d 0a20 2066 6f72 2079 6561 7220 696e  e..  for year in
+0001ada0: 2065 652e 4c69 7374 2e73 6571 7565 6e63   ee.List.sequenc
+0001adb0: 6528 7374 6172 7459 6561 722b 7469 6d65  e(startYear+time
+0001adc0: 6275 6666 6572 2c65 6e64 5965 6172 2d74  buffer,endYear-t
+0001add0: 696d 6562 7566 6665 7229 2e67 6574 496e  imebuffer).getIn
+0001ade0: 666f 2829 3a0d 0a20 2020 2070 7269 6e74  fo():..    print
+0001adf0: 2827 4578 706f 7274 696e 673a 272c 7965  ('Exporting:',ye
+0001ae00: 6172 290d 0a20 2020 2023 5365 7420 7570  ar)..    #Set up
+0001ae10: 2064 6174 6573 0d0a 2020 2020 7374 6172   dates..    star
+0001ae20: 7459 6561 7254 203d 2079 6561 722d 7469  tYearT = year-ti
+0001ae30: 6d65 6275 6666 6572 0d0a 2020 2020 656e  mebuffer..    en
+0001ae40: 6459 6561 7254 203d 2079 6561 722b 7469  dYearT = year+ti
+0001ae50: 6d65 6275 6666 6572 2b79 6561 7257 6974  mebuffer+yearWit
+0001ae60: 684d 616a 6f72 6974 790d 0a0d 0a20 2020  hMajority....   
+0001ae70: 2023 4765 7420 7965 6172 6c79 2063 6f6d   #Get yearly com
+0001ae80: 706f 7369 7465 0d0a 2020 2020 636f 6d70  posite..    comp
+0001ae90: 6f73 6974 6520 3d20 636f 6c6c 6563 7469  osite = collecti
+0001aea0: 6f6e 2e66 696c 7465 7228 6565 2e46 696c  on.filter(ee.Fil
+0001aeb0: 7465 722e 6361 6c65 6e64 6172 5261 6e67  ter.calendarRang
+0001aec0: 6528 7965 6172 2b79 6561 7257 6974 684d  e(year+yearWithM
+0001aed0: 616a 6f72 6974 792c 7965 6172 2b79 6561  ajority,year+yea
+0001aee0: 7257 6974 684d 616a 6f72 6974 792c 2779  rWithMajority,'y
+0001aef0: 6561 7227 2929 0d0a 2020 2020 636f 6d70  ear'))..    comp
+0001af00: 6f73 6974 6520 3d20 6565 2e49 6d61 6765  osite = ee.Image
+0001af10: 2863 6f6d 706f 7369 7465 2e66 6972 7374  (composite.first
+0001af20: 2829 292e 636c 6970 2873 7475 6479 4172  ()).clip(studyAr
+0001af30: 6561 290d 0a0d 0a20 2020 2023 4164 6420  ea)....    #Add 
+0001af40: 6d65 7461 6461 7461 2c20 6361 7374 2074  metadata, cast t
+0001af50: 6f20 696e 7465 6765 722c 2061 6e64 2065  o integer, and e
+0001af60: 7870 6f72 7420 636f 6d70 6f73 6974 650d  xport composite.
+0001af70: 0a20 2020 2063 6f6d 706f 7369 7465 203d  .    composite =
+0001af80: 2063 6f6d 706f 7369 7465 2e73 6574 287b   composite.set({
+0001af90: 5c0d 0a20 2020 2020 2027 7379 7374 656d  \..      'system
+0001afa0: 3a74 696d 655f 7374 6172 7427 3a20 6565  :time_start': ee
+0001afb0: 2e44 6174 652e 6672 6f6d 594d 4428 7965  .Date.fromYMD(ye
+0001afc0: 6172 2b79 6561 7257 6974 684d 616a 6f72  ar+yearWithMajor
+0001afd0: 6974 792c 362c 3129 2e6d 696c 6c69 7328  ity,6,1).millis(
+0001afe0: 292c 5c0d 0a20 2020 2020 2027 7965 6172  ),\..      'year
+0001aff0: 4275 6666 6572 273a 7469 6d65 6275 6666  Buffer':timebuff
+0001b000: 6572 5c0d 0a20 2020 207d 290d 0a0d 0a20  er\..    }).... 
+0001b010: 2020 2023 4578 706f 7274 2074 6865 2063     #Export the c
+0001b020: 6f6d 706f 7369 7465 0d0a 2020 2020 2353  omposite..    #S
+0001b030: 6574 2075 7020 6578 706f 7274 206e 616d  et up export nam
+0001b040: 6520 616e 6420 7061 7468 0d0a 2020 2020  e and path..    
+0001b050: 6578 706f 7274 4e61 6d65 203d 206f 7574  exportName = out
+0001b060: 7075 744e 616d 6520 202b 275f 2720 202b  putName  +'_'  +
+0001b070: 2073 7472 2869 6e74 2873 7461 7274 5965   str(int(startYe
+0001b080: 6172 5429 2920 2b20 275f 2720 2b20 7374  arT)) + '_' + st
+0001b090: 7228 696e 7428 656e 6459 6561 7254 2929  r(int(endYearT))
+0001b0a0: 2b27 5f27 202b 2073 7472 2869 6e74 2873  +'_' + str(int(s
+0001b0b0: 7461 7274 4a75 6c69 616e 2929 202b 2027  tartJulian)) + '
+0001b0c0: 5f27 202b 2073 7472 2869 6e74 2865 6e64  _' + str(int(end
+0001b0d0: 4a75 6c69 616e 2929 0d0a 0d0a 2020 2020  Julian))....    
+0001b0e0: 6578 706f 7274 5061 7468 203d 2065 7870  exportPath = exp
+0001b0f0: 6f72 7450 6174 6852 6f6f 7420 2b20 272f  ortPathRoot + '/
+0001b100: 2720 2b20 6578 706f 7274 4e61 6d65 0d0a  ' + exportName..
+0001b110: 0d0a 2020 2020 6578 706f 7274 546f 4173  ..    exportToAs
+0001b120: 7365 7457 7261 7070 6572 2863 6f6d 706f  setWrapper(compo
+0001b130: 7369 7465 2c65 7870 6f72 744e 616d 652c  site,exportName,
+0001b140: 6578 706f 7274 5061 7468 2c27 6d65 616e  exportPath,'mean
+0001b150: 272c 7374 7564 7941 7265 612c 7363 616c  ',studyArea,scal
+0001b160: 652c 6372 732c 7472 616e 7366 6f72 6d2c  e,crs,transform,
+0001b170: 6f76 6572 7772 6974 6529 3b0d 0a0d 0a23  overwrite);....#
 0001b180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b1c0: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
+0001b1c0: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
 0001b1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b200: 2323 2323 2323 2323 2323 2323 0d0a 2346  ############..#F
-0001b210: 756e 6374 696f 6e20 746f 2065 7870 6f72  unction to expor
-0001b220: 7420 636f 6d70 6f73 6974 6520 636f 6c6c  t composite coll
-0001b230: 6563 7469 6f6e 0d0a 6465 6620 6578 706f  ection..def expo
-0001b240: 7274 436f 6d70 6f73 6974 6543 6f6c 6c65  rtCompositeColle
-0001b250: 6374 696f 6e28 0d0a 2020 636f 6c6c 6563  ction(..  collec
-0001b260: 7469 6f6e 2c0d 0a20 2065 7870 6f72 7450  tion,..  exportP
-0001b270: 6174 6852 6f6f 742c 0d0a 2020 6f75 7470  athRoot,..  outp
-0001b280: 7574 4e61 6d65 2c0d 0a20 206f 7269 6769  utName,..  origi
-0001b290: 6e2c 0d0a 2020 7374 7564 7941 7265 612c  n,..  studyArea,
-0001b2a0: 0d0a 2020 6372 732c 0d0a 2020 7472 616e  ..  crs,..  tran
-0001b2b0: 7366 6f72 6d2c 0d0a 2020 7363 616c 652c  sform,..  scale,
-0001b2c0: 0d0a 2020 7374 6172 7459 6561 722c 0d0a  ..  startYear,..
-0001b2d0: 2020 656e 6459 6561 722c 0d0a 2020 7374    endYear,..  st
-0001b2e0: 6172 744a 756c 6961 6e2c 0d0a 2020 656e  artJulian,..  en
-0001b2f0: 644a 756c 6961 6e2c 0d0a 2020 636f 6d70  dJulian,..  comp
-0001b300: 6f73 6974 696e 674d 6574 686f 642c 0d0a  ositingMethod,..
-0001b310: 2020 7469 6d65 6275 6666 6572 2c0d 0a20    timebuffer,.. 
-0001b320: 2074 6f61 4f72 5352 2c0d 0a20 206e 6f6e   toaOrSR,..  non
-0001b330: 4469 7669 6465 4261 6e64 732c 0d0a 2020  DivideBands,..  
-0001b340: 6578 706f 7274 4261 6e64 732c 0d0a 2020  exportBands,..  
-0001b350: 6164 6469 7469 6f6e 616c 5072 6f70 6572  additionalProper
-0001b360: 7479 4469 6374 203d 204e 6f6e 652c 0d0a  tyDict = None,..
-0001b370: 2020 6f76 6572 7772 6974 653d 4661 6c73    overwrite=Fals
-0001b380: 6529 3a0d 0a0d 0a20 2061 7267 7320 3d20  e):....  args = 
-0001b390: 666f 726d 6174 4172 6773 286c 6f63 616c  formatArgs(local
-0001b3a0: 7328 2929 0d0a 0d0a 2020 7079 7261 6d69  s())....  pyrami
-0001b3b0: 6469 6e67 506f 6c69 6379 203d 2027 6d65  dingPolicy = 'me
-0001b3c0: 616e 270d 0a20 2064 6174 6557 7261 7070  an'..  dateWrapp
-0001b3d0: 696e 6720 3d20 7772 6170 4461 7465 7328  ing = wrapDates(
-0001b3e0: 7374 6172 744a 756c 6961 6e2c 2065 6e64  startJulian, end
-0001b3f0: 4a75 6c69 616e 290d 0a20 2077 7261 704f  Julian)..  wrapO
-0001b400: 6666 7365 7420 3d20 6461 7465 5772 6170  ffset = dateWrap
-0001b410: 7069 6e67 5b30 5d0d 0a20 2079 6561 7257  ping[0]..  yearW
-0001b420: 6974 684d 616a 6f72 6974 7920 3d20 6461  ithMajority = da
-0001b430: 7465 5772 6170 7069 6e67 5b31 5d0d 0a0d  teWrapping[1]...
-0001b440: 0a20 2023 436c 6561 6e20 7570 206f 7574  .  #Clean up out
-0001b450: 7075 7420 6e61 6d65 0d0a 2020 6f75 7470  put name..  outp
-0001b460: 7574 4e61 6d65 203d 206f 7574 7075 744e  utName = outputN
-0001b470: 616d 652e 7265 706c 6163 6528 272f 5c73  ame.replace('/\s
-0001b480: 2b2f 6727 2c27 2d27 290d 0a20 206f 7574  +/g','-')..  out
-0001b490: 7075 744e 616d 6520 3d20 6f75 7470 7574  putName = output
-0001b4a0: 4e61 6d65 2e72 6570 6c61 6365 2827 2f5c  Name.replace('/\
-0001b4b0: 2f2f 6727 2c27 2d27 290d 0a0d 0a20 2063  //g','-')....  c
-0001b4c0: 6f6c 6c65 6374 696f 6e20 3d20 636f 6c6c  ollection = coll
-0001b4d0: 6563 7469 6f6e 2e73 656c 6563 7428 6578  ection.select(ex
-0001b4e0: 706f 7274 4261 6e64 7329 0d0a 2020 666f  portBands)..  fo
-0001b4f0: 7220 7965 6172 2069 6e20 6565 2e4c 6973  r year in ee.Lis
-0001b500: 742e 7365 7175 656e 6365 2873 7461 7274  t.sequence(start
-0001b510: 5965 6172 2b74 696d 6562 7566 6665 722c  Year+timebuffer,
-0001b520: 656e 6459 6561 722d 7469 6d65 6275 6666  endYear-timebuff
-0001b530: 6572 292e 6765 7449 6e66 6f28 293a 0d0a  er).getInfo():..
-0001b540: 2020 2020 2353 6574 2075 7020 6461 7465      #Set up date
-0001b550: 730d 0a20 2020 2073 7461 7274 5965 6172  s..    startYear
-0001b560: 5420 3d20 7965 6172 2d74 696d 6562 7566  T = year-timebuf
-0001b570: 6665 720d 0a20 2020 2065 6e64 5965 6172  fer..    endYear
-0001b580: 5420 3d20 7965 6172 2b74 696d 6562 7566  T = year+timebuf
-0001b590: 6665 722b 7965 6172 5769 7468 4d61 6a6f  fer+yearWithMajo
-0001b5a0: 7269 7479 0d0a 0d0a 2020 2020 2347 6574  rity....    #Get
-0001b5b0: 2079 6561 726c 7920 636f 6d70 6f73 6974   yearly composit
-0001b5c0: 650d 0a20 2020 2063 6f6d 706f 7369 7465  e..    composite
-0001b5d0: 203d 2063 6f6c 6c65 6374 696f 6e2e 6669   = collection.fi
-0001b5e0: 6c74 6572 2865 652e 4669 6c74 6572 2e63  lter(ee.Filter.c
-0001b5f0: 616c 656e 6461 7252 616e 6765 2879 6561  alendarRange(yea
-0001b600: 722b 7965 6172 5769 7468 4d61 6a6f 7269  r+yearWithMajori
-0001b610: 7479 2c20 7965 6172 2b79 6561 7257 6974  ty, year+yearWit
-0001b620: 684d 616a 6f72 6974 792c 2027 7965 6172  hMajority, 'year
-0001b630: 2729 290d 0a20 2020 2063 6f6d 706f 7369  '))..    composi
-0001b640: 7465 203d 2065 652e 496d 6167 6528 636f  te = ee.Image(co
-0001b650: 6d70 6f73 6974 652e 6669 7273 7428 2929  mposite.first())
-0001b660: 0d0a 0d0a 2020 2020 2352 6566 6f72 6d61  ....    #Reforma
-0001b670: 7420 6461 7461 2066 6f72 2065 7870 6f72  t data for expor
-0001b680: 740d 0a20 2020 2063 6f6d 706f 7369 7465  t..    composite
-0001b690: 4261 6e64 7320 3d20 636f 6d70 6f73 6974  Bands = composit
-0001b6a0: 652e 6261 6e64 4e61 6d65 7328 290d 0a20  e.bandNames().. 
-0001b6b0: 2020 2069 6620 6e6f 6e44 6976 6964 6542     if nonDivideB
-0001b6c0: 616e 6473 2021 3d20 4e6f 6e65 3a0d 0a20  ands != None:.. 
-0001b6d0: 2020 2020 2063 6f6d 706f 7369 7465 3130       composite10
-0001b6e0: 6b20 3d20 636f 6d70 6f73 6974 652e 7365  k = composite.se
-0001b6f0: 6c65 6374 2863 6f6d 706f 7369 7465 4261  lect(compositeBa
-0001b700: 6e64 732e 7265 6d6f 7665 416c 6c28 6e6f  nds.removeAll(no
-0001b710: 6e44 6976 6964 6542 616e 6473 2929 2e6d  nDivideBands)).m
-0001b720: 756c 7469 706c 7928 3130 3030 3029 0d0a  ultiply(10000)..
-0001b730: 2020 2020 2020 636f 6d70 6f73 6974 6520        composite 
-0001b740: 3d20 636f 6d70 6f73 6974 6531 306b 2e61  = composite10k.a
-0001b750: 6464 4261 6e64 7328 636f 6d70 6f73 6974  ddBands(composit
-0001b760: 652e 7365 6c65 6374 286e 6f6e 4469 7669  e.select(nonDivi
-0001b770: 6465 4261 6e64 7329 292e 7365 6c65 6374  deBands)).select
-0001b780: 2863 6f6d 706f 7369 7465 4261 6e64 7329  (compositeBands)
-0001b790: 2e69 6e74 3136 2829 0d0a 0d0a 2020 2020  .int16()....    
-0001b7a0: 656c 7365 3a0d 0a20 2020 2020 2063 6f6d  else:..      com
-0001b7b0: 706f 7369 7465 203d 2063 6f6d 706f 7369  posite = composi
-0001b7c0: 7465 2e6d 756c 7469 706c 7928 3130 3030  te.multiply(1000
-0001b7d0: 3029 2e69 6e74 3136 2829 0d0a 0d0a 2020  0).int16()....  
-0001b7e0: 2020 7374 6172 7459 6561 7243 6f6d 706f    startYearCompo
-0001b7f0: 7369 7465 203d 2073 7461 7274 5965 6172  site = startYear
-0001b800: 540d 0a20 2020 2065 6e64 5965 6172 436f  T..    endYearCo
-0001b810: 6d70 6f73 6974 6520 3d20 656e 6459 6561  mposite = endYea
-0001b820: 7254 0d0a 2020 2020 7379 7374 656d 5469  rT..    systemTi
-0001b830: 6d65 5374 6172 7459 6561 7220 3d20 7965  meStartYear = ye
-0001b840: 6172 2b79 6561 7257 6974 684d 616a 6f72  ar+yearWithMajor
-0001b850: 6974 790d 0a20 2020 2079 6561 724f 7269  ity..    yearOri
-0001b860: 6769 6e61 6c20 3d20 7965 6172 0d0a 2020  ginal = year..  
-0001b870: 2020 7965 6172 5573 6564 203d 2073 7973    yearUsed = sys
-0001b880: 7465 6d54 696d 6553 7461 7274 5965 6172  temTimeStartYear
-0001b890: 0d0a 2020 2020 2320 6172 6773 5b27 7379  ..    # args['sy
-0001b8a0: 7374 656d 3a74 696d 655f 7374 6172 7427  stem:time_start'
-0001b8b0: 5d20 3d20 6565 2e44 6174 652e 6672 6f6d  ] = ee.Date.from
-0001b8c0: 594d 4428 7379 7374 656d 5469 6d65 5374  YMD(systemTimeSt
-0001b8d0: 6172 7459 6561 722c 2036 2c20 3129 2e6d  artYear, 6, 1).m
-0001b8e0: 696c 6c69 7328 290d 0a0d 0a20 2020 2063  illis()....    c
-0001b8f0: 6f6d 706f 7369 7465 203d 2063 6f6d 706f  omposite = compo
-0001b900: 7369 7465 2e73 6574 2866 6f72 6d61 7441  site.set(formatA
-0001b910: 7267 7328 6172 6773 2929 0d0a 0d0a 2020  rgs(args))....  
-0001b920: 2020 636f 6d70 6f73 6974 6520 3d20 636f    composite = co
-0001b930: 6d70 6f73 6974 652e 7365 7428 2773 7973  mposite.set('sys
-0001b940: 7465 6d3a 7469 6d65 5f73 7461 7274 272c  tem:time_start',
-0001b950: 6565 2e44 6174 652e 6672 6f6d 594d 4428  ee.Date.fromYMD(
-0001b960: 7379 7374 656d 5469 6d65 5374 6172 7459  systemTimeStartY
-0001b970: 6561 722c 2036 2c20 3129 2e6d 696c 6c69  ear, 6, 1).milli
-0001b980: 7328 2929 0d0a 0d0a 2020 2020 6966 2061  s())....    if a
-0001b990: 6464 6974 696f 6e61 6c50 726f 7065 7274  dditionalPropert
-0001b9a0: 7944 6963 7420 213d 204e 6f6e 653a 0d0a  yDict != None:..
-0001b9b0: 2020 2020 2020 6966 2027 6172 6773 2720        if 'args' 
-0001b9c0: 696e 2061 6464 6974 696f 6e61 6c50 726f  in additionalPro
-0001b9d0: 7065 7274 7944 6963 742e 6b65 7973 2829  pertyDict.keys()
-0001b9e0: 3a0d 0a20 2020 2020 2020 2064 656c 2061  :..        del a
-0001b9f0: 6464 6974 696f 6e61 6c50 726f 7065 7274  dditionalPropert
-0001ba00: 7944 6963 745b 2761 7267 7327 5d0d 0a20  yDict['args'].. 
-0001ba10: 2020 2020 2063 6f6d 706f 7369 7465 203d       composite =
-0001ba20: 2063 6f6d 706f 7369 7465 2e73 6574 2866   composite.set(f
-0001ba30: 6f72 6d61 7441 7267 7328 6164 6469 7469  ormatArgs(additi
-0001ba40: 6f6e 616c 5072 6f70 6572 7479 4469 6374  onalPropertyDict
-0001ba50: 2929 0d0a 0d0a 2020 2020 2345 7870 6f72  ))....    #Expor
-0001ba60: 7420 7468 6520 636f 6d70 6f73 6974 650d  t the composite.
-0001ba70: 0a20 2020 2023 5365 7420 7570 2065 7870  .    #Set up exp
-0001ba80: 6f72 7420 6e61 6d65 2061 6e64 2070 6174  ort name and pat
-0001ba90: 680d 0a20 2020 2065 7870 6f72 744e 616d  h..    exportNam
-0001baa0: 6520 3d20 6f75 7470 7574 4e61 6d65 2020  e = outputName  
-0001bab0: 2b20 275f 2720 2b20 746f 614f 7253 5220  + '_' + toaOrSR 
-0001bac0: 2b20 275f 2720 2b20 636f 6d70 6f73 6974  + '_' + composit
-0001bad0: 696e 674d 6574 686f 6420 2b20 275f 2720  ingMethod + '_' 
-0001bae0: 202b 2073 7472 2869 6e74 2873 7461 7274   + str(int(start
-0001baf0: 5965 6172 5429 2920 2b20 275f 2720 2b20  YearT)) + '_' + 
-0001bb00: 7374 7228 696e 7428 656e 6459 6561 7254  str(int(endYearT
-0001bb10: 2929 2b27 5f27 202b 2073 7472 2869 6e74  ))+'_' + str(int
-0001bb20: 2873 7461 7274 4a75 6c69 616e 2929 202b  (startJulian)) +
-0001bb30: 2027 5f27 202b 2073 7472 2869 6e74 2865   '_' + str(int(e
-0001bb40: 6e64 4a75 6c69 616e 2929 0d0a 2020 2020  ndJulian))..    
-0001bb50: 6578 706f 7274 5061 7468 203d 2065 7870  exportPath = exp
-0001bb60: 6f72 7450 6174 6852 6f6f 742b 272f 272b  ortPathRoot+'/'+
-0001bb70: 6578 706f 7274 4e61 6d65 0d0a 0d0a 0d0a  exportName......
-0001bb80: 2020 2020 6578 706f 7274 546f 4173 7365      exportToAsse
-0001bb90: 7457 7261 7070 6572 285c 0d0a 2020 2020  tWrapper(\..    
-0001bba0: 2020 696d 6167 6546 6f72 4578 706f 7274    imageForExport
-0001bbb0: 203d 2063 6f6d 706f 7369 7465 2c0d 0a20   = composite,.. 
-0001bbc0: 2020 2020 2061 7373 6574 4e61 6d65 203d       assetName =
-0001bbd0: 2065 7870 6f72 744e 616d 652c 0d0a 2020   exportName,..  
-0001bbe0: 2020 2020 6173 7365 7450 6174 6820 3d20      assetPath = 
-0001bbf0: 6578 706f 7274 5061 7468 2c0d 0a20 2020  exportPath,..   
-0001bc00: 2020 2070 7972 616d 6964 696e 6750 6f6c     pyramidingPol
-0001bc10: 6963 794f 626a 6563 7420 3d20 7079 7261  icyObject = pyra
-0001bc20: 6d69 6469 6e67 506f 6c69 6379 2c0d 0a20  midingPolicy,.. 
-0001bc30: 2020 2020 2072 6f69 3d20 7374 7564 7941       roi= studyA
-0001bc40: 7265 612c 0d0a 2020 2020 2020 7363 616c  rea,..      scal
-0001bc50: 653d 2073 6361 6c65 2c0d 0a20 2020 2020  e= scale,..     
-0001bc60: 2063 7273 203d 2063 7273 2c0d 0a20 2020   crs = crs,..   
-0001bc70: 2020 2074 7261 6e73 666f 726d 203d 2074     transform = t
-0001bc80: 7261 6e73 666f 726d 2c0d 0a20 2020 2020  ransform,..     
-0001bc90: 206f 7665 7277 7269 7465 3d6f 7665 7277   overwrite=overw
-0001bca0: 7269 7465 290d 0a0d 0a0d 0a23 2323 2323  rite)......#####
-0001bcb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b210: 2323 230d 0a23 4675 6e63 7469 6f6e 2074  ###..#Function t
+0001b220: 6f20 6578 706f 7274 2063 6f6d 706f 7369  o export composi
+0001b230: 7465 2063 6f6c 6c65 6374 696f 6e0d 0a64  te collection..d
+0001b240: 6566 2065 7870 6f72 7443 6f6d 706f 7369  ef exportComposi
+0001b250: 7465 436f 6c6c 6563 7469 6f6e 280d 0a20  teCollection(.. 
+0001b260: 2063 6f6c 6c65 6374 696f 6e2c 0d0a 2020   collection,..  
+0001b270: 6578 706f 7274 5061 7468 526f 6f74 2c0d  exportPathRoot,.
+0001b280: 0a20 206f 7574 7075 744e 616d 652c 0d0a  .  outputName,..
+0001b290: 2020 6f72 6967 696e 2c0d 0a20 2073 7475    origin,..  stu
+0001b2a0: 6479 4172 6561 2c0d 0a20 2063 7273 2c0d  dyArea,..  crs,.
+0001b2b0: 0a20 2074 7261 6e73 666f 726d 2c0d 0a20  .  transform,.. 
+0001b2c0: 2073 6361 6c65 2c0d 0a20 2073 7461 7274   scale,..  start
+0001b2d0: 5965 6172 2c0d 0a20 2065 6e64 5965 6172  Year,..  endYear
+0001b2e0: 2c0d 0a20 2073 7461 7274 4a75 6c69 616e  ,..  startJulian
+0001b2f0: 2c0d 0a20 2065 6e64 4a75 6c69 616e 2c0d  ,..  endJulian,.
+0001b300: 0a20 2063 6f6d 706f 7369 7469 6e67 4d65  .  compositingMe
+0001b310: 7468 6f64 2c0d 0a20 2074 696d 6562 7566  thod,..  timebuf
+0001b320: 6665 722c 0d0a 2020 746f 614f 7253 522c  fer,..  toaOrSR,
+0001b330: 0d0a 2020 6e6f 6e44 6976 6964 6542 616e  ..  nonDivideBan
+0001b340: 6473 2c0d 0a20 2065 7870 6f72 7442 616e  ds,..  exportBan
+0001b350: 6473 2c0d 0a20 2061 6464 6974 696f 6e61  ds,..  additiona
+0001b360: 6c50 726f 7065 7274 7944 6963 7420 3d20  lPropertyDict = 
+0001b370: 4e6f 6e65 2c0d 0a20 206f 7665 7277 7269  None,..  overwri
+0001b380: 7465 3d46 616c 7365 293a 0d0a 0d0a 2020  te=False):....  
+0001b390: 6172 6773 203d 2066 6f72 6d61 7441 7267  args = formatArg
+0001b3a0: 7328 6c6f 6361 6c73 2829 290d 0a0d 0a20  s(locals()).... 
+0001b3b0: 2070 7972 616d 6964 696e 6750 6f6c 6963   pyramidingPolic
+0001b3c0: 7920 3d20 276d 6561 6e27 0d0a 2020 6461  y = 'mean'..  da
+0001b3d0: 7465 5772 6170 7069 6e67 203d 2077 7261  teWrapping = wra
+0001b3e0: 7044 6174 6573 2873 7461 7274 4a75 6c69  pDates(startJuli
+0001b3f0: 616e 2c20 656e 644a 756c 6961 6e29 0d0a  an, endJulian)..
+0001b400: 2020 7772 6170 4f66 6673 6574 203d 2064    wrapOffset = d
+0001b410: 6174 6557 7261 7070 696e 675b 305d 0d0a  ateWrapping[0]..
+0001b420: 2020 7965 6172 5769 7468 4d61 6a6f 7269    yearWithMajori
+0001b430: 7479 203d 2064 6174 6557 7261 7070 696e  ty = dateWrappin
+0001b440: 675b 315d 0d0a 0d0a 2020 2343 6c65 616e  g[1]....  #Clean
+0001b450: 2075 7020 6f75 7470 7574 206e 616d 650d   up output name.
+0001b460: 0a20 206f 7574 7075 744e 616d 6520 3d20  .  outputName = 
+0001b470: 6f75 7470 7574 4e61 6d65 2e72 6570 6c61  outputName.repla
+0001b480: 6365 2827 2f5c 732b 2f67 272c 272d 2729  ce('/\s+/g','-')
+0001b490: 0d0a 2020 6f75 7470 7574 4e61 6d65 203d  ..  outputName =
+0001b4a0: 206f 7574 7075 744e 616d 652e 7265 706c   outputName.repl
+0001b4b0: 6163 6528 272f 5c2f 2f67 272c 272d 2729  ace('/\//g','-')
+0001b4c0: 0d0a 0d0a 2020 636f 6c6c 6563 7469 6f6e  ....  collection
+0001b4d0: 203d 2063 6f6c 6c65 6374 696f 6e2e 7365   = collection.se
+0001b4e0: 6c65 6374 2865 7870 6f72 7442 616e 6473  lect(exportBands
+0001b4f0: 290d 0a20 2066 6f72 2079 6561 7220 696e  )..  for year in
+0001b500: 2065 652e 4c69 7374 2e73 6571 7565 6e63   ee.List.sequenc
+0001b510: 6528 7374 6172 7459 6561 722b 7469 6d65  e(startYear+time
+0001b520: 6275 6666 6572 2c65 6e64 5965 6172 2d74  buffer,endYear-t
+0001b530: 696d 6562 7566 6665 7229 2e67 6574 496e  imebuffer).getIn
+0001b540: 666f 2829 3a0d 0a20 2020 2023 5365 7420  fo():..    #Set 
+0001b550: 7570 2064 6174 6573 0d0a 2020 2020 7374  up dates..    st
+0001b560: 6172 7459 6561 7254 203d 2079 6561 722d  artYearT = year-
+0001b570: 7469 6d65 6275 6666 6572 0d0a 2020 2020  timebuffer..    
+0001b580: 656e 6459 6561 7254 203d 2079 6561 722b  endYearT = year+
+0001b590: 7469 6d65 6275 6666 6572 2b79 6561 7257  timebuffer+yearW
+0001b5a0: 6974 684d 616a 6f72 6974 790d 0a0d 0a20  ithMajority.... 
+0001b5b0: 2020 2023 4765 7420 7965 6172 6c79 2063     #Get yearly c
+0001b5c0: 6f6d 706f 7369 7465 0d0a 2020 2020 636f  omposite..    co
+0001b5d0: 6d70 6f73 6974 6520 3d20 636f 6c6c 6563  mposite = collec
+0001b5e0: 7469 6f6e 2e66 696c 7465 7228 6565 2e46  tion.filter(ee.F
+0001b5f0: 696c 7465 722e 6361 6c65 6e64 6172 5261  ilter.calendarRa
+0001b600: 6e67 6528 7965 6172 2b79 6561 7257 6974  nge(year+yearWit
+0001b610: 684d 616a 6f72 6974 792c 2079 6561 722b  hMajority, year+
+0001b620: 7965 6172 5769 7468 4d61 6a6f 7269 7479  yearWithMajority
+0001b630: 2c20 2779 6561 7227 2929 0d0a 2020 2020  , 'year'))..    
+0001b640: 636f 6d70 6f73 6974 6520 3d20 6565 2e49  composite = ee.I
+0001b650: 6d61 6765 2863 6f6d 706f 7369 7465 2e66  mage(composite.f
+0001b660: 6972 7374 2829 290d 0a0d 0a20 2020 2023  irst())....    #
+0001b670: 5265 666f 726d 6174 2064 6174 6120 666f  Reformat data fo
+0001b680: 7220 6578 706f 7274 0d0a 2020 2020 636f  r export..    co
+0001b690: 6d70 6f73 6974 6542 616e 6473 203d 2063  mpositeBands = c
+0001b6a0: 6f6d 706f 7369 7465 2e62 616e 644e 616d  omposite.bandNam
+0001b6b0: 6573 2829 0d0a 2020 2020 6966 206e 6f6e  es()..    if non
+0001b6c0: 4469 7669 6465 4261 6e64 7320 213d 204e  DivideBands != N
+0001b6d0: 6f6e 653a 0d0a 2020 2020 2020 636f 6d70  one:..      comp
+0001b6e0: 6f73 6974 6531 306b 203d 2063 6f6d 706f  osite10k = compo
+0001b6f0: 7369 7465 2e73 656c 6563 7428 636f 6d70  site.select(comp
+0001b700: 6f73 6974 6542 616e 6473 2e72 656d 6f76  ositeBands.remov
+0001b710: 6541 6c6c 286e 6f6e 4469 7669 6465 4261  eAll(nonDivideBa
+0001b720: 6e64 7329 292e 6d75 6c74 6970 6c79 2831  nds)).multiply(1
+0001b730: 3030 3030 290d 0a20 2020 2020 2063 6f6d  0000)..      com
+0001b740: 706f 7369 7465 203d 2063 6f6d 706f 7369  posite = composi
+0001b750: 7465 3130 6b2e 6164 6442 616e 6473 2863  te10k.addBands(c
+0001b760: 6f6d 706f 7369 7465 2e73 656c 6563 7428  omposite.select(
+0001b770: 6e6f 6e44 6976 6964 6542 616e 6473 2929  nonDivideBands))
+0001b780: 2e73 656c 6563 7428 636f 6d70 6f73 6974  .select(composit
+0001b790: 6542 616e 6473 292e 696e 7431 3628 290d  eBands).int16().
+0001b7a0: 0a0d 0a20 2020 2065 6c73 653a 0d0a 2020  ...    else:..  
+0001b7b0: 2020 2020 636f 6d70 6f73 6974 6520 3d20      composite = 
+0001b7c0: 636f 6d70 6f73 6974 652e 6d75 6c74 6970  composite.multip
+0001b7d0: 6c79 2831 3030 3030 292e 696e 7431 3628  ly(10000).int16(
+0001b7e0: 290d 0a0d 0a20 2020 2073 7461 7274 5965  )....    startYe
+0001b7f0: 6172 436f 6d70 6f73 6974 6520 3d20 7374  arComposite = st
+0001b800: 6172 7459 6561 7254 0d0a 2020 2020 656e  artYearT..    en
+0001b810: 6459 6561 7243 6f6d 706f 7369 7465 203d  dYearComposite =
+0001b820: 2065 6e64 5965 6172 540d 0a20 2020 2073   endYearT..    s
+0001b830: 7973 7465 6d54 696d 6553 7461 7274 5965  ystemTimeStartYe
+0001b840: 6172 203d 2079 6561 722b 7965 6172 5769  ar = year+yearWi
+0001b850: 7468 4d61 6a6f 7269 7479 0d0a 2020 2020  thMajority..    
+0001b860: 7965 6172 4f72 6967 696e 616c 203d 2079  yearOriginal = y
+0001b870: 6561 720d 0a20 2020 2079 6561 7255 7365  ear..    yearUse
+0001b880: 6420 3d20 7379 7374 656d 5469 6d65 5374  d = systemTimeSt
+0001b890: 6172 7459 6561 720d 0a20 2020 2023 2061  artYear..    # a
+0001b8a0: 7267 735b 2773 7973 7465 6d3a 7469 6d65  rgs['system:time
+0001b8b0: 5f73 7461 7274 275d 203d 2065 652e 4461  _start'] = ee.Da
+0001b8c0: 7465 2e66 726f 6d59 4d44 2873 7973 7465  te.fromYMD(syste
+0001b8d0: 6d54 696d 6553 7461 7274 5965 6172 2c20  mTimeStartYear, 
+0001b8e0: 362c 2031 292e 6d69 6c6c 6973 2829 0d0a  6, 1).millis()..
+0001b8f0: 0d0a 2020 2020 636f 6d70 6f73 6974 6520  ..    composite 
+0001b900: 3d20 636f 6d70 6f73 6974 652e 7365 7428  = composite.set(
+0001b910: 666f 726d 6174 4172 6773 2861 7267 7329  formatArgs(args)
+0001b920: 290d 0a0d 0a20 2020 2063 6f6d 706f 7369  )....    composi
+0001b930: 7465 203d 2063 6f6d 706f 7369 7465 2e73  te = composite.s
+0001b940: 6574 2827 7379 7374 656d 3a74 696d 655f  et('system:time_
+0001b950: 7374 6172 7427 2c65 652e 4461 7465 2e66  start',ee.Date.f
+0001b960: 726f 6d59 4d44 2873 7973 7465 6d54 696d  romYMD(systemTim
+0001b970: 6553 7461 7274 5965 6172 2c20 362c 2031  eStartYear, 6, 1
+0001b980: 292e 6d69 6c6c 6973 2829 290d 0a0d 0a20  ).millis()).... 
+0001b990: 2020 2069 6620 6164 6469 7469 6f6e 616c     if additional
+0001b9a0: 5072 6f70 6572 7479 4469 6374 2021 3d20  PropertyDict != 
+0001b9b0: 4e6f 6e65 3a0d 0a20 2020 2020 2069 6620  None:..      if 
+0001b9c0: 2761 7267 7327 2069 6e20 6164 6469 7469  'args' in additi
+0001b9d0: 6f6e 616c 5072 6f70 6572 7479 4469 6374  onalPropertyDict
+0001b9e0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+0001b9f0: 2020 6465 6c20 6164 6469 7469 6f6e 616c    del additional
+0001ba00: 5072 6f70 6572 7479 4469 6374 5b27 6172  PropertyDict['ar
+0001ba10: 6773 275d 0d0a 2020 2020 2020 636f 6d70  gs']..      comp
+0001ba20: 6f73 6974 6520 3d20 636f 6d70 6f73 6974  osite = composit
+0001ba30: 652e 7365 7428 666f 726d 6174 4172 6773  e.set(formatArgs
+0001ba40: 2861 6464 6974 696f 6e61 6c50 726f 7065  (additionalPrope
+0001ba50: 7274 7944 6963 7429 290d 0a0d 0a20 2020  rtyDict))....   
+0001ba60: 2023 4578 706f 7274 2074 6865 2063 6f6d   #Export the com
+0001ba70: 706f 7369 7465 0d0a 2020 2020 2353 6574  posite..    #Set
+0001ba80: 2075 7020 6578 706f 7274 206e 616d 6520   up export name 
+0001ba90: 616e 6420 7061 7468 0d0a 2020 2020 6578  and path..    ex
+0001baa0: 706f 7274 4e61 6d65 203d 206f 7574 7075  portName = outpu
+0001bab0: 744e 616d 6520 202b 2027 5f27 202b 2074  tName  + '_' + t
+0001bac0: 6f61 4f72 5352 202b 2027 5f27 202b 2063  oaOrSR + '_' + c
+0001bad0: 6f6d 706f 7369 7469 6e67 4d65 7468 6f64  ompositingMethod
+0001bae0: 202b 2027 5f27 2020 2b20 7374 7228 696e   + '_'  + str(in
+0001baf0: 7428 7374 6172 7459 6561 7254 2929 202b  t(startYearT)) +
+0001bb00: 2027 5f27 202b 2073 7472 2869 6e74 2865   '_' + str(int(e
+0001bb10: 6e64 5965 6172 5429 292b 275f 2720 2b20  ndYearT))+'_' + 
+0001bb20: 7374 7228 696e 7428 7374 6172 744a 756c  str(int(startJul
+0001bb30: 6961 6e29 2920 2b20 275f 2720 2b20 7374  ian)) + '_' + st
+0001bb40: 7228 696e 7428 656e 644a 756c 6961 6e29  r(int(endJulian)
+0001bb50: 290d 0a20 2020 2065 7870 6f72 7450 6174  )..    exportPat
+0001bb60: 6820 3d20 6578 706f 7274 5061 7468 526f  h = exportPathRo
+0001bb70: 6f74 2b27 2f27 2b65 7870 6f72 744e 616d  ot+'/'+exportNam
+0001bb80: 650d 0a0d 0a0d 0a20 2020 2065 7870 6f72  e......    expor
+0001bb90: 7454 6f41 7373 6574 5772 6170 7065 7228  tToAssetWrapper(
+0001bba0: 5c0d 0a20 2020 2020 2069 6d61 6765 466f  \..      imageFo
+0001bbb0: 7245 7870 6f72 7420 3d20 636f 6d70 6f73  rExport = compos
+0001bbc0: 6974 652c 0d0a 2020 2020 2020 6173 7365  ite,..      asse
+0001bbd0: 744e 616d 6520 3d20 6578 706f 7274 4e61  tName = exportNa
+0001bbe0: 6d65 2c0d 0a20 2020 2020 2061 7373 6574  me,..      asset
+0001bbf0: 5061 7468 203d 2065 7870 6f72 7450 6174  Path = exportPat
+0001bc00: 682c 0d0a 2020 2020 2020 7079 7261 6d69  h,..      pyrami
+0001bc10: 6469 6e67 506f 6c69 6379 4f62 6a65 6374  dingPolicyObject
+0001bc20: 203d 2070 7972 616d 6964 696e 6750 6f6c   = pyramidingPol
+0001bc30: 6963 792c 0d0a 2020 2020 2020 726f 693d  icy,..      roi=
+0001bc40: 2073 7475 6479 4172 6561 2c0d 0a20 2020   studyArea,..   
+0001bc50: 2020 2073 6361 6c65 3d20 7363 616c 652c     scale= scale,
+0001bc60: 0d0a 2020 2020 2020 6372 7320 3d20 6372  ..      crs = cr
+0001bc70: 732c 0d0a 2020 2020 2020 7472 616e 7366  s,..      transf
+0001bc80: 6f72 6d20 3d20 7472 616e 7366 6f72 6d2c  orm = transform,
+0001bc90: 0d0a 2020 2020 2020 6f76 6572 7772 6974  ..      overwrit
+0001bca0: 653d 6f76 6572 7772 6974 6529 0d0a 0d0a  e=overwrite)....
+0001bcb0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
 0001bcc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001bcd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001bce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bcf0: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
+0001bcf0: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
 0001bd00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001bd10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001bd20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bd30: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-0001bd40: 0a23 5772 6170 7065 7220 6675 6e63 7469  .#Wrapper functi
-0001bd50: 6f6e 2066 6f72 2067 6574 7469 6e67 204c  on for getting L
-0001bd60: 616e 6473 6174 2069 6d61 6765 7279 0d0a  andsat imagery..
-0001bd70: 6465 6620 6765 744c 616e 6473 6174 5772  def getLandsatWr
-0001bd80: 6170 7065 7228 0d0a 2020 7374 7564 7941  apper(..  studyA
-0001bd90: 7265 612c 0d0a 2020 7374 6172 7459 6561  rea,..  startYea
-0001bda0: 722c 0d0a 2020 656e 6459 6561 722c 0d0a  r,..  endYear,..
-0001bdb0: 2020 7374 6172 744a 756c 6961 6e2c 0d0a    startJulian,..
-0001bdc0: 2020 656e 644a 756c 6961 6e2c 0d0a 2020    endJulian,..  
-0001bdd0: 7469 6d65 6275 6666 6572 203d 2030 2c0d  timebuffer = 0,.
-0001bde0: 0a20 2077 6569 6768 7473 203d 205b 315d  .  weights = [1]
-0001bdf0: 2c0d 0a20 2063 6f6d 706f 7369 7469 6e67  ,..  compositing
-0001be00: 4d65 7468 6f64 203d 2027 6d65 646f 6964  Method = 'medoid
-0001be10: 272c 0d0a 2020 746f 614f 7253 5220 3d20  ',..  toaOrSR = 
-0001be20: 2753 5227 2c0d 0a20 2069 6e63 6c75 6465  'SR',..  include
-0001be30: 534c 434f 6666 4c37 203d 2046 616c 7365  SLCOffL7 = False
-0001be40: 2c0d 0a20 2064 6566 7269 6e67 654c 3520  ,..  defringeL5 
-0001be50: 3d20 4661 6c73 652c 0d0a 2020 6170 706c  = False,..  appl
-0001be60: 7943 6c6f 7564 5363 6f72 6520 3d20 4661  yCloudScore = Fa
-0001be70: 6c73 652c 0d0a 2020 6170 706c 7946 6d61  lse,..  applyFma
-0001be80: 736b 436c 6f75 644d 6173 6b20 3d20 5472  skCloudMask = Tr
-0001be90: 7565 2c0d 0a20 2061 7070 6c79 5444 4f4d  ue,..  applyTDOM
-0001bea0: 203d 2046 616c 7365 2c0d 0a20 2061 7070   = False,..  app
-0001beb0: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
-0001bec0: 6f77 4d61 736b 203d 2054 7275 652c 0d0a  owMask = True,..
-0001bed0: 2020 6170 706c 7946 6d61 736b 536e 6f77    applyFmaskSnow
-0001bee0: 4d61 736b 203d 2046 616c 7365 2c0d 0a20  Mask = False,.. 
-0001bef0: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
-0001bf00: 6820 3d20 3130 2c0d 0a20 2070 6572 666f  h = 10,..  perfo
-0001bf10: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
-0001bf20: 6574 203d 2054 7275 652c 0d0a 2020 636c  et = True,..  cl
-0001bf30: 6f75 6453 636f 7265 5063 746c 203d 2031  oudScorePctl = 1
-0001bf40: 302c 0d0a 2020 7a53 636f 7265 5468 7265  0,..  zScoreThre
-0001bf50: 7368 203d 202d 312c 0d0a 2020 7368 6164  sh = -1,..  shad
-0001bf60: 6f77 5375 6d54 6872 6573 6820 3d20 302e  owSumThresh = 0.
-0001bf70: 3335 2c0d 0a20 2063 6f6e 7472 6163 7450  35,..  contractP
-0001bf80: 6978 656c 7320 3d20 312e 352c 0d0a 2020  ixels = 1.5,..  
-0001bf90: 6469 6c61 7465 5069 7865 6c73 203d 2033  dilatePixels = 3
-0001bfa0: 2e35 2c0d 0a20 2063 6f72 7265 6374 496c  .5,..  correctIl
-0001bfb0: 6c75 6d69 6e61 7469 6f6e 203d 2046 616c  lumination = Fal
-0001bfc0: 7365 2c0d 0a20 2063 6f72 7265 6374 5363  se,..  correctSc
-0001bfd0: 616c 6520 3d20 3235 302c 0d0a 2020 6578  ale = 250,..  ex
-0001bfe0: 706f 7274 436f 6d70 6f73 6974 6573 203d  portComposites =
-0001bff0: 2046 616c 7365 2c0d 0a20 206f 7574 7075   False,..  outpu
-0001c000: 744e 616d 6520 3d20 274c 616e 6473 6174  tName = 'Landsat
-0001c010: 2d43 6f6d 706f 7369 7465 272c 0d0a 2020  -Composite',..  
-0001c020: 6578 706f 7274 5061 7468 526f 6f74 203d  exportPathRoot =
-0001c030: 2027 7573 6572 732f 6961 6e68 6f75 736d   'users/ianhousm
-0001c040: 616e 2f74 6573 7427 2c0d 0a20 2063 7273  an/test',..  crs
-0001c050: 203d 2027 4550 5347 3a35 3037 3027 2c0d   = 'EPSG:5070',.
-0001c060: 0a20 2074 7261 6e73 666f 726d 203d 205b  .  transform = [
-0001c070: 3330 2c30 2c2d 3233 3631 3931 352e 302c  30,0,-2361915.0,
-0001c080: 302c 2d33 302c 3331 3737 3733 352e 305d  0,-30,3177735.0]
-0001c090: 2c0d 0a20 2073 6361 6c65 203d 204e 6f6e  ,..  scale = Non
-0001c0a0: 652c 0d0a 2020 7265 7361 6d70 6c65 4d65  e,..  resampleMe
-0001c0b0: 7468 6f64 203d 2027 6e65 6172 272c 0d0a  thod = 'near',..
-0001c0c0: 2020 7072 6543 6f6d 7075 7465 6443 6c6f    preComputedClo
-0001c0d0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
-0001c0e0: 4e6f 6e65 2c0d 0a20 2070 7265 436f 6d70  None,..  preComp
-0001c0f0: 7574 6564 5444 4f4d 4952 4d65 616e 203d  utedTDOMIRMean =
-0001c100: 204e 6f6e 652c 0d0a 2020 7072 6543 6f6d   None,..  preCom
-0001c110: 7075 7465 6454 444f 4d49 5253 7464 4465  putedTDOMIRStdDe
-0001c120: 7620 3d20 4e6f 6e65 2c0d 0a20 2063 6f6d  v = None,..  com
-0001c130: 706f 7369 7469 6e67 5265 6475 6365 7220  positingReducer 
-0001c140: 3d20 4e6f 6e65 2c0d 0a20 2068 6172 6d6f  = None,..  harmo
-0001c150: 6e69 7a65 4f4c 4920 3d20 4661 6c73 652c  nizeOLI = False,
-0001c160: 0d0a 2020 6c61 6e64 7361 7443 6f6c 6c65  ..  landsatColle
-0001c170: 6374 696f 6e56 6572 7369 6f6e 203d 2027  ctionVersion = '
-0001c180: 4332 272c 0d0a 2020 6f76 6572 7772 6974  C2',..  overwrit
-0001c190: 6520 3d20 4661 6c73 6529 3a0d 0a0d 0a20  e = False):.... 
-0001c1a0: 2074 6f61 4f72 5352 203d 2074 6f61 4f72   toaOrSR = toaOr
-0001c1b0: 5352 2e75 7070 6572 2829 0d0a 2020 6f72  SR.upper()..  or
-0001c1c0: 6967 696e 203d 2027 4c61 6e64 7361 7427  igin = 'Landsat'
-0001c1d0: 0d0a 2020 6172 6773 203d 2066 6f72 6d61  ..  args = forma
-0001c1e0: 7441 7267 7328 6c6f 6361 6c73 2829 290d  tArgs(locals()).
-0001c1f0: 0a20 2069 6620 2761 7267 7327 2069 6e20  .  if 'args' in 
-0001c200: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
-0001c210: 2020 6465 6c20 6172 6773 5b27 6172 6773    del args['args
-0001c220: 275d 0d0a 0d0a 2020 2350 7265 7061 7265  ']....  #Prepare
-0001c230: 2064 6174 6573 0d0a 2020 7772 6170 4f66   dates..  wrapOf
-0001c240: 6673 6574 203d 2030 0d0a 2020 6966 2073  fset = 0..  if s
-0001c250: 7461 7274 4a75 6c69 616e 203e 2065 6e64  tartJulian > end
-0001c260: 4a75 6c69 616e 3a0d 0a20 2020 2077 7261  Julian:..    wra
-0001c270: 704f 6666 7365 7420 3d20 3336 350d 0a20  pOffset = 365.. 
-0001c280: 2073 7461 7274 4461 7465 203d 2065 652e   startDate = ee.
-0001c290: 4461 7465 2e66 726f 6d59 4d44 2873 7461  Date.fromYMD(sta
-0001c2a0: 7274 5965 6172 2c31 2c31 292e 6164 7661  rtYear,1,1).adva
-0001c2b0: 6e63 6528 7374 6172 744a 756c 6961 6e2d  nce(startJulian-
-0001c2c0: 312c 2764 6179 2729 0d0a 2020 656e 6444  1,'day')..  endD
-0001c2d0: 6174 6520 3d20 6565 2e44 6174 652e 6672  ate = ee.Date.fr
-0001c2e0: 6f6d 594d 4428 656e 6459 6561 722c 312c  omYMD(endYear,1,
-0001c2f0: 3129 2e61 6476 616e 6365 2865 6e64 4a75  1).advance(endJu
-0001c300: 6c69 616e 2d31 2b77 7261 704f 6666 7365  lian-1+wrapOffse
-0001c310: 742c 2764 6179 2729 0d0a 0d0a 2020 2320  t,'day')....  # 
-0001c320: 4765 7420 4c61 6e64 7361 7420 696d 6167  Get Landsat imag
-0001c330: 6520 636f 6c6c 6563 7469 6f6e 2061 6e64  e collection and
-0001c340: 2061 7070 6c79 2063 6c6f 7564 206d 6173   apply cloud mas
-0001c350: 6b69 6e67 0d0a 2020 6c73 203d 2067 6574  king..  ls = get
-0001c360: 5072 6f63 6573 7365 644c 616e 6473 6174  ProcessedLandsat
-0001c370: 5363 656e 6573 280d 0a20 2020 2073 7475  Scenes(..    stu
-0001c380: 6479 4172 6561 203d 2073 7475 6479 4172  dyArea = studyAr
-0001c390: 6561 2c0d 0a20 2020 2073 7461 7274 5965  ea,..    startYe
-0001c3a0: 6172 203d 2073 7461 7274 5965 6172 2c0d  ar = startYear,.
-0001c3b0: 0a20 2020 2065 6e64 5965 6172 203d 2065  .    endYear = e
-0001c3c0: 6e64 5965 6172 2c0d 0a20 2020 2073 7461  ndYear,..    sta
-0001c3d0: 7274 4a75 6c69 616e 203d 2073 7461 7274  rtJulian = start
-0001c3e0: 4a75 6c69 616e 2c0d 0a20 2020 2065 6e64  Julian,..    end
-0001c3f0: 4a75 6c69 616e 203d 2065 6e64 4a75 6c69  Julian = endJuli
-0001c400: 616e 2c0d 0a20 2020 2074 6f61 4f72 5352  an,..    toaOrSR
-0001c410: 203d 2074 6f61 4f72 5352 2c0d 0a20 2020   = toaOrSR,..   
-0001c420: 2069 6e63 6c75 6465 534c 434f 6666 4c37   includeSLCOffL7
-0001c430: 203d 2069 6e63 6c75 6465 534c 434f 6666   = includeSLCOff
-0001c440: 4c37 2c0d 0a20 2020 2064 6566 7269 6e67  L7,..    defring
-0001c450: 654c 3520 3d20 6465 6672 696e 6765 4c35  eL5 = defringeL5
-0001c460: 2c0d 0a20 2020 2061 7070 6c79 436c 6f75  ,..    applyClou
-0001c470: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
-0001c480: 6f75 6453 636f 7265 2c0d 0a20 2020 2061  oudScore,..    a
-0001c490: 7070 6c79 466d 6173 6b43 6c6f 7564 4d61  pplyFmaskCloudMa
-0001c4a0: 736b 203d 2061 7070 6c79 466d 6173 6b43  sk = applyFmaskC
-0001c4b0: 6c6f 7564 4d61 736b 2c0d 0a20 2020 2061  loudMask,..    a
-0001c4c0: 7070 6c79 5444 4f4d 203d 2061 7070 6c79  pplyTDOM = apply
-0001c4d0: 5444 4f4d 2c0d 0a20 2020 2061 7070 6c79  TDOM,..    apply
-0001c4e0: 466d 6173 6b43 6c6f 7564 5368 6164 6f77  FmaskCloudShadow
-0001c4f0: 4d61 736b 203d 2061 7070 6c79 466d 6173  Mask = applyFmas
-0001c500: 6b43 6c6f 7564 5368 6164 6f77 4d61 736b  kCloudShadowMask
-0001c510: 2c0d 0a20 2020 2061 7070 6c79 466d 6173  ,..    applyFmas
-0001c520: 6b53 6e6f 774d 6173 6b20 3d20 6170 706c  kSnowMask = appl
-0001c530: 7946 6d61 736b 536e 6f77 4d61 736b 2c0d  yFmaskSnowMask,.
-0001c540: 0a20 2020 2063 6c6f 7564 5363 6f72 6554  .    cloudScoreT
-0001c550: 6872 6573 6820 3d20 636c 6f75 6453 636f  hresh = cloudSco
-0001c560: 7265 5468 7265 7368 2c0d 0a20 2020 2070  reThresh,..    p
-0001c570: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
-0001c580: 4f66 6673 6574 203d 2070 6572 666f 726d  Offset = perform
-0001c590: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-0001c5a0: 2c0d 0a20 2020 2063 6c6f 7564 5363 6f72  ,..    cloudScor
-0001c5b0: 6550 6374 6c20 3d20 636c 6f75 6453 636f  ePctl = cloudSco
-0001c5c0: 7265 5063 746c 2c0d 0a20 2020 207a 5363  rePctl,..    zSc
-0001c5d0: 6f72 6554 6872 6573 6820 3d20 7a53 636f  oreThresh = zSco
-0001c5e0: 7265 5468 7265 7368 2c0d 0a20 2020 2073  reThresh,..    s
-0001c5f0: 6861 646f 7753 756d 5468 7265 7368 203d  hadowSumThresh =
-0001c600: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
-0001c610: 2c0d 0a20 2020 2063 6f6e 7472 6163 7450  ,..    contractP
-0001c620: 6978 656c 7320 3d20 636f 6e74 7261 6374  ixels = contract
-0001c630: 5069 7865 6c73 2c0d 0a20 2020 2064 696c  Pixels,..    dil
-0001c640: 6174 6550 6978 656c 7320 3d20 6469 6c61  atePixels = dila
-0001c650: 7465 5069 7865 6c73 2c0d 0a20 2020 2072  tePixels,..    r
-0001c660: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
-0001c670: 7265 7361 6d70 6c65 4d65 7468 6f64 2c0d  resampleMethod,.
-0001c680: 0a20 2020 2068 6172 6d6f 6e69 7a65 4f4c  .    harmonizeOL
-0001c690: 4920 3d20 6861 726d 6f6e 697a 654f 4c49  I = harmonizeOLI
-0001c6a0: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
-0001c6b0: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
-0001c6c0: 6574 203d 2070 7265 436f 6d70 7574 6564  et = preComputed
-0001c6d0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-0001c6e0: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
-0001c6f0: 6564 5444 4f4d 4952 4d65 616e 203d 2070  edTDOMIRMean = p
-0001c700: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
-0001c710: 4d65 616e 2c0d 0a20 2020 2070 7265 436f  Mean,..    preCo
-0001c720: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
-0001c730: 6576 203d 2070 7265 436f 6d70 7574 6564  ev = preComputed
-0001c740: 5444 4f4d 4952 5374 6444 6576 2c0d 0a20  TDOMIRStdDev,.. 
-0001c750: 2020 206c 616e 6473 6174 436f 6c6c 6563     landsatCollec
-0001c760: 7469 6f6e 5665 7273 696f 6e20 3d20 6c61  tionVersion = la
+0001bd30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bd40: 2323 2323 2323 0d0a 2357 7261 7070 6572  ######..#Wrapper
+0001bd50: 2066 756e 6374 696f 6e20 666f 7220 6765   function for ge
+0001bd60: 7474 696e 6720 4c61 6e64 7361 7420 696d  tting Landsat im
+0001bd70: 6167 6572 790d 0a64 6566 2067 6574 4c61  agery..def getLa
+0001bd80: 6e64 7361 7457 7261 7070 6572 280d 0a20  ndsatWrapper(.. 
+0001bd90: 2073 7475 6479 4172 6561 2c0d 0a20 2073   studyArea,..  s
+0001bda0: 7461 7274 5965 6172 2c0d 0a20 2065 6e64  tartYear,..  end
+0001bdb0: 5965 6172 2c0d 0a20 2073 7461 7274 4a75  Year,..  startJu
+0001bdc0: 6c69 616e 2c0d 0a20 2065 6e64 4a75 6c69  lian,..  endJuli
+0001bdd0: 616e 2c0d 0a20 2074 696d 6562 7566 6665  an,..  timebuffe
+0001bde0: 7220 3d20 302c 0d0a 2020 7765 6967 6874  r = 0,..  weight
+0001bdf0: 7320 3d20 5b31 5d2c 0d0a 2020 636f 6d70  s = [1],..  comp
+0001be00: 6f73 6974 696e 674d 6574 686f 6420 3d20  ositingMethod = 
+0001be10: 276d 6564 6f69 6427 2c0d 0a20 2074 6f61  'medoid',..  toa
+0001be20: 4f72 5352 203d 2027 5352 272c 0d0a 2020  OrSR = 'SR',..  
+0001be30: 696e 636c 7564 6553 4c43 4f66 664c 3720  includeSLCOffL7 
+0001be40: 3d20 4661 6c73 652c 0d0a 2020 6465 6672  = False,..  defr
+0001be50: 696e 6765 4c35 203d 2046 616c 7365 2c0d  ingeL5 = False,.
+0001be60: 0a20 2061 7070 6c79 436c 6f75 6453 636f  .  applyCloudSco
+0001be70: 7265 203d 2046 616c 7365 2c0d 0a20 2061  re = False,..  a
+0001be80: 7070 6c79 466d 6173 6b43 6c6f 7564 4d61  pplyFmaskCloudMa
+0001be90: 736b 203d 2054 7275 652c 0d0a 2020 6170  sk = True,..  ap
+0001bea0: 706c 7954 444f 4d20 3d20 4661 6c73 652c  plyTDOM = False,
+0001beb0: 0d0a 2020 6170 706c 7946 6d61 736b 436c  ..  applyFmaskCl
+0001bec0: 6f75 6453 6861 646f 774d 6173 6b20 3d20  oudShadowMask = 
+0001bed0: 5472 7565 2c0d 0a20 2061 7070 6c79 466d  True,..  applyFm
+0001bee0: 6173 6b53 6e6f 774d 6173 6b20 3d20 4661  askSnowMask = Fa
+0001bef0: 6c73 652c 0d0a 2020 636c 6f75 6453 636f  lse,..  cloudSco
+0001bf00: 7265 5468 7265 7368 203d 2031 302c 0d0a  reThresh = 10,..
+0001bf10: 2020 7065 7266 6f72 6d43 6c6f 7564 5363    performCloudSc
+0001bf20: 6f72 654f 6666 7365 7420 3d20 5472 7565  oreOffset = True
+0001bf30: 2c0d 0a20 2063 6c6f 7564 5363 6f72 6550  ,..  cloudScoreP
+0001bf40: 6374 6c20 3d20 3130 2c0d 0a20 207a 5363  ctl = 10,..  zSc
+0001bf50: 6f72 6554 6872 6573 6820 3d20 2d31 2c0d  oreThresh = -1,.
+0001bf60: 0a20 2073 6861 646f 7753 756d 5468 7265  .  shadowSumThre
+0001bf70: 7368 203d 2030 2e33 352c 0d0a 2020 636f  sh = 0.35,..  co
+0001bf80: 6e74 7261 6374 5069 7865 6c73 203d 2031  ntractPixels = 1
+0001bf90: 2e35 2c0d 0a20 2064 696c 6174 6550 6978  .5,..  dilatePix
+0001bfa0: 656c 7320 3d20 332e 352c 0d0a 2020 636f  els = 3.5,..  co
+0001bfb0: 7272 6563 7449 6c6c 756d 696e 6174 696f  rrectIlluminatio
+0001bfc0: 6e20 3d20 4661 6c73 652c 0d0a 2020 636f  n = False,..  co
+0001bfd0: 7272 6563 7453 6361 6c65 203d 2032 3530  rrectScale = 250
+0001bfe0: 2c0d 0a20 2065 7870 6f72 7443 6f6d 706f  ,..  exportCompo
+0001bff0: 7369 7465 7320 3d20 4661 6c73 652c 0d0a  sites = False,..
+0001c000: 2020 6f75 7470 7574 4e61 6d65 203d 2027    outputName = '
+0001c010: 4c61 6e64 7361 742d 436f 6d70 6f73 6974  Landsat-Composit
+0001c020: 6527 2c0d 0a20 2065 7870 6f72 7450 6174  e',..  exportPat
+0001c030: 6852 6f6f 7420 3d20 2775 7365 7273 2f69  hRoot = 'users/i
+0001c040: 616e 686f 7573 6d61 6e2f 7465 7374 272c  anhousman/test',
+0001c050: 0d0a 2020 6372 7320 3d20 2745 5053 473a  ..  crs = 'EPSG:
+0001c060: 3530 3730 272c 0d0a 2020 7472 616e 7366  5070',..  transf
+0001c070: 6f72 6d20 3d20 5b33 302c 302c 2d32 3336  orm = [30,0,-236
+0001c080: 3139 3135 2e30 2c30 2c2d 3330 2c33 3137  1915.0,0,-30,317
+0001c090: 3737 3335 2e30 5d2c 0d0a 2020 7363 616c  7735.0],..  scal
+0001c0a0: 6520 3d20 4e6f 6e65 2c0d 0a20 2072 6573  e = None,..  res
+0001c0b0: 616d 706c 654d 6574 686f 6420 3d20 276e  ampleMethod = 'n
+0001c0c0: 6561 7227 2c0d 0a20 2070 7265 436f 6d70  ear',..  preComp
+0001c0d0: 7574 6564 436c 6f75 6453 636f 7265 4f66  utedCloudScoreOf
+0001c0e0: 6673 6574 203d 204e 6f6e 652c 0d0a 2020  fset = None,..  
+0001c0f0: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
+0001c100: 524d 6561 6e20 3d20 4e6f 6e65 2c0d 0a20  RMean = None,.. 
+0001c110: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
+0001c120: 4952 5374 6444 6576 203d 204e 6f6e 652c  IRStdDev = None,
+0001c130: 0d0a 2020 636f 6d70 6f73 6974 696e 6752  ..  compositingR
+0001c140: 6564 7563 6572 203d 204e 6f6e 652c 0d0a  educer = None,..
+0001c150: 2020 6861 726d 6f6e 697a 654f 4c49 203d    harmonizeOLI =
+0001c160: 2046 616c 7365 2c0d 0a20 206c 616e 6473   False,..  lands
+0001c170: 6174 436f 6c6c 6563 7469 6f6e 5665 7273  atCollectionVers
+0001c180: 696f 6e20 3d20 2743 3227 2c0d 0a20 206f  ion = 'C2',..  o
+0001c190: 7665 7277 7269 7465 203d 2046 616c 7365  verwrite = False
+0001c1a0: 2c0d 0a20 2076 6572 626f 7365 203d 2046  ,..  verbose = F
+0001c1b0: 616c 7365 293a 0d0a 0d0a 2020 746f 614f  alse):....  toaO
+0001c1c0: 7253 5220 3d20 746f 614f 7253 522e 7570  rSR = toaOrSR.up
+0001c1d0: 7065 7228 290d 0a20 206f 7269 6769 6e20  per()..  origin 
+0001c1e0: 3d20 274c 616e 6473 6174 270d 0a20 2061  = 'Landsat'..  a
+0001c1f0: 7267 7320 3d20 666f 726d 6174 4172 6773  rgs = formatArgs
+0001c200: 286c 6f63 616c 7328 2929 0d0a 2020 6966  (locals())..  if
+0001c210: 2027 6172 6773 2720 696e 2061 7267 732e   'args' in args.
+0001c220: 6b65 7973 2829 3a0d 0a20 2020 2064 656c  keys():..    del
+0001c230: 2061 7267 735b 2761 7267 7327 5d0d 0a0d   args['args']...
+0001c240: 0a20 2023 5072 6570 6172 6520 6461 7465  .  #Prepare date
+0001c250: 730d 0a20 2077 7261 704f 6666 7365 7420  s..  wrapOffset 
+0001c260: 3d20 300d 0a20 2069 6620 7374 6172 744a  = 0..  if startJ
+0001c270: 756c 6961 6e20 3e20 656e 644a 756c 6961  ulian > endJulia
+0001c280: 6e3a 0d0a 2020 2020 7772 6170 4f66 6673  n:..    wrapOffs
+0001c290: 6574 203d 2033 3635 0d0a 2020 7374 6172  et = 365..  star
+0001c2a0: 7444 6174 6520 3d20 6565 2e44 6174 652e  tDate = ee.Date.
+0001c2b0: 6672 6f6d 594d 4428 7374 6172 7459 6561  fromYMD(startYea
+0001c2c0: 722c 312c 3129 2e61 6476 616e 6365 2873  r,1,1).advance(s
+0001c2d0: 7461 7274 4a75 6c69 616e 2d31 2c27 6461  tartJulian-1,'da
+0001c2e0: 7927 290d 0a20 2065 6e64 4461 7465 203d  y')..  endDate =
+0001c2f0: 2065 652e 4461 7465 2e66 726f 6d59 4d44   ee.Date.fromYMD
+0001c300: 2865 6e64 5965 6172 2c31 2c31 292e 6164  (endYear,1,1).ad
+0001c310: 7661 6e63 6528 656e 644a 756c 6961 6e2d  vance(endJulian-
+0001c320: 312b 7772 6170 4f66 6673 6574 2c27 6461  1+wrapOffset,'da
+0001c330: 7927 290d 0a0d 0a20 2023 2047 6574 204c  y')....  # Get L
+0001c340: 616e 6473 6174 2069 6d61 6765 2063 6f6c  andsat image col
+0001c350: 6c65 6374 696f 6e20 616e 6420 6170 706c  lection and appl
+0001c360: 7920 636c 6f75 6420 6d61 736b 696e 670d  y cloud masking.
+0001c370: 0a20 206c 7320 3d20 6765 7450 726f 6365  .  ls = getProce
+0001c380: 7373 6564 4c61 6e64 7361 7453 6365 6e65  ssedLandsatScene
+0001c390: 7328 0d0a 2020 2020 7374 7564 7941 7265  s(..    studyAre
+0001c3a0: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
+0001c3b0: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
+0001c3c0: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
+0001c3d0: 656e 6459 6561 7220 3d20 656e 6459 6561  endYear = endYea
+0001c3e0: 722c 0d0a 2020 2020 7374 6172 744a 756c  r,..    startJul
+0001c3f0: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
+0001c400: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
+0001c410: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
+0001c420: 2020 2020 746f 614f 7253 5220 3d20 746f      toaOrSR = to
+0001c430: 614f 7253 522c 0d0a 2020 2020 696e 636c  aOrSR,..    incl
+0001c440: 7564 6553 4c43 4f66 664c 3720 3d20 696e  udeSLCOffL7 = in
+0001c450: 636c 7564 6553 4c43 4f66 664c 372c 0d0a  cludeSLCOffL7,..
+0001c460: 2020 2020 6465 6672 696e 6765 4c35 203d      defringeL5 =
+0001c470: 2064 6566 7269 6e67 654c 352c 0d0a 2020   defringeL5,..  
+0001c480: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
+0001c490: 6520 3d20 6170 706c 7943 6c6f 7564 5363  e = applyCloudSc
+0001c4a0: 6f72 652c 0d0a 2020 2020 6170 706c 7946  ore,..    applyF
+0001c4b0: 6d61 736b 436c 6f75 644d 6173 6b20 3d20  maskCloudMask = 
+0001c4c0: 6170 706c 7946 6d61 736b 436c 6f75 644d  applyFmaskCloudM
+0001c4d0: 6173 6b2c 0d0a 2020 2020 6170 706c 7954  ask,..    applyT
+0001c4e0: 444f 4d20 3d20 6170 706c 7954 444f 4d2c  DOM = applyTDOM,
+0001c4f0: 0d0a 2020 2020 6170 706c 7946 6d61 736b  ..    applyFmask
+0001c500: 436c 6f75 6453 6861 646f 774d 6173 6b20  CloudShadowMask 
+0001c510: 3d20 6170 706c 7946 6d61 736b 436c 6f75  = applyFmaskClou
+0001c520: 6453 6861 646f 774d 6173 6b2c 0d0a 2020  dShadowMask,..  
+0001c530: 2020 6170 706c 7946 6d61 736b 536e 6f77    applyFmaskSnow
+0001c540: 4d61 736b 203d 2061 7070 6c79 466d 6173  Mask = applyFmas
+0001c550: 6b53 6e6f 774d 6173 6b2c 0d0a 2020 2020  kSnowMask,..    
+0001c560: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
+0001c570: 203d 2063 6c6f 7564 5363 6f72 6554 6872   = cloudScoreThr
+0001c580: 6573 682c 0d0a 2020 2020 7065 7266 6f72  esh,..    perfor
+0001c590: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
+0001c5a0: 7420 3d20 7065 7266 6f72 6d43 6c6f 7564  t = performCloud
+0001c5b0: 5363 6f72 654f 6666 7365 742c 0d0a 2020  ScoreOffset,..  
+0001c5c0: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
+0001c5d0: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
+0001c5e0: 6c2c 0d0a 2020 2020 7a53 636f 7265 5468  l,..    zScoreTh
+0001c5f0: 7265 7368 203d 207a 5363 6f72 6554 6872  resh = zScoreThr
+0001c600: 6573 682c 0d0a 2020 2020 7368 6164 6f77  esh,..    shadow
+0001c610: 5375 6d54 6872 6573 6820 3d20 7368 6164  SumThresh = shad
+0001c620: 6f77 5375 6d54 6872 6573 682c 0d0a 2020  owSumThresh,..  
+0001c630: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+0001c640: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
+0001c650: 732c 0d0a 2020 2020 6469 6c61 7465 5069  s,..    dilatePi
+0001c660: 7865 6c73 203d 2064 696c 6174 6550 6978  xels = dilatePix
+0001c670: 656c 732c 0d0a 2020 2020 7265 7361 6d70  els,..    resamp
+0001c680: 6c65 4d65 7468 6f64 203d 2072 6573 616d  leMethod = resam
+0001c690: 706c 654d 6574 686f 642c 0d0a 2020 2020  pleMethod,..    
+0001c6a0: 6861 726d 6f6e 697a 654f 4c49 203d 2068  harmonizeOLI = h
+0001c6b0: 6172 6d6f 6e69 7a65 4f4c 492c 0d0a 2020  armonizeOLI,..  
+0001c6c0: 2020 7072 6543 6f6d 7075 7465 6443 6c6f    preComputedClo
+0001c6d0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+0001c6e0: 7072 6543 6f6d 7075 7465 6443 6c6f 7564  preComputedCloud
+0001c6f0: 5363 6f72 654f 6666 7365 742c 0d0a 2020  ScoreOffset,..  
+0001c700: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
+0001c710: 4d49 524d 6561 6e20 3d20 7072 6543 6f6d  MIRMean = preCom
+0001c720: 7075 7465 6454 444f 4d49 524d 6561 6e2c  putedTDOMIRMean,
+0001c730: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
+0001c740: 6454 444f 4d49 5253 7464 4465 7620 3d20  dTDOMIRStdDev = 
+0001c750: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
+0001c760: 5253 7464 4465 762c 0d0a 2020 2020 6c61  RStdDev,..    la
 0001c770: 6e64 7361 7443 6f6c 6c65 6374 696f 6e56  ndsatCollectionV
-0001c780: 6572 7369 6f6e 290d 0a0d 0a20 2023 4164  ersion)....  #Ad
-0001c790: 6420 7a65 6e69 7468 2061 6e64 2061 7a69  d zenith and azi
-0001c7a0: 6d75 7468 0d0a 2020 6966 2063 6f72 7265  muth..  if corre
-0001c7b0: 6374 496c 6c75 6d69 6e61 7469 6f6e 3a0d  ctIllumination:.
-0001c7c0: 0a20 2020 2070 7269 6e74 2827 4164 6469  .    print('Addi
-0001c7d0: 6e67 207a 656e 6974 6820 616e 6420 617a  ng zenith and az
-0001c7e0: 696d 7574 6820 666f 7220 7465 7272 6169  imuth for terrai
-0001c7f0: 6e20 636f 7272 6563 7469 6f6e 2729 0d0a  n correction')..
-0001c800: 2020 2020 6c73 203d 206c 732e 6d61 7028      ls = ls.map(
-0001c810: 6c61 6d62 6461 2069 6d67 3a20 6164 645a  lambda img: addZ
-0001c820: 656e 6974 6841 7a69 6d75 7468 2869 6d67  enithAzimuth(img
-0001c830: 2c20 746f 614f 7253 5229 290d 0a0d 0a20  , toaOrSR)).... 
-0001c840: 2023 4372 6561 7465 2063 6f6d 706f 7369   #Create composi
-0001c850: 7465 2074 696d 6520 7365 7269 6573 0d0a  te time series..
-0001c860: 2020 7473 203d 2063 6f6d 706f 7369 7465    ts = composite
-0001c870: 5469 6d65 5365 7269 6573 285c 0d0a 2020  TimeSeries(\..  
-0001c880: 2020 6c73 203d 206c 732c 0d0a 2020 2020    ls = ls,..    
-0001c890: 7374 6172 7459 6561 7220 3d20 7374 6172  startYear = star
-0001c8a0: 7459 6561 722c 0d0a 2020 2020 656e 6459  tYear,..    endY
-0001c8b0: 6561 7220 3d20 656e 6459 6561 722c 0d0a  ear = endYear,..
-0001c8c0: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
-0001c8d0: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
-0001c8e0: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
-0001c8f0: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
-0001c900: 7469 6d65 6275 6666 6572 203d 2074 696d  timebuffer = tim
-0001c910: 6562 7566 6665 722c 0d0a 2020 2020 7765  ebuffer,..    we
-0001c920: 6967 6874 7320 3d20 7765 6967 6874 732c  ights = weights,
-0001c930: 0d0a 2020 2020 636f 6d70 6f73 6974 696e  ..    compositin
-0001c940: 674d 6574 686f 6420 3d20 636f 6d70 6f73  gMethod = compos
-0001c950: 6974 696e 674d 6574 686f 642c 0d0a 2020  itingMethod,..  
-0001c960: 2020 636f 6d70 6f73 6974 696e 6752 6564    compositingRed
-0001c970: 7563 6572 203d 2063 6f6d 706f 7369 7469  ucer = compositi
-0001c980: 6e67 5265 6475 6365 7229 0d0a 0d0a 2020  ngReducer)....  
-0001c990: 2320 436f 7272 6563 7420 696c 6c75 6d69  # Correct illumi
-0001c9a0: 6e61 7469 6f6e 0d0a 2020 6966 2063 6f72  nation..  if cor
-0001c9b0: 7265 6374 496c 6c75 6d69 6e61 7469 6f6e  rectIllumination
-0001c9c0: 3a0d 0a20 2020 2070 7269 6e74 2827 436f  :..    print('Co
-0001c9d0: 7272 6563 7469 6e67 2069 6c6c 756d 696e  rrecting illumin
-0001c9e0: 6174 696f 6e27 293b 0d0a 2020 2020 7473  ation');..    ts
-0001c9f0: 203d 2074 732e 6d61 7028 696c 6c75 6d69   = ts.map(illumi
-0001ca00: 6e61 7469 6f6e 436f 6e64 6974 696f 6e29  nationCondition)
-0001ca10: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
-0001ca20: 2069 6c6c 756d 696e 6174 696f 6e43 6f72   illuminationCor
-0001ca30: 7265 6374 696f 6e28 696d 672c 2063 6f72  rection(img, cor
-0001ca40: 7265 6374 5363 616c 652c 2073 7475 6479  rectScale, study
-0001ca50: 4172 6561 2929 0d0a 0d0a 2020 2345 7870  Area))....  #Exp
-0001ca60: 6f72 7420 636f 6d70 6f73 6974 6573 0d0a  ort composites..
-0001ca70: 2020 6966 2065 7870 6f72 7443 6f6d 706f    if exportCompo
-0001ca80: 7369 7465 733a 0d0a 2020 2020 6966 2063  sites:..    if c
-0001ca90: 6f6d 706f 7369 7469 6e67 4d65 7468 6f64  ompositingMethod
-0001caa0: 203d 3d20 276d 6564 6f69 6427 3a0d 0a20   == 'medoid':.. 
-0001cab0: 2020 2020 2065 7870 6f72 7442 616e 6473       exportBands
-0001cac0: 203d 205b 2762 6c75 6527 2c20 2767 7265   = ['blue', 'gre
-0001cad0: 656e 272c 2027 7265 6427 2c20 276e 6972  en', 'red', 'nir
-0001cae0: 272c 2027 7377 6972 3127 2c20 2773 7769  ', 'swir1', 'swi
-0001caf0: 7232 272c 2027 7465 6d70 272c 2027 636f  r2', 'temp', 'co
-0001cb00: 6d70 6f73 6974 654f 6273 436f 756e 7427  mpositeObsCount'
-0001cb10: 2c20 2773 656e 736f 7227 2c20 2779 6561  , 'sensor', 'yea
-0001cb20: 7227 2c20 276a 756c 6961 6e44 6179 275d  r', 'julianDay']
-0001cb30: 0d0a 2020 2020 2020 6e6f 6e44 6976 6964  ..      nonDivid
-0001cb40: 6542 616e 6473 203d 205b 2774 656d 7027  eBands = ['temp'
-0001cb50: 2c20 2763 6f6d 706f 7369 7465 4f62 7343  , 'compositeObsC
-0001cb60: 6f75 6e74 272c 2027 7365 6e73 6f72 272c  ount', 'sensor',
-0001cb70: 2027 7965 6172 272c 2027 6a75 6c69 616e   'year', 'julian
-0001cb80: 4461 7927 5d0d 0a20 2020 2065 6c73 653a  Day']..    else:
-0001cb90: 0d0a 2020 2020 2020 6578 706f 7274 4261  ..      exportBa
-0001cba0: 6e64 7320 3d20 5b27 626c 7565 272c 2027  nds = ['blue', '
-0001cbb0: 6772 6565 6e27 2c20 2772 6564 272c 2027  green', 'red', '
-0001cbc0: 6e69 7227 2c20 2773 7769 7231 272c 2027  nir', 'swir1', '
-0001cbd0: 7377 6972 3227 2c20 2774 656d 7027 2c20  swir2', 'temp', 
-0001cbe0: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-0001cbf0: 6e74 275d 0d0a 2020 2020 2020 6e6f 6e44  nt']..      nonD
-0001cc00: 6976 6964 6542 616e 6473 203d 205b 2774  ivideBands = ['t
-0001cc10: 656d 7027 2c20 2763 6f6d 706f 7369 7465  emp', 'composite
-0001cc20: 4f62 7343 6f75 6e74 275d 0d0a 0d0a 2020  ObsCount']....  
-0001cc30: 2020 6578 706f 7274 436f 6d70 6f73 6974    exportComposit
-0001cc40: 6543 6f6c 6c65 6374 696f 6e28 5c0d 0a20  eCollection(\.. 
-0001cc50: 2020 2020 2063 6f6c 6c65 6374 696f 6e20       collection 
-0001cc60: 3d20 7473 2c0d 0a20 2020 2020 2065 7870  = ts,..      exp
-0001cc70: 6f72 7450 6174 6852 6f6f 7420 3d20 6578  ortPathRoot = ex
-0001cc80: 706f 7274 5061 7468 526f 6f74 2c0d 0a20  portPathRoot,.. 
-0001cc90: 2020 2020 206f 7574 7075 744e 616d 6520       outputName 
-0001cca0: 3d20 6f75 7470 7574 4e61 6d65 2c0d 0a20  = outputName,.. 
-0001ccb0: 2020 2020 206f 7269 6769 6e20 3d20 6f72       origin = or
-0001ccc0: 6967 696e 2c0d 0a20 2020 2020 2073 7475  igin,..      stu
-0001ccd0: 6479 4172 6561 203d 2073 7475 6479 4172  dyArea = studyAr
-0001cce0: 6561 2c0d 0a20 2020 2020 2063 7273 203d  ea,..      crs =
-0001ccf0: 2063 7273 2c0d 0a20 2020 2020 2074 7261   crs,..      tra
-0001cd00: 6e73 666f 726d 203d 2074 7261 6e73 666f  nsform = transfo
-0001cd10: 726d 2c0d 0a20 2020 2020 2073 6361 6c65  rm,..      scale
-0001cd20: 203d 2073 6361 6c65 2c0d 0a20 2020 2020   = scale,..     
-0001cd30: 2073 7461 7274 5965 6172 203d 2073 7461   startYear = sta
-0001cd40: 7274 5965 6172 2c0d 0a20 2020 2020 2065  rtYear,..      e
-0001cd50: 6e64 5965 6172 203d 2065 6e64 5965 6172  ndYear = endYear
-0001cd60: 2c0d 0a20 2020 2020 2073 7461 7274 4a75  ,..      startJu
-0001cd70: 6c69 616e 203d 2073 7461 7274 4a75 6c69  lian = startJuli
-0001cd80: 616e 2c0d 0a20 2020 2020 2065 6e64 4a75  an,..      endJu
-0001cd90: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
-0001cda0: 2c0d 0a20 2020 2020 2063 6f6d 706f 7369  ,..      composi
-0001cdb0: 7469 6e67 4d65 7468 6f64 203d 2063 6f6d  tingMethod = com
-0001cdc0: 706f 7369 7469 6e67 4d65 7468 6f64 2c0d  positingMethod,.
-0001cdd0: 0a20 2020 2020 2074 696d 6562 7566 6665  .      timebuffe
-0001cde0: 7220 3d20 7469 6d65 6275 6666 6572 2c0d  r = timebuffer,.
-0001cdf0: 0a20 2020 2020 2074 6f61 4f72 5352 203d  .      toaOrSR =
-0001ce00: 2074 6f61 4f72 5352 2c0d 0a20 2020 2020   toaOrSR,..     
-0001ce10: 206e 6f6e 4469 7669 6465 4261 6e64 7320   nonDivideBands 
-0001ce20: 3d20 6e6f 6e44 6976 6964 6542 616e 6473  = nonDivideBands
-0001ce30: 2c0d 0a20 2020 2020 2065 7870 6f72 7442  ,..      exportB
-0001ce40: 616e 6473 203d 2065 7870 6f72 7442 616e  ands = exportBan
-0001ce50: 6473 2c0d 0a20 2020 2020 2023 2077 6569  ds,..      # wei
-0001ce60: 6768 7473 203d 2077 6569 6768 7473 2c0d  ghts = weights,.
-0001ce70: 0a20 2020 2020 2023 2064 6566 7269 6e67  .      # defring
-0001ce80: 654c 3520 3d20 4661 6c73 652c 0d0a 2020  eL5 = False,..  
-0001ce90: 2020 2020 2320 696e 636c 7564 6553 4c43      # includeSLC
-0001cea0: 4f66 664c 3720 3d20 696e 636c 7564 6553  OffL7 = includeS
-0001ceb0: 4c43 4f66 664c 372c 0d0a 2020 2020 2020  LCOffL7,..      
-0001cec0: 2320 636f 6e76 6572 7454 6f44 6169 6c79  # convertToDaily
-0001ced0: 4d6f 7361 6963 7320 3d20 274e 4127 2c0d  Mosaics = 'NA',.
-0001cee0: 0a20 2020 2020 2023 2061 7070 6c79 5141  .      # applyQA
-0001cef0: 4261 6e64 203d 2046 616c 7365 2c0d 0a20  Band = False,.. 
-0001cf00: 2020 2020 2023 2061 7070 6c79 436c 6f75       # applyClou
-0001cf10: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
-0001cf20: 6f75 6453 636f 7265 2c0d 0a20 2020 2020  oudScore,..     
-0001cf30: 2023 2061 7070 6c79 466d 6173 6b43 6c6f   # applyFmaskClo
-0001cf40: 7564 4d61 736b 203d 2061 7070 6c79 466d  udMask = applyFm
-0001cf50: 6173 6b43 6c6f 7564 4d61 736b 2c0d 0a20  askCloudMask,.. 
-0001cf60: 2020 2020 2023 2061 7070 6c79 436c 6f75       # applyClou
-0001cf70: 6450 726f 6261 6269 6c69 7479 203d 2027  dProbability = '
-0001cf80: 4e41 272c 0d0a 2020 2020 2020 2320 6170  NA',..      # ap
-0001cf90: 706c 7954 444f 4d20 3d20 6170 706c 7954  plyTDOM = applyT
-0001cfa0: 444f 4d2c 0d0a 2020 2020 2020 2320 6170  DOM,..      # ap
-0001cfb0: 706c 7946 6d61 736b 436c 6f75 6453 6861  plyFmaskCloudSha
-0001cfc0: 646f 774d 6173 6b20 3d20 6170 706c 7946  dowMask = applyF
-0001cfd0: 6d61 736b 436c 6f75 6453 6861 646f 774d  maskCloudShadowM
-0001cfe0: 6173 6b2c 0d0a 2020 2020 2020 2320 6170  ask,..      # ap
-0001cff0: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
-0001d000: 203d 2061 7070 6c79 466d 6173 6b53 6e6f   = applyFmaskSno
-0001d010: 774d 6173 6b2c 0d0a 2020 2020 2020 2320  wMask,..      # 
-0001d020: 6170 706c 7953 6861 646f 7753 6869 6674  applyShadowShift
-0001d030: 203d 2027 4e41 272c 0d0a 2020 2020 2020   = 'NA',..      
-0001d040: 2320 636c 6f75 6448 6569 6768 7473 203d  # cloudHeights =
-0001d050: 2063 6c6f 7564 4865 6967 6874 732c 0d0a   cloudHeights,..
-0001d060: 2020 2020 2020 2320 636c 6f75 6453 636f        # cloudSco
-0001d070: 7265 5468 7265 7368 203d 2063 6c6f 7564  reThresh = cloud
-0001d080: 5363 6f72 6554 6872 6573 682c 0d0a 2020  ScoreThresh,..  
-0001d090: 2020 2020 2320 7065 7266 6f72 6d43 6c6f      # performClo
-0001d0a0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
-0001d0b0: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
-0001d0c0: 654f 6666 7365 742c 0d0a 2020 2020 2020  eOffset,..      
-0001d0d0: 2320 636c 6f75 6453 636f 7265 5063 746c  # cloudScorePctl
-0001d0e0: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
-0001d0f0: 6c2c 0d0a 2020 2020 2020 2320 7a53 636f  l,..      # zSco
-0001d100: 7265 5468 7265 7368 203d 207a 5363 6f72  reThresh = zScor
-0001d110: 6554 6872 6573 682c 0d0a 2020 2020 2020  eThresh,..      
-0001d120: 2320 7368 6164 6f77 5375 6d54 6872 6573  # shadowSumThres
-0001d130: 6820 3d20 7368 6164 6f77 5375 6d54 6872  h = shadowSumThr
-0001d140: 6573 682c 0d0a 2020 2020 2020 2320 636f  esh,..      # co
-0001d150: 6e74 7261 6374 5069 7865 6c73 203d 2063  ntractPixels = c
-0001d160: 6f6e 7472 6163 7450 6978 656c 732c 0d0a  ontractPixels,..
-0001d170: 2020 2020 2020 2320 6469 6c61 7465 5069        # dilatePi
-0001d180: 7865 6c73 203d 2064 696c 6174 6550 6978  xels = dilatePix
-0001d190: 656c 732c 0d0a 2020 2020 2020 2320 636f  els,..      # co
-0001d1a0: 7272 6563 7449 6c6c 756d 696e 6174 696f  rrectIlluminatio
-0001d1b0: 6e20 3d20 636f 7272 6563 7449 6c6c 756d  n = correctIllum
-0001d1c0: 696e 6174 696f 6e2c 0d0a 2020 2020 2020  ination,..      
-0001d1d0: 2320 636f 7272 6563 7453 6361 6c65 203d  # correctScale =
-0001d1e0: 2063 6f72 7265 6374 5363 616c 652c 0d0a   correctScale,..
-0001d1f0: 2020 2020 2020 2320 6e6f 6e44 6976 6964        # nonDivid
-0001d200: 6542 616e 6473 203d 206e 6f6e 4469 7669  eBands = nonDivi
-0001d210: 6465 4261 6e64 732c 0d0a 2020 2020 2020  deBands,..      
-0001d220: 2320 6578 706f 7274 4261 6e64 7320 3d20  # exportBands = 
-0001d230: 6578 706f 7274 4261 6e64 732c 0d0a 2020  exportBands,..  
-0001d240: 2020 2020 2320 7265 7361 6d70 6c65 4d65      # resampleMe
-0001d250: 7468 6f64 203d 2072 6573 616d 706c 654d  thod = resampleM
-0001d260: 6574 686f 642c 0d0a 2020 2020 2020 2320  ethod,..      # 
-0001d270: 7275 6e43 6861 7374 6169 6e48 6172 6d6f  runChastainHarmo
-0001d280: 6e69 7a61 7469 6f6e 203d 2027 4e41 272c  nization = 'NA',
-0001d290: 0d0a 2020 2020 2020 6164 6469 7469 6f6e  ..      addition
-0001d2a0: 616c 5072 6f70 6572 7479 4469 6374 203d  alPropertyDict =
-0001d2b0: 2061 7267 732c 0d0a 2020 2020 2020 6f76   args,..      ov
-0001d2c0: 6572 7772 6974 6520 3d20 6f76 6572 7772  erwrite = overwr
-0001d2d0: 6974 6529 0d0a 0d0a 2020 6172 6773 5b27  ite)....  args['
-0001d2e0: 7072 6f63 6573 7365 6453 6365 6e65 7327  processedScenes'
-0001d2f0: 5d20 3d20 6c73 0d0a 2020 6172 6773 5b27  ] = ls..  args['
-0001d300: 7072 6f63 6573 7365 6443 6f6d 706f 7369  processedComposi
-0001d310: 7465 7327 5d20 3d20 7473 0d0a 0d0a 2020  tes'] = ts....  
-0001d320: 7265 7475 726e 2061 7267 730d 0a0d 0a23  return args....#
-0001d330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d370: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
+0001c780: 6572 7369 6f6e 203d 206c 616e 6473 6174  ersion = landsat
+0001c790: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
+0001c7a0: 6e2c 0d0a 2020 2020 7665 7262 6f73 6520  n,..    verbose 
+0001c7b0: 3d20 7665 7262 6f73 6529 0d0a 0d0a 2020  = verbose)....  
+0001c7c0: 2341 6464 207a 656e 6974 6820 616e 6420  #Add zenith and 
+0001c7d0: 617a 696d 7574 680d 0a20 2069 6620 636f  azimuth..  if co
+0001c7e0: 7272 6563 7449 6c6c 756d 696e 6174 696f  rrectIlluminatio
+0001c7f0: 6e3a 0d0a 2020 2020 7072 696e 7428 2741  n:..    print('A
+0001c800: 6464 696e 6720 7a65 6e69 7468 2061 6e64  dding zenith and
+0001c810: 2061 7a69 6d75 7468 2066 6f72 2074 6572   azimuth for ter
+0001c820: 7261 696e 2063 6f72 7265 6374 696f 6e27  rain correction'
+0001c830: 290d 0a20 2020 206c 7320 3d20 6c73 2e6d  )..    ls = ls.m
+0001c840: 6170 286c 616d 6264 6120 696d 673a 2061  ap(lambda img: a
+0001c850: 6464 5a65 6e69 7468 417a 696d 7574 6828  ddZenithAzimuth(
+0001c860: 696d 672c 2074 6f61 4f72 5352 2929 0d0a  img, toaOrSR))..
+0001c870: 0d0a 2020 2343 7265 6174 6520 636f 6d70  ..  #Create comp
+0001c880: 6f73 6974 6520 7469 6d65 2073 6572 6965  osite time serie
+0001c890: 730d 0a20 2074 7320 3d20 636f 6d70 6f73  s..  ts = compos
+0001c8a0: 6974 6554 696d 6553 6572 6965 7328 5c0d  iteTimeSeries(\.
+0001c8b0: 0a20 2020 206c 7320 3d20 6c73 2c0d 0a20  .    ls = ls,.. 
+0001c8c0: 2020 2073 7461 7274 5965 6172 203d 2073     startYear = s
+0001c8d0: 7461 7274 5965 6172 2c0d 0a20 2020 2065  tartYear,..    e
+0001c8e0: 6e64 5965 6172 203d 2065 6e64 5965 6172  ndYear = endYear
+0001c8f0: 2c0d 0a20 2020 2073 7461 7274 4a75 6c69  ,..    startJuli
+0001c900: 616e 203d 2073 7461 7274 4a75 6c69 616e  an = startJulian
+0001c910: 2c0d 0a20 2020 2065 6e64 4a75 6c69 616e  ,..    endJulian
+0001c920: 203d 2065 6e64 4a75 6c69 616e 2c0d 0a20   = endJulian,.. 
+0001c930: 2020 2074 696d 6562 7566 6665 7220 3d20     timebuffer = 
+0001c940: 7469 6d65 6275 6666 6572 2c0d 0a20 2020  timebuffer,..   
+0001c950: 2077 6569 6768 7473 203d 2077 6569 6768   weights = weigh
+0001c960: 7473 2c0d 0a20 2020 2063 6f6d 706f 7369  ts,..    composi
+0001c970: 7469 6e67 4d65 7468 6f64 203d 2063 6f6d  tingMethod = com
+0001c980: 706f 7369 7469 6e67 4d65 7468 6f64 2c0d  positingMethod,.
+0001c990: 0a20 2020 2063 6f6d 706f 7369 7469 6e67  .    compositing
+0001c9a0: 5265 6475 6365 7220 3d20 636f 6d70 6f73  Reducer = compos
+0001c9b0: 6974 696e 6752 6564 7563 6572 290d 0a0d  itingReducer)...
+0001c9c0: 0a20 2023 2043 6f72 7265 6374 2069 6c6c  .  # Correct ill
+0001c9d0: 756d 696e 6174 696f 6e0d 0a20 2069 6620  umination..  if 
+0001c9e0: 636f 7272 6563 7449 6c6c 756d 696e 6174  correctIlluminat
+0001c9f0: 696f 6e3a 0d0a 2020 2020 7072 696e 7428  ion:..    print(
+0001ca00: 2743 6f72 7265 6374 696e 6720 696c 6c75  'Correcting illu
+0001ca10: 6d69 6e61 7469 6f6e 2729 3b0d 0a20 2020  mination');..   
+0001ca20: 2074 7320 3d20 7473 2e6d 6170 2869 6c6c   ts = ts.map(ill
+0001ca30: 756d 696e 6174 696f 6e43 6f6e 6469 7469  uminationConditi
+0001ca40: 6f6e 292e 6d61 7028 6c61 6d62 6461 2069  on).map(lambda i
+0001ca50: 6d67 3a20 696c 6c75 6d69 6e61 7469 6f6e  mg: illumination
+0001ca60: 436f 7272 6563 7469 6f6e 2869 6d67 2c20  Correction(img, 
+0001ca70: 636f 7272 6563 7453 6361 6c65 2c20 7374  correctScale, st
+0001ca80: 7564 7941 7265 6129 290d 0a0d 0a20 2023  udyArea))....  #
+0001ca90: 4578 706f 7274 2063 6f6d 706f 7369 7465  Export composite
+0001caa0: 730d 0a20 2069 6620 6578 706f 7274 436f  s..  if exportCo
+0001cab0: 6d70 6f73 6974 6573 3a0d 0a20 2020 2069  mposites:..    i
+0001cac0: 6620 636f 6d70 6f73 6974 696e 674d 6574  f compositingMet
+0001cad0: 686f 6420 3d3d 2027 6d65 646f 6964 273a  hod == 'medoid':
+0001cae0: 0d0a 2020 2020 2020 6578 706f 7274 4261  ..      exportBa
+0001caf0: 6e64 7320 3d20 5b27 626c 7565 272c 2027  nds = ['blue', '
+0001cb00: 6772 6565 6e27 2c20 2772 6564 272c 2027  green', 'red', '
+0001cb10: 6e69 7227 2c20 2773 7769 7231 272c 2027  nir', 'swir1', '
+0001cb20: 7377 6972 3227 2c20 2774 656d 7027 2c20  swir2', 'temp', 
+0001cb30: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
+0001cb40: 6e74 272c 2027 7365 6e73 6f72 272c 2027  nt', 'sensor', '
+0001cb50: 7965 6172 272c 2027 6a75 6c69 616e 4461  year', 'julianDa
+0001cb60: 7927 5d0d 0a20 2020 2020 206e 6f6e 4469  y']..      nonDi
+0001cb70: 7669 6465 4261 6e64 7320 3d20 5b27 7465  videBands = ['te
+0001cb80: 6d70 272c 2027 636f 6d70 6f73 6974 654f  mp', 'compositeO
+0001cb90: 6273 436f 756e 7427 2c20 2773 656e 736f  bsCount', 'senso
+0001cba0: 7227 2c20 2779 6561 7227 2c20 276a 756c  r', 'year', 'jul
+0001cbb0: 6961 6e44 6179 275d 0d0a 2020 2020 656c  ianDay']..    el
+0001cbc0: 7365 3a0d 0a20 2020 2020 2065 7870 6f72  se:..      expor
+0001cbd0: 7442 616e 6473 203d 205b 2762 6c75 6527  tBands = ['blue'
+0001cbe0: 2c20 2767 7265 656e 272c 2027 7265 6427  , 'green', 'red'
+0001cbf0: 2c20 276e 6972 272c 2027 7377 6972 3127  , 'nir', 'swir1'
+0001cc00: 2c20 2773 7769 7232 272c 2027 7465 6d70  , 'swir2', 'temp
+0001cc10: 272c 2027 636f 6d70 6f73 6974 654f 6273  ', 'compositeObs
+0001cc20: 436f 756e 7427 5d0d 0a20 2020 2020 206e  Count']..      n
+0001cc30: 6f6e 4469 7669 6465 4261 6e64 7320 3d20  onDivideBands = 
+0001cc40: 5b27 7465 6d70 272c 2027 636f 6d70 6f73  ['temp', 'compos
+0001cc50: 6974 654f 6273 436f 756e 7427 5d0d 0a0d  iteObsCount']...
+0001cc60: 0a20 2020 2065 7870 6f72 7443 6f6d 706f  .    exportCompo
+0001cc70: 7369 7465 436f 6c6c 6563 7469 6f6e 285c  siteCollection(\
+0001cc80: 0d0a 2020 2020 2020 636f 6c6c 6563 7469  ..      collecti
+0001cc90: 6f6e 203d 2074 732c 0d0a 2020 2020 2020  on = ts,..      
+0001cca0: 6578 706f 7274 5061 7468 526f 6f74 203d  exportPathRoot =
+0001ccb0: 2065 7870 6f72 7450 6174 6852 6f6f 742c   exportPathRoot,
+0001ccc0: 0d0a 2020 2020 2020 6f75 7470 7574 4e61  ..      outputNa
+0001ccd0: 6d65 203d 206f 7574 7075 744e 616d 652c  me = outputName,
+0001cce0: 0d0a 2020 2020 2020 6f72 6967 696e 203d  ..      origin =
+0001ccf0: 206f 7269 6769 6e2c 0d0a 2020 2020 2020   origin,..      
+0001cd00: 7374 7564 7941 7265 6120 3d20 7374 7564  studyArea = stud
+0001cd10: 7941 7265 612c 0d0a 2020 2020 2020 6372  yArea,..      cr
+0001cd20: 7320 3d20 6372 732c 0d0a 2020 2020 2020  s = crs,..      
+0001cd30: 7472 616e 7366 6f72 6d20 3d20 7472 616e  transform = tran
+0001cd40: 7366 6f72 6d2c 0d0a 2020 2020 2020 7363  sform,..      sc
+0001cd50: 616c 6520 3d20 7363 616c 652c 0d0a 2020  ale = scale,..  
+0001cd60: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
+0001cd70: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
+0001cd80: 2020 656e 6459 6561 7220 3d20 656e 6459    endYear = endY
+0001cd90: 6561 722c 0d0a 2020 2020 2020 7374 6172  ear,..      star
+0001cda0: 744a 756c 6961 6e20 3d20 7374 6172 744a  tJulian = startJ
+0001cdb0: 756c 6961 6e2c 0d0a 2020 2020 2020 656e  ulian,..      en
+0001cdc0: 644a 756c 6961 6e20 3d20 656e 644a 756c  dJulian = endJul
+0001cdd0: 6961 6e2c 0d0a 2020 2020 2020 636f 6d70  ian,..      comp
+0001cde0: 6f73 6974 696e 674d 6574 686f 6420 3d20  ositingMethod = 
+0001cdf0: 636f 6d70 6f73 6974 696e 674d 6574 686f  compositingMetho
+0001ce00: 642c 0d0a 2020 2020 2020 7469 6d65 6275  d,..      timebu
+0001ce10: 6666 6572 203d 2074 696d 6562 7566 6665  ffer = timebuffe
+0001ce20: 722c 0d0a 2020 2020 2020 746f 614f 7253  r,..      toaOrS
+0001ce30: 5220 3d20 746f 614f 7253 522c 0d0a 2020  R = toaOrSR,..  
+0001ce40: 2020 2020 6e6f 6e44 6976 6964 6542 616e      nonDivideBan
+0001ce50: 6473 203d 206e 6f6e 4469 7669 6465 4261  ds = nonDivideBa
+0001ce60: 6e64 732c 0d0a 2020 2020 2020 6578 706f  nds,..      expo
+0001ce70: 7274 4261 6e64 7320 3d20 6578 706f 7274  rtBands = export
+0001ce80: 4261 6e64 732c 0d0a 2020 2020 2020 2320  Bands,..      # 
+0001ce90: 7765 6967 6874 7320 3d20 7765 6967 6874  weights = weight
+0001cea0: 732c 0d0a 2020 2020 2020 2320 6465 6672  s,..      # defr
+0001ceb0: 696e 6765 4c35 203d 2046 616c 7365 2c0d  ingeL5 = False,.
+0001cec0: 0a20 2020 2020 2023 2069 6e63 6c75 6465  .      # include
+0001ced0: 534c 434f 6666 4c37 203d 2069 6e63 6c75  SLCOffL7 = inclu
+0001cee0: 6465 534c 434f 6666 4c37 2c0d 0a20 2020  deSLCOffL7,..   
+0001cef0: 2020 2023 2063 6f6e 7665 7274 546f 4461     # convertToDa
+0001cf00: 696c 794d 6f73 6169 6373 203d 2027 4e41  ilyMosaics = 'NA
+0001cf10: 272c 0d0a 2020 2020 2020 2320 6170 706c  ',..      # appl
+0001cf20: 7951 4142 616e 6420 3d20 4661 6c73 652c  yQABand = False,
+0001cf30: 0d0a 2020 2020 2020 2320 6170 706c 7943  ..      # applyC
+0001cf40: 6c6f 7564 5363 6f72 6520 3d20 6170 706c  loudScore = appl
+0001cf50: 7943 6c6f 7564 5363 6f72 652c 0d0a 2020  yCloudScore,..  
+0001cf60: 2020 2020 2320 6170 706c 7946 6d61 736b      # applyFmask
+0001cf70: 436c 6f75 644d 6173 6b20 3d20 6170 706c  CloudMask = appl
+0001cf80: 7946 6d61 736b 436c 6f75 644d 6173 6b2c  yFmaskCloudMask,
+0001cf90: 0d0a 2020 2020 2020 2320 6170 706c 7943  ..      # applyC
+0001cfa0: 6c6f 7564 5072 6f62 6162 696c 6974 7920  loudProbability 
+0001cfb0: 3d20 274e 4127 2c0d 0a20 2020 2020 2023  = 'NA',..      #
+0001cfc0: 2061 7070 6c79 5444 4f4d 203d 2061 7070   applyTDOM = app
+0001cfd0: 6c79 5444 4f4d 2c0d 0a20 2020 2020 2023  lyTDOM,..      #
+0001cfe0: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+0001cff0: 5368 6164 6f77 4d61 736b 203d 2061 7070  ShadowMask = app
+0001d000: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
+0001d010: 6f77 4d61 736b 2c0d 0a20 2020 2020 2023  owMask,..      #
+0001d020: 2061 7070 6c79 466d 6173 6b53 6e6f 774d   applyFmaskSnowM
+0001d030: 6173 6b20 3d20 6170 706c 7946 6d61 736b  ask = applyFmask
+0001d040: 536e 6f77 4d61 736b 2c0d 0a20 2020 2020  SnowMask,..     
+0001d050: 2023 2061 7070 6c79 5368 6164 6f77 5368   # applyShadowSh
+0001d060: 6966 7420 3d20 274e 4127 2c0d 0a20 2020  ift = 'NA',..   
+0001d070: 2020 2023 2063 6c6f 7564 4865 6967 6874     # cloudHeight
+0001d080: 7320 3d20 636c 6f75 6448 6569 6768 7473  s = cloudHeights
+0001d090: 2c0d 0a20 2020 2020 2023 2063 6c6f 7564  ,..      # cloud
+0001d0a0: 5363 6f72 6554 6872 6573 6820 3d20 636c  ScoreThresh = cl
+0001d0b0: 6f75 6453 636f 7265 5468 7265 7368 2c0d  oudScoreThresh,.
+0001d0c0: 0a20 2020 2020 2023 2070 6572 666f 726d  .      # perform
+0001d0d0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+0001d0e0: 203d 2070 6572 666f 726d 436c 6f75 6453   = performCloudS
+0001d0f0: 636f 7265 4f66 6673 6574 2c0d 0a20 2020  coreOffset,..   
+0001d100: 2020 2023 2063 6c6f 7564 5363 6f72 6550     # cloudScoreP
+0001d110: 6374 6c20 3d20 636c 6f75 6453 636f 7265  ctl = cloudScore
+0001d120: 5063 746c 2c0d 0a20 2020 2020 2023 207a  Pctl,..      # z
+0001d130: 5363 6f72 6554 6872 6573 6820 3d20 7a53  ScoreThresh = zS
+0001d140: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
+0001d150: 2020 2023 2073 6861 646f 7753 756d 5468     # shadowSumTh
+0001d160: 7265 7368 203d 2073 6861 646f 7753 756d  resh = shadowSum
+0001d170: 5468 7265 7368 2c0d 0a20 2020 2020 2023  Thresh,..      #
+0001d180: 2063 6f6e 7472 6163 7450 6978 656c 7320   contractPixels 
+0001d190: 3d20 636f 6e74 7261 6374 5069 7865 6c73  = contractPixels
+0001d1a0: 2c0d 0a20 2020 2020 2023 2064 696c 6174  ,..      # dilat
+0001d1b0: 6550 6978 656c 7320 3d20 6469 6c61 7465  ePixels = dilate
+0001d1c0: 5069 7865 6c73 2c0d 0a20 2020 2020 2023  Pixels,..      #
+0001d1d0: 2063 6f72 7265 6374 496c 6c75 6d69 6e61   correctIllumina
+0001d1e0: 7469 6f6e 203d 2063 6f72 7265 6374 496c  tion = correctIl
+0001d1f0: 6c75 6d69 6e61 7469 6f6e 2c0d 0a20 2020  lumination,..   
+0001d200: 2020 2023 2063 6f72 7265 6374 5363 616c     # correctScal
+0001d210: 6520 3d20 636f 7272 6563 7453 6361 6c65  e = correctScale
+0001d220: 2c0d 0a20 2020 2020 2023 206e 6f6e 4469  ,..      # nonDi
+0001d230: 7669 6465 4261 6e64 7320 3d20 6e6f 6e44  videBands = nonD
+0001d240: 6976 6964 6542 616e 6473 2c0d 0a20 2020  ivideBands,..   
+0001d250: 2020 2023 2065 7870 6f72 7442 616e 6473     # exportBands
+0001d260: 203d 2065 7870 6f72 7442 616e 6473 2c0d   = exportBands,.
+0001d270: 0a20 2020 2020 2023 2072 6573 616d 706c  .      # resampl
+0001d280: 654d 6574 686f 6420 3d20 7265 7361 6d70  eMethod = resamp
+0001d290: 6c65 4d65 7468 6f64 2c0d 0a20 2020 2020  leMethod,..     
+0001d2a0: 2023 2072 756e 4368 6173 7461 696e 4861   # runChastainHa
+0001d2b0: 726d 6f6e 697a 6174 696f 6e20 3d20 274e  rmonization = 'N
+0001d2c0: 4127 2c0d 0a20 2020 2020 2061 6464 6974  A',..      addit
+0001d2d0: 696f 6e61 6c50 726f 7065 7274 7944 6963  ionalPropertyDic
+0001d2e0: 7420 3d20 6172 6773 2c0d 0a20 2020 2020  t = args,..     
+0001d2f0: 206f 7665 7277 7269 7465 203d 206f 7665   overwrite = ove
+0001d300: 7277 7269 7465 290d 0a0d 0a20 2061 7267  rwrite)....  arg
+0001d310: 735b 2770 726f 6365 7373 6564 5363 656e  s['processedScen
+0001d320: 6573 275d 203d 206c 730d 0a20 2061 7267  es'] = ls..  arg
+0001d330: 735b 2770 726f 6365 7373 6564 436f 6d70  s['processedComp
+0001d340: 6f73 6974 6573 275d 203d 2074 730d 0a0d  osites'] = ts...
+0001d350: 0a20 2072 6574 7572 6e20 6172 6773 0d0a  .  return args..
+0001d360: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+0001d370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001d380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001d390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3a0: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
 0001d3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d3c0: 2323 230d 0a23 5772 6170 7065 7220 6675  ###..#Wrapper fu
-0001d3d0: 6e63 7469 6f6e 2066 6f72 2067 6574 7469  nction for getti
-0001d3e0: 6e67 204c 616e 6473 6174 2069 6d61 6765  ng Landsat image
-0001d3f0: 7279 0d0a 6465 6620 6765 7450 726f 6365  ry..def getProce
-0001d400: 7373 6564 4c61 6e64 7361 7453 6365 6e65  ssedLandsatScene
-0001d410: 7328 0d0a 2020 7374 7564 7941 7265 612c  s(..  studyArea,
-0001d420: 0d0a 2020 7374 6172 7459 6561 722c 0d0a  ..  startYear,..
-0001d430: 2020 656e 6459 6561 722c 0d0a 2020 7374    endYear,..  st
-0001d440: 6172 744a 756c 6961 6e2c 0d0a 2020 656e  artJulian,..  en
-0001d450: 644a 756c 6961 6e2c 0d0a 2020 746f 614f  dJulian,..  toaO
-0001d460: 7253 5220 3d20 2753 5227 2c0d 0a20 2069  rSR = 'SR',..  i
-0001d470: 6e63 6c75 6465 534c 434f 6666 4c37 203d  ncludeSLCOffL7 =
-0001d480: 2046 616c 7365 2c0d 0a20 2064 6566 7269   False,..  defri
-0001d490: 6e67 654c 3520 3d20 4661 6c73 652c 0d0a  ngeL5 = False,..
-0001d4a0: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
-0001d4b0: 6520 3d20 4661 6c73 652c 0d0a 2020 6170  e = False,..  ap
-0001d4c0: 706c 7946 6d61 736b 436c 6f75 644d 6173  plyFmaskCloudMas
-0001d4d0: 6b20 3d20 5472 7565 2c0d 0a20 2061 7070  k = True,..  app
-0001d4e0: 6c79 5444 4f4d 203d 2046 616c 7365 2c0d  lyTDOM = False,.
-0001d4f0: 0a20 2061 7070 6c79 466d 6173 6b43 6c6f  .  applyFmaskClo
-0001d500: 7564 5368 6164 6f77 4d61 736b 203d 2054  udShadowMask = T
-0001d510: 7275 652c 0d0a 2020 6170 706c 7946 6d61  rue,..  applyFma
-0001d520: 736b 536e 6f77 4d61 736b 203d 2046 616c  skSnowMask = Fal
-0001d530: 7365 2c0d 0a20 2063 6c6f 7564 5363 6f72  se,..  cloudScor
-0001d540: 6554 6872 6573 6820 3d20 3130 2c0d 0a20  eThresh = 10,.. 
-0001d550: 2070 6572 666f 726d 436c 6f75 6453 636f   performCloudSco
-0001d560: 7265 4f66 6673 6574 203d 2054 7275 652c  reOffset = True,
-0001d570: 0d0a 2020 636c 6f75 6453 636f 7265 5063  ..  cloudScorePc
-0001d580: 746c 203d 2031 302c 0d0a 2020 7a53 636f  tl = 10,..  zSco
-0001d590: 7265 5468 7265 7368 203d 202d 312c 0d0a  reThresh = -1,..
-0001d5a0: 2020 7368 6164 6f77 5375 6d54 6872 6573    shadowSumThres
-0001d5b0: 6820 3d20 302e 3335 2c0d 0a20 2063 6f6e  h = 0.35,..  con
-0001d5c0: 7472 6163 7450 6978 656c 7320 3d20 312e  tractPixels = 1.
-0001d5d0: 352c 0d0a 2020 6469 6c61 7465 5069 7865  5,..  dilatePixe
-0001d5e0: 6c73 203d 2033 2e35 2c0d 0a20 2073 6861  ls = 3.5,..  sha
-0001d5f0: 646f 7753 756d 4261 6e64 7320 3d20 5b27  dowSumBands = ['
-0001d600: 6e69 7227 2c27 7377 6972 3127 5d2c 0d0a  nir','swir1'],..
-0001d610: 2020 7265 7361 6d70 6c65 4d65 7468 6f64    resampleMethod
-0001d620: 203d 2027 6e65 6172 272c 0d0a 2020 6861   = 'near',..  ha
-0001d630: 726d 6f6e 697a 654f 4c49 203d 2046 616c  rmonizeOLI = Fal
-0001d640: 7365 2c0d 0a20 2070 7265 436f 6d70 7574  se,..  preComput
-0001d650: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
-0001d660: 6574 203d 204e 6f6e 652c 0d0a 2020 7072  et = None,..  pr
-0001d670: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
-0001d680: 6561 6e20 3d20 4e6f 6e65 2c0d 0a20 2070  ean = None,..  p
-0001d690: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
-0001d6a0: 5374 6444 6576 203d 204e 6f6e 652c 0d0a  StdDev = None,..
-0001d6b0: 2020 6c61 6e64 7361 7443 6f6c 6c65 6374    landsatCollect
-0001d6c0: 696f 6e56 6572 7369 6f6e 203d 2027 4332  ionVersion = 'C2
-0001d6d0: 2729 3a0d 0a0d 0a20 206f 7269 6769 6e20  '):....  origin 
-0001d6e0: 3d20 274c 616e 6473 6174 270d 0a20 2074  = 'Landsat'..  t
-0001d6f0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
-0001d700: 2e75 7070 6572 2829 0d0a 2020 6966 2074  .upper()..  if t
-0001d710: 6f61 4f72 5352 2e6c 6f77 6572 2829 203d  oaOrSR.lower() =
-0001d720: 3d20 2774 6f61 2720 616e 6420 6c61 6e64  = 'toa' and land
-0001d730: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
-0001d740: 7369 6f6e 2e6c 6f77 6572 2829 203d 3d20  sion.lower() == 
-0001d750: 2763 3127 2061 6e64 2028 6170 706c 7946  'c1' and (applyF
-0001d760: 6d61 736b 436c 6f75 644d 6173 6b20 6f72  maskCloudMask or
-0001d770: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
-0001d780: 5368 6164 6f77 4d61 736b 2020 6f72 2061  ShadowMask  or a
-0001d790: 7070 6c79 466d 6173 6b53 6e6f 774d 6173  pplyFmaskSnowMas
-0001d7a0: 6b20 293a 0d0a 2020 2020 6164 6450 6978  k ):..    addPix
-0001d7b0: 656c 5141 203d 2054 7275 650d 0a20 2065  elQA = True..  e
-0001d7c0: 6c73 653a 0d0a 2020 2020 6164 6450 6978  lse:..    addPix
-0001d7d0: 656c 5141 203d 2046 616c 7365 0d0a 0d0a  elQA = False....
-0001d7e0: 2020 2350 7265 7061 7265 2064 6174 6573    #Prepare dates
-0001d7f0: 0d0a 2020 2357 7261 7020 7468 6520 6461  ..  #Wrap the da
-0001d800: 7465 7320 6966 206e 6565 6465 640d 0a20  tes if needed.. 
-0001d810: 2077 7261 704f 6666 7365 7420 3d20 300d   wrapOffset = 0.
-0001d820: 0a20 2069 6620 7374 6172 744a 756c 6961  .  if startJulia
-0001d830: 6e20 3e20 656e 644a 756c 6961 6e3a 0d0a  n > endJulian:..
-0001d840: 2020 2020 7772 6170 4f66 6673 6574 203d      wrapOffset =
-0001d850: 2033 3635 0d0a 2020 7374 6172 7444 6174   365..  startDat
-0001d860: 6520 3d20 6565 2e44 6174 652e 6672 6f6d  e = ee.Date.from
-0001d870: 594d 4428 7374 6172 7459 6561 722c 312c  YMD(startYear,1,
-0001d880: 3129 2e61 6476 616e 6365 2873 7461 7274  1).advance(start
-0001d890: 4a75 6c69 616e 2d31 2c27 6461 7927 290d  Julian-1,'day').
-0001d8a0: 0a20 2065 6e64 4461 7465 203d 2065 652e  .  endDate = ee.
-0001d8b0: 4461 7465 2e66 726f 6d59 4d44 2865 6e64  Date.fromYMD(end
+0001d3c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3f0: 2323 2323 2323 0d0a 2357 7261 7070 6572  ######..#Wrapper
+0001d400: 2066 756e 6374 696f 6e20 666f 7220 6765   function for ge
+0001d410: 7474 696e 6720 4c61 6e64 7361 7420 696d  tting Landsat im
+0001d420: 6167 6572 790d 0a64 6566 2067 6574 5072  agery..def getPr
+0001d430: 6f63 6573 7365 644c 616e 6473 6174 5363  ocessedLandsatSc
+0001d440: 656e 6573 280d 0a20 2073 7475 6479 4172  enes(..  studyAr
+0001d450: 6561 2c0d 0a20 2073 7461 7274 5965 6172  ea,..  startYear
+0001d460: 2c0d 0a20 2065 6e64 5965 6172 2c0d 0a20  ,..  endYear,.. 
+0001d470: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
+0001d480: 2065 6e64 4a75 6c69 616e 2c0d 0a20 2074   endJulian,..  t
+0001d490: 6f61 4f72 5352 203d 2027 5352 272c 0d0a  oaOrSR = 'SR',..
+0001d4a0: 2020 696e 636c 7564 6553 4c43 4f66 664c    includeSLCOffL
+0001d4b0: 3720 3d20 4661 6c73 652c 0d0a 2020 6465  7 = False,..  de
+0001d4c0: 6672 696e 6765 4c35 203d 2046 616c 7365  fringeL5 = False
+0001d4d0: 2c0d 0a20 2061 7070 6c79 436c 6f75 6453  ,..  applyCloudS
+0001d4e0: 636f 7265 203d 2046 616c 7365 2c0d 0a20  core = False,.. 
+0001d4f0: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+0001d500: 4d61 736b 203d 2054 7275 652c 0d0a 2020  Mask = True,..  
+0001d510: 6170 706c 7954 444f 4d20 3d20 4661 6c73  applyTDOM = Fals
+0001d520: 652c 0d0a 2020 6170 706c 7946 6d61 736b  e,..  applyFmask
+0001d530: 436c 6f75 6453 6861 646f 774d 6173 6b20  CloudShadowMask 
+0001d540: 3d20 5472 7565 2c0d 0a20 2061 7070 6c79  = True,..  apply
+0001d550: 466d 6173 6b53 6e6f 774d 6173 6b20 3d20  FmaskSnowMask = 
+0001d560: 4661 6c73 652c 0d0a 2020 636c 6f75 6453  False,..  cloudS
+0001d570: 636f 7265 5468 7265 7368 203d 2031 302c  coreThresh = 10,
+0001d580: 0d0a 2020 7065 7266 6f72 6d43 6c6f 7564  ..  performCloud
+0001d590: 5363 6f72 654f 6666 7365 7420 3d20 5472  ScoreOffset = Tr
+0001d5a0: 7565 2c0d 0a20 2063 6c6f 7564 5363 6f72  ue,..  cloudScor
+0001d5b0: 6550 6374 6c20 3d20 3130 2c0d 0a20 207a  ePctl = 10,..  z
+0001d5c0: 5363 6f72 6554 6872 6573 6820 3d20 2d31  ScoreThresh = -1
+0001d5d0: 2c0d 0a20 2073 6861 646f 7753 756d 5468  ,..  shadowSumTh
+0001d5e0: 7265 7368 203d 2030 2e33 352c 0d0a 2020  resh = 0.35,..  
+0001d5f0: 636f 6e74 7261 6374 5069 7865 6c73 203d  contractPixels =
+0001d600: 2031 2e35 2c0d 0a20 2064 696c 6174 6550   1.5,..  dilateP
+0001d610: 6978 656c 7320 3d20 332e 352c 0d0a 2020  ixels = 3.5,..  
+0001d620: 7368 6164 6f77 5375 6d42 616e 6473 203d  shadowSumBands =
+0001d630: 205b 276e 6972 272c 2773 7769 7231 275d   ['nir','swir1']
+0001d640: 2c0d 0a20 2072 6573 616d 706c 654d 6574  ,..  resampleMet
+0001d650: 686f 6420 3d20 276e 6561 7227 2c0d 0a20  hod = 'near',.. 
+0001d660: 2068 6172 6d6f 6e69 7a65 4f4c 4920 3d20   harmonizeOLI = 
+0001d670: 4661 6c73 652c 0d0a 2020 7072 6543 6f6d  False,..  preCom
+0001d680: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
+0001d690: 6666 7365 7420 3d20 4e6f 6e65 2c0d 0a20  ffset = None,.. 
+0001d6a0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
+0001d6b0: 4952 4d65 616e 203d 204e 6f6e 652c 0d0a  IRMean = None,..
+0001d6c0: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
+0001d6d0: 4d49 5253 7464 4465 7620 3d20 4e6f 6e65  MIRStdDev = None
+0001d6e0: 2c0d 0a20 206c 616e 6473 6174 436f 6c6c  ,..  landsatColl
+0001d6f0: 6563 7469 6f6e 5665 7273 696f 6e20 3d20  ectionVersion = 
+0001d700: 2743 3227 2c0d 0a20 2076 6572 626f 7365  'C2',..  verbose
+0001d710: 203d 2046 616c 7365 293a 0d0a 0d0a 2020   = False):....  
+0001d720: 6f72 6967 696e 203d 2027 4c61 6e64 7361  origin = 'Landsa
+0001d730: 7427 0d0a 2020 746f 614f 7253 5220 3d20  t'..  toaOrSR = 
+0001d740: 746f 614f 7253 522e 7570 7065 7228 290d  toaOrSR.upper().
+0001d750: 0a20 2069 6620 746f 614f 7253 522e 6c6f  .  if toaOrSR.lo
+0001d760: 7765 7228 2920 3d3d 2027 746f 6127 2061  wer() == 'toa' a
+0001d770: 6e64 206c 616e 6473 6174 436f 6c6c 6563  nd landsatCollec
+0001d780: 7469 6f6e 5665 7273 696f 6e2e 6c6f 7765  tionVersion.lowe
+0001d790: 7228 2920 3d3d 2027 6331 2720 616e 6420  r() == 'c1' and 
+0001d7a0: 2861 7070 6c79 466d 6173 6b43 6c6f 7564  (applyFmaskCloud
+0001d7b0: 4d61 736b 206f 7220 6170 706c 7946 6d61  Mask or applyFma
+0001d7c0: 736b 436c 6f75 6453 6861 646f 774d 6173  skCloudShadowMas
+0001d7d0: 6b20 206f 7220 6170 706c 7946 6d61 736b  k  or applyFmask
+0001d7e0: 536e 6f77 4d61 736b 2029 3a0d 0a20 2020  SnowMask ):..   
+0001d7f0: 2061 6464 5069 7865 6c51 4120 3d20 5472   addPixelQA = Tr
+0001d800: 7565 0d0a 2020 656c 7365 3a0d 0a20 2020  ue..  else:..   
+0001d810: 2061 6464 5069 7865 6c51 4120 3d20 4661   addPixelQA = Fa
+0001d820: 6c73 650d 0a0d 0a20 2023 5072 6570 6172  lse....  #Prepar
+0001d830: 6520 6461 7465 730d 0a20 2023 5772 6170  e dates..  #Wrap
+0001d840: 2074 6865 2064 6174 6573 2069 6620 6e65   the dates if ne
+0001d850: 6564 6564 0d0a 2020 7772 6170 4f66 6673  eded..  wrapOffs
+0001d860: 6574 203d 2030 0d0a 2020 6966 2073 7461  et = 0..  if sta
+0001d870: 7274 4a75 6c69 616e 203e 2065 6e64 4a75  rtJulian > endJu
+0001d880: 6c69 616e 3a0d 0a20 2020 2077 7261 704f  lian:..    wrapO
+0001d890: 6666 7365 7420 3d20 3336 350d 0a20 2073  ffset = 365..  s
+0001d8a0: 7461 7274 4461 7465 203d 2065 652e 4461  tartDate = ee.Da
+0001d8b0: 7465 2e66 726f 6d59 4d44 2873 7461 7274  te.fromYMD(start
 0001d8c0: 5965 6172 2c31 2c31 292e 6164 7661 6e63  Year,1,1).advanc
-0001d8d0: 6528 656e 644a 756c 6961 6e2d 312b 7772  e(endJulian-1+wr
-0001d8e0: 6170 4f66 6673 6574 2c27 6461 7927 290d  apOffset,'day').
-0001d8f0: 0a0d 0a20 2061 7267 7320 3d20 666f 726d  ...  args = form
-0001d900: 6174 4172 6773 286c 6f63 616c 7328 2929  atArgs(locals())
-0001d910: 0d0a 2020 6966 2027 6172 6773 2720 696e  ..  if 'args' in
-0001d920: 2061 7267 732e 6b65 7973 2829 3a0d 0a20   args.keys():.. 
-0001d930: 2020 2064 656c 2061 7267 735b 2761 7267     del args['arg
-0001d940: 7327 5d0d 0a0d 0a20 2070 7269 6e74 2827  s']....  print('
-0001d950: 4765 7420 5072 6f63 6573 7365 6420 4c61  Get Processed La
-0001d960: 6e64 7361 743a 2027 290d 0a20 2023 2070  ndsat: ')..  # p
-0001d970: 7269 6e74 2827 5374 6172 7420 6461 7465  rint('Start date
-0001d980: 3a27 2c20 7374 6172 7444 6174 652e 666f  :', startDate.fo
-0001d990: 726d 6174 2827 4d4d 4d20 6464 2079 7979  rmat('MMM dd yyy
-0001d9a0: 7927 292e 6765 7449 6e66 6f28 292c 272c  y').getInfo(),',
-0001d9b0: 2045 6e64 2064 6174 653a 272c 2065 6e64   End date:', end
-0001d9c0: 4461 7465 2e66 6f72 6d61 7428 274d 4d4d  Date.format('MMM
-0001d9d0: 2064 6420 7979 7979 2729 2e67 6574 496e   dd yyyy').getIn
-0001d9e0: 666f 2829 290d 0a20 2023 2066 6f72 2061  fo())..  # for a
-0001d9f0: 7267 2069 6e20 6172 6773 2e6b 6579 7328  rg in args.keys(
-0001da00: 293a 0d0a 2020 2320 2020 7072 696e 7428  ):..  #   print(
-0001da10: 6172 672c 2027 3a20 272c 2061 7267 735b  arg, ': ', args[
-0001da20: 6172 675d 290d 0a0d 0a20 2023 4765 7420  arg])....  #Get 
-0001da30: 4c61 6e64 7361 7420 696d 6167 6520 636f  Landsat image co
-0001da40: 6c6c 6563 7469 6f6e 0d0a 2020 6c73 203d  llection..  ls =
-0001da50: 2067 6574 4c61 6e64 7361 7428 5c0d 0a20   getLandsat(\.. 
-0001da60: 2020 2073 7475 6479 4172 6561 203d 2073     studyArea = s
-0001da70: 7475 6479 4172 6561 2c0d 0a20 2020 2073  tudyArea,..    s
-0001da80: 7461 7274 4461 7465 203d 2073 7461 7274  tartDate = start
-0001da90: 4461 7465 2c0d 0a20 2020 2065 6e64 4461  Date,..    endDa
-0001daa0: 7465 203d 2065 6e64 4461 7465 2c0d 0a20  te = endDate,.. 
-0001dab0: 2020 2073 7461 7274 4a75 6c69 616e 203d     startJulian =
-0001dac0: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
-0001dad0: 2020 2065 6e64 4a75 6c69 616e 203d 2065     endJulian = e
-0001dae0: 6e64 4a75 6c69 616e 2c0d 0a20 2020 2074  ndJulian,..    t
-0001daf0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
-0001db00: 2c0d 0a20 2020 2069 6e63 6c75 6465 534c  ,..    includeSL
-0001db10: 434f 6666 4c37 203d 2069 6e63 6c75 6465  COffL7 = include
-0001db20: 534c 434f 6666 4c37 2c0d 0a20 2020 2064  SLCOffL7,..    d
-0001db30: 6566 7269 6e67 654c 3520 3d20 6465 6672  efringeL5 = defr
-0001db40: 696e 6765 4c35 2c0d 0a20 2020 2061 6464  ingeL5,..    add
-0001db50: 5069 7865 6c51 4120 3d20 6164 6450 6978  PixelQA = addPix
-0001db60: 656c 5141 2c0d 0a20 2020 2072 6573 616d  elQA,..    resam
-0001db70: 706c 654d 6574 686f 6420 3d20 7265 7361  pleMethod = resa
-0001db80: 6d70 6c65 4d65 7468 6f64 2c0d 0a20 2020  mpleMethod,..   
-0001db90: 206c 616e 6473 6174 436f 6c6c 6563 7469   landsatCollecti
-0001dba0: 6f6e 5665 7273 696f 6e20 3d20 6c61 6e64  onVersion = land
-0001dbb0: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
-0001dbc0: 7369 6f6e 290d 0a0d 0a20 2023 4170 706c  sion)....  #Appl
-0001dbd0: 7920 7265 6c65 7661 6e74 2063 6c6f 7564  y relevant cloud
-0001dbe0: 206d 6173 6b69 6e67 206d 6574 686f 6473   masking methods
-0001dbf0: 0d0a 2020 6966 2061 7070 6c79 436c 6f75  ..  if applyClou
-0001dc00: 6453 636f 7265 3a0d 0a20 2020 2070 7269  dScore:..    pri
-0001dc10: 6e74 2827 4170 706c 7969 6e67 2043 6c6f  nt('Applying Clo
-0001dc20: 7564 2053 636f 7265 2729 0d0a 2020 2020  ud Score')..    
-0001dc30: 6c73 203d 2061 7070 6c79 436c 6f75 6453  ls = applyCloudS
-0001dc40: 636f 7265 416c 676f 7269 7468 6d28 5c0d  coreAlgorithm(\.
-0001dc50: 0a20 2020 2020 2063 6f6c 6c65 6374 696f  .      collectio
-0001dc60: 6e20 3d20 6c73 2c0d 0a20 2020 2020 2063  n = ls,..      c
-0001dc70: 6c6f 7564 5363 6f72 6546 756e 6374 696f  loudScoreFunctio
-0001dc80: 6e20 3d20 6c61 6e64 7361 7443 6c6f 7564  n = landsatCloud
-0001dc90: 5363 6f72 652c 0d0a 2020 2020 2020 636c  Score,..      cl
-0001dca0: 6f75 6453 636f 7265 5468 7265 7368 203d  oudScoreThresh =
-0001dcb0: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
-0001dcc0: 682c 0d0a 2020 2020 2020 636c 6f75 6453  h,..      cloudS
-0001dcd0: 636f 7265 5063 746c 203d 2063 6c6f 7564  corePctl = cloud
-0001dce0: 5363 6f72 6550 6374 6c2c 0d0a 2020 2020  ScorePctl,..    
-0001dcf0: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
-0001dd00: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
-0001dd10: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
-0001dd20: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
-0001dd30: 6978 656c 732c 0d0a 2020 2020 2020 7065  ixels,..      pe
-0001dd40: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
-0001dd50: 6666 7365 7420 3d20 7065 7266 6f72 6d43  ffset = performC
-0001dd60: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
-0001dd70: 0d0a 2020 2020 2020 7072 6543 6f6d 7075  ..      preCompu
-0001dd80: 7465 6443 6c6f 7564 5363 6f72 654f 6666  tedCloudScoreOff
-0001dd90: 7365 7420 3d20 7072 6543 6f6d 7075 7465  set = preCompute
-0001dda0: 6443 6c6f 7564 5363 6f72 654f 6666 7365  dCloudScoreOffse
-0001ddb0: 7429 0d0a 0d0a 2020 6966 2061 7070 6c79  t)....  if apply
-0001ddc0: 466d 6173 6b43 6c6f 7564 4d61 736b 3a0d  FmaskCloudMask:.
-0001ddd0: 0a20 2020 2070 7269 6e74 2827 4170 706c  .    print('Appl
-0001dde0: 7969 6e67 2046 6d61 736b 2043 6c6f 7564  ying Fmask Cloud
-0001ddf0: 204d 6173 6b27 290d 0a20 2020 206c 7320   Mask')..    ls 
-0001de00: 3d20 6c73 2e6d 6170 286c 616d 6264 6120  = ls.map(lambda 
-0001de10: 696d 673a 2061 7070 6c79 4269 744d 6173  img: applyBitMas
-0001de20: 6b28 696d 672c 666d 6173 6b42 6974 4469  k(img,fmaskBitDi
-0001de30: 6374 5b6c 616e 6473 6174 436f 6c6c 6563  ct[landsatCollec
-0001de40: 7469 6f6e 5665 7273 696f 6e5d 5b27 636c  tionVersion]['cl
-0001de50: 6f75 6427 5d2c 6c61 6e64 7361 7446 6d61  oud'],landsatFma
-0001de60: 736b 4261 6e64 4e61 6d65 4469 6374 5b6c  skBandNameDict[l
-0001de70: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
-0001de80: 5665 7273 696f 6e5d 2929 0d0a 0d0a 2020  Version]))....  
-0001de90: 6966 2061 7070 6c79 5444 4f4d 3a0d 0a20  if applyTDOM:.. 
-0001dea0: 2020 2070 7269 6e74 2827 4170 706c 7969     print('Applyi
-0001deb0: 6e67 2054 444f 4d20 5368 6164 6f77 204d  ng TDOM Shadow M
-0001dec0: 6173 6b27 290d 0a20 2020 206c 7320 3d20  ask')..    ls = 
-0001ded0: 7369 6d70 6c65 5444 4f4d 3228 5c0d 0a20  simpleTDOM2(\.. 
-0001dee0: 2020 2020 2063 6f6c 6c65 6374 696f 6e20       collection 
-0001def0: 3d20 6c73 2c0d 0a20 2020 2020 207a 5363  = ls,..      zSc
-0001df00: 6f72 6554 6872 6573 6820 3d20 7a53 636f  oreThresh = zSco
-0001df10: 7265 5468 7265 7368 2c0d 0a20 2020 2020  reThresh,..     
-0001df20: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
-0001df30: 203d 2073 6861 646f 7753 756d 5468 7265   = shadowSumThre
-0001df40: 7368 2c0d 0a20 2020 2020 2063 6f6e 7472  sh,..      contr
-0001df50: 6163 7450 6978 656c 7320 3d20 636f 6e74  actPixels = cont
-0001df60: 7261 6374 5069 7865 6c73 2c0d 0a20 2020  ractPixels,..   
-0001df70: 2020 2064 696c 6174 6550 6978 656c 7320     dilatePixels 
-0001df80: 3d20 6469 6c61 7465 5069 7865 6c73 2c0d  = dilatePixels,.
-0001df90: 0a20 2020 2020 2073 6861 646f 7753 756d  .      shadowSum
-0001dfa0: 4261 6e64 7320 3d20 5b27 6e69 7227 2c27  Bands = ['nir','
-0001dfb0: 7377 6972 3127 5d2c 0d0a 2020 2020 2020  swir1'],..      
-0001dfc0: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
-0001dfd0: 524d 6561 6e20 3d20 7072 6543 6f6d 7075  RMean = preCompu
-0001dfe0: 7465 6454 444f 4d49 524d 6561 6e2c 0d0a  tedTDOMIRMean,..
-0001dff0: 2020 2020 2020 7072 6543 6f6d 7075 7465        preCompute
-0001e000: 6454 444f 4d49 5253 7464 4465 7620 3d20  dTDOMIRStdDev = 
-0001e010: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
-0001e020: 5253 7464 4465 7629 0d0a 0d0a 2020 6966  RStdDev)....  if
-0001e030: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
-0001e040: 5368 6164 6f77 4d61 736b 3a0d 0a20 2020  ShadowMask:..   
-0001e050: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
-0001e060: 2046 6d61 736b 2053 6861 646f 7720 4d61   Fmask Shadow Ma
-0001e070: 736b 2729 0d0a 2020 2020 6c73 203d 206c  sk')..    ls = l
-0001e080: 732e 6d61 7028 6c61 6d62 6461 2069 6d67  s.map(lambda img
-0001e090: 3a20 6170 706c 7942 6974 4d61 736b 2869  : applyBitMask(i
-0001e0a0: 6d67 2c66 6d61 736b 4269 7444 6963 745b  mg,fmaskBitDict[
-0001e0b0: 6c61 6e64 7361 7443 6f6c 6c65 6374 696f  landsatCollectio
-0001e0c0: 6e56 6572 7369 6f6e 5d5b 2773 6861 646f  nVersion]['shado
-0001e0d0: 7727 5d2c 6c61 6e64 7361 7446 6d61 736b  w'],landsatFmask
-0001e0e0: 4261 6e64 4e61 6d65 4469 6374 5b6c 616e  BandNameDict[lan
-0001e0f0: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
-0001e100: 7273 696f 6e5d 2929 0d0a 0d0a 0d0a 2020  rsion]))......  
-0001e110: 6966 2061 7070 6c79 466d 6173 6b53 6e6f  if applyFmaskSno
-0001e120: 774d 6173 6b3a 0d0a 2020 2020 7072 696e  wMask:..    prin
-0001e130: 7428 2741 7070 6c79 696e 6720 466d 6173  t('Applying Fmas
-0001e140: 6b20 736e 6f77 206d 6173 6b27 290d 0a20  k snow mask').. 
-0001e150: 2020 206c 7320 3d20 6c73 2e6d 6170 286c     ls = ls.map(l
-0001e160: 616d 6264 6120 696d 673a 2061 7070 6c79  ambda img: apply
-0001e170: 4269 744d 6173 6b28 696d 672c 666d 6173  BitMask(img,fmas
-0001e180: 6b42 6974 4469 6374 5b6c 616e 6473 6174  kBitDict[landsat
-0001e190: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
-0001e1a0: 6e5d 5b27 736e 6f77 275d 2c6c 616e 6473  n]['snow'],lands
-0001e1b0: 6174 466d 6173 6b42 616e 644e 616d 6544  atFmaskBandNameD
-0001e1c0: 6963 745b 6c61 6e64 7361 7443 6f6c 6c65  ict[landsatColle
-0001e1d0: 6374 696f 6e56 6572 7369 6f6e 5d29 290d  ctionVersion])).
-0001e1e0: 0a0d 0a0d 0a20 2023 2041 6464 2063 6f6d  .....  # Add com
-0001e1f0: 6d6f 6e20 696e 6469 6365 730d 0a20 206c  mon indices..  l
-0001e200: 7320 3d20 6c73 2e6d 6170 2873 696d 706c  s = ls.map(simpl
-0001e210: 6541 6464 496e 6469 6365 7329 5c0d 0a20  eAddIndices)\.. 
-0001e220: 2020 2020 2020 2020 202e 6d61 7028 6765           .map(ge
-0001e230: 7454 6173 7365 6c65 6443 6170 295c 0d0a  tTasseledCap)\..
-0001e240: 2020 2020 2020 2020 2020 2e6d 6170 2873            .map(s
-0001e250: 696d 706c 6541 6464 5443 416e 676c 6573  impleAddTCAngles
-0001e260: 290d 0a0d 0a20 2023 2041 6464 2053 656e  )....  # Add Sen
-0001e270: 736f 7220 4261 6e64 0d0a 2020 6c73 203d  sor Band..  ls =
-0001e280: 206c 732e 6d61 7028 6c61 6d62 6461 2069   ls.map(lambda i
-0001e290: 6d67 3a20 6164 6453 656e 736f 7242 616e  mg: addSensorBan
-0001e2a0: 6428 696d 672c 206c 616e 6473 6174 436f  d(img, landsatCo
-0001e2b0: 6c6c 6563 7469 6f6e 5665 7273 696f 6e2b  llectionVersion+
-0001e2c0: 275f 6c61 6e64 7361 7427 2c20 746f 614f  '_landsat', toaO
-0001e2d0: 7253 5229 290d 0a0d 0a20 2072 6574 7572  rSR))....  retur
-0001e2e0: 6e20 6c73 2e73 6574 2861 7267 7329 0d0a  n ls.set(args)..
-0001e2f0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-0001e300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e330: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
-0001e340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d8d0: 6528 7374 6172 744a 756c 6961 6e2d 312c  e(startJulian-1,
+0001d8e0: 2764 6179 2729 0d0a 2020 656e 6444 6174  'day')..  endDat
+0001d8f0: 6520 3d20 6565 2e44 6174 652e 6672 6f6d  e = ee.Date.from
+0001d900: 594d 4428 656e 6459 6561 722c 312c 3129  YMD(endYear,1,1)
+0001d910: 2e61 6476 616e 6365 2865 6e64 4a75 6c69  .advance(endJuli
+0001d920: 616e 2d31 2b77 7261 704f 6666 7365 742c  an-1+wrapOffset,
+0001d930: 2764 6179 2729 0d0a 0d0a 2020 6172 6773  'day')....  args
+0001d940: 203d 2066 6f72 6d61 7441 7267 7328 6c6f   = formatArgs(lo
+0001d950: 6361 6c73 2829 290d 0a20 2069 6620 2761  cals())..  if 'a
+0001d960: 7267 7327 2069 6e20 6172 6773 2e6b 6579  rgs' in args.key
+0001d970: 7328 293a 0d0a 2020 2020 6465 6c20 6172  s():..    del ar
+0001d980: 6773 5b27 6172 6773 275d 0d0a 0d0a 2020  gs['args']....  
+0001d990: 7072 696e 7428 2747 6574 2050 726f 6365  print('Get Proce
+0001d9a0: 7373 6564 204c 616e 6473 6174 3a20 2729  ssed Landsat: ')
+0001d9b0: 0d0a 2020 7072 696e 7428 2753 7461 7274  ..  print('Start
+0001d9c0: 2064 6174 653a 272c 2073 7461 7274 4461   date:', startDa
+0001d9d0: 7465 2e66 6f72 6d61 7428 274d 4d4d 2064  te.format('MMM d
+0001d9e0: 6420 7979 7979 2729 2e67 6574 496e 666f  d yyyy').getInfo
+0001d9f0: 2829 2c27 2c20 456e 6420 6461 7465 3a27  (),', End date:'
+0001da00: 2c20 656e 6444 6174 652e 666f 726d 6174  , endDate.format
+0001da10: 2827 4d4d 4d20 6464 2079 7979 7927 292e  ('MMM dd yyyy').
+0001da20: 6765 7449 6e66 6f28 2929 0d0a 2020 6966  getInfo())..  if
+0001da30: 2076 6572 626f 7365 3a0d 0a20 2020 2066   verbose:..    f
+0001da40: 6f72 2061 7267 2069 6e20 6172 6773 2e6b  or arg in args.k
+0001da50: 6579 7328 293a 0d0a 2020 2020 2020 7072  eys():..      pr
+0001da60: 696e 7428 6172 672c 2027 3a20 272c 2061  int(arg, ': ', a
+0001da70: 7267 735b 6172 675d 290d 0a0d 0a20 2023  rgs[arg])....  #
+0001da80: 4765 7420 4c61 6e64 7361 7420 696d 6167  Get Landsat imag
+0001da90: 6520 636f 6c6c 6563 7469 6f6e 0d0a 2020  e collection..  
+0001daa0: 6c73 203d 2067 6574 4c61 6e64 7361 7428  ls = getLandsat(
+0001dab0: 5c0d 0a20 2020 2073 7475 6479 4172 6561  \..    studyArea
+0001dac0: 203d 2073 7475 6479 4172 6561 2c0d 0a20   = studyArea,.. 
+0001dad0: 2020 2073 7461 7274 4461 7465 203d 2073     startDate = s
+0001dae0: 7461 7274 4461 7465 2c0d 0a20 2020 2065  tartDate,..    e
+0001daf0: 6e64 4461 7465 203d 2065 6e64 4461 7465  ndDate = endDate
+0001db00: 2c0d 0a20 2020 2073 7461 7274 4a75 6c69  ,..    startJuli
+0001db10: 616e 203d 2073 7461 7274 4a75 6c69 616e  an = startJulian
+0001db20: 2c0d 0a20 2020 2065 6e64 4a75 6c69 616e  ,..    endJulian
+0001db30: 203d 2065 6e64 4a75 6c69 616e 2c0d 0a20   = endJulian,.. 
+0001db40: 2020 2074 6f61 4f72 5352 203d 2074 6f61     toaOrSR = toa
+0001db50: 4f72 5352 2c0d 0a20 2020 2069 6e63 6c75  OrSR,..    inclu
+0001db60: 6465 534c 434f 6666 4c37 203d 2069 6e63  deSLCOffL7 = inc
+0001db70: 6c75 6465 534c 434f 6666 4c37 2c0d 0a20  ludeSLCOffL7,.. 
+0001db80: 2020 2064 6566 7269 6e67 654c 3520 3d20     defringeL5 = 
+0001db90: 6465 6672 696e 6765 4c35 2c0d 0a20 2020  defringeL5,..   
+0001dba0: 2061 6464 5069 7865 6c51 4120 3d20 6164   addPixelQA = ad
+0001dbb0: 6450 6978 656c 5141 2c0d 0a20 2020 2072  dPixelQA,..    r
+0001dbc0: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+0001dbd0: 7265 7361 6d70 6c65 4d65 7468 6f64 2c0d  resampleMethod,.
+0001dbe0: 0a20 2020 206c 616e 6473 6174 436f 6c6c  .    landsatColl
+0001dbf0: 6563 7469 6f6e 5665 7273 696f 6e20 3d20  ectionVersion = 
+0001dc00: 6c61 6e64 7361 7443 6f6c 6c65 6374 696f  landsatCollectio
+0001dc10: 6e56 6572 7369 6f6e 290d 0a0d 0a20 2023  nVersion)....  #
+0001dc20: 4170 706c 7920 7265 6c65 7661 6e74 2063  Apply relevant c
+0001dc30: 6c6f 7564 206d 6173 6b69 6e67 206d 6574  loud masking met
+0001dc40: 686f 6473 0d0a 2020 6966 2061 7070 6c79  hods..  if apply
+0001dc50: 436c 6f75 6453 636f 7265 3a0d 0a20 2020  CloudScore:..   
+0001dc60: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
+0001dc70: 2043 6c6f 7564 2053 636f 7265 2729 0d0a   Cloud Score')..
+0001dc80: 2020 2020 6c73 203d 2061 7070 6c79 436c      ls = applyCl
+0001dc90: 6f75 6453 636f 7265 416c 676f 7269 7468  oudScoreAlgorith
+0001dca0: 6d28 5c0d 0a20 2020 2020 2063 6f6c 6c65  m(\..      colle
+0001dcb0: 6374 696f 6e20 3d20 6c73 2c0d 0a20 2020  ction = ls,..   
+0001dcc0: 2020 2063 6c6f 7564 5363 6f72 6546 756e     cloudScoreFun
+0001dcd0: 6374 696f 6e20 3d20 6c61 6e64 7361 7443  ction = landsatC
+0001dce0: 6c6f 7564 5363 6f72 652c 0d0a 2020 2020  loudScore,..    
+0001dcf0: 2020 636c 6f75 6453 636f 7265 5468 7265    cloudScoreThre
+0001dd00: 7368 203d 2063 6c6f 7564 5363 6f72 6554  sh = cloudScoreT
+0001dd10: 6872 6573 682c 0d0a 2020 2020 2020 636c  hresh,..      cl
+0001dd20: 6f75 6453 636f 7265 5063 746c 203d 2063  oudScorePctl = c
+0001dd30: 6c6f 7564 5363 6f72 6550 6374 6c2c 0d0a  loudScorePctl,..
+0001dd40: 2020 2020 2020 636f 6e74 7261 6374 5069        contractPi
+0001dd50: 7865 6c73 203d 2063 6f6e 7472 6163 7450  xels = contractP
+0001dd60: 6978 656c 732c 0d0a 2020 2020 2020 6469  ixels,..      di
+0001dd70: 6c61 7465 5069 7865 6c73 203d 2064 696c  latePixels = dil
+0001dd80: 6174 6550 6978 656c 732c 0d0a 2020 2020  atePixels,..    
+0001dd90: 2020 7065 7266 6f72 6d43 6c6f 7564 5363    performCloudSc
+0001dda0: 6f72 654f 6666 7365 7420 3d20 7065 7266  oreOffset = perf
+0001ddb0: 6f72 6d43 6c6f 7564 5363 6f72 654f 6666  ormCloudScoreOff
+0001ddc0: 7365 742c 0d0a 2020 2020 2020 7072 6543  set,..      preC
+0001ddd0: 6f6d 7075 7465 6443 6c6f 7564 5363 6f72  omputedCloudScor
+0001dde0: 654f 6666 7365 7420 3d20 7072 6543 6f6d  eOffset = preCom
+0001ddf0: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
+0001de00: 6666 7365 7429 0d0a 0d0a 2020 6966 2061  ffset)....  if a
+0001de10: 7070 6c79 466d 6173 6b43 6c6f 7564 4d61  pplyFmaskCloudMa
+0001de20: 736b 3a0d 0a20 2020 2070 7269 6e74 2827  sk:..    print('
+0001de30: 4170 706c 7969 6e67 2046 6d61 736b 2043  Applying Fmask C
+0001de40: 6c6f 7564 204d 6173 6b27 290d 0a20 2020  loud Mask')..   
+0001de50: 206c 7320 3d20 6c73 2e6d 6170 286c 616d   ls = ls.map(lam
+0001de60: 6264 6120 696d 673a 2061 7070 6c79 4269  bda img: applyBi
+0001de70: 744d 6173 6b28 696d 672c 666d 6173 6b42  tMask(img,fmaskB
+0001de80: 6974 4469 6374 5b6c 616e 6473 6174 436f  itDict[landsatCo
+0001de90: 6c6c 6563 7469 6f6e 5665 7273 696f 6e5d  llectionVersion]
+0001dea0: 5b27 636c 6f75 6427 5d2c 6c61 6e64 7361  ['cloud'],landsa
+0001deb0: 7446 6d61 736b 4261 6e64 4e61 6d65 4469  tFmaskBandNameDi
+0001dec0: 6374 5b6c 616e 6473 6174 436f 6c6c 6563  ct[landsatCollec
+0001ded0: 7469 6f6e 5665 7273 696f 6e5d 2929 0d0a  tionVersion]))..
+0001dee0: 0d0a 2020 6966 2061 7070 6c79 5444 4f4d  ..  if applyTDOM
+0001def0: 3a0d 0a20 2020 2070 7269 6e74 2827 4170  :..    print('Ap
+0001df00: 706c 7969 6e67 2054 444f 4d20 5368 6164  plying TDOM Shad
+0001df10: 6f77 204d 6173 6b27 290d 0a20 2020 206c  ow Mask')..    l
+0001df20: 7320 3d20 7369 6d70 6c65 5444 4f4d 3228  s = simpleTDOM2(
+0001df30: 5c0d 0a20 2020 2020 2063 6f6c 6c65 6374  \..      collect
+0001df40: 696f 6e20 3d20 6c73 2c0d 0a20 2020 2020  ion = ls,..     
+0001df50: 207a 5363 6f72 6554 6872 6573 6820 3d20   zScoreThresh = 
+0001df60: 7a53 636f 7265 5468 7265 7368 2c0d 0a20  zScoreThresh,.. 
+0001df70: 2020 2020 2073 6861 646f 7753 756d 5468       shadowSumTh
+0001df80: 7265 7368 203d 2073 6861 646f 7753 756d  resh = shadowSum
+0001df90: 5468 7265 7368 2c0d 0a20 2020 2020 2063  Thresh,..      c
+0001dfa0: 6f6e 7472 6163 7450 6978 656c 7320 3d20  ontractPixels = 
+0001dfb0: 636f 6e74 7261 6374 5069 7865 6c73 2c0d  contractPixels,.
+0001dfc0: 0a20 2020 2020 2064 696c 6174 6550 6978  .      dilatePix
+0001dfd0: 656c 7320 3d20 6469 6c61 7465 5069 7865  els = dilatePixe
+0001dfe0: 6c73 2c0d 0a20 2020 2020 2073 6861 646f  ls,..      shado
+0001dff0: 7753 756d 4261 6e64 7320 3d20 5b27 6e69  wSumBands = ['ni
+0001e000: 7227 2c27 7377 6972 3127 5d2c 0d0a 2020  r','swir1'],..  
+0001e010: 2020 2020 7072 6543 6f6d 7075 7465 6454      preComputedT
+0001e020: 444f 4d49 524d 6561 6e20 3d20 7072 6543  DOMIRMean = preC
+0001e030: 6f6d 7075 7465 6454 444f 4d49 524d 6561  omputedTDOMIRMea
+0001e040: 6e2c 0d0a 2020 2020 2020 7072 6543 6f6d  n,..      preCom
+0001e050: 7075 7465 6454 444f 4d49 5253 7464 4465  putedTDOMIRStdDe
+0001e060: 7620 3d20 7072 6543 6f6d 7075 7465 6454  v = preComputedT
+0001e070: 444f 4d49 5253 7464 4465 7629 0d0a 0d0a  DOMIRStdDev)....
+0001e080: 2020 6966 2061 7070 6c79 466d 6173 6b43    if applyFmaskC
+0001e090: 6c6f 7564 5368 6164 6f77 4d61 736b 3a0d  loudShadowMask:.
+0001e0a0: 0a20 2020 2070 7269 6e74 2827 4170 706c  .    print('Appl
+0001e0b0: 7969 6e67 2046 6d61 736b 2053 6861 646f  ying Fmask Shado
+0001e0c0: 7720 4d61 736b 2729 0d0a 2020 2020 6c73  w Mask')..    ls
+0001e0d0: 203d 206c 732e 6d61 7028 6c61 6d62 6461   = ls.map(lambda
+0001e0e0: 2069 6d67 3a20 6170 706c 7942 6974 4d61   img: applyBitMa
+0001e0f0: 736b 2869 6d67 2c66 6d61 736b 4269 7444  sk(img,fmaskBitD
+0001e100: 6963 745b 6c61 6e64 7361 7443 6f6c 6c65  ict[landsatColle
+0001e110: 6374 696f 6e56 6572 7369 6f6e 5d5b 2773  ctionVersion]['s
+0001e120: 6861 646f 7727 5d2c 6c61 6e64 7361 7446  hadow'],landsatF
+0001e130: 6d61 736b 4261 6e64 4e61 6d65 4469 6374  maskBandNameDict
+0001e140: 5b6c 616e 6473 6174 436f 6c6c 6563 7469  [landsatCollecti
+0001e150: 6f6e 5665 7273 696f 6e5d 2929 0d0a 0d0a  onVersion]))....
+0001e160: 0d0a 2020 6966 2061 7070 6c79 466d 6173  ..  if applyFmas
+0001e170: 6b53 6e6f 774d 6173 6b3a 0d0a 2020 2020  kSnowMask:..    
+0001e180: 7072 696e 7428 2741 7070 6c79 696e 6720  print('Applying 
+0001e190: 466d 6173 6b20 736e 6f77 206d 6173 6b27  Fmask snow mask'
+0001e1a0: 290d 0a20 2020 206c 7320 3d20 6c73 2e6d  )..    ls = ls.m
+0001e1b0: 6170 286c 616d 6264 6120 696d 673a 2061  ap(lambda img: a
+0001e1c0: 7070 6c79 4269 744d 6173 6b28 696d 672c  pplyBitMask(img,
+0001e1d0: 666d 6173 6b42 6974 4469 6374 5b6c 616e  fmaskBitDict[lan
+0001e1e0: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
+0001e1f0: 7273 696f 6e5d 5b27 736e 6f77 275d 2c6c  rsion]['snow'],l
+0001e200: 616e 6473 6174 466d 6173 6b42 616e 644e  andsatFmaskBandN
+0001e210: 616d 6544 6963 745b 6c61 6e64 7361 7443  ameDict[landsatC
+0001e220: 6f6c 6c65 6374 696f 6e56 6572 7369 6f6e  ollectionVersion
+0001e230: 5d29 290d 0a0d 0a0d 0a20 2023 2041 6464  ]))......  # Add
+0001e240: 2063 6f6d 6d6f 6e20 696e 6469 6365 730d   common indices.
+0001e250: 0a20 206c 7320 3d20 6c73 2e6d 6170 2873  .  ls = ls.map(s
+0001e260: 696d 706c 6541 6464 496e 6469 6365 7329  impleAddIndices)
+0001e270: 5c0d 0a20 2020 2020 2020 2020 202e 6d61  \..          .ma
+0001e280: 7028 6765 7454 6173 7365 6c65 6443 6170  p(getTasseledCap
+0001e290: 295c 0d0a 2020 2020 2020 2020 2020 2e6d  )\..          .m
+0001e2a0: 6170 2873 696d 706c 6541 6464 5443 416e  ap(simpleAddTCAn
+0001e2b0: 676c 6573 290d 0a0d 0a20 2023 2041 6464  gles)....  # Add
+0001e2c0: 2053 656e 736f 7220 4261 6e64 0d0a 2020   Sensor Band..  
+0001e2d0: 6c73 203d 206c 732e 6d61 7028 6c61 6d62  ls = ls.map(lamb
+0001e2e0: 6461 2069 6d67 3a20 6164 6453 656e 736f  da img: addSenso
+0001e2f0: 7242 616e 6428 696d 672c 206c 616e 6473  rBand(img, lands
+0001e300: 6174 436f 6c6c 6563 7469 6f6e 5665 7273  atCollectionVers
+0001e310: 696f 6e2b 275f 6c61 6e64 7361 7427 2c20  ion+'_landsat', 
+0001e320: 746f 614f 7253 5229 290d 0a0d 0a20 2072  toaOrSR))....  r
+0001e330: 6574 7572 6e20 6c73 2e73 6574 2861 7267  eturn ls.set(arg
+0001e340: 7329 0d0a 0d0a 2323 2323 2323 2323 2323  s)....##########
 0001e350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e380: 2323 2323 2323 0d0a 2357 7261 7070 6572  ######..#Wrapper
-0001e390: 2066 756e 6374 696f 6e20 666f 7220 6765   function for ge
-0001e3a0: 7474 696e 6720 5365 6e74 696e 656c 3220  tting Sentinel2 
-0001e3b0: 696d 6167 6572 790d 0a64 6566 2067 6574  imagery..def get
-0001e3c0: 5072 6f63 6573 7365 6453 656e 7469 6e65  ProcessedSentine
-0001e3d0: 6c32 5363 656e 6573 285c 0d0a 2020 7374  l2Scenes(\..  st
-0001e3e0: 7564 7941 7265 612c 0d0a 2020 7374 6172  udyArea,..  star
-0001e3f0: 7459 6561 722c 0d0a 2020 656e 6459 6561  tYear,..  endYea
-0001e400: 722c 0d0a 2020 7374 6172 744a 756c 6961  r,..  startJulia
-0001e410: 6e2c 0d0a 2020 656e 644a 756c 6961 6e2c  n,..  endJulian,
-0001e420: 0d0a 2020 6170 706c 7951 4142 616e 6420  ..  applyQABand 
-0001e430: 3d20 4661 6c73 652c 0d0a 2020 6170 706c  = False,..  appl
-0001e440: 7943 6c6f 7564 5363 6f72 6520 3d20 4661  yCloudScore = Fa
-0001e450: 6c73 652c 0d0a 2020 6170 706c 7953 6861  lse,..  applySha
-0001e460: 646f 7753 6869 6674 203d 2046 616c 7365  dowShift = False
-0001e470: 2c0d 0a20 2061 7070 6c79 5444 4f4d 203d  ,..  applyTDOM =
-0001e480: 2054 7275 652c 0d0a 2020 636c 6f75 6453   True,..  cloudS
-0001e490: 636f 7265 5468 7265 7368 203d 2032 302c  coreThresh = 20,
-0001e4a0: 0d0a 2020 7065 7266 6f72 6d43 6c6f 7564  ..  performCloud
-0001e4b0: 5363 6f72 654f 6666 7365 7420 3d20 5472  ScoreOffset = Tr
-0001e4c0: 7565 2c0d 0a20 2063 6c6f 7564 5363 6f72  ue,..  cloudScor
-0001e4d0: 6550 6374 6c20 3d20 3130 2c0d 0a20 2063  ePctl = 10,..  c
-0001e4e0: 6c6f 7564 4865 6967 6874 7320 3d20 6565  loudHeights = ee
-0001e4f0: 2e4c 6973 742e 7365 7175 656e 6365 2835  .List.sequence(5
-0001e500: 3030 2c31 3030 3030 2c35 3030 292c 0d0a  00,10000,500),..
-0001e510: 2020 7a53 636f 7265 5468 7265 7368 203d    zScoreThresh =
-0001e520: 202d 312c 0d0a 2020 7368 6164 6f77 5375   -1,..  shadowSu
-0001e530: 6d54 6872 6573 6820 3d20 302e 3335 2c0d  mThresh = 0.35,.
-0001e540: 0a20 2063 6f6e 7472 6163 7450 6978 656c  .  contractPixel
-0001e550: 7320 3d20 312e 352c 0d0a 2020 6469 6c61  s = 1.5,..  dila
-0001e560: 7465 5069 7865 6c73 203d 2033 2e35 2c0d  tePixels = 3.5,.
-0001e570: 0a20 2073 6861 646f 7753 756d 4261 6e64  .  shadowSumBand
-0001e580: 7320 3d20 5b27 6e69 7227 2c27 7377 6972  s = ['nir','swir
-0001e590: 3127 5d2c 0d0a 2020 7265 7361 6d70 6c65  1'],..  resample
-0001e5a0: 4d65 7468 6f64 203d 2027 6167 6772 6567  Method = 'aggreg
-0001e5b0: 6174 6527 2c0d 0a20 2074 6f61 4f72 5352  ate',..  toaOrSR
-0001e5c0: 203d 2027 544f 4127 2c0d 0a20 2063 6f6e   = 'TOA',..  con
-0001e5d0: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
-0001e5e0: 6373 203d 2054 7275 652c 0d0a 2020 6170  cs = True,..  ap
-0001e5f0: 706c 7943 6c6f 7564 5072 6f62 6162 696c  plyCloudProbabil
-0001e600: 6974 7920 3d20 5472 7565 2c0d 0a20 2070  ity = True,..  p
-0001e610: 7265 436f 6d70 7574 6564 436c 6f75 6453  reComputedCloudS
-0001e620: 636f 7265 4f66 6673 6574 203d 204e 6f6e  coreOffset = Non
-0001e630: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
-0001e640: 6454 444f 4d49 524d 6561 6e20 3d20 4e6f  dTDOMIRMean = No
-0001e650: 6e65 2c0d 0a20 2070 7265 436f 6d70 7574  ne,..  preComput
-0001e660: 6564 5444 4f4d 4952 5374 6444 6576 203d  edTDOMIRStdDev =
-0001e670: 204e 6f6e 652c 0d0a 2020 636c 6f75 6450   None,..  cloudP
-0001e680: 726f 6254 6872 6573 6820 3d20 3430 293a  robThresh = 40):
-0001e690: 0d0a 0d0a 2020 6f72 6967 696e 203d 2027  ....  origin = '
-0001e6a0: 5365 6e74 696e 656c 3227 0d0a 2020 746f  Sentinel2'..  to
-0001e6b0: 614f 7253 5220 3d20 746f 614f 7253 522e  aOrSR = toaOrSR.
-0001e6c0: 7570 7065 7228 290d 0a0d 0a20 2023 5072  upper()....  #Pr
-0001e6d0: 6570 6172 6520 6461 7465 730d 0a20 2023  epare dates..  #
-0001e6e0: 5772 6170 2074 6865 2064 6174 6573 2069  Wrap the dates i
-0001e6f0: 6620 6e65 6564 6564 0d0a 2020 7772 6170  f needed..  wrap
-0001e700: 4f66 6673 6574 203d 2030 0d0a 2020 6966  Offset = 0..  if
-0001e710: 2073 7461 7274 4a75 6c69 616e 203e 2065   startJulian > e
-0001e720: 6e64 4a75 6c69 616e 3a0d 0a20 2020 2077  ndJulian:..    w
-0001e730: 7261 704f 6666 7365 7420 3d20 3336 350d  rapOffset = 365.
-0001e740: 0a20 2073 7461 7274 4461 7465 203d 2065  .  startDate = e
-0001e750: 652e 4461 7465 2e66 726f 6d59 4d44 2873  e.Date.fromYMD(s
-0001e760: 7461 7274 5965 6172 2c31 2c31 292e 6164  tartYear,1,1).ad
-0001e770: 7661 6e63 6528 7374 6172 744a 756c 6961  vance(startJulia
-0001e780: 6e2d 312c 2764 6179 2729 0d0a 2020 656e  n-1,'day')..  en
-0001e790: 6444 6174 6520 3d20 6565 2e44 6174 652e  dDate = ee.Date.
-0001e7a0: 6672 6f6d 594d 4428 656e 6459 6561 722c  fromYMD(endYear,
-0001e7b0: 312c 3129 2e61 6476 616e 6365 2865 6e64  1,1).advance(end
-0001e7c0: 4a75 6c69 616e 2d31 2b77 7261 704f 6666  Julian-1+wrapOff
-0001e7d0: 7365 742c 2764 6179 2729 0d0a 0d0a 2020  set,'day')....  
-0001e7e0: 6172 6773 203d 2066 6f72 6d61 7441 7267  args = formatArg
-0001e7f0: 7328 6c6f 6361 6c73 2829 290d 0a20 2069  s(locals())..  i
-0001e800: 6620 2761 7267 7327 2069 6e20 6172 6773  f 'args' in args
-0001e810: 2e6b 6579 7328 293a 0d0a 2020 2020 6465  .keys():..    de
-0001e820: 6c20 6172 6773 5b27 6172 6773 275d 0d0a  l args['args']..
-0001e830: 0d0a 2020 7072 696e 7428 2747 6574 2050  ..  print('Get P
-0001e840: 726f 6365 7373 6564 2053 656e 7469 6e65  rocessed Sentine
-0001e850: 6c32 3a20 2729 0d0a 2020 7072 696e 7428  l2: ')..  print(
-0001e860: 2753 7461 7274 2064 6174 653a 272c 2073  'Start date:', s
-0001e870: 7461 7274 4461 7465 2e66 6f72 6d61 7428  tartDate.format(
-0001e880: 274d 4d4d 2064 6420 7979 7979 2729 2e67  'MMM dd yyyy').g
-0001e890: 6574 496e 666f 2829 2c27 2c20 456e 6420  etInfo(),', End 
-0001e8a0: 6461 7465 3a27 2c20 656e 6444 6174 652e  date:', endDate.
-0001e8b0: 666f 726d 6174 2827 4d4d 4d20 6464 2079  format('MMM dd y
-0001e8c0: 7979 7927 292e 6765 7449 6e66 6f28 2929  yyy').getInfo())
-0001e8d0: 0d0a 2020 666f 7220 6172 6720 696e 2061  ..  for arg in a
-0001e8e0: 7267 732e 6b65 7973 2829 3a0d 0a20 2020  rgs.keys():..   
-0001e8f0: 2070 7269 6e74 2861 7267 2c20 273a 2027   print(arg, ': '
-0001e900: 2c20 6172 6773 5b61 7267 5d29 0d0a 0d0a  , args[arg])....
-0001e910: 2020 2347 6574 2053 656e 7469 6e65 6c32    #Get Sentinel2
-0001e920: 2069 6d61 6765 2063 6f6c 6c65 6374 696f   image collectio
-0001e930: 6e0d 0a20 2073 3273 203d 2067 6574 5332  n..  s2s = getS2
-0001e940: 285c 0d0a 2020 2020 7374 7564 7941 7265  (\..    studyAre
-0001e950: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
-0001e960: 2020 2020 7374 6172 7444 6174 6520 3d20      startDate = 
-0001e970: 7374 6172 7444 6174 652c 0d0a 2020 2020  startDate,..    
-0001e980: 656e 6444 6174 6520 3d20 656e 6444 6174  endDate = endDat
-0001e990: 652c 0d0a 2020 2020 7374 6172 744a 756c  e,..    startJul
-0001e9a0: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
-0001e9b0: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
-0001e9c0: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
-0001e9d0: 2020 2020 7265 7361 6d70 6c65 4d65 7468      resampleMeth
-0001e9e0: 6f64 203d 2072 6573 616d 706c 654d 6574  od = resampleMet
-0001e9f0: 686f 642c 0d0a 2020 2020 746f 614f 7253  hod,..    toaOrS
-0001ea00: 5220 3d20 746f 614f 7253 522c 0d0a 2020  R = toaOrSR,..  
-0001ea10: 2020 636f 6e76 6572 7454 6f44 6169 6c79    convertToDaily
-0001ea20: 4d6f 7361 6963 7320 3d20 636f 6e76 6572  Mosaics = conver
-0001ea30: 7454 6f44 6169 6c79 4d6f 7361 6963 732c  tToDailyMosaics,
-0001ea40: 0d0a 2020 2020 6164 6443 6c6f 7564 5072  ..    addCloudPr
-0001ea50: 6f62 6162 696c 6974 7920 3d20 6170 706c  obability = appl
-0001ea60: 7943 6c6f 7564 5072 6f62 6162 696c 6974  yCloudProbabilit
-0001ea70: 7929 0d0a 0d0a 2020 6966 2061 7070 6c79  y)....  if apply
-0001ea80: 5141 4261 6e64 3a0d 0a20 2020 2070 7269  QABand:..    pri
-0001ea90: 6e74 2827 4170 706c 7969 6e67 2051 4120  nt('Applying QA 
-0001eaa0: 4261 6e64 2043 6c6f 7564 204d 6173 6b27  Band Cloud Mask'
-0001eab0: 290d 0a20 2020 2073 3273 203d 2073 3273  )..    s2s = s2s
-0001eac0: 2e6d 6170 286d 6173 6b53 3263 6c6f 7564  .map(maskS2cloud
-0001ead0: 7329 0d0a 0d0a 2020 6966 2061 7070 6c79  s)....  if apply
-0001eae0: 436c 6f75 6453 636f 7265 3a0d 0a20 2020  CloudScore:..   
-0001eaf0: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
-0001eb00: 2043 6c6f 7564 2053 636f 7265 2729 0d0a   Cloud Score')..
-0001eb10: 2020 2020 7332 7320 3d20 6170 706c 7943      s2s = applyC
-0001eb20: 6c6f 7564 5363 6f72 6541 6c67 6f72 6974  loudScoreAlgorit
-0001eb30: 686d 285c 0d0a 2020 2020 2020 636f 6c6c  hm(\..      coll
-0001eb40: 6563 7469 6f6e 203d 2073 3273 2c0d 0a20  ection = s2s,.. 
-0001eb50: 2020 2020 2063 6c6f 7564 5363 6f72 6546       cloudScoreF
-0001eb60: 756e 6374 696f 6e20 3d20 7365 6e74 696e  unction = sentin
-0001eb70: 656c 3243 6c6f 7564 5363 6f72 652c 0d0a  el2CloudScore,..
-0001eb80: 2020 2020 2020 636c 6f75 6453 636f 7265        cloudScore
-0001eb90: 5468 7265 7368 203d 2063 6c6f 7564 5363  Thresh = cloudSc
-0001eba0: 6f72 6554 6872 6573 682c 0d0a 2020 2020  oreThresh,..    
-0001ebb0: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
-0001ebc0: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
-0001ebd0: 6c2c 0d0a 2020 2020 2020 636f 6e74 7261  l,..      contra
-0001ebe0: 6374 5069 7865 6c73 203d 2063 6f6e 7472  ctPixels = contr
-0001ebf0: 6163 7450 6978 656c 732c 0d0a 2020 2020  actPixels,..    
-0001ec00: 2020 6469 6c61 7465 5069 7865 6c73 203d    dilatePixels =
-0001ec10: 2064 696c 6174 6550 6978 656c 732c 0d0a   dilatePixels,..
-0001ec20: 2020 2020 2020 7065 7266 6f72 6d43 6c6f        performClo
-0001ec30: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
-0001ec40: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
-0001ec50: 654f 6666 7365 742c 0d0a 2020 2020 2020  eOffset,..      
-0001ec60: 7072 6543 6f6d 7075 7465 6443 6c6f 7564  preComputedCloud
-0001ec70: 5363 6f72 654f 6666 7365 7420 3d20 7072  ScoreOffset = pr
-0001ec80: 6543 6f6d 7075 7465 6443 6c6f 7564 5363  eComputedCloudSc
-0001ec90: 6f72 654f 6666 7365 7429 0d0a 0d0a 2020  oreOffset)....  
-0001eca0: 6966 2061 7070 6c79 436c 6f75 6450 726f  if applyCloudPro
-0001ecb0: 6261 6269 6c69 7479 3a0d 0a20 2020 2070  bability:..    p
-0001ecc0: 7269 6e74 2827 4170 706c 7920 436c 6f75  rint('Apply Clou
-0001ecd0: 6420 5072 6f62 6162 696c 6974 7927 290d  d Probability').
-0001ece0: 0a20 2020 2073 3273 203d 2073 3273 2e6d  .    s2s = s2s.m
-0001ecf0: 6170 286c 616d 6264 6120 696d 673a 2069  ap(lambda img: i
-0001ed00: 6d67 2e75 7064 6174 654d 6173 6b28 696d  mg.updateMask(im
-0001ed10: 672e 7365 6c65 6374 285b 2763 6c6f 7564  g.select(['cloud
-0001ed20: 5f70 726f 6261 6269 6c69 7479 275d 292e  _probability']).
-0001ed30: 6c74 6528 636c 6f75 6450 726f 6254 6872  lte(cloudProbThr
-0001ed40: 6573 6829 2929 0d0a 0d0a 2020 6966 2061  esh)))....  if a
-0001ed50: 7070 6c79 5368 6164 6f77 5368 6966 743a  pplyShadowShift:
-0001ed60: 0d0a 2020 2020 7072 696e 7428 2741 7070  ..    print('App
-0001ed70: 6c79 696e 6720 5368 6164 6f77 2053 6869  lying Shadow Shi
-0001ed80: 6674 2729 0d0a 2020 2020 7332 7320 3d20  ft')..    s2s = 
-0001ed90: 7332 732e 6d61 7028 6c61 6d62 6461 2069  s2s.map(lambda i
-0001eda0: 6d67 3a20 7072 6f6a 6563 7453 6861 646f  mg: projectShado
-0001edb0: 7773 5772 6170 7065 7228 5c0d 0a20 2020  wsWrapper(\..   
-0001edc0: 2020 2069 6d67 203d 2069 6d67 2c0d 0a20     img = img,.. 
-0001edd0: 2020 2020 2063 6c6f 7564 5468 7265 7368       cloudThresh
-0001ede0: 203d 2063 6c6f 7564 5363 6f72 6554 6872   = cloudScoreThr
-0001edf0: 6573 682c 0d0a 2020 2020 2020 6972 5375  esh,..      irSu
-0001ee00: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
-0001ee10: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
-0001ee20: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
-0001ee30: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
-0001ee40: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
-0001ee50: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
-0001ee60: 6978 656c 732c 0d0a 2020 2020 2020 636c  ixels,..      cl
-0001ee70: 6f75 6448 6569 6768 7473 203d 2063 6c6f  oudHeights = clo
-0001ee80: 7564 4865 6967 6874 7329 290d 0a0d 0a20  udHeights)).... 
-0001ee90: 2069 6620 6170 706c 7954 444f 4d3a 0d0a   if applyTDOM:..
-0001eea0: 2020 2020 7072 696e 7428 2741 7070 6c79      print('Apply
-0001eeb0: 696e 6720 5444 4f4d 2729 0d0a 2020 2020  ing TDOM')..    
-0001eec0: 7332 7320 3d20 7369 6d70 6c65 5444 4f4d  s2s = simpleTDOM
-0001eed0: 3228 5c0d 0a20 2020 2020 2063 6f6c 6c65  2(\..      colle
-0001eee0: 6374 696f 6e20 3d20 7332 732c 0d0a 2020  ction = s2s,..  
-0001eef0: 2020 2020 7a53 636f 7265 5468 7265 7368      zScoreThresh
-0001ef00: 203d 207a 5363 6f72 6554 6872 6573 682c   = zScoreThresh,
-0001ef10: 0d0a 2020 2020 2020 7368 6164 6f77 5375  ..      shadowSu
-0001ef20: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
-0001ef30: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
-0001ef40: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
-0001ef50: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
-0001ef60: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
-0001ef70: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
-0001ef80: 6978 656c 732c 0d0a 2020 2020 2020 7368  ixels,..      sh
-0001ef90: 6164 6f77 5375 6d42 616e 6473 203d 205b  adowSumBands = [
-0001efa0: 276e 6972 272c 2773 7769 7231 275d 2c0d  'nir','swir1'],.
-0001efb0: 0a20 2020 2020 2070 7265 436f 6d70 7574  .      preComput
-0001efc0: 6564 5444 4f4d 4952 4d65 616e 203d 2070  edTDOMIRMean = p
-0001efd0: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
-0001efe0: 4d65 616e 2c0d 0a20 2020 2020 2070 7265  Mean,..      pre
-0001eff0: 436f 6d70 7574 6564 5444 4f4d 4952 5374  ComputedTDOMIRSt
-0001f000: 6444 6576 203d 2070 7265 436f 6d70 7574  dDev = preComput
-0001f010: 6564 5444 4f4d 4952 5374 6444 6576 290d  edTDOMIRStdDev).
-0001f020: 0a0d 0a20 2023 2041 6464 2063 6f6d 6d6f  ...  # Add commo
-0001f030: 6e20 696e 6469 6365 730d 0a20 2073 3273  n indices..  s2s
-0001f040: 203d 2073 3273 2e6d 6170 2873 696d 706c   = s2s.map(simpl
-0001f050: 6541 6464 496e 6469 6365 7329 5c0d 0a20  eAddIndices)\.. 
-0001f060: 2020 2020 2020 2020 2020 2e6d 6170 2867            .map(g
-0001f070: 6574 5461 7373 656c 6564 4361 7029 5c0d  etTasseledCap)\.
-0001f080: 0a20 2020 2020 2020 2020 2020 2e6d 6170  .           .map
-0001f090: 2873 696d 706c 6541 6464 5443 416e 676c  (simpleAddTCAngl
-0001f0a0: 6573 295c 0d0a 2020 2020 2020 2020 2020  es)\..          
-0001f0b0: 202e 6d61 7028 6c61 6d62 6461 2069 6d67   .map(lambda img
-0001f0c0: 3a20 696d 672e 6164 6442 616e 6473 2869  : img.addBands(i
-0001f0d0: 6d67 2e6e 6f72 6d61 6c69 7a65 6444 6966  mg.normalizedDif
-0001f0e0: 6665 7265 6e63 6528 5b27 7265 3127 2c20  ference(['re1', 
-0001f0f0: 2772 6564 275d 292e 7365 6c65 6374 285b  'red']).select([
-0001f100: 305d 2c5b 274e 4443 4927 5d29 2929 0d0a  0],['NDCI'])))..
-0001f110: 2020 2320 4164 6420 5365 6e73 6f72 2042    # Add Sensor B
-0001f120: 616e 640d 0a20 2073 3273 203d 2073 3273  and..  s2s = s2s
-0001f130: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
-0001f140: 2061 6464 5365 6e73 6f72 4261 6e64 2869   addSensorBand(i
-0001f150: 6d67 2c20 2773 656e 7469 6e65 6c32 272c  mg, 'sentinel2',
-0001f160: 2074 6f61 4f72 5352 2929 0d0a 0d0a 200d   toaOrSR)).... .
-0001f170: 0a20 2072 6574 7572 6e20 7332 732e 7365  .  return s2s.se
-0001f180: 7428 6172 6773 290d 0a0d 0a0d 0a23 2323  t(args)......###
-0001f190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1d0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
-0001f1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e380: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+0001e390: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+0001e3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e3c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e3d0: 2323 2323 2323 2323 2323 0d0a 2357 7261  ##########..#Wra
+0001e3e0: 7070 6572 2066 756e 6374 696f 6e20 666f  pper function fo
+0001e3f0: 7220 6765 7474 696e 6720 5365 6e74 696e  r getting Sentin
+0001e400: 656c 3220 696d 6167 6572 790d 0a64 6566  el2 imagery..def
+0001e410: 2067 6574 5072 6f63 6573 7365 6453 656e   getProcessedSen
+0001e420: 7469 6e65 6c32 5363 656e 6573 285c 0d0a  tinel2Scenes(\..
+0001e430: 2020 7374 7564 7941 7265 612c 0d0a 2020    studyArea,..  
+0001e440: 7374 6172 7459 6561 722c 0d0a 2020 656e  startYear,..  en
+0001e450: 6459 6561 722c 0d0a 2020 7374 6172 744a  dYear,..  startJ
+0001e460: 756c 6961 6e2c 0d0a 2020 656e 644a 756c  ulian,..  endJul
+0001e470: 6961 6e2c 0d0a 2020 6170 706c 7951 4142  ian,..  applyQAB
+0001e480: 616e 6420 3d20 4661 6c73 652c 0d0a 2020  and = False,..  
+0001e490: 6170 706c 7943 6c6f 7564 5363 6f72 6520  applyCloudScore 
+0001e4a0: 3d20 4661 6c73 652c 0d0a 2020 6170 706c  = False,..  appl
+0001e4b0: 7953 6861 646f 7753 6869 6674 203d 2046  yShadowShift = F
+0001e4c0: 616c 7365 2c0d 0a20 2061 7070 6c79 5444  alse,..  applyTD
+0001e4d0: 4f4d 203d 2054 7275 652c 0d0a 2020 636c  OM = True,..  cl
+0001e4e0: 6f75 6453 636f 7265 5468 7265 7368 203d  oudScoreThresh =
+0001e4f0: 2032 302c 0d0a 2020 7065 7266 6f72 6d43   20,..  performC
+0001e500: 6c6f 7564 5363 6f72 654f 6666 7365 7420  loudScoreOffset 
+0001e510: 3d20 5472 7565 2c0d 0a20 2063 6c6f 7564  = True,..  cloud
+0001e520: 5363 6f72 6550 6374 6c20 3d20 3130 2c0d  ScorePctl = 10,.
+0001e530: 0a20 2063 6c6f 7564 4865 6967 6874 7320  .  cloudHeights 
+0001e540: 3d20 6565 2e4c 6973 742e 7365 7175 656e  = ee.List.sequen
+0001e550: 6365 2835 3030 2c31 3030 3030 2c35 3030  ce(500,10000,500
+0001e560: 292c 0d0a 2020 7a53 636f 7265 5468 7265  ),..  zScoreThre
+0001e570: 7368 203d 202d 312c 0d0a 2020 7368 6164  sh = -1,..  shad
+0001e580: 6f77 5375 6d54 6872 6573 6820 3d20 302e  owSumThresh = 0.
+0001e590: 3335 2c0d 0a20 2063 6f6e 7472 6163 7450  35,..  contractP
+0001e5a0: 6978 656c 7320 3d20 312e 352c 0d0a 2020  ixels = 1.5,..  
+0001e5b0: 6469 6c61 7465 5069 7865 6c73 203d 2033  dilatePixels = 3
+0001e5c0: 2e35 2c0d 0a20 2073 6861 646f 7753 756d  .5,..  shadowSum
+0001e5d0: 4261 6e64 7320 3d20 5b27 6e69 7227 2c27  Bands = ['nir','
+0001e5e0: 7377 6972 3127 5d2c 0d0a 2020 7265 7361  swir1'],..  resa
+0001e5f0: 6d70 6c65 4d65 7468 6f64 203d 2027 6167  mpleMethod = 'ag
+0001e600: 6772 6567 6174 6527 2c0d 0a20 2074 6f61  gregate',..  toa
+0001e610: 4f72 5352 203d 2027 544f 4127 2c0d 0a20  OrSR = 'TOA',.. 
+0001e620: 2063 6f6e 7665 7274 546f 4461 696c 794d   convertToDailyM
+0001e630: 6f73 6169 6373 203d 2054 7275 652c 0d0a  osaics = True,..
+0001e640: 2020 6170 706c 7943 6c6f 7564 5072 6f62    applyCloudProb
+0001e650: 6162 696c 6974 7920 3d20 5472 7565 2c0d  ability = True,.
+0001e660: 0a20 2070 7265 436f 6d70 7574 6564 436c  .  preComputedCl
+0001e670: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
+0001e680: 204e 6f6e 652c 0d0a 2020 7072 6543 6f6d   None,..  preCom
+0001e690: 7075 7465 6454 444f 4d49 524d 6561 6e20  putedTDOMIRMean 
+0001e6a0: 3d20 4e6f 6e65 2c0d 0a20 2070 7265 436f  = None,..  preCo
+0001e6b0: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
+0001e6c0: 6576 203d 204e 6f6e 652c 0d0a 2020 636c  ev = None,..  cl
+0001e6d0: 6f75 6450 726f 6254 6872 6573 6820 3d20  oudProbThresh = 
+0001e6e0: 3430 2c0d 0a20 2076 6572 626f 7365 203d  40,..  verbose =
+0001e6f0: 2046 616c 7365 293a 0d0a 0d0a 2020 6f72   False):....  or
+0001e700: 6967 696e 203d 2027 5365 6e74 696e 656c  igin = 'Sentinel
+0001e710: 3227 0d0a 2020 746f 614f 7253 5220 3d20  2'..  toaOrSR = 
+0001e720: 746f 614f 7253 522e 7570 7065 7228 290d  toaOrSR.upper().
+0001e730: 0a0d 0a20 2023 5072 6570 6172 6520 6461  ...  #Prepare da
+0001e740: 7465 730d 0a20 2023 5772 6170 2074 6865  tes..  #Wrap the
+0001e750: 2064 6174 6573 2069 6620 6e65 6564 6564   dates if needed
+0001e760: 0d0a 2020 7772 6170 4f66 6673 6574 203d  ..  wrapOffset =
+0001e770: 2030 0d0a 2020 6966 2073 7461 7274 4a75   0..  if startJu
+0001e780: 6c69 616e 203e 2065 6e64 4a75 6c69 616e  lian > endJulian
+0001e790: 3a0d 0a20 2020 2077 7261 704f 6666 7365  :..    wrapOffse
+0001e7a0: 7420 3d20 3336 350d 0a20 2073 7461 7274  t = 365..  start
+0001e7b0: 4461 7465 203d 2065 652e 4461 7465 2e66  Date = ee.Date.f
+0001e7c0: 726f 6d59 4d44 2873 7461 7274 5965 6172  romYMD(startYear
+0001e7d0: 2c31 2c31 292e 6164 7661 6e63 6528 7374  ,1,1).advance(st
+0001e7e0: 6172 744a 756c 6961 6e2d 312c 2764 6179  artJulian-1,'day
+0001e7f0: 2729 0d0a 2020 656e 6444 6174 6520 3d20  ')..  endDate = 
+0001e800: 6565 2e44 6174 652e 6672 6f6d 594d 4428  ee.Date.fromYMD(
+0001e810: 656e 6459 6561 722c 312c 3129 2e61 6476  endYear,1,1).adv
+0001e820: 616e 6365 2865 6e64 4a75 6c69 616e 2d31  ance(endJulian-1
+0001e830: 2b77 7261 704f 6666 7365 742c 2764 6179  +wrapOffset,'day
+0001e840: 2729 0d0a 0d0a 2020 6172 6773 203d 2066  ')....  args = f
+0001e850: 6f72 6d61 7441 7267 7328 6c6f 6361 6c73  ormatArgs(locals
+0001e860: 2829 290d 0a20 2069 6620 2761 7267 7327  ())..  if 'args'
+0001e870: 2069 6e20 6172 6773 2e6b 6579 7328 293a   in args.keys():
+0001e880: 0d0a 2020 2020 6465 6c20 6172 6773 5b27  ..    del args['
+0001e890: 6172 6773 275d 0d0a 0d0a 2020 7072 696e  args']....  prin
+0001e8a0: 7428 2747 6574 2050 726f 6365 7373 6564  t('Get Processed
+0001e8b0: 2053 656e 7469 6e65 6c32 3a20 2729 0d0a   Sentinel2: ')..
+0001e8c0: 2020 7072 696e 7428 2753 7461 7274 2064    print('Start d
+0001e8d0: 6174 653a 272c 2073 7461 7274 4461 7465  ate:', startDate
+0001e8e0: 2e66 6f72 6d61 7428 274d 4d4d 2064 6420  .format('MMM dd 
+0001e8f0: 7979 7979 2729 2e67 6574 496e 666f 2829  yyyy').getInfo()
+0001e900: 2c27 2c20 456e 6420 6461 7465 3a27 2c20  ,', End date:', 
+0001e910: 656e 6444 6174 652e 666f 726d 6174 2827  endDate.format('
+0001e920: 4d4d 4d20 6464 2079 7979 7927 292e 6765  MMM dd yyyy').ge
+0001e930: 7449 6e66 6f28 2929 0d0a 2020 6966 2076  tInfo())..  if v
+0001e940: 6572 626f 7365 3a0d 0a20 2020 2066 6f72  erbose:..    for
+0001e950: 2061 7267 2069 6e20 6172 6773 2e6b 6579   arg in args.key
+0001e960: 7328 293a 0d0a 2020 2020 2020 7072 696e  s():..      prin
+0001e970: 7428 6172 672c 2027 3a20 272c 2061 7267  t(arg, ': ', arg
+0001e980: 735b 6172 675d 290d 0a0d 0a20 2023 4765  s[arg])....  #Ge
+0001e990: 7420 5365 6e74 696e 656c 3220 696d 6167  t Sentinel2 imag
+0001e9a0: 6520 636f 6c6c 6563 7469 6f6e 0d0a 2020  e collection..  
+0001e9b0: 7332 7320 3d20 6765 7453 3228 5c0d 0a20  s2s = getS2(\.. 
+0001e9c0: 2020 2073 7475 6479 4172 6561 203d 2073     studyArea = s
+0001e9d0: 7475 6479 4172 6561 2c0d 0a20 2020 2073  tudyArea,..    s
+0001e9e0: 7461 7274 4461 7465 203d 2073 7461 7274  tartDate = start
+0001e9f0: 4461 7465 2c0d 0a20 2020 2065 6e64 4461  Date,..    endDa
+0001ea00: 7465 203d 2065 6e64 4461 7465 2c0d 0a20  te = endDate,.. 
+0001ea10: 2020 2073 7461 7274 4a75 6c69 616e 203d     startJulian =
+0001ea20: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
+0001ea30: 2020 2065 6e64 4a75 6c69 616e 203d 2065     endJulian = e
+0001ea40: 6e64 4a75 6c69 616e 2c0d 0a20 2020 2072  ndJulian,..    r
+0001ea50: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+0001ea60: 7265 7361 6d70 6c65 4d65 7468 6f64 2c0d  resampleMethod,.
+0001ea70: 0a20 2020 2074 6f61 4f72 5352 203d 2074  .    toaOrSR = t
+0001ea80: 6f61 4f72 5352 2c0d 0a20 2020 2063 6f6e  oaOrSR,..    con
+0001ea90: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
+0001eaa0: 6373 203d 2063 6f6e 7665 7274 546f 4461  cs = convertToDa
+0001eab0: 696c 794d 6f73 6169 6373 2c0d 0a20 2020  ilyMosaics,..   
+0001eac0: 2061 6464 436c 6f75 6450 726f 6261 6269   addCloudProbabi
+0001ead0: 6c69 7479 203d 2061 7070 6c79 436c 6f75  lity = applyClou
+0001eae0: 6450 726f 6261 6269 6c69 7479 290d 0a0d  dProbability)...
+0001eaf0: 0a20 2069 6620 6170 706c 7951 4142 616e  .  if applyQABan
+0001eb00: 643a 0d0a 2020 2020 7072 696e 7428 2741  d:..    print('A
+0001eb10: 7070 6c79 696e 6720 5141 2042 616e 6420  pplying QA Band 
+0001eb20: 436c 6f75 6420 4d61 736b 2729 0d0a 2020  Cloud Mask')..  
+0001eb30: 2020 7332 7320 3d20 7332 732e 6d61 7028    s2s = s2s.map(
+0001eb40: 6d61 736b 5332 636c 6f75 6473 290d 0a0d  maskS2clouds)...
+0001eb50: 0a20 2069 6620 6170 706c 7943 6c6f 7564  .  if applyCloud
+0001eb60: 5363 6f72 653a 0d0a 2020 2020 7072 696e  Score:..    prin
+0001eb70: 7428 2741 7070 6c79 696e 6720 436c 6f75  t('Applying Clou
+0001eb80: 6420 5363 6f72 6527 290d 0a20 2020 2073  d Score')..    s
+0001eb90: 3273 203d 2061 7070 6c79 436c 6f75 6453  2s = applyCloudS
+0001eba0: 636f 7265 416c 676f 7269 7468 6d28 5c0d  coreAlgorithm(\.
+0001ebb0: 0a20 2020 2020 2063 6f6c 6c65 6374 696f  .      collectio
+0001ebc0: 6e20 3d20 7332 732c 0d0a 2020 2020 2020  n = s2s,..      
+0001ebd0: 636c 6f75 6453 636f 7265 4675 6e63 7469  cloudScoreFuncti
+0001ebe0: 6f6e 203d 2073 656e 7469 6e65 6c32 436c  on = sentinel2Cl
+0001ebf0: 6f75 6453 636f 7265 2c0d 0a20 2020 2020  oudScore,..     
+0001ec00: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
+0001ec10: 6820 3d20 636c 6f75 6453 636f 7265 5468  h = cloudScoreTh
+0001ec20: 7265 7368 2c0d 0a20 2020 2020 2063 6c6f  resh,..      clo
+0001ec30: 7564 5363 6f72 6550 6374 6c20 3d20 636c  udScorePctl = cl
+0001ec40: 6f75 6453 636f 7265 5063 746c 2c0d 0a20  oudScorePctl,.. 
+0001ec50: 2020 2020 2063 6f6e 7472 6163 7450 6978       contractPix
+0001ec60: 656c 7320 3d20 636f 6e74 7261 6374 5069  els = contractPi
+0001ec70: 7865 6c73 2c0d 0a20 2020 2020 2064 696c  xels,..      dil
+0001ec80: 6174 6550 6978 656c 7320 3d20 6469 6c61  atePixels = dila
+0001ec90: 7465 5069 7865 6c73 2c0d 0a20 2020 2020  tePixels,..     
+0001eca0: 2070 6572 666f 726d 436c 6f75 6453 636f   performCloudSco
+0001ecb0: 7265 4f66 6673 6574 203d 2070 6572 666f  reOffset = perfo
+0001ecc0: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
+0001ecd0: 6574 2c0d 0a20 2020 2020 2070 7265 436f  et,..      preCo
+0001ece0: 6d70 7574 6564 436c 6f75 6453 636f 7265  mputedCloudScore
+0001ecf0: 4f66 6673 6574 203d 2070 7265 436f 6d70  Offset = preComp
+0001ed00: 7574 6564 436c 6f75 6453 636f 7265 4f66  utedCloudScoreOf
+0001ed10: 6673 6574 290d 0a0d 0a20 2069 6620 6170  fset)....  if ap
+0001ed20: 706c 7943 6c6f 7564 5072 6f62 6162 696c  plyCloudProbabil
+0001ed30: 6974 793a 0d0a 2020 2020 7072 696e 7428  ity:..    print(
+0001ed40: 2741 7070 6c79 2043 6c6f 7564 2050 726f  'Apply Cloud Pro
+0001ed50: 6261 6269 6c69 7479 2729 0d0a 2020 2020  bability')..    
+0001ed60: 7332 7320 3d20 7332 732e 6d61 7028 6c61  s2s = s2s.map(la
+0001ed70: 6d62 6461 2069 6d67 3a20 696d 672e 7570  mbda img: img.up
+0001ed80: 6461 7465 4d61 736b 2869 6d67 2e73 656c  dateMask(img.sel
+0001ed90: 6563 7428 5b27 636c 6f75 645f 7072 6f62  ect(['cloud_prob
+0001eda0: 6162 696c 6974 7927 5d29 2e6c 7465 2863  ability']).lte(c
+0001edb0: 6c6f 7564 5072 6f62 5468 7265 7368 2929  loudProbThresh))
+0001edc0: 290d 0a0d 0a20 2069 6620 6170 706c 7953  )....  if applyS
+0001edd0: 6861 646f 7753 6869 6674 3a0d 0a20 2020  hadowShift:..   
+0001ede0: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
+0001edf0: 2053 6861 646f 7720 5368 6966 7427 290d   Shadow Shift').
+0001ee00: 0a20 2020 2073 3273 203d 2073 3273 2e6d  .    s2s = s2s.m
+0001ee10: 6170 286c 616d 6264 6120 696d 673a 2070  ap(lambda img: p
+0001ee20: 726f 6a65 6374 5368 6164 6f77 7357 7261  rojectShadowsWra
+0001ee30: 7070 6572 285c 0d0a 2020 2020 2020 696d  pper(\..      im
+0001ee40: 6720 3d20 696d 672c 0d0a 2020 2020 2020  g = img,..      
+0001ee50: 636c 6f75 6454 6872 6573 6820 3d20 636c  cloudThresh = cl
+0001ee60: 6f75 6453 636f 7265 5468 7265 7368 2c0d  oudScoreThresh,.
+0001ee70: 0a20 2020 2020 2069 7253 756d 5468 7265  .      irSumThre
+0001ee80: 7368 203d 2073 6861 646f 7753 756d 5468  sh = shadowSumTh
+0001ee90: 7265 7368 2c0d 0a20 2020 2020 2063 6f6e  resh,..      con
+0001eea0: 7472 6163 7450 6978 656c 7320 3d20 636f  tractPixels = co
+0001eeb0: 6e74 7261 6374 5069 7865 6c73 2c0d 0a20  ntractPixels,.. 
+0001eec0: 2020 2020 2064 696c 6174 6550 6978 656c       dilatePixel
+0001eed0: 7320 3d20 6469 6c61 7465 5069 7865 6c73  s = dilatePixels
+0001eee0: 2c0d 0a20 2020 2020 2063 6c6f 7564 4865  ,..      cloudHe
+0001eef0: 6967 6874 7320 3d20 636c 6f75 6448 6569  ights = cloudHei
+0001ef00: 6768 7473 2929 0d0a 0d0a 2020 6966 2061  ghts))....  if a
+0001ef10: 7070 6c79 5444 4f4d 3a0d 0a20 2020 2070  pplyTDOM:..    p
+0001ef20: 7269 6e74 2827 4170 706c 7969 6e67 2054  rint('Applying T
+0001ef30: 444f 4d27 290d 0a20 2020 2073 3273 203d  DOM')..    s2s =
+0001ef40: 2073 696d 706c 6554 444f 4d32 285c 0d0a   simpleTDOM2(\..
+0001ef50: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
+0001ef60: 203d 2073 3273 2c0d 0a20 2020 2020 207a   = s2s,..      z
+0001ef70: 5363 6f72 6554 6872 6573 6820 3d20 7a53  ScoreThresh = zS
+0001ef80: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
+0001ef90: 2020 2073 6861 646f 7753 756d 5468 7265     shadowSumThre
+0001efa0: 7368 203d 2073 6861 646f 7753 756d 5468  sh = shadowSumTh
+0001efb0: 7265 7368 2c0d 0a20 2020 2020 2063 6f6e  resh,..      con
+0001efc0: 7472 6163 7450 6978 656c 7320 3d20 636f  tractPixels = co
+0001efd0: 6e74 7261 6374 5069 7865 6c73 2c0d 0a20  ntractPixels,.. 
+0001efe0: 2020 2020 2064 696c 6174 6550 6978 656c       dilatePixel
+0001eff0: 7320 3d20 6469 6c61 7465 5069 7865 6c73  s = dilatePixels
+0001f000: 2c0d 0a20 2020 2020 2073 6861 646f 7753  ,..      shadowS
+0001f010: 756d 4261 6e64 7320 3d20 5b27 6e69 7227  umBands = ['nir'
+0001f020: 2c27 7377 6972 3127 5d2c 0d0a 2020 2020  ,'swir1'],..    
+0001f030: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
+0001f040: 4d49 524d 6561 6e20 3d20 7072 6543 6f6d  MIRMean = preCom
+0001f050: 7075 7465 6454 444f 4d49 524d 6561 6e2c  putedTDOMIRMean,
+0001f060: 0d0a 2020 2020 2020 7072 6543 6f6d 7075  ..      preCompu
+0001f070: 7465 6454 444f 4d49 5253 7464 4465 7620  tedTDOMIRStdDev 
+0001f080: 3d20 7072 6543 6f6d 7075 7465 6454 444f  = preComputedTDO
+0001f090: 4d49 5253 7464 4465 7629 0d0a 0d0a 2020  MIRStdDev)....  
+0001f0a0: 2320 4164 6420 636f 6d6d 6f6e 2069 6e64  # Add common ind
+0001f0b0: 6963 6573 0d0a 2020 7332 7320 3d20 7332  ices..  s2s = s2
+0001f0c0: 732e 6d61 7028 7369 6d70 6c65 4164 6449  s.map(simpleAddI
+0001f0d0: 6e64 6963 6573 295c 0d0a 2020 2020 2020  ndices)\..      
+0001f0e0: 2020 2020 202e 6d61 7028 6765 7454 6173       .map(getTas
+0001f0f0: 7365 6c65 6443 6170 295c 0d0a 2020 2020  seledCap)\..    
+0001f100: 2020 2020 2020 202e 6d61 7028 7369 6d70         .map(simp
+0001f110: 6c65 4164 6454 4341 6e67 6c65 7329 5c0d  leAddTCAngles)\.
+0001f120: 0a20 2020 2020 2020 2020 2020 2e6d 6170  .           .map
+0001f130: 286c 616d 6264 6120 696d 673a 2069 6d67  (lambda img: img
+0001f140: 2e61 6464 4261 6e64 7328 696d 672e 6e6f  .addBands(img.no
+0001f150: 726d 616c 697a 6564 4469 6666 6572 656e  rmalizedDifferen
+0001f160: 6365 285b 2772 6531 272c 2027 7265 6427  ce(['re1', 'red'
+0001f170: 5d29 2e73 656c 6563 7428 5b30 5d2c 5b27  ]).select([0],['
+0001f180: 4e44 4349 275d 2929 290d 0a20 2023 2041  NDCI'])))..  # A
+0001f190: 6464 2053 656e 736f 7220 4261 6e64 0d0a  dd Sensor Band..
+0001f1a0: 2020 7332 7320 3d20 7332 732e 6d61 7028    s2s = s2s.map(
+0001f1b0: 6c61 6d62 6461 2069 6d67 3a20 6164 6453  lambda img: addS
+0001f1c0: 656e 736f 7242 616e 6428 696d 672c 2027  ensorBand(img, '
+0001f1d0: 7365 6e74 696e 656c 3227 2c20 746f 614f  sentinel2', toaO
+0001f1e0: 7253 5229 290d 0a0d 0a20 0d0a 2020 7265  rSR)).... ..  re
+0001f1f0: 7475 726e 2073 3273 2e73 6574 2861 7267  turn s2s.set(arg
+0001f200: 7329 0d0a 0d0a 0d0a 2323 2323 2323 2323  s)......########
 0001f210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f220: 230d 0a23 2057 7261 7070 6572 2066 756e  #..# Wrapper fun
-0001f230: 6374 696f 6e20 666f 7220 6765 7474 696e  ction for gettin
-0001f240: 6720 5365 6e74 696e 656c 2032 2069 6d61  g Sentinel 2 ima
-0001f250: 6765 7279 0d0a 6465 6620 6765 7453 656e  gery..def getSen
-0001f260: 7469 6e65 6c32 5772 6170 7065 7228 5c0d  tinel2Wrapper(\.
-0001f270: 0a20 2073 7475 6479 4172 6561 2c0d 0a20  .  studyArea,.. 
-0001f280: 2073 7461 7274 5965 6172 2c0d 0a20 2065   startYear,..  e
-0001f290: 6e64 5965 6172 2c0d 0a20 2073 7461 7274  ndYear,..  start
-0001f2a0: 4a75 6c69 616e 2c0d 0a20 2065 6e64 4a75  Julian,..  endJu
-0001f2b0: 6c69 616e 2c0d 0a20 2074 696d 6562 7566  lian,..  timebuf
-0001f2c0: 6665 7220 3d20 302c 0d0a 2020 7765 6967  fer = 0,..  weig
-0001f2d0: 6874 7320 3d20 5b31 5d2c 0d0a 2020 636f  hts = [1],..  co
-0001f2e0: 6d70 6f73 6974 696e 674d 6574 686f 6420  mpositingMethod 
-0001f2f0: 3d20 276d 6564 6f69 6427 2c0d 0a20 2061  = 'medoid',..  a
-0001f300: 7070 6c79 5141 4261 6e64 203d 2046 616c  pplyQABand = Fal
-0001f310: 7365 2c0d 0a20 2061 7070 6c79 436c 6f75  se,..  applyClou
-0001f320: 6453 636f 7265 203d 2046 616c 7365 2c0d  dScore = False,.
-0001f330: 0a20 2061 7070 6c79 5368 6164 6f77 5368  .  applyShadowSh
-0001f340: 6966 7420 3d20 4661 6c73 652c 0d0a 2020  ift = False,..  
-0001f350: 6170 706c 7954 444f 4d20 3d20 5472 7565  applyTDOM = True
-0001f360: 2c0d 0a20 2063 6c6f 7564 5363 6f72 6554  ,..  cloudScoreT
-0001f370: 6872 6573 6820 3d20 3230 2c0d 0a20 2070  hresh = 20,..  p
-0001f380: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
-0001f390: 4f66 6673 6574 203d 2054 7275 652c 0d0a  Offset = True,..
-0001f3a0: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
-0001f3b0: 203d 2031 302c 0d0a 2020 636c 6f75 6448   = 10,..  cloudH
-0001f3c0: 6569 6768 7473 203d 6565 2e4c 6973 742e  eights =ee.List.
-0001f3d0: 7365 7175 656e 6365 2835 3030 2c31 3030  sequence(500,100
-0001f3e0: 3030 2c35 3030 292c 0d0a 2020 7a53 636f  00,500),..  zSco
-0001f3f0: 7265 5468 7265 7368 203d 202d 312c 0d0a  reThresh = -1,..
-0001f400: 2020 7368 6164 6f77 5375 6d54 6872 6573    shadowSumThres
-0001f410: 6820 3d20 302e 3335 2c0d 0a20 2063 6f6e  h = 0.35,..  con
-0001f420: 7472 6163 7450 6978 656c 7320 3d20 312e  tractPixels = 1.
-0001f430: 352c 0d0a 2020 6469 6c61 7465 5069 7865  5,..  dilatePixe
-0001f440: 6c73 203d 2033 2e35 2c0d 0a20 2073 6861  ls = 3.5,..  sha
-0001f450: 646f 7753 756d 4261 6e64 7320 3d20 5b27  dowSumBands = ['
-0001f460: 6e69 7227 2c27 7377 6972 3127 5d2c 0d0a  nir','swir1'],..
-0001f470: 2020 636f 7272 6563 7449 6c6c 756d 696e    correctIllumin
-0001f480: 6174 696f 6e20 3d20 4661 6c73 652c 0d0a  ation = False,..
-0001f490: 2020 636f 7272 6563 7453 6361 6c65 203d    correctScale =
-0001f4a0: 2032 3530 2c0d 0a20 2065 7870 6f72 7443   250,..  exportC
-0001f4b0: 6f6d 706f 7369 7465 7320 3d20 4661 6c73  omposites = Fals
-0001f4c0: 652c 0d0a 2020 6f75 7470 7574 4e61 6d65  e,..  outputName
-0001f4d0: 203d 2027 5365 6e74 696e 656c 322d 436f   = 'Sentinel2-Co
-0001f4e0: 6d70 6f73 6974 6527 2c0d 0a20 2065 7870  mposite',..  exp
-0001f4f0: 6f72 7450 6174 6852 6f6f 7420 3d20 2775  ortPathRoot = 'u
-0001f500: 7365 7273 2f69 616e 686f 7573 6d61 6e2f  sers/ianhousman/
-0001f510: 7465 7374 272c 0d0a 2020 6372 7320 3d20  test',..  crs = 
-0001f520: 2745 5053 473a 3530 3730 272c 0d0a 2020  'EPSG:5070',..  
-0001f530: 7472 616e 7366 6f72 6d20 3d20 5b31 302c  transform = [10,
-0001f540: 302c 2d32 3336 3139 3135 2e30 2c30 2c2d  0,-2361915.0,0,-
-0001f550: 3130 2c33 3137 3737 3335 2e30 5d2c 0d0a  10,3177735.0],..
-0001f560: 2020 7363 616c 6520 3d20 4e6f 6e65 2c0d    scale = None,.
-0001f570: 0a20 2072 6573 616d 706c 654d 6574 686f  .  resampleMetho
-0001f580: 6420 3d20 2761 6767 7265 6761 7465 272c  d = 'aggregate',
-0001f590: 0d0a 2020 746f 614f 7253 5220 3d20 2754  ..  toaOrSR = 'T
-0001f5a0: 4f41 272c 0d0a 2020 636f 6e76 6572 7454  OA',..  convertT
-0001f5b0: 6f44 6169 6c79 4d6f 7361 6963 7320 3d20  oDailyMosaics = 
-0001f5c0: 5472 7565 2c0d 0a20 2061 7070 6c79 436c  True,..  applyCl
-0001f5d0: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
-0001f5e0: 2054 7275 652c 0d0a 2020 7072 6543 6f6d   True,..  preCom
-0001f5f0: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
-0001f600: 6666 7365 7420 3d20 4e6f 6e65 2c0d 0a20  ffset = None,.. 
-0001f610: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
-0001f620: 4952 4d65 616e 203d 204e 6f6e 652c 0d0a  IRMean = None,..
-0001f630: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
-0001f640: 4d49 5253 7464 4465 7620 3d20 4e6f 6e65  MIRStdDev = None
-0001f650: 2c0d 0a20 2063 6c6f 7564 5072 6f62 5468  ,..  cloudProbTh
-0001f660: 7265 7368 203d 2034 302c 0d0a 2020 6f76  resh = 40,..  ov
-0001f670: 6572 7772 6974 6520 3d20 4661 6c73 6529  erwrite = False)
-0001f680: 3a0d 0a0d 0a20 206f 7269 6769 6e20 3d20  :....  origin = 
-0001f690: 2753 656e 7469 6e65 6c32 270d 0a20 2074  'Sentinel2'..  t
-0001f6a0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
-0001f6b0: 2e75 7070 6572 2829 0d0a 0d0a 2020 6172  .upper()....  ar
-0001f6c0: 6773 203d 2066 6f72 6d61 7441 7267 7328  gs = formatArgs(
-0001f6d0: 6c6f 6361 6c73 2829 290d 0a20 2069 6620  locals())..  if 
-0001f6e0: 2761 7267 7327 2069 6e20 6172 6773 2e6b  'args' in args.k
-0001f6f0: 6579 7328 293a 0d0a 2020 2020 6465 6c20  eys():..    del 
-0001f700: 6172 6773 5b27 6172 6773 275d 0d0a 0d0a  args['args']....
-0001f710: 2020 7332 7320 3d20 6765 7450 726f 6365    s2s = getProce
-0001f720: 7373 6564 5365 6e74 696e 656c 3253 6365  ssedSentinel2Sce
-0001f730: 6e65 7328 5c0d 0a20 2020 2073 7475 6479  nes(\..    study
-0001f740: 4172 6561 203d 2073 7475 6479 4172 6561  Area = studyArea
-0001f750: 2c0d 0a20 2020 2073 7461 7274 5965 6172  ,..    startYear
-0001f760: 203d 2073 7461 7274 5965 6172 2c0d 0a20   = startYear,.. 
-0001f770: 2020 2065 6e64 5965 6172 203d 2065 6e64     endYear = end
-0001f780: 5965 6172 2c0d 0a20 2020 2073 7461 7274  Year,..    start
-0001f790: 4a75 6c69 616e 203d 2073 7461 7274 4a75  Julian = startJu
-0001f7a0: 6c69 616e 2c0d 0a20 2020 2065 6e64 4a75  lian,..    endJu
-0001f7b0: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
-0001f7c0: 2c0d 0a20 2020 2061 7070 6c79 5141 4261  ,..    applyQABa
-0001f7d0: 6e64 203d 2061 7070 6c79 5141 4261 6e64  nd = applyQABand
-0001f7e0: 2c0d 0a20 2020 2061 7070 6c79 436c 6f75  ,..    applyClou
-0001f7f0: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
-0001f800: 6f75 6453 636f 7265 2c0d 0a20 2020 2061  oudScore,..    a
-0001f810: 7070 6c79 5368 6164 6f77 5368 6966 7420  pplyShadowShift 
-0001f820: 3d20 6170 706c 7953 6861 646f 7753 6869  = applyShadowShi
-0001f830: 6674 2c0d 0a20 2020 2061 7070 6c79 5444  ft,..    applyTD
-0001f840: 4f4d 203d 2061 7070 6c79 5444 4f4d 2c0d  OM = applyTDOM,.
-0001f850: 0a20 2020 2063 6c6f 7564 5363 6f72 6554  .    cloudScoreT
-0001f860: 6872 6573 6820 3d20 636c 6f75 6453 636f  hresh = cloudSco
-0001f870: 7265 5468 7265 7368 2c0d 0a20 2020 2070  reThresh,..    p
-0001f880: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
-0001f890: 4f66 6673 6574 203d 2070 6572 666f 726d  Offset = perform
-0001f8a0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-0001f8b0: 2c0d 0a20 2020 2063 6c6f 7564 5363 6f72  ,..    cloudScor
-0001f8c0: 6550 6374 6c20 3d20 636c 6f75 6453 636f  ePctl = cloudSco
-0001f8d0: 7265 5063 746c 2c0d 0a20 2020 2063 6c6f  rePctl,..    clo
-0001f8e0: 7564 4865 6967 6874 7320 3d20 636c 6f75  udHeights = clou
-0001f8f0: 6448 6569 6768 7473 2c0d 0a20 2020 207a  dHeights,..    z
-0001f900: 5363 6f72 6554 6872 6573 6820 3d20 7a53  ScoreThresh = zS
-0001f910: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
-0001f920: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
-0001f930: 203d 2073 6861 646f 7753 756d 5468 7265   = shadowSumThre
-0001f940: 7368 2c0d 0a20 2020 2063 6f6e 7472 6163  sh,..    contrac
-0001f950: 7450 6978 656c 7320 3d20 636f 6e74 7261  tPixels = contra
-0001f960: 6374 5069 7865 6c73 2c0d 0a20 2020 2064  ctPixels,..    d
-0001f970: 696c 6174 6550 6978 656c 7320 3d20 6469  ilatePixels = di
-0001f980: 6c61 7465 5069 7865 6c73 2c0d 0a20 2020  latePixels,..   
-0001f990: 2073 6861 646f 7753 756d 4261 6e64 7320   shadowSumBands 
-0001f9a0: 3d20 7368 6164 6f77 5375 6d42 616e 6473  = shadowSumBands
-0001f9b0: 2c0d 0a20 2020 2072 6573 616d 706c 654d  ,..    resampleM
-0001f9c0: 6574 686f 6420 3d20 7265 7361 6d70 6c65  ethod = resample
-0001f9d0: 4d65 7468 6f64 2c0d 0a20 2020 2074 6f61  Method,..    toa
-0001f9e0: 4f72 5352 203d 2074 6f61 4f72 5352 2c0d  OrSR = toaOrSR,.
-0001f9f0: 0a20 2020 2063 6f6e 7665 7274 546f 4461  .    convertToDa
-0001fa00: 696c 794d 6f73 6169 6373 203d 2063 6f6e  ilyMosaics = con
-0001fa10: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
-0001fa20: 6373 2c0d 0a20 2020 2061 7070 6c79 436c  cs,..    applyCl
-0001fa30: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
-0001fa40: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
-0001fa50: 6269 6c69 7479 2c0d 0a20 2020 2070 7265  bility,..    pre
-0001fa60: 436f 6d70 7574 6564 436c 6f75 6453 636f  ComputedCloudSco
-0001fa70: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
-0001fa80: 6d70 7574 6564 436c 6f75 6453 636f 7265  mputedCloudScore
-0001fa90: 4f66 6673 6574 2c0d 0a20 2020 2070 7265  Offset,..    pre
-0001faa0: 436f 6d70 7574 6564 5444 4f4d 4952 4d65  ComputedTDOMIRMe
-0001fab0: 616e 203d 2070 7265 436f 6d70 7574 6564  an = preComputed
-0001fac0: 5444 4f4d 4952 4d65 616e 2c0d 0a20 2020  TDOMIRMean,..   
-0001fad0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
-0001fae0: 4952 5374 6444 6576 203d 2070 7265 436f  IRStdDev = preCo
-0001faf0: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
-0001fb00: 6576 2c0d 0a20 2020 2063 6c6f 7564 5072  ev,..    cloudPr
-0001fb10: 6f62 5468 7265 7368 203d 2063 6c6f 7564  obThresh = cloud
-0001fb20: 5072 6f62 5468 7265 7368 290d 0a0d 0a20  ProbThresh).... 
-0001fb30: 2023 4164 6420 7a65 6e69 7468 2061 6e64   #Add zenith and
-0001fb40: 2061 7a69 6d75 7468 0d0a 2020 2369 6620   azimuth..  #if 
-0001fb50: 636f 7272 6563 7449 6c6c 756d 696e 6174  correctIlluminat
-0001fb60: 696f 6e3a 0d0a 2020 2320 2073 3273 203d  ion:..  #  s2s =
-0001fb70: 2073 3273 2e6d 6170 2866 756e 6374 696f   s2s.map(functio
-0001fb80: 6e28 696d 6729 7b0d 0a20 2023 2020 2020  n(img){..  #    
-0001fb90: 7265 7475 726e 2061 6464 5a65 6e69 7468  return addZenith
-0001fba0: 417a 696d 7574 6828 696d 672c 2754 4f41  Azimuth(img,'TOA
-0001fbb0: 272c 7b27 544f 4127 3a27 4d45 414e 5f53  ',{'TOA':'MEAN_S
-0001fbc0: 4f4c 4152 5f5a 454e 4954 485f 414e 474c  OLAR_ZENITH_ANGL
-0001fbd0: 4527 7d2c 7b27 544f 4127 3a27 4d45 414e  E'},{'TOA':'MEAN
-0001fbe0: 5f53 4f4c 4152 5f41 5a49 4d55 5448 5f41  _SOLAR_AZIMUTH_A
-0001fbf0: 4e47 4c45 277d 293b 0d0a 2020 2320 207d  NGLE'});..  #  }
-0001fc00: 293b 0d0a 2020 237d 0d0a 0d0a 2020 2343  );..  #}....  #C
-0001fc10: 7265 6174 6520 636f 6d70 6f73 6974 6520  reate composite 
-0001fc20: 7469 6d65 2073 6572 6965 730d 0a20 2074  time series..  t
-0001fc30: 7320 3d20 636f 6d70 6f73 6974 6554 696d  s = compositeTim
-0001fc40: 6553 6572 6965 7328 5c0d 0a20 2020 206c  eSeries(\..    l
-0001fc50: 7320 3d20 7332 732c 0d0a 2020 2020 7374  s = s2s,..    st
-0001fc60: 6172 7459 6561 7220 3d20 7374 6172 7459  artYear = startY
-0001fc70: 6561 722c 0d0a 2020 2020 656e 6459 6561  ear,..    endYea
-0001fc80: 7220 3d20 656e 6459 6561 722c 0d0a 2020  r = endYear,..  
-0001fc90: 2020 7374 6172 744a 756c 6961 6e20 3d20    startJulian = 
-0001fca0: 7374 6172 744a 756c 6961 6e2c 0d0a 2020  startJulian,..  
-0001fcb0: 2020 656e 644a 756c 6961 6e20 3d20 656e    endJulian = en
-0001fcc0: 644a 756c 6961 6e2c 0d0a 2020 2020 7469  dJulian,..    ti
-0001fcd0: 6d65 6275 6666 6572 203d 2074 696d 6562  mebuffer = timeb
-0001fce0: 7566 6665 722c 0d0a 2020 2020 7765 6967  uffer,..    weig
-0001fcf0: 6874 7320 3d20 7765 6967 6874 732c 0d0a  hts = weights,..
-0001fd00: 2020 2020 636f 6d70 6f73 6974 696e 674d      compositingM
-0001fd10: 6574 686f 6420 3d20 636f 6d70 6f73 6974  ethod = composit
-0001fd20: 696e 674d 6574 686f 6429 0d0a 0d0a 2020  ingMethod)....  
-0001fd30: 2343 6f72 7265 6374 2069 6c6c 756d 696e  #Correct illumin
-0001fd40: 6174 696f 6e0d 0a20 2023 2069 6620 2863  ation..  # if (c
-0001fd50: 6f72 7265 6374 496c 6c75 6d69 6e61 7469  orrectIlluminati
-0001fd60: 6f6e 297b 0d0a 2020 2320 2020 6620 3d20  on){..  #   f = 
-0001fd70: 6565 2e49 6d61 6765 2874 732e 6669 7273  ee.Image(ts.firs
-0001fd80: 7428 2929 3b0d 0a20 2023 2020 204d 6170  t());..  #   Map
-0001fd90: 2e61 6464 4c61 7965 7228 662c 7669 7a50  .addLayer(f,vizP
-0001fda0: 6172 616d 7346 616c 7365 2c27 4669 7273  aramsFalse,'Firs
-0001fdb0: 742d 6e6f 6e2d 696c 6c75 6d69 6e61 7465  t-non-illuminate
-0001fdc0: 6427 2c66 616c 7365 293b 0d0a 0d0a 2020  d',false);....  
-0001fdd0: 2320 2020 7072 696e 7428 2743 6f72 7265  #   print('Corre
-0001fde0: 6374 696e 6720 696c 6c75 6d69 6e61 7469  cting illuminati
-0001fdf0: 6f6e 2729 3b0d 0a20 2023 2020 2074 7320  on');..  #   ts 
-0001fe00: 3d20 7473 2e6d 6170 2869 6c6c 756d 696e  = ts.map(illumin
-0001fe10: 6174 696f 6e43 6f6e 6469 7469 6f6e 290d  ationCondition).
-0001fe20: 0a20 2023 2020 2020 202e 6d61 7028 6675  .  #     .map(fu
-0001fe30: 6e63 7469 6f6e 2869 6d67 297b 0d0a 2020  nction(img){..  
-0001fe40: 2320 2020 2020 2020 7265 7475 726e 2069  #       return i
-0001fe50: 6c6c 756d 696e 6174 696f 6e43 6f72 7265  lluminationCorre
-0001fe60: 6374 696f 6e28 696d 672c 2063 6f72 7265  ction(img, corre
-0001fe70: 6374 5363 616c 652c 7374 7564 7941 7265  ctScale,studyAre
-0001fe80: 612c 5b20 2762 6c75 6527 2c20 2767 7265  a,[ 'blue', 'gre
-0001fe90: 656e 272c 2027 7265 6427 2c27 6e69 7227  en', 'red','nir'
-0001fea0: 2c27 7377 6972 3127 2c20 2773 7769 7232  ,'swir1', 'swir2
-0001feb0: 275d 293b 0d0a 2020 2320 2020 2020 7d29  ']);..  #     })
-0001fec0: 3b0d 0a20 2023 2020 2066 203d 2065 652e  ;..  #   f = ee.
-0001fed0: 496d 6167 6528 7473 2e66 6972 7374 2829  Image(ts.first()
-0001fee0: 293b 0d0a 2020 2320 2020 4d61 702e 6164  );..  #   Map.ad
-0001fef0: 644c 6179 6572 2866 2c76 697a 5061 7261  dLayer(f,vizPara
-0001ff00: 6d73 4661 6c73 652c 2746 6972 7374 2d69  msFalse,'First-i
-0001ff10: 6c6c 756d 696e 6174 6564 272c 6661 6c73  lluminated',fals
-0001ff20: 6529 3b0d 0a0d 0a20 2023 2045 7870 6f72  e);....  # Expor
-0001ff30: 7420 636f 6d70 6f73 6974 6573 0d0a 2020  t composites..  
-0001ff40: 6966 2065 7870 6f72 7443 6f6d 706f 7369  if exportComposi
-0001ff50: 7465 733a 0d0a 2020 2020 6578 706f 7274  tes:..    export
-0001ff60: 4261 6e64 4469 6374 203d 207b 5c0d 0a20  BandDict = {\.. 
-0001ff70: 2020 2020 2027 5352 5f6d 6564 6f69 6427       'SR_medoid'
-0001ff80: 3a5b 2763 6227 2c20 2762 6c75 6527 2c20  :['cb', 'blue', 
-0001ff90: 2767 7265 656e 272c 2027 7265 6427 2c20  'green', 'red', 
-0001ffa0: 2772 6531 272c 2772 6532 272c 2772 6533  're1','re2','re3
-0001ffb0: 272c 276e 6972 272c 2027 6e69 7232 272c  ','nir', 'nir2',
-0001ffc0: 2027 7761 7465 7256 6170 6f72 272c 2027   'waterVapor', '
-0001ffd0: 7377 6972 3127 2c20 2773 7769 7232 272c  swir1', 'swir2',
-0001ffe0: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-0001fff0: 6e74 272c 2773 656e 736f 7227 2c27 7965  nt','sensor','ye
-00020000: 6172 272c 276a 756c 6961 6e44 6179 275d  ar','julianDay']
-00020010: 2c0d 0a20 2020 2020 2027 5352 5f6d 6564  ,..      'SR_med
-00020020: 6961 6e27 3a5b 2763 6227 2c20 2762 6c75  ian':['cb', 'blu
-00020030: 6527 2c20 2767 7265 656e 272c 2027 7265  e', 'green', 're
-00020040: 6427 2c20 2772 6531 272c 2772 6532 272c  d', 're1','re2',
-00020050: 2772 6533 272c 276e 6972 272c 2027 6e69  're3','nir', 'ni
-00020060: 7232 272c 2027 7761 7465 7256 6170 6f72  r2', 'waterVapor
-00020070: 272c 2027 7377 6972 3127 2c20 2773 7769  ', 'swir1', 'swi
-00020080: 7232 272c 2763 6f6d 706f 7369 7465 4f62  r2','compositeOb
-00020090: 7343 6f75 6e74 275d 2c0d 0a20 2020 2020  sCount'],..     
-000200a0: 2027 544f 415f 6d65 646f 6964 273a 5b27   'TOA_medoid':['
-000200b0: 6362 272c 2027 626c 7565 272c 2027 6772  cb', 'blue', 'gr
-000200c0: 6565 6e27 2c20 2772 6564 272c 2027 7265  een', 'red', 're
-000200d0: 3127 2c27 7265 3227 2c27 7265 3327 2c27  1','re2','re3','
-000200e0: 6e69 7227 2c20 276e 6972 3227 2c20 2777  nir', 'nir2', 'w
-000200f0: 6174 6572 5661 706f 7227 2c20 2763 6972  aterVapor', 'cir
-00020100: 7275 7327 2c20 2773 7769 7231 272c 2027  rus', 'swir1', '
-00020110: 7377 6972 3227 2c27 636f 6d70 6f73 6974  swir2','composit
-00020120: 654f 6273 436f 756e 7427 2c27 7365 6e73  eObsCount','sens
-00020130: 6f72 272c 2779 6561 7227 2c27 6a75 6c69  or','year','juli
-00020140: 616e 4461 7927 5d2c 0d0a 2020 2020 2020  anDay'],..      
-00020150: 2754 4f41 5f6d 6564 6961 6e27 3a5b 2763  'TOA_median':['c
-00020160: 6227 2c20 2762 6c75 6527 2c20 2767 7265  b', 'blue', 'gre
-00020170: 656e 272c 2027 7265 6427 2c20 2772 6531  en', 'red', 're1
-00020180: 272c 2772 6532 272c 2772 6533 272c 276e  ','re2','re3','n
-00020190: 6972 272c 2027 6e69 7232 272c 2027 7761  ir', 'nir2', 'wa
-000201a0: 7465 7256 6170 6f72 272c 2027 6369 7272  terVapor', 'cirr
-000201b0: 7573 272c 2027 7377 6972 3127 2c20 2773  us', 'swir1', 's
-000201c0: 7769 7232 272c 2763 6f6d 706f 7369 7465  wir2','composite
-000201d0: 4f62 7343 6f75 6e74 275d 5c0d 0a20 2020  ObsCount']\..   
-000201e0: 207d 0d0a 2020 2020 6e6f 6e44 6976 6964   }..    nonDivid
-000201f0: 6542 616e 6444 6963 7420 3d20 7b5c 0d0a  eBandDict = {\..
-00020200: 2020 2020 2020 276d 6564 6f69 6427 3a5b        'medoid':[
-00020210: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-00020220: 6e74 272c 2773 656e 736f 7227 2c27 7965  nt','sensor','ye
-00020230: 6172 272c 276a 756c 6961 6e44 6179 275d  ar','julianDay']
-00020240: 2c0d 0a20 2020 2020 2027 6d65 6469 616e  ,..      'median
-00020250: 273a 5b27 636f 6d70 6f73 6974 654f 6273  ':['compositeObs
-00020260: 436f 756e 7427 5d5c 0d0a 2020 2020 7d0d  Count']\..    }.
-00020270: 0a20 2020 2065 7870 6f72 7442 616e 6473  .    exportBands
-00020280: 203d 2065 7870 6f72 7442 616e 6444 6963   = exportBandDic
-00020290: 745b 746f 614f 7253 5220 2b20 275f 2720  t[toaOrSR + '_' 
-000202a0: 2b20 636f 6d70 6f73 6974 696e 674d 6574  + compositingMet
-000202b0: 686f 645d 0d0a 2020 2020 6e6f 6e44 6976  hod]..    nonDiv
-000202c0: 6964 6542 616e 6473 203d 206e 6f6e 4469  ideBands = nonDi
-000202d0: 7669 6465 4261 6e64 4469 6374 5b63 6f6d  videBandDict[com
-000202e0: 706f 7369 7469 6e67 4d65 7468 6f64 5d0d  positingMethod].
-000202f0: 0a0d 0a20 2020 2065 7870 6f72 7443 6f6d  ...    exportCom
-00020300: 706f 7369 7465 436f 6c6c 6563 7469 6f6e  positeCollection
-00020310: 285c 0d0a 2020 2020 2020 636f 6c6c 6563  (\..      collec
-00020320: 7469 6f6e 203d 2074 732c 0d0a 2020 2020  tion = ts,..    
-00020330: 2020 6578 706f 7274 5061 7468 526f 6f74    exportPathRoot
-00020340: 203d 2065 7870 6f72 7450 6174 6852 6f6f   = exportPathRoo
-00020350: 742c 0d0a 2020 2020 2020 6f75 7470 7574  t,..      output
-00020360: 4e61 6d65 203d 206f 7574 7075 744e 616d  Name = outputNam
-00020370: 652c 0d0a 2020 2020 2020 6f72 6967 696e  e,..      origin
-00020380: 203d 206f 7269 6769 6e2c 0d0a 2020 2020   = origin,..    
-00020390: 2020 7374 7564 7941 7265 6120 3d20 7374    studyArea = st
-000203a0: 7564 7941 7265 612c 0d0a 2020 2020 2020  udyArea,..      
-000203b0: 6372 7320 3d20 6372 732c 0d0a 2020 2020  crs = crs,..    
-000203c0: 2020 7472 616e 7366 6f72 6d20 3d20 7472    transform = tr
-000203d0: 616e 7366 6f72 6d2c 0d0a 2020 2020 2020  ansform,..      
-000203e0: 7363 616c 6520 3d20 7363 616c 652c 0d0a  scale = scale,..
-000203f0: 2020 2020 2020 7374 6172 7459 6561 7220        startYear 
-00020400: 3d20 7374 6172 7459 6561 722c 0d0a 2020  = startYear,..  
-00020410: 2020 2020 656e 6459 6561 7220 3d20 656e      endYear = en
-00020420: 6459 6561 722c 0d0a 2020 2020 2020 7374  dYear,..      st
-00020430: 6172 744a 756c 6961 6e20 3d20 7374 6172  artJulian = star
-00020440: 744a 756c 6961 6e2c 0d0a 2020 2020 2020  tJulian,..      
-00020450: 656e 644a 756c 6961 6e20 3d20 656e 644a  endJulian = endJ
-00020460: 756c 6961 6e2c 0d0a 2020 2020 2020 636f  ulian,..      co
-00020470: 6d70 6f73 6974 696e 674d 6574 686f 6420  mpositingMethod 
-00020480: 3d20 636f 6d70 6f73 6974 696e 674d 6574  = compositingMet
-00020490: 686f 642c 0d0a 2020 2020 2020 7469 6d65  hod,..      time
-000204a0: 6275 6666 6572 203d 2074 696d 6562 7566  buffer = timebuf
-000204b0: 6665 722c 0d0a 2020 2020 2020 746f 614f  fer,..      toaO
-000204c0: 7253 5220 3d20 746f 614f 7253 522c 0d0a  rSR = toaOrSR,..
-000204d0: 2020 2020 2020 6e6f 6e44 6976 6964 6542        nonDivideB
-000204e0: 616e 6473 203d 206e 6f6e 4469 7669 6465  ands = nonDivide
-000204f0: 4261 6e64 732c 0d0a 2020 2020 2020 6578  Bands,..      ex
-00020500: 706f 7274 4261 6e64 7320 3d20 6578 706f  portBands = expo
-00020510: 7274 4261 6e64 732c 0d0a 2020 2020 2020  rtBands,..      
-00020520: 6164 6469 7469 6f6e 616c 5072 6f70 6572  additionalProper
-00020530: 7479 4469 6374 203d 2061 7267 732c 0d0a  tyDict = args,..
-00020540: 2020 2020 2020 6f76 6572 7772 6974 6520        overwrite 
-00020550: 3d20 6f76 6572 7772 6974 6529 0d0a 0d0a  = overwrite)....
-00020560: 2020 6172 6773 5b27 7072 6f63 6573 7365    args['processe
-00020570: 6453 6365 6e65 7327 5d20 3d20 7332 730d  dScenes'] = s2s.
-00020580: 0a20 2061 7267 735b 2770 726f 6365 7373  .  args['process
-00020590: 6564 436f 6d70 6f73 6974 6573 275d 203d  edComposites'] =
-000205a0: 2074 730d 0a0d 0a20 2072 6574 7572 6e20   ts....  return 
-000205b0: 6172 6773 0d0a 0d0a 2320 4879 6272 6964  args....# Hybrid
-000205c0: 2067 6574 204c 616e 6473 6174 2061 6e64   get Landsat and
-000205d0: 2053 656e 7469 6e65 6c20 3220 7072 6f63   Sentinel 2 proc
-000205e0: 6573 7365 6420 7363 656e 6573 0d0a 2320  essed scenes..# 
-000205f0: 4861 6e64 6c65 7320 6765 7474 696e 6720  Handles getting 
-00020600: 7072 6f63 6573 7365 6420 7363 656e 6573  processed scenes
-00020610: 2020 7769 7468 204c 616e 6473 6174 2061    with Landsat a
-00020620: 6e64 2053 656e 7469 6e65 6c20 320d 0a64  nd Sentinel 2..d
-00020630: 6566 2067 6574 5072 6f63 6573 7365 644c  ef getProcessedL
-00020640: 616e 6473 6174 416e 6453 656e 7469 6e65  andsatAndSentine
-00020650: 6c32 5363 656e 6573 280d 0a20 2020 2020  l2Scenes(..     
-00020660: 2073 7475 6479 4172 6561 2c0d 0a20 2020   studyArea,..   
-00020670: 2020 2073 7461 7274 5965 6172 2c0d 0a20     startYear,.. 
-00020680: 2020 2020 2065 6e64 5965 6172 2c0d 0a20       endYear,.. 
-00020690: 2020 2020 2073 7461 7274 4a75 6c69 616e       startJulian
-000206a0: 2c0d 0a20 2020 2020 2065 6e64 4a75 6c69  ,..      endJuli
-000206b0: 616e 2c0d 0a20 2020 2020 2074 6f61 4f72  an,..      toaOr
-000206c0: 5352 203d 2027 544f 4127 2c0d 0a20 2020  SR = 'TOA',..   
-000206d0: 2020 2069 6e63 6c75 6465 534c 434f 6666     includeSLCOff
-000206e0: 4c37 203d 2046 616c 7365 2c0d 0a20 2020  L7 = False,..   
-000206f0: 2020 2064 6566 7269 6e67 654c 3520 3d20     defringeL5 = 
-00020700: 4661 6c73 652c 0d0a 2020 2020 2020 6170  False,..      ap
-00020710: 706c 7951 4142 616e 6420 3d20 4661 6c73  plyQABand = Fals
-00020720: 652c 0d0a 2020 2020 2020 6170 706c 7943  e,..      applyC
-00020730: 6c6f 7564 5072 6f62 6162 696c 6974 7920  loudProbability 
-00020740: 3d20 5472 7565 2c0d 0a20 2020 2020 2061  = True,..      a
-00020750: 7070 6c79 5368 6164 6f77 5368 6966 7420  pplyShadowShift 
-00020760: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00020770: 6170 706c 7943 6c6f 7564 5363 6f72 654c  applyCloudScoreL
-00020780: 616e 6473 6174 203d 2046 616c 7365 2c0d  andsat = False,.
-00020790: 0a20 2020 2020 2061 7070 6c79 436c 6f75  .      applyClou
-000207a0: 6453 636f 7265 5365 6e74 696e 656c 3220  dScoreSentinel2 
-000207b0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-000207c0: 6170 706c 7954 444f 4d4c 616e 6473 6174  applyTDOMLandsat
-000207d0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-000207e0: 6170 706c 7954 444f 4d53 656e 7469 6e65  applyTDOMSentine
-000207f0: 6c32 203d 2054 7275 652c 0d0a 2020 2020  l2 = True,..    
-00020800: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
-00020810: 644d 6173 6b20 3d20 5472 7565 2c0d 0a20  dMask = True,.. 
-00020820: 2020 2020 2061 7070 6c79 466d 6173 6b43       applyFmaskC
-00020830: 6c6f 7564 5368 6164 6f77 4d61 736b 203d  loudShadowMask =
-00020840: 2054 7275 652c 0d0a 2020 2020 2020 6170   True,..      ap
-00020850: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
-00020860: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00020870: 2063 6c6f 7564 4865 6967 6874 7320 3d20   cloudHeights = 
-00020880: 6565 2e4c 6973 742e 7365 7175 656e 6365  ee.List.sequence
-00020890: 2835 3030 2c31 3030 3030 2c35 3030 292c  (500,10000,500),
-000208a0: 0d0a 2020 2020 2020 636c 6f75 6453 636f  ..      cloudSco
-000208b0: 7265 5468 7265 7368 203d 2032 302c 0d0a  reThresh = 20,..
-000208c0: 2020 2020 2020 7065 7266 6f72 6d43 6c6f        performClo
-000208d0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
-000208e0: 5472 7565 2c0d 0a20 2020 2020 2063 6c6f  True,..      clo
-000208f0: 7564 5363 6f72 6550 6374 6c20 3d20 3130  udScorePctl = 10
-00020900: 2c0d 0a20 2020 2020 207a 5363 6f72 6554  ,..      zScoreT
-00020910: 6872 6573 6820 3d20 2d31 2c0d 0a20 2020  hresh = -1,..   
-00020920: 2020 2073 6861 646f 7753 756d 5468 7265     shadowSumThre
-00020930: 7368 203d 2030 2e33 352c 0d0a 2020 2020  sh = 0.35,..    
-00020940: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
-00020950: 203d 2031 2e35 2c0d 0a20 2020 2020 2064   = 1.5,..      d
-00020960: 696c 6174 6550 6978 656c 7320 3d20 332e  ilatePixels = 3.
-00020970: 352c 0d0a 2020 2020 2020 7368 6164 6f77  5,..      shadow
-00020980: 5375 6d42 616e 6473 203d 205b 276e 6972  SumBands = ['nir
-00020990: 272c 2773 7769 7231 275d 2c0d 0a20 2020  ','swir1'],..   
-000209a0: 2020 206c 616e 6473 6174 5265 7361 6d70     landsatResamp
-000209b0: 6c65 4d65 7468 6f64 203d 2027 6e65 6172  leMethod = 'near
-000209c0: 272c 0d0a 2020 2020 2020 7365 6e74 696e  ',..      sentin
-000209d0: 656c 3252 6573 616d 706c 654d 6574 686f  el2ResampleMetho
-000209e0: 6420 3d20 2761 6767 7265 6761 7465 272c  d = 'aggregate',
-000209f0: 0d0a 2020 2020 2020 636f 6e76 6572 7454  ..      convertT
-00020a00: 6f44 6169 6c79 4d6f 7361 6963 7320 3d20  oDailyMosaics = 
-00020a10: 5472 7565 2c0d 0a20 2020 2020 2072 756e  True,..      run
-00020a20: 4368 6173 7461 696e 4861 726d 6f6e 697a  ChastainHarmoniz
-00020a30: 6174 696f 6e20 3d20 5472 7565 2c0d 0a20  ation = True,.. 
-00020a40: 2020 2020 2063 6f72 7265 6374 496c 6c75       correctIllu
-00020a50: 6d69 6e61 7469 6f6e 203d 2046 616c 7365  mination = False
-00020a60: 2c0d 0a20 2020 2020 2063 6f72 7265 6374  ,..      correct
-00020a70: 5363 616c 6520 3d20 3235 302c 0d0a 2020  Scale = 250,..  
-00020a80: 2020 2020 7072 6543 6f6d 7075 7465 644c      preComputedL
-00020a90: 616e 6473 6174 436c 6f75 6453 636f 7265  andsatCloudScore
-00020aa0: 4f66 6673 6574 203d 204e 6f6e 652c 0d0a  Offset = None,..
-00020ab0: 2020 2020 2020 7072 6543 6f6d 7075 7465        preCompute
-00020ac0: 644c 616e 6473 6174 5444 4f4d 4952 4d65  dLandsatTDOMIRMe
-00020ad0: 616e 203d 204e 6f6e 652c 0d0a 2020 2020  an = None,..    
-00020ae0: 2020 7072 6543 6f6d 7075 7465 644c 616e    preComputedLan
-00020af0: 6473 6174 5444 4f4d 4952 5374 6444 6576  dsatTDOMIRStdDev
-00020b00: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00020b10: 7072 6543 6f6d 7075 7465 6453 656e 7469  preComputedSenti
-00020b20: 6e65 6c32 436c 6f75 6453 636f 7265 4f66  nel2CloudScoreOf
-00020b30: 6673 6574 203d 204e 6f6e 652c 0d0a 2020  fset = None,..  
-00020b40: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
-00020b50: 656e 7469 6e65 6c32 5444 4f4d 4952 4d65  entinel2TDOMIRMe
-00020b60: 616e 203d 204e 6f6e 652c 0d0a 2020 2020  an = None,..    
-00020b70: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
-00020b80: 7469 6e65 6c32 5444 4f4d 4952 5374 6444  tinel2TDOMIRStdD
-00020b90: 6576 203d 204e 6f6e 652c 0d0a 2020 2020  ev = None,..    
-00020ba0: 2020 636c 6f75 6450 726f 6254 6872 6573    cloudProbThres
-00020bb0: 6820 3d20 3430 2c0d 0a20 2020 2020 206c  h = 40,..      l
-00020bc0: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
-00020bd0: 5665 7273 696f 6e20 3d20 2743 3227 293a  Version = 'C2'):
-00020be0: 0d0a 0d0a 2020 6966 2074 6f61 4f72 5352  ....  if toaOrSR
-00020bf0: 203d 3d20 2753 5227 3a0d 0a20 2020 2072   == 'SR':..    r
-00020c00: 756e 4368 6173 7461 696e 4861 726d 6f6e  unChastainHarmon
-00020c10: 697a 6174 696f 6e20 3d20 4661 6c73 650d  ization = False.
-00020c20: 0a0d 0a20 206f 7269 6769 6e20 3d20 274c  ...  origin = 'L
-00020c30: 616e 6473 6174 2d53 656e 7469 6e65 6c32  andsat-Sentinel2
-00020c40: 2d48 7962 7269 6427 0d0a 2020 746f 614f  -Hybrid'..  toaO
-00020c50: 7253 5220 3d20 746f 614f 7253 522e 7570  rSR = toaOrSR.up
-00020c60: 7065 7228 290d 0a0d 0a20 2023 5072 6570  per()....  #Prep
-00020c70: 6172 6520 6461 7465 730d 0a20 2023 5772  are dates..  #Wr
-00020c80: 6170 2074 6865 2064 6174 6573 2069 6620  ap the dates if 
-00020c90: 6e65 6564 6564 0d0a 2020 7772 6170 4f66  needed..  wrapOf
-00020ca0: 6673 6574 203d 2030 0d0a 2020 6966 2073  fset = 0..  if s
-00020cb0: 7461 7274 4a75 6c69 616e 203e 2065 6e64  tartJulian > end
-00020cc0: 4a75 6c69 616e 3a0d 0a20 2020 2077 7261  Julian:..    wra
-00020cd0: 704f 6666 7365 7420 3d20 3336 350d 0a20  pOffset = 365.. 
-00020ce0: 2073 7461 7274 4461 7465 203d 2065 652e   startDate = ee.
-00020cf0: 4461 7465 2e66 726f 6d59 4d44 2873 7461  Date.fromYMD(sta
-00020d00: 7274 5965 6172 2c31 2c31 292e 6164 7661  rtYear,1,1).adva
-00020d10: 6e63 6528 7374 6172 744a 756c 6961 6e2d  nce(startJulian-
-00020d20: 312c 2764 6179 2729 0d0a 2020 656e 6444  1,'day')..  endD
-00020d30: 6174 6520 3d20 6565 2e44 6174 652e 6672  ate = ee.Date.fr
-00020d40: 6f6d 594d 4428 656e 6459 6561 722c 312c  omYMD(endYear,1,
-00020d50: 3129 2e61 6476 616e 6365 2865 6e64 4a75  1).advance(endJu
-00020d60: 6c69 616e 2d31 2b77 7261 704f 6666 7365  lian-1+wrapOffse
-00020d70: 742c 2764 6179 2729 0d0a 0d0a 2020 6172  t,'day')....  ar
-00020d80: 6773 203d 2066 6f72 6d61 7441 7267 7328  gs = formatArgs(
-00020d90: 6c6f 6361 6c73 2829 290d 0a20 2069 6620  locals())..  if 
-00020da0: 2761 7267 7327 2069 6e20 6172 6773 2e6b  'args' in args.k
-00020db0: 6579 7328 293a 0d0a 2020 2020 6465 6c20  eys():..    del 
-00020dc0: 6172 6773 5b27 6172 6773 275d 0d0a 0d0a  args['args']....
-00020dd0: 2020 7072 696e 7428 2747 6574 2050 726f    print('Get Pro
-00020de0: 6365 7373 6564 204c 616e 6473 6174 2061  cessed Landsat a
-00020df0: 6e64 2053 656e 7469 6e65 6c32 2053 6365  nd Sentinel2 Sce
-00020e00: 6e65 733a 2027 290d 0a20 2070 7269 6e74  nes: ')..  print
-00020e10: 2827 5374 6172 7420 6461 7465 3a27 2c20  ('Start date:', 
-00020e20: 7374 6172 7444 6174 652e 666f 726d 6174  startDate.format
-00020e30: 2827 4d4d 4d20 6464 2079 7979 7927 292e  ('MMM dd yyyy').
-00020e40: 6765 7449 6e66 6f28 292c 272c 2045 6e64  getInfo(),', End
-00020e50: 2064 6174 653a 272c 2065 6e64 4461 7465   date:', endDate
-00020e60: 2e66 6f72 6d61 7428 274d 4d4d 2064 6420  .format('MMM dd 
-00020e70: 7979 7979 2729 2e67 6574 496e 666f 2829  yyyy').getInfo()
-00020e80: 290d 0a20 2066 6f72 2061 7267 2069 6e20  )..  for arg in 
-00020e90: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
-00020ea0: 2020 7072 696e 7428 6172 672c 2027 3a20    print(arg, ': 
-00020eb0: 272c 2061 7267 735b 6172 675d 290d 0a0d  ', args[arg])...
-00020ec0: 0a20 2023 4765 7420 4c61 6e64 7361 740d  .  #Get Landsat.
-00020ed0: 0a20 206c 7320 3d20 6765 7450 726f 6365  .  ls = getProce
-00020ee0: 7373 6564 4c61 6e64 7361 7453 6365 6e65  ssedLandsatScene
-00020ef0: 7328 5c0d 0a20 2020 2073 7475 6479 4172  s(\..    studyAr
-00020f00: 6561 203d 2073 7475 6479 4172 6561 2c0d  ea = studyArea,.
-00020f10: 0a20 2020 2073 7461 7274 5965 6172 203d  .    startYear =
-00020f20: 2073 7461 7274 5965 6172 2c0d 0a20 2020   startYear,..   
-00020f30: 2065 6e64 5965 6172 203d 2065 6e64 5965   endYear = endYe
-00020f40: 6172 2c0d 0a20 2020 2073 7461 7274 4a75  ar,..    startJu
-00020f50: 6c69 616e 203d 2073 7461 7274 4a75 6c69  lian = startJuli
-00020f60: 616e 2c0d 0a20 2020 2065 6e64 4a75 6c69  an,..    endJuli
-00020f70: 616e 203d 2065 6e64 4a75 6c69 616e 2c0d  an = endJulian,.
-00020f80: 0a20 2020 2074 6f61 4f72 5352 203d 2074  .    toaOrSR = t
-00020f90: 6f61 4f72 5352 2c0d 0a20 2020 2069 6e63  oaOrSR,..    inc
-00020fa0: 6c75 6465 534c 434f 6666 4c37 203d 2069  ludeSLCOffL7 = i
-00020fb0: 6e63 6c75 6465 534c 434f 6666 4c37 2c0d  ncludeSLCOffL7,.
-00020fc0: 0a20 2020 2064 6566 7269 6e67 654c 3520  .    defringeL5 
-00020fd0: 3d20 6465 6672 696e 6765 4c35 2c0d 0a20  = defringeL5,.. 
-00020fe0: 2020 2061 7070 6c79 436c 6f75 6453 636f     applyCloudSco
-00020ff0: 7265 203d 2061 7070 6c79 436c 6f75 6453  re = applyCloudS
-00021000: 636f 7265 4c61 6e64 7361 742c 0d0a 2020  coreLandsat,..  
-00021010: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
-00021020: 644d 6173 6b20 3d20 6170 706c 7946 6d61  dMask = applyFma
-00021030: 736b 436c 6f75 644d 6173 6b2c 0d0a 2020  skCloudMask,..  
-00021040: 2020 6170 706c 7954 444f 4d20 3d20 6170    applyTDOM = ap
-00021050: 706c 7954 444f 4d4c 616e 6473 6174 2c0d  plyTDOMLandsat,.
-00021060: 0a20 2020 2061 7070 6c79 466d 6173 6b43  .    applyFmaskC
-00021070: 6c6f 7564 5368 6164 6f77 4d61 736b 203d  loudShadowMask =
-00021080: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
-00021090: 5368 6164 6f77 4d61 736b 2c0d 0a20 2020  ShadowMask,..   
-000210a0: 2061 7070 6c79 466d 6173 6b53 6e6f 774d   applyFmaskSnowM
-000210b0: 6173 6b20 3d20 6170 706c 7946 6d61 736b  ask = applyFmask
-000210c0: 536e 6f77 4d61 736b 2c0d 0a20 2020 2063  SnowMask,..    c
-000210d0: 6c6f 7564 5363 6f72 6554 6872 6573 6820  loudScoreThresh 
-000210e0: 3d20 636c 6f75 6453 636f 7265 5468 7265  = cloudScoreThre
-000210f0: 7368 2c0d 0a20 2020 2070 6572 666f 726d  sh,..    perform
-00021100: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-00021110: 203d 2070 6572 666f 726d 436c 6f75 6453   = performCloudS
-00021120: 636f 7265 4f66 6673 6574 2c0d 0a20 2020  coreOffset,..   
-00021130: 2063 6c6f 7564 5363 6f72 6550 6374 6c20   cloudScorePctl 
-00021140: 3d20 636c 6f75 6453 636f 7265 5063 746c  = cloudScorePctl
-00021150: 2c0d 0a20 2020 207a 5363 6f72 6554 6872  ,..    zScoreThr
-00021160: 6573 6820 3d20 7a53 636f 7265 5468 7265  esh = zScoreThre
-00021170: 7368 2c0d 0a20 2020 2073 6861 646f 7753  sh,..    shadowS
-00021180: 756d 5468 7265 7368 203d 2073 6861 646f  umThresh = shado
-00021190: 7753 756d 5468 7265 7368 2c0d 0a20 2020  wSumThresh,..   
-000211a0: 2063 6f6e 7472 6163 7450 6978 656c 7320   contractPixels 
-000211b0: 3d20 636f 6e74 7261 6374 5069 7865 6c73  = contractPixels
-000211c0: 2c0d 0a20 2020 2064 696c 6174 6550 6978  ,..    dilatePix
-000211d0: 656c 7320 3d20 6469 6c61 7465 5069 7865  els = dilatePixe
-000211e0: 6c73 2c0d 0a20 2020 2073 6861 646f 7753  ls,..    shadowS
-000211f0: 756d 4261 6e64 7320 3d20 7368 6164 6f77  umBands = shadow
-00021200: 5375 6d42 616e 6473 2c0d 0a20 2020 2072  SumBands,..    r
-00021210: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
-00021220: 6c61 6e64 7361 7452 6573 616d 706c 654d  landsatResampleM
-00021230: 6574 686f 642c 0d0a 2020 2020 2368 6172  ethod,..    #har
-00021240: 6d6f 6e69 7a65 4f4c 4920 3d20 6861 726d  monizeOLI = harm
-00021250: 6f6e 697a 654f 4c49 2c0d 0a20 2020 2070  onizeOLI,..    p
-00021260: 7265 436f 6d70 7574 6564 436c 6f75 6453  reComputedCloudS
-00021270: 636f 7265 4f66 6673 6574 203d 2070 7265  coreOffset = pre
-00021280: 436f 6d70 7574 6564 4c61 6e64 7361 7443  ComputedLandsatC
-00021290: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
-000212a0: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
-000212b0: 6454 444f 4d49 524d 6561 6e20 3d20 7072  dTDOMIRMean = pr
-000212c0: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-000212d0: 5444 4f4d 4952 4d65 616e 2c0d 0a20 2020  TDOMIRMean,..   
-000212e0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
-000212f0: 4952 5374 6444 6576 203d 2070 7265 436f  IRStdDev = preCo
-00021300: 6d70 7574 6564 5365 6e74 696e 656c 3254  mputedSentinel2T
-00021310: 444f 4d49 5253 7464 4465 762c 0d0a 2020  DOMIRStdDev,..  
-00021320: 2020 6c61 6e64 7361 7443 6f6c 6c65 6374    landsatCollect
-00021330: 696f 6e56 6572 7369 6f6e 203d 206c 616e  ionVersion = lan
-00021340: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
-00021350: 7273 696f 6e29 0d0a 0d0a 2020 2347 6574  rsion)....  #Get
-00021360: 2053 656e 7469 6e65 6c20 320d 0a20 2073   Sentinel 2..  s
-00021370: 3273 203d 2067 6574 5072 6f63 6573 7365  2s = getProcesse
-00021380: 6453 656e 7469 6e65 6c32 5363 656e 6573  dSentinel2Scenes
-00021390: 285c 0d0a 2020 2020 7374 7564 7941 7265  (\..    studyAre
-000213a0: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
-000213b0: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
-000213c0: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
-000213d0: 656e 6459 6561 7220 3d20 656e 6459 6561  endYear = endYea
-000213e0: 722c 0d0a 2020 2020 7374 6172 744a 756c  r,..    startJul
-000213f0: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
-00021400: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
-00021410: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
-00021420: 2020 2020 6170 706c 7951 4142 616e 6420      applyQABand 
-00021430: 3d20 6170 706c 7951 4142 616e 642c 0d0a  = applyQABand,..
-00021440: 2020 2020 6170 706c 7943 6c6f 7564 5363      applyCloudSc
-00021450: 6f72 6520 3d20 6170 706c 7943 6c6f 7564  ore = applyCloud
-00021460: 5363 6f72 6553 656e 7469 6e65 6c32 2c0d  ScoreSentinel2,.
-00021470: 0a20 2020 2061 7070 6c79 5368 6164 6f77  .    applyShadow
-00021480: 5368 6966 7420 3d20 6170 706c 7953 6861  Shift = applySha
-00021490: 646f 7753 6869 6674 2c0d 0a20 2020 2061  dowShift,..    a
-000214a0: 7070 6c79 5444 4f4d 203d 2061 7070 6c79  pplyTDOM = apply
-000214b0: 5444 4f4d 5365 6e74 696e 656c 322c 0d0a  TDOMSentinel2,..
-000214c0: 2020 2020 636c 6f75 6453 636f 7265 5468      cloudScoreTh
-000214d0: 7265 7368 203d 2063 6c6f 7564 5363 6f72  resh = cloudScor
-000214e0: 6554 6872 6573 682c 0d0a 2020 2020 7065  eThresh,..    pe
-000214f0: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
-00021500: 6666 7365 7420 3d20 7065 7266 6f72 6d43  ffset = performC
-00021510: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
-00021520: 0d0a 2020 2020 636c 6f75 6453 636f 7265  ..    cloudScore
-00021530: 5063 746c 203d 2063 6c6f 7564 5363 6f72  Pctl = cloudScor
-00021540: 6550 6374 6c2c 0d0a 2020 2020 636c 6f75  ePctl,..    clou
-00021550: 6448 6569 6768 7473 203d 2063 6c6f 7564  dHeights = cloud
-00021560: 4865 6967 6874 732c 0d0a 2020 2020 7a53  Heights,..    zS
-00021570: 636f 7265 5468 7265 7368 203d 207a 5363  coreThresh = zSc
-00021580: 6f72 6554 6872 6573 682c 0d0a 2020 2020  oreThresh,..    
-00021590: 7368 6164 6f77 5375 6d54 6872 6573 6820  shadowSumThresh 
-000215a0: 3d20 7368 6164 6f77 5375 6d54 6872 6573  = shadowSumThres
-000215b0: 682c 0d0a 2020 2020 636f 6e74 7261 6374  h,..    contract
-000215c0: 5069 7865 6c73 203d 2063 6f6e 7472 6163  Pixels = contrac
-000215d0: 7450 6978 656c 732c 0d0a 2020 2020 6469  tPixels,..    di
-000215e0: 6c61 7465 5069 7865 6c73 203d 2064 696c  latePixels = dil
-000215f0: 6174 6550 6978 656c 732c 0d0a 2020 2020  atePixels,..    
-00021600: 7368 6164 6f77 5375 6d42 616e 6473 203d  shadowSumBands =
-00021610: 2073 6861 646f 7753 756d 4261 6e64 732c   shadowSumBands,
-00021620: 0d0a 2020 2020 7265 7361 6d70 6c65 4d65  ..    resampleMe
-00021630: 7468 6f64 203d 2073 656e 7469 6e65 6c32  thod = sentinel2
-00021640: 5265 7361 6d70 6c65 4d65 7468 6f64 2c0d  ResampleMethod,.
-00021650: 0a20 2020 2074 6f61 4f72 5352 203d 2074  .    toaOrSR = t
-00021660: 6f61 4f72 5352 2c0d 0a20 2020 2063 6f6e  oaOrSR,..    con
-00021670: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
-00021680: 6373 203d 2063 6f6e 7665 7274 546f 4461  cs = convertToDa
-00021690: 696c 794d 6f73 6169 6373 2c0d 0a20 2020  ilyMosaics,..   
-000216a0: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
-000216b0: 6269 6c69 7479 203d 2061 7070 6c79 436c  bility = applyCl
-000216c0: 6f75 6450 726f 6261 6269 6c69 7479 2c0d  oudProbability,.
-000216d0: 0a20 2020 2070 7265 436f 6d70 7574 6564  .    preComputed
-000216e0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-000216f0: 203d 2070 7265 436f 6d70 7574 6564 5365   = preComputedSe
-00021700: 6e74 696e 656c 3243 6c6f 7564 5363 6f72  ntinel2CloudScor
-00021710: 654f 6666 7365 742c 0d0a 2020 2020 7072  eOffset,..    pr
-00021720: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
-00021730: 6561 6e20 3d20 7072 6543 6f6d 7075 7465  ean = preCompute
-00021740: 6453 656e 7469 6e65 6c32 5444 4f4d 4952  dSentinel2TDOMIR
-00021750: 4d65 616e 2c0d 0a20 2020 2070 7265 436f  Mean,..    preCo
-00021760: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
-00021770: 6576 203d 2070 7265 436f 6d70 7574 6564  ev = preComputed
-00021780: 5365 6e74 696e 656c 3254 444f 4d49 5253  Sentinel2TDOMIRS
-00021790: 7464 4465 762c 0d0a 2020 2020 636c 6f75  tdDev,..    clou
-000217a0: 6450 726f 6254 6872 6573 6820 3d20 636c  dProbThresh = cl
-000217b0: 6f75 6450 726f 6254 6872 6573 6829 0d0a  oudProbThresh)..
-000217c0: 0d0a 0d0a 2020 2353 656c 6563 7420 6f66  ....  #Select of
-000217d0: 6620 636f 6d6d 6f6e 2062 616e 6473 2062  f common bands b
-000217e0: 6574 7765 656e 204c 616e 6473 6174 2061  etween Landsat a
-000217f0: 6e64 2053 656e 7469 6e65 6c20 320d 0a20  nd Sentinel 2.. 
-00021800: 2063 6f6d 6d6f 6e42 616e 6473 203d 2020   commonBands =  
-00021810: 5b27 626c 7565 272c 2027 6772 6565 6e27  ['blue', 'green'
-00021820: 2c20 2772 6564 272c 2027 6e69 7227 2c20  , 'red', 'nir', 
-00021830: 2773 7769 7231 272c 2027 7377 6972 3227  'swir1', 'swir2'
-00021840: 2c20 2773 656e 736f 7227 5d0d 0a20 206c  , 'sensor']..  l
-00021850: 7320 3d20 6c73 2e73 656c 6563 7428 636f  s = ls.select(co
-00021860: 6d6d 6f6e 4261 6e64 7329 0d0a 2020 7332  mmonBands)..  s2
-00021870: 7320 3d20 7332 732e 7365 6c65 6374 2863  s = s2s.select(c
-00021880: 6f6d 6d6f 6e42 616e 6473 290d 0a20 2023  ommonBands)..  #
-00021890: 4669 6c6c 2069 6e20 616e 7920 656d 7074  Fill in any empt
-000218a0: 7920 636f 6c6c 6563 7469 6f6e 730d 0a20  y collections.. 
-000218b0: 2023 4966 2074 6865 7927 7265 2062 6f74   #If they're bot
-000218c0: 6820 656d 7074 792c 2074 6869 7320 7769  h empty, this wi
-000218d0: 6c6c 206e 6f74 2077 6f72 6b0d 0a20 2064  ll not work..  d
-000218e0: 756d 6d79 496d 6167 6520 3d65 652e 496d  ummyImage =ee.Im
-000218f0: 6167 6528 6565 2e49 6d61 6765 436f 6c6c  age(ee.ImageColl
-00021900: 6563 7469 6f6e 2865 652e 416c 676f 7269  ection(ee.Algori
-00021910: 7468 6d73 2e49 6628 6c73 2e74 6f4c 6973  thms.If(ls.toLis
-00021920: 7428 3129 2e6c 656e 6774 6828 292e 6774  t(1).length().gt
-00021930: 2830 292c 6c73 2c73 3273 2929 2e66 6972  (0),ls,s2s)).fir
-00021940: 7374 2829 290d 0a20 206c 7320 3d20 6669  st())..  ls = fi
-00021950: 6c6c 456d 7074 7943 6f6c 6c65 6374 696f  llEmptyCollectio
-00021960: 6e73 286c 732c 6475 6d6d 7949 6d61 6765  ns(ls,dummyImage
-00021970: 290d 0a20 2073 3273 203d 2066 696c 6c45  )..  s2s = fillE
-00021980: 6d70 7479 436f 6c6c 6563 7469 6f6e 7328  mptyCollections(
-00021990: 7332 732c 6475 6d6d 7949 6d61 6765 290d  s2s,dummyImage).
-000219a0: 0a0d 0a0d 0a20 2069 6620 7275 6e43 6861  .....  if runCha
-000219b0: 7374 6169 6e48 6172 6d6f 6e69 7a61 7469  stainHarmonizati
-000219c0: 6f6e 2061 6e64 2074 6f61 4f72 5352 203d  on and toaOrSR =
-000219d0: 3d20 2754 4f41 273a 0d0a 0d0a 2020 2020  = 'TOA':....    
-000219e0: 2320 5365 7061 7261 7465 2065 6163 6820  # Separate each 
-000219f0: 7365 6e73 6f72 0d0a 0d0a 2020 2020 746d  sensor....    tm
-00021a00: 203d 206c 732e 6669 6c74 6572 2865 652e   = ls.filter(ee.
-00021a10: 4669 6c74 6572 2e69 6e4c 6973 7428 2753  Filter.inList('S
-00021a20: 454e 534f 525f 4944 272c 5b27 544d 272c  ENSOR_ID',['TM',
-00021a30: 2745 544d 275d 2929 0d0a 2020 2020 6f6c  'ETM']))..    ol
-00021a40: 6920 3d20 6c73 2e66 696c 7465 7228 6565  i = ls.filter(ee
-00021a50: 2e46 696c 7465 722e 6571 2827 5345 4e53  .Filter.eq('SENS
-00021a60: 4f52 5f49 4427 2c27 4f4c 495f 5449 5253  OR_ID','OLI_TIRS
-00021a70: 2729 290d 0a20 2020 2023 2065 6c73 653a  '))..    # else:
-00021a80: 0d0a 2020 2020 2320 2020 746d 203d 206c  ..    #   tm = l
-00021a90: 732e 6669 6c74 6572 2865 652e 4669 6c74  s.filter(ee.Filt
-00021aa0: 6572 2e69 6e4c 6973 7428 2773 656e 736f  er.inList('senso
-00021ab0: 7227 2c5b 274c 414e 4453 4154 5f34 272c  r',['LANDSAT_4',
-00021ac0: 274c 414e 4453 4154 5f35 272c 274c 414e  'LANDSAT_5','LAN
-00021ad0: 4453 4154 5f37 275d 2929 0d0a 2020 2020  DSAT_7']))..    
-00021ae0: 2320 2020 6f6c 6920 3d20 6c73 2e66 696c  #   oli = ls.fil
-00021af0: 7465 7228 6565 2e46 696c 7465 722e 6571  ter(ee.Filter.eq
-00021b00: 2827 7365 6e73 6f72 272c 274c 414e 4453  ('sensor','LANDS
-00021b10: 4154 5f38 2729 290d 0a20 2020 206d 7369  AT_8'))..    msi
-00021b20: 203d 2073 3273 0d0a 0d0a 2020 2020 2320   = s2s....    # 
-00021b30: 4669 6c6c 2069 6620 6e6f 2069 6d61 6765  Fill if no image
-00021b40: 7320 6578 6973 7420 666f 7220 7061 7274  s exist for part
-00021b50: 6963 756c 6172 204c 616e 6473 6174 2073  icular Landsat s
-00021b60: 656e 736f 720d 0a20 2020 2023 2041 6c6c  ensor..    # All
-00021b70: 6f77 2069 7420 746f 2066 6169 6c20 6f66  ow it to fail of
-00021b80: 206e 6f20 696d 6167 6573 2065 7869 7374   no images exist
-00021b90: 2066 6f72 2053 656e 7469 6e65 6c20 3220   for Sentinel 2 
-00021ba0: 7369 6e63 6520 7468 6520 706f 696e 740d  since the point.
-00021bb0: 0a20 2020 2023 206f 6620 7468 6973 206d  .    # of this m
-00021bc0: 6574 686f 6420 6973 2074 6f20 696e 636c  ethod is to incl
-00021bd0: 7564 6520 5332 0d0a 2020 2020 746d 203d  ude S2..    tm =
-00021be0: 2066 696c 6c45 6d70 7479 436f 6c6c 6563   fillEmptyCollec
-00021bf0: 7469 6f6e 7328 746d 2c20 6565 2e49 6d61  tions(tm, ee.Ima
-00021c00: 6765 286c 732e 6669 7273 7428 2929 290d  ge(ls.first())).
-00021c10: 0a20 2020 206f 6c69 203d 2066 696c 6c45  .    oli = fillE
-00021c20: 6d70 7479 436f 6c6c 6563 7469 6f6e 7328  mptyCollections(
-00021c30: 6f6c 692c 2065 652e 496d 6167 6528 6c73  oli, ee.Image(ls
-00021c40: 2e66 6972 7374 2829 2929 0d0a 0d0a 2020  .first()))....  
-00021c50: 2020 7072 696e 7428 2752 756e 6e69 6e67    print('Running
-00021c60: 2043 6861 7374 6169 6e20 6574 2061 6c20   Chastain et al 
-00021c70: 3230 3139 2068 6172 6d6f 6e69 7a61 7469  2019 harmonizati
-00021c80: 6f6e 2729 0d0a 0d0a 2020 2020 2341 7070  on')....    #App
-00021c90: 6c79 2063 6f72 7265 6374 696f 6e0d 0a20  ly correction.. 
-00021ca0: 2020 2023 4375 7272 656e 746c 7920 636f     #Currently co
-00021cb0: 6465 6420 746f 2067 6f20 746f 2045 544d  ded to go to ETM
-00021cc0: 2b0d 0a0d 0a20 2020 2023 4e6f 206e 6565  +....    #No nee
-00021cd0: 6420 746f 2063 6f72 7265 6374 2045 544d  d to correct ETM
-00021ce0: 2074 6f20 4554 4d0d 0a20 2020 2023 2074   to ETM..    # t
-00021cf0: 6d20 3d20 746d 2e6d 6170 2866 756e 6374  m = tm.map(funct
-00021d00: 696f 6e28 696d 6729 7b72 6574 7572 6e20  ion(img){return 
-00021d10: 6765 7449 6d61 6765 734c 6962 2e68 6172  getImagesLib.har
-00021d20: 6d6f 6e69 7a61 7469 6f6e 4368 6173 7461  monizationChasta
-00021d30: 696e 2869 6d67 2c20 2745 544d 272c 2745  in(img, 'ETM','E
-00021d40: 544d 2729 7d29 0d0a 2020 2020 2320 6574  TM')})..    # et
-00021d50: 6d20 3d20 6574 6d2e 6d61 7028 6675 6e63  m = etm.map(func
-00021d60: 7469 6f6e 2869 6d67 297b 7265 7475 726e  tion(img){return
-00021d70: 2067 6574 496d 6167 6573 4c69 622e 6861   getImagesLib.ha
-00021d80: 726d 6f6e 697a 6174 696f 6e43 6861 7374  rmonizationChast
-00021d90: 6169 6e28 696d 672c 2027 4554 4d27 2c27  ain(img, 'ETM','
-00021da0: 4554 4d27 297d 290d 0a0d 0a20 2020 2023  ETM')})....    #
-00021db0: 4861 726d 6f6e 697a 6520 7468 6520 6f74  Harmonize the ot
-00021dc0: 6865 7220 7477 6f0d 0a20 2020 206f 6c69  her two..    oli
-00021dd0: 203d 206f 6c69 2e6d 6170 286c 616d 6264   = oli.map(lambd
-00021de0: 6120 696d 673a 2068 6172 6d6f 6e69 7a61  a img: harmoniza
-00021df0: 7469 6f6e 4368 6173 7461 696e 2869 6d67  tionChastain(img
-00021e00: 2c20 274f 4c49 272c 2745 544d 2729 290d  , 'OLI','ETM')).
-00021e10: 0a20 2020 206d 7369 203d 206d 7369 2e6d  .    msi = msi.m
-00021e20: 6170 286c 616d 6264 6120 696d 673a 2068  ap(lambda img: h
-00021e30: 6172 6d6f 6e69 7a61 7469 6f6e 4368 6173  armonizationChas
-00021e40: 7461 696e 2869 6d67 2c20 274d 5349 272c  tain(img, 'MSI',
-00021e50: 2745 544d 2729 290d 0a0d 0a20 2020 2073  'ETM'))....    s
-00021e60: 3273 203d 206d 7369 0d0a 0d0a 2020 2020  2s = msi....    
-00021e70: 234d 6572 6765 204c 616e 6473 6174 2062  #Merge Landsat b
-00021e80: 6163 6b20 746f 6765 7468 6572 0d0a 2020  ack together..  
-00021e90: 2020 6c73 203d 2065 652e 496d 6167 6543    ls = ee.ImageC
-00021ea0: 6f6c 6c65 6374 696f 6e28 746d 2e6d 6572  ollection(tm.mer
-00021eb0: 6765 286f 6c69 2929 0d0a 0d0a 0d0a 2020  ge(oli))......  
-00021ec0: 2320 4d65 7267 6520 4c61 6e64 7361 7420  # Merge Landsat 
-00021ed0: 616e 6420 5332 0d0a 2020 6d65 7267 6564  and S2..  merged
-00021ee0: 203d 2065 652e 496d 6167 6543 6f6c 6c65   = ee.ImageColle
-00021ef0: 6374 696f 6e28 6c73 2e6d 6572 6765 2873  ction(ls.merge(s
-00021f00: 3273 2929 0d0a 2020 6d65 7267 6564 203d  2s))..  merged =
-00021f10: 206d 6572 6765 642e 6d61 7028 7369 6d70   merged.map(simp
-00021f20: 6c65 4164 6449 6e64 6963 6573 295c 0d0a  leAddIndices)\..
-00021f30: 2020 2020 2020 2020 2020 2020 2e6d 6170              .map
-00021f40: 2867 6574 5461 7373 656c 6564 4361 7029  (getTasseledCap)
-00021f50: 5c0d 0a20 2020 2020 2020 2020 2020 202e  \..            .
-00021f60: 6d61 7028 7369 6d70 6c65 4164 6454 4341  map(simpleAddTCA
-00021f70: 6e67 6c65 7329 0d0a 0d0a 2020 6d65 7267  ngles)....  merg
-00021f80: 6564 203d 206d 6572 6765 642e 7365 7428  ed = merged.set(
-00021f90: 6172 6773 290d 0a0d 0a0d 0a20 2072 6574  args)......  ret
-00021fa0: 7572 6e20 6d65 7267 6564 0d0a 2323 2323  urn merged..####
-00021fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021ff0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-00022000: 4675 6e63 7469 6f6e 2074 6f20 7265 6769  Function to regi
-00022010: 7374 6572 2061 6e20 696d 6167 6543 6f6c  ster an imageCol
-00022020: 6c65 6374 696f 6e20 746f 2069 6d61 6765  lection to image
-00022030: 7320 7769 7468 696e 2069 740d 0a23 416c  s within it..#Al
-00022040: 7761 7973 2075 7365 7320 7468 6520 6669  ways uses the fi
-00022050: 7273 7420 696d 6167 6520 6173 2074 6865  rst image as the
-00022060: 2072 6566 6572 656e 6365 2069 6d61 6765   reference image
-00022070: 0d0a 6465 6620 636f 5265 6769 7374 6572  ..def coRegister
-00022080: 436f 6c6c 6563 7469 6f6e 2869 6d61 6765  Collection(image
-00022090: 732c 7265 6665 7265 6e63 6542 616e 6473  s,referenceBands
-000220a0: 203d 205b 276e 6972 275d 293a 0d0a 2020   = ['nir']):..  
-000220b0: 2020 7265 6665 7265 6e63 6549 6d61 6765    referenceImage
-000220c0: 496e 6465 7820 3d20 300d 0a20 2020 2072  Index = 0..    r
-000220d0: 6566 6572 656e 6365 496d 6167 6520 3d20  eferenceImage = 
-000220e0: 6565 2e49 6d61 6765 2869 6d61 6765 732e  ee.Image(images.
-000220f0: 746f 4c69 7374 2872 6566 6572 656e 6365  toList(reference
-00022100: 496d 6167 6549 6e64 6578 2b31 292e 6765  ImageIndex+1).ge
-00022110: 7428 7265 6665 7265 6e63 6549 6d61 6765  t(referenceImage
-00022120: 496e 6465 7829 292e 7365 6c65 6374 2872  Index)).select(r
-00022130: 6566 6572 656e 6365 4261 6e64 7329 0d0a  eferenceBands)..
-00022140: 0d0a 2020 2020 6465 6620 7265 6769 7374  ..    def regist
-00022150: 6572 496d 6167 6528 696d 6167 6529 3a0d  erImage(image):.
-00022160: 0a20 2020 2020 2020 2023 4465 7465 726d  .        #Determ
-00022170: 696e 6520 7468 6520 6469 7370 6c61 6365  ine the displace
-00022180: 6d65 6e74 2062 7920 6d61 7463 6869 6e67  ment by matching
-00022190: 206f 6e6c 7920 7468 6520 7265 6665 7265   only the refere
-000221a0: 6e63 6542 616e 6420 6261 6e64 732e 0d0a  nceBand bands...
-000221b0: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
-000221c0: 6d65 6e74 5f70 6172 616d 7320 3d20 7b0d  ment_params = {.
-000221d0: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
-000221e0: 6665 7265 6e63 6549 6d61 6765 273a 2072  ferenceImage': r
-000221f0: 6566 6572 656e 6365 496d 6167 652c 0d0a  eferenceImage,..
-00022200: 2020 2020 2020 2020 2020 2020 276d 6178              'max
-00022210: 4f66 6673 6574 273a 2032 302e 302c 0d0a  Offset': 20.0,..
-00022220: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-00022230: 6a65 6374 696f 6e27 3a20 4e6f 6e65 2c0d  jection': None,.
-00022240: 0a20 2020 2020 2020 2020 2020 2027 7061  .            'pa
-00022250: 7463 6857 6964 7468 273a 2032 302e 302c  tchWidth': 20.0,
-00022260: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
-00022270: 7469 6666 6e65 7373 273a 2035 0d0a 2020  tiffness': 5..  
-00022280: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00022290: 2020 2020 2064 6973 706c 6163 656d 656e       displacemen
-000222a0: 7420 3d20 696d 6167 652e 7365 6c65 6374  t = image.select
-000222b0: 2872 6566 6572 656e 6365 4261 6e64 7329  (referenceBands)
-000222c0: 2e64 6973 706c 6163 656d 656e 7428 2a2a  .displacement(**
-000222d0: 6469 7370 6c61 6365 6d65 6e74 5f70 6172  displacement_par
-000222e0: 616d 7329 0d0a 2020 2020 2020 2020 7265  ams)..        re
-000222f0: 7475 726e 2069 6d61 6765 2e64 6973 706c  turn image.displ
-00022300: 6163 6528 6469 7370 6c61 6365 6d65 6e74  ace(displacement
-00022310: 290d 0a0d 0a20 2020 206f 7574 203d 2065  )....    out = e
-00022320: 652e 496d 6167 6543 6f6c 6c65 6374 696f  e.ImageCollectio
-00022330: 6e28 6565 2e49 6d61 6765 436f 6c6c 6563  n(ee.ImageCollec
-00022340: 7469 6f6e 2869 6d61 6765 732e 746f 4c69  tion(images.toLi
-00022350: 7374 2831 3030 3030 2c31 2929 2e6d 6170  st(10000,1)).map
-00022360: 2872 6567 6973 7465 7249 6d61 6765 2929  (registerImage))
-00022370: 2328 6565 2e49 6d61 6765 2869 6d61 6765  #(ee.Image(image
-00022380: 732e 746f 4c69 7374 2831 3030 3030 2c30  s.toList(10000,0
-00022390: 292e 6765 7428 3129 292c 7265 6665 7265  ).get(1)),refere
-000223a0: 6e63 6549 6d61 6765 290d 0a20 2020 206f  nceImage)..    o
-000223b0: 7574 203d 2065 652e 496d 6167 6543 6f6c  ut = ee.ImageCol
-000223c0: 6c65 6374 696f 6e28 696d 6167 6573 2e6c  lection(images.l
-000223d0: 696d 6974 2831 292e 6d65 7267 6528 6f75  imit(1).merge(ou
-000223e0: 7429 290d 0a0d 0a20 2020 2072 6574 7572  t))....    retur
-000223f0: 6e20 6f75 740d 0a23 2323 2323 2323 2323  n out..#########
-00022400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022440: 2323 2323 2323 2323 0d0a 2346 756e 6374  ########..#Funct
-00022450: 696f 6e20 746f 2066 696e 6420 6120 7375  ion to find a su
-00022460: 6273 6574 206f 6620 6120 636f 6c6c 6563  bset of a collec
-00022470: 7469 6f6e 0d0a 2346 6f72 2065 6163 6820  tion..#For each 
-00022480: 6772 6f75 7020 2865 2e67 2e20 7469 6c65  group (e.g. tile
-00022490: 206f 7220 6f72 6269 7420 6f72 2070 6174   or orbit or pat
-000224a0: 6829 2c20 616c 6c20 696d 6167 6573 2077  h), all images w
-000224b0: 6974 6869 6e20 7468 6174 2067 726f 7570  ithin that group
-000224c0: 2077 696c 6c20 6265 2072 6567 6973 7465   will be registe
-000224d0: 7265 640d 0a23 4173 2073 696e 676c 6520  red..#As single 
-000224e0: 636f 6c6c 6563 7469 6f6e 2069 7320 7265  collection is re
-000224f0: 7475 726e 6564 0d0a 6465 6620 636f 5265  turned..def coRe
-00022500: 6769 7374 6572 4772 6f75 7073 2869 6d67  gisterGroups(img
-00022510: 732c 6669 656c 644e 616d 6520 3d20 2753  s,fieldName = 'S
-00022520: 454e 5349 4e47 5f4f 5242 4954 5f4e 554d  ENSING_ORBIT_NUM
-00022530: 4245 5227 2c66 6965 6c64 4973 4e75 6d65  BER',fieldIsNume
-00022540: 7269 6320 3d20 5472 7565 293a 0d0a 2020  ric = True):..  
-00022550: 2020 6772 6f75 7073 203d 2065 652e 4469    groups = ee.Di
-00022560: 6374 696f 6e61 7279 2869 6d67 732e 6167  ctionary(imgs.ag
-00022570: 6772 6567 6174 655f 6869 7374 6f67 7261  gregate_histogra
-00022580: 6d28 6669 656c 644e 616d 6529 292e 6b65  m(fieldName)).ke
-00022590: 7973 2829 0d0a 2020 2020 6966 2066 6965  ys()..    if fie
-000225a0: 6c64 4973 4e75 6d65 7269 633a 0d0a 2020  ldIsNumeric:..  
-000225b0: 2020 2020 2020 6772 6f75 7073 203d 2067        groups = g
-000225c0: 726f 7570 732e 6d61 7028 6c61 6d62 6461  roups.map(lambda
-000225d0: 206e 3a20 6565 2e4e 756d 6265 722e 7061   n: ee.Number.pa
-000225e0: 7273 6528 6e29 290d 0a0d 0a20 2020 206f  rse(n))....    o
-000225f0: 7574 203d 6565 2e49 6d61 6765 436f 6c6c  ut =ee.ImageColl
-00022600: 6563 7469 6f6e 2865 652e 4665 6174 7572  ection(ee.Featur
-00022610: 6543 6f6c 6c65 6374 696f 6e28 6772 6f75  eCollection(grou
-00022620: 7073 2e6d 6170 286c 616d 6264 6120 6772  ps.map(lambda gr
-00022630: 6f75 703a 636f 5265 6769 7374 6572 436f  oup:coRegisterCo
-00022640: 6c6c 6563 7469 6f6e 2869 6d67 732e 6669  llection(imgs.fi
-00022650: 6c74 6572 2865 652e 4669 6c74 6572 2e65  lter(ee.Filter.e
-00022660: 7128 6669 656c 644e 616d 652c 6772 6f75  q(fieldName,grou
-00022670: 7029 2929 2929 2e66 6c61 7474 656e 2829  p))))).flatten()
-00022680: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
-00022690: 6f75 740d 0a23 2323 2323 2323 2323 2323  out..###########
-000226a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000226b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000226c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000226d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000226e0: 2323 2323 2323 0d0a 6465 6620 6765 744c  ######..def getL
-000226f0: 616e 6473 6174 416e 6453 656e 7469 6e65  andsatAndSentine
-00022700: 6c32 4879 6272 6964 5772 6170 7065 7228  l2HybridWrapper(
-00022710: 5c0d 0a20 2073 7475 6479 4172 6561 2c0d  \..  studyArea,.
-00022720: 0a20 2073 7461 7274 5965 6172 2c0d 0a20  .  startYear,.. 
-00022730: 2065 6e64 5965 6172 2c0d 0a20 2073 7461   endYear,..  sta
-00022740: 7274 4a75 6c69 616e 2c0d 0a20 2065 6e64  rtJulian,..  end
-00022750: 4a75 6c69 616e 2c0d 0a20 2074 696d 6562  Julian,..  timeb
-00022760: 7566 6665 7220 3d20 2030 2c0d 0a20 2077  uffer =  0,..  w
-00022770: 6569 6768 7473 203d 2020 5b31 5d2c 0d0a  eights =  [1],..
-00022780: 2020 636f 6d70 6f73 6974 696e 674d 6574    compositingMet
-00022790: 686f 6420 3d20 276d 6564 6f69 6427 2c0d  hod = 'medoid',.
-000227a0: 0a20 2074 6f61 4f72 5352 203d 2027 544f  .  toaOrSR = 'TO
-000227b0: 4127 2c0d 0a20 2069 6e63 6c75 6465 534c  A',..  includeSL
-000227c0: 434f 6666 4c37 203d 2046 616c 7365 2c0d  COffL7 = False,.
-000227d0: 0a20 2064 6566 7269 6e67 654c 3520 3d20  .  defringeL5 = 
-000227e0: 4661 6c73 652c 0d0a 2020 6170 706c 7951  False,..  applyQ
-000227f0: 4142 616e 6420 3d20 4661 6c73 652c 0d0a  ABand = False,..
-00022800: 2020 6170 706c 7943 6c6f 7564 5072 6f62    applyCloudProb
-00022810: 6162 696c 6974 7920 3d20 5472 7565 2c0d  ability = True,.
-00022820: 0a20 2061 7070 6c79 5368 6164 6f77 5368  .  applyShadowSh
-00022830: 6966 7420 3d20 4661 6c73 652c 0d0a 2020  ift = False,..  
-00022840: 6170 706c 7943 6c6f 7564 5363 6f72 654c  applyCloudScoreL
-00022850: 616e 6473 6174 203d 2046 616c 7365 2c0d  andsat = False,.
-00022860: 0a20 2061 7070 6c79 436c 6f75 6453 636f  .  applyCloudSco
-00022870: 7265 5365 6e74 696e 656c 3220 3d20 4661  reSentinel2 = Fa
-00022880: 6c73 652c 0d0a 2020 6170 706c 7954 444f  lse,..  applyTDO
-00022890: 4d4c 616e 6473 6174 203d 2054 7275 652c  MLandsat = True,
-000228a0: 0d0a 2020 6170 706c 7954 444f 4d53 656e  ..  applyTDOMSen
-000228b0: 7469 6e65 6c32 203d 2054 7275 652c 0d0a  tinel2 = True,..
-000228c0: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
-000228d0: 644d 6173 6b20 3d20 5472 7565 2c0d 0a20  dMask = True,.. 
-000228e0: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
-000228f0: 5368 6164 6f77 4d61 736b 203d 2054 7275  ShadowMask = Tru
-00022900: 652c 0d0a 2020 6170 706c 7946 6d61 736b  e,..  applyFmask
-00022910: 536e 6f77 4d61 736b 203d 2046 616c 7365  SnowMask = False
-00022920: 2c0d 0a20 2063 6c6f 7564 4865 6967 6874  ,..  cloudHeight
-00022930: 7320 3d20 6565 2e4c 6973 742e 7365 7175  s = ee.List.sequ
-00022940: 656e 6365 2835 3030 2c31 3030 3030 2c35  ence(500,10000,5
-00022950: 3030 292c 0d0a 2020 636c 6f75 6453 636f  00),..  cloudSco
-00022960: 7265 5468 7265 7368 203d 2032 302c 0d0a  reThresh = 20,..
-00022970: 2020 7065 7266 6f72 6d43 6c6f 7564 5363    performCloudSc
-00022980: 6f72 654f 6666 7365 7420 3d20 5472 7565  oreOffset = True
-00022990: 2c0d 0a20 2063 6c6f 7564 5363 6f72 6550  ,..  cloudScoreP
-000229a0: 6374 6c20 3d20 3130 2c0d 0a20 207a 5363  ctl = 10,..  zSc
-000229b0: 6f72 6554 6872 6573 6820 3d20 2d31 2c0d  oreThresh = -1,.
-000229c0: 0a20 2073 6861 646f 7753 756d 5468 7265  .  shadowSumThre
-000229d0: 7368 203d 2030 2e33 352c 0d0a 2020 636f  sh = 0.35,..  co
-000229e0: 6e74 7261 6374 5069 7865 6c73 203d 2031  ntractPixels = 1
-000229f0: 2e35 2c0d 0a20 2064 696c 6174 6550 6978  .5,..  dilatePix
-00022a00: 656c 7320 3d20 332e 352c 0d0a 2020 7368  els = 3.5,..  sh
-00022a10: 6164 6f77 5375 6d42 616e 6473 203d 205b  adowSumBands = [
-00022a20: 276e 6972 272c 2773 7769 7231 275d 2c0d  'nir','swir1'],.
-00022a30: 0a20 206c 616e 6473 6174 5265 7361 6d70  .  landsatResamp
-00022a40: 6c65 4d65 7468 6f64 203d 2027 6e65 6172  leMethod = 'near
-00022a50: 272c 0d0a 2020 7365 6e74 696e 656c 3252  ',..  sentinel2R
-00022a60: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
-00022a70: 2761 6767 7265 6761 7465 272c 0d0a 2020  'aggregate',..  
-00022a80: 636f 6e76 6572 7454 6f44 6169 6c79 4d6f  convertToDailyMo
-00022a90: 7361 6963 7320 3d20 5472 7565 2c0d 0a20  saics = True,.. 
-00022aa0: 2072 756e 4368 6173 7461 696e 4861 726d   runChastainHarm
-00022ab0: 6f6e 697a 6174 696f 6e20 3d20 5472 7565  onization = True
-00022ac0: 2c0d 0a20 2063 6f72 7265 6374 496c 6c75  ,..  correctIllu
-00022ad0: 6d69 6e61 7469 6f6e 203d 2046 616c 7365  mination = False
-00022ae0: 2c0d 0a20 2063 6f72 7265 6374 5363 616c  ,..  correctScal
-00022af0: 6520 3d20 3235 302c 0d0a 2020 6578 706f  e = 250,..  expo
-00022b00: 7274 436f 6d70 6f73 6974 6573 203d 2046  rtComposites = F
-00022b10: 616c 7365 2c0d 0a20 206f 7574 7075 744e  alse,..  outputN
-00022b20: 616d 6520 3d20 274c 616e 6473 6174 2d53  ame = 'Landsat-S
-00022b30: 656e 7469 6e65 6c32 2d48 7962 7269 6427  entinel2-Hybrid'
-00022b40: 2c0d 0a20 2065 7870 6f72 7450 6174 6852  ,..  exportPathR
-00022b50: 6f6f 7420 3d20 4e6f 6e65 2c0d 0a20 2063  oot = None,..  c
-00022b60: 7273 203d 2027 4550 5347 3a35 3037 3027  rs = 'EPSG:5070'
-00022b70: 2c0d 0a20 2074 7261 6e73 666f 726d 203d  ,..  transform =
-00022b80: 205b 3330 2c30 2c2d 3233 3631 3931 352e   [30,0,-2361915.
-00022b90: 302c 302c 2d33 302c 3331 3737 3733 352e  0,0,-30,3177735.
-00022ba0: 305d 2c0d 0a20 2073 6361 6c65 203d 204e  0],..  scale = N
-00022bb0: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
-00022bc0: 7465 644c 616e 6473 6174 436c 6f75 6453  tedLandsatCloudS
-00022bd0: 636f 7265 4f66 6673 6574 203d 204e 6f6e  coreOffset = Non
-00022be0: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
-00022bf0: 644c 616e 6473 6174 5444 4f4d 4952 4d65  dLandsatTDOMIRMe
-00022c00: 616e 203d 204e 6f6e 652c 0d0a 2020 7072  an = None,..  pr
-00022c10: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-00022c20: 5444 4f4d 4952 5374 6444 6576 203d 204e  TDOMIRStdDev = N
-00022c30: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
-00022c40: 7465 6453 656e 7469 6e65 6c32 436c 6f75  tedSentinel2Clou
-00022c50: 6453 636f 7265 4f66 6673 6574 203d 204e  dScoreOffset = N
-00022c60: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
-00022c70: 7465 6453 656e 7469 6e65 6c32 5444 4f4d  tedSentinel2TDOM
-00022c80: 4952 4d65 616e 203d 204e 6f6e 652c 0d0a  IRMean = None,..
-00022c90: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
-00022ca0: 7469 6e65 6c32 5444 4f4d 4952 5374 6444  tinel2TDOMIRStdD
-00022cb0: 6576 203d 204e 6f6e 652c 0d0a 2020 636c  ev = None,..  cl
-00022cc0: 6f75 6450 726f 6254 6872 6573 6820 3d20  oudProbThresh = 
-00022cd0: 3430 2c0d 0a20 206c 616e 6473 6174 436f  40,..  landsatCo
-00022ce0: 6c6c 6563 7469 6f6e 5665 7273 696f 6e20  llectionVersion 
-00022cf0: 3d20 2743 3227 2c0d 0a20 206f 7665 7277  = 'C2',..  overw
-00022d00: 7269 7465 203d 2046 616c 7365 293a 0d0a  rite = False):..
-00022d10: 0d0a 2020 6f72 6967 696e 203d 2027 4c61  ..  origin = 'La
-00022d20: 6e64 7361 742d 5365 6e74 696e 656c 322d  ndsat-Sentinel2-
-00022d30: 4879 6272 6964 270d 0a20 2074 6f61 4f72  Hybrid'..  toaOr
-00022d40: 5352 203d 2074 6f61 4f72 5352 2e75 7070  SR = toaOrSR.upp
-00022d50: 6572 2829 0d0a 0d0a 2020 6172 6773 203d  er()....  args =
-00022d60: 2066 6f72 6d61 7441 7267 7328 6c6f 6361   formatArgs(loca
-00022d70: 6c73 2829 290d 0a20 2069 6620 2761 7267  ls())..  if 'arg
-00022d80: 7327 2069 6e20 6172 6773 2e6b 6579 7328  s' in args.keys(
-00022d90: 293a 0d0a 2020 2020 6465 6c20 6172 6773  ):..    del args
-00022da0: 5b27 6172 6773 275d 0d0a 0d0a 2020 6d65  ['args']....  me
-00022db0: 7267 6564 203d 2067 6574 5072 6f63 6573  rged = getProces
-00022dc0: 7365 644c 616e 6473 6174 416e 6453 656e  sedLandsatAndSen
-00022dd0: 7469 6e65 6c32 5363 656e 6573 285c 0d0a  tinel2Scenes(\..
-00022de0: 2020 2020 7374 7564 7941 7265 6120 3d20      studyArea = 
-00022df0: 7374 7564 7941 7265 612c 0d0a 2020 2020  studyArea,..    
-00022e00: 7374 6172 7459 6561 7220 3d20 7374 6172  startYear = star
-00022e10: 7459 6561 722c 0d0a 2020 2020 656e 6459  tYear,..    endY
-00022e20: 6561 7220 3d20 656e 6459 6561 722c 0d0a  ear = endYear,..
-00022e30: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
-00022e40: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
-00022e50: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
-00022e60: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
-00022e70: 746f 614f 7253 5220 3d20 746f 614f 7253  toaOrSR = toaOrS
-00022e80: 522c 0d0a 2020 2020 696e 636c 7564 6553  R,..    includeS
-00022e90: 4c43 4f66 664c 3720 3d20 696e 636c 7564  LCOffL7 = includ
-00022ea0: 6553 4c43 4f66 664c 372c 0d0a 2020 2020  eSLCOffL7,..    
-00022eb0: 6465 6672 696e 6765 4c35 203d 2064 6566  defringeL5 = def
-00022ec0: 7269 6e67 654c 352c 0d0a 2020 2020 6170  ringeL5,..    ap
-00022ed0: 706c 7951 4142 616e 6420 3d20 6170 706c  plyQABand = appl
-00022ee0: 7951 4142 616e 642c 0d0a 2020 2020 6170  yQABand,..    ap
-00022ef0: 706c 7943 6c6f 7564 5072 6f62 6162 696c  plyCloudProbabil
-00022f00: 6974 7920 3d20 6170 706c 7943 6c6f 7564  ity = applyCloud
-00022f10: 5072 6f62 6162 696c 6974 792c 0d0a 2020  Probability,..  
-00022f20: 2020 6170 706c 7953 6861 646f 7753 6869    applyShadowShi
-00022f30: 6674 203d 2061 7070 6c79 5368 6164 6f77  ft = applyShadow
-00022f40: 5368 6966 742c 0d0a 2020 2020 6170 706c  Shift,..    appl
-00022f50: 7943 6c6f 7564 5363 6f72 654c 616e 6473  yCloudScoreLands
-00022f60: 6174 203d 2061 7070 6c79 436c 6f75 6453  at = applyCloudS
-00022f70: 636f 7265 4c61 6e64 7361 742c 0d0a 2020  coreLandsat,..  
-00022f80: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
-00022f90: 6553 656e 7469 6e65 6c32 203d 2061 7070  eSentinel2 = app
-00022fa0: 6c79 436c 6f75 6453 636f 7265 5365 6e74  lyCloudScoreSent
-00022fb0: 696e 656c 322c 0d0a 2020 2020 6170 706c  inel2,..    appl
-00022fc0: 7954 444f 4d4c 616e 6473 6174 203d 2061  yTDOMLandsat = a
-00022fd0: 7070 6c79 5444 4f4d 4c61 6e64 7361 742c  pplyTDOMLandsat,
-00022fe0: 0d0a 2020 2020 6170 706c 7954 444f 4d53  ..    applyTDOMS
-00022ff0: 656e 7469 6e65 6c32 203d 2061 7070 6c79  entinel2 = apply
-00023000: 5444 4f4d 5365 6e74 696e 656c 322c 0d0a  TDOMSentinel2,..
-00023010: 2020 2020 6170 706c 7946 6d61 736b 436c      applyFmaskCl
-00023020: 6f75 644d 6173 6b20 3d20 6170 706c 7946  oudMask = applyF
-00023030: 6d61 736b 436c 6f75 644d 6173 6b2c 0d0a  maskCloudMask,..
-00023040: 2020 2020 6170 706c 7946 6d61 736b 436c      applyFmaskCl
-00023050: 6f75 6453 6861 646f 774d 6173 6b20 3d20  oudShadowMask = 
-00023060: 6170 706c 7946 6d61 736b 436c 6f75 6453  applyFmaskCloudS
-00023070: 6861 646f 774d 6173 6b2c 0d0a 2020 2020  hadowMask,..    
-00023080: 6170 706c 7946 6d61 736b 536e 6f77 4d61  applyFmaskSnowMa
-00023090: 736b 203d 2061 7070 6c79 466d 6173 6b53  sk = applyFmaskS
-000230a0: 6e6f 774d 6173 6b2c 0d0a 2020 2020 636c  nowMask,..    cl
-000230b0: 6f75 6448 6569 6768 7473 203d 2063 6c6f  oudHeights = clo
-000230c0: 7564 4865 6967 6874 732c 0d0a 2020 2020  udHeights,..    
-000230d0: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
-000230e0: 203d 2063 6c6f 7564 5363 6f72 6554 6872   = cloudScoreThr
-000230f0: 6573 682c 0d0a 2020 2020 7065 7266 6f72  esh,..    perfor
-00023100: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
-00023110: 7420 3d20 7065 7266 6f72 6d43 6c6f 7564  t = performCloud
-00023120: 5363 6f72 654f 6666 7365 742c 0d0a 2020  ScoreOffset,..  
-00023130: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
-00023140: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
-00023150: 6c2c 0d0a 2020 2020 7a53 636f 7265 5468  l,..    zScoreTh
-00023160: 7265 7368 203d 207a 5363 6f72 6554 6872  resh = zScoreThr
-00023170: 6573 682c 0d0a 2020 2020 7368 6164 6f77  esh,..    shadow
-00023180: 5375 6d54 6872 6573 6820 3d20 7368 6164  SumThresh = shad
-00023190: 6f77 5375 6d54 6872 6573 682c 0d0a 2020  owSumThresh,..  
-000231a0: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
-000231b0: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
-000231c0: 732c 0d0a 2020 2020 6469 6c61 7465 5069  s,..    dilatePi
-000231d0: 7865 6c73 203d 2064 696c 6174 6550 6978  xels = dilatePix
-000231e0: 656c 732c 0d0a 2020 2020 7368 6164 6f77  els,..    shadow
-000231f0: 5375 6d42 616e 6473 203d 2073 6861 646f  SumBands = shado
-00023200: 7753 756d 4261 6e64 732c 0d0a 2020 2020  wSumBands,..    
-00023210: 6c61 6e64 7361 7452 6573 616d 706c 654d  landsatResampleM
-00023220: 6574 686f 6420 3d20 6c61 6e64 7361 7452  ethod = landsatR
-00023230: 6573 616d 706c 654d 6574 686f 642c 0d0a  esampleMethod,..
-00023240: 2020 2020 7365 6e74 696e 656c 3252 6573      sentinel2Res
-00023250: 616d 706c 654d 6574 686f 6420 3d20 7365  ampleMethod = se
-00023260: 6e74 696e 656c 3252 6573 616d 706c 654d  ntinel2ResampleM
-00023270: 6574 686f 642c 0d0a 2020 2020 636f 6e76  ethod,..    conv
-00023280: 6572 7454 6f44 6169 6c79 4d6f 7361 6963  ertToDailyMosaic
-00023290: 7320 3d20 636f 6e76 6572 7454 6f44 6169  s = convertToDai
-000232a0: 6c79 4d6f 7361 6963 732c 0d0a 2020 2020  lyMosaics,..    
-000232b0: 7275 6e43 6861 7374 6169 6e48 6172 6d6f  runChastainHarmo
-000232c0: 6e69 7a61 7469 6f6e 203d 2072 756e 4368  nization = runCh
-000232d0: 6173 7461 696e 4861 726d 6f6e 697a 6174  astainHarmonizat
-000232e0: 696f 6e2c 0d0a 2020 2020 636f 7272 6563  ion,..    correc
-000232f0: 7449 6c6c 756d 696e 6174 696f 6e20 3d20  tIllumination = 
-00023300: 636f 7272 6563 7449 6c6c 756d 696e 6174  correctIlluminat
-00023310: 696f 6e2c 0d0a 2020 2020 636f 7272 6563  ion,..    correc
-00023320: 7453 6361 6c65 203d 2063 6f72 7265 6374  tScale = correct
-00023330: 5363 616c 652c 0d0a 2020 2020 7072 6543  Scale,..    preC
-00023340: 6f6d 7075 7465 644c 616e 6473 6174 436c  omputedLandsatCl
-00023350: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
-00023360: 2070 7265 436f 6d70 7574 6564 4c61 6e64   preComputedLand
-00023370: 7361 7443 6c6f 7564 5363 6f72 654f 6666  satCloudScoreOff
-00023380: 7365 742c 0d0a 2020 2020 7072 6543 6f6d  set,..    preCom
-00023390: 7075 7465 644c 616e 6473 6174 5444 4f4d  putedLandsatTDOM
-000233a0: 4952 4d65 616e 203d 2070 7265 436f 6d70  IRMean = preComp
-000233b0: 7574 6564 4c61 6e64 7361 7454 444f 4d49  utedLandsatTDOMI
-000233c0: 524d 6561 6e2c 0d0a 2020 2020 7072 6543  RMean,..    preC
-000233d0: 6f6d 7075 7465 644c 616e 6473 6174 5444  omputedLandsatTD
-000233e0: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
-000233f0: 436f 6d70 7574 6564 4c61 6e64 7361 7454  ComputedLandsatT
-00023400: 444f 4d49 5253 7464 4465 762c 0d0a 2020  DOMIRStdDev,..  
-00023410: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
-00023420: 7469 6e65 6c32 436c 6f75 6453 636f 7265  tinel2CloudScore
-00023430: 4f66 6673 6574 203d 2070 7265 436f 6d70  Offset = preComp
-00023440: 7574 6564 5365 6e74 696e 656c 3243 6c6f  utedSentinel2Clo
-00023450: 7564 5363 6f72 654f 6666 7365 742c 0d0a  udScoreOffset,..
-00023460: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
-00023470: 656e 7469 6e65 6c32 5444 4f4d 4952 4d65  entinel2TDOMIRMe
-00023480: 616e 203d 2070 7265 436f 6d70 7574 6564  an = preComputed
-00023490: 5365 6e74 696e 656c 3254 444f 4d49 524d  Sentinel2TDOMIRM
-000234a0: 6561 6e2c 0d0a 2020 2020 7072 6543 6f6d  ean,..    preCom
-000234b0: 7075 7465 6453 656e 7469 6e65 6c32 5444  putedSentinel2TD
-000234c0: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
-000234d0: 436f 6d70 7574 6564 5365 6e74 696e 656c  ComputedSentinel
-000234e0: 3254 444f 4d49 5253 7464 4465 762c 0d0a  2TDOMIRStdDev,..
-000234f0: 2020 2020 636c 6f75 6450 726f 6254 6872      cloudProbThr
-00023500: 6573 6820 3d20 636c 6f75 6450 726f 6254  esh = cloudProbT
-00023510: 6872 6573 682c 0d0a 2020 2020 6c61 6e64  hresh,..    land
-00023520: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
-00023530: 7369 6f6e 203d 206c 616e 6473 6174 436f  sion = landsatCo
-00023540: 6c6c 6563 7469 6f6e 5665 7273 696f 6e29  llectionVersion)
-00023550: 0d0a 0d0a 2020 2343 7265 6174 6520 6879  ....  #Create hy
-00023560: 6272 6964 2063 6f6d 706f 7369 7465 730d  brid composites.
-00023570: 0a20 2063 6f6d 706f 7369 7465 7320 3d20  .  composites = 
-00023580: 636f 6d70 6f73 6974 6554 696d 6553 6572  compositeTimeSer
-00023590: 6965 7328 5c0d 0a20 2020 206c 7320 3d20  ies(\..    ls = 
-000235a0: 6d65 7267 6564 2c0d 0a20 2020 2073 7461  merged,..    sta
-000235b0: 7274 5965 6172 203d 2073 7461 7274 5965  rtYear = startYe
-000235c0: 6172 2c0d 0a20 2020 2065 6e64 5965 6172  ar,..    endYear
-000235d0: 203d 2065 6e64 5965 6172 2c0d 0a20 2020   = endYear,..   
-000235e0: 2073 7461 7274 4a75 6c69 616e 203d 2073   startJulian = s
-000235f0: 7461 7274 4a75 6c69 616e 2c0d 0a20 2020  tartJulian,..   
-00023600: 2065 6e64 4a75 6c69 616e 203d 2065 6e64   endJulian = end
-00023610: 4a75 6c69 616e 2c0d 0a20 2020 2074 696d  Julian,..    tim
-00023620: 6562 7566 6665 7220 3d20 7469 6d65 6275  ebuffer = timebu
-00023630: 6666 6572 2c0d 0a20 2020 2077 6569 6768  ffer,..    weigh
-00023640: 7473 203d 2077 6569 6768 7473 2c0d 0a20  ts = weights,.. 
-00023650: 2020 2063 6f6d 706f 7369 7469 6e67 4d65     compositingMe
-00023660: 7468 6f64 203d 2063 6f6d 706f 7369 7469  thod = compositi
-00023670: 6e67 4d65 7468 6f64 290d 0a0d 0a20 2023  ngMethod)....  #
-00023680: 2045 7870 6f72 7420 636f 6d70 6f73 6974   Export composit
-00023690: 6520 636f 6c6c 6563 7469 6f6e 0d0a 2020  e collection..  
-000236a0: 6966 2065 7870 6f72 7443 6f6d 706f 7369  if exportComposi
-000236b0: 7465 733a 0d0a 0d0a 2020 2020 6578 706f  tes:....    expo
-000236c0: 7274 4261 6e64 4469 6374 203d 207b 5c0d  rtBandDict = {\.
-000236d0: 0a20 2020 2020 2027 6d65 646f 6964 273a  .      'medoid':
-000236e0: 5b27 626c 7565 272c 2027 6772 6565 6e27  ['blue', 'green'
-000236f0: 2c20 2772 6564 272c 276e 6972 272c 2773  , 'red','nir','s
-00023700: 7769 7231 272c 2027 7377 6972 3227 2c27  wir1', 'swir2','
-00023710: 636f 6d70 6f73 6974 654f 6273 436f 756e  compositeObsCoun
-00023720: 7427 2c27 7365 6e73 6f72 272c 2779 6561  t','sensor','yea
-00023730: 7227 2c27 6a75 6c69 616e 4461 7927 5d2c  r','julianDay'],
-00023740: 0d0a 2020 2020 2020 276d 6564 6961 6e27  ..      'median'
-00023750: 3a5b 2762 6c75 6527 2c20 2767 7265 656e  :['blue', 'green
-00023760: 272c 2027 7265 6427 2c27 6e69 7227 2c27  ', 'red','nir','
-00023770: 7377 6972 3127 2c20 2773 7769 7232 272c  swir1', 'swir2',
-00023780: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-00023790: 6e74 275d 5c0d 0a20 2020 207d 3b0d 0a20  nt']\..    };.. 
-000237a0: 2020 206e 6f6e 4469 7669 6465 4261 6e64     nonDivideBand
-000237b0: 4469 6374 203d 207b 5c0d 0a20 2020 2020  Dict = {\..     
-000237c0: 2027 6d65 646f 6964 273a 5b27 636f 6d70   'medoid':['comp
-000237d0: 6f73 6974 654f 6273 436f 756e 7427 2c27  ositeObsCount','
-000237e0: 7365 6e73 6f72 272c 2779 6561 7227 2c27  sensor','year','
-000237f0: 6a75 6c69 616e 4461 7927 5d2c 0d0a 2020  julianDay'],..  
-00023800: 2020 2020 276d 6564 6961 6e27 3a5b 2763      'median':['c
-00023810: 6f6d 706f 7369 7465 4f62 7343 6f75 6e74  ompositeObsCount
-00023820: 275d 5c0d 0a20 2020 207d 3b0d 0a20 2020  ']\..    };..   
-00023830: 2065 7870 6f72 7442 616e 6473 203d 2065   exportBands = e
-00023840: 7870 6f72 7442 616e 6444 6963 745b 636f  xportBandDict[co
-00023850: 6d70 6f73 6974 696e 674d 6574 686f 645d  mpositingMethod]
-00023860: 0d0a 2020 2020 6e6f 6e44 6976 6964 6542  ..    nonDivideB
-00023870: 616e 6473 203d 206e 6f6e 4469 7669 6465  ands = nonDivide
-00023880: 4261 6e64 4469 6374 5b63 6f6d 706f 7369  BandDict[composi
-00023890: 7469 6e67 4d65 7468 6f64 5d0d 0a0d 0a20  tingMethod].... 
-000238a0: 2020 2065 7870 6f72 7443 6f6d 706f 7369     exportComposi
-000238b0: 7465 436f 6c6c 6563 7469 6f6e 285c 0d0a  teCollection(\..
-000238c0: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
-000238d0: 203d 2063 6f6d 706f 7369 7465 732c 0d0a   = composites,..
-000238e0: 2020 2020 2020 6578 706f 7274 5061 7468        exportPath
-000238f0: 526f 6f74 203d 2065 7870 6f72 7450 6174  Root = exportPat
-00023900: 6852 6f6f 742c 0d0a 2020 2020 2020 6f75  hRoot,..      ou
-00023910: 7470 7574 4e61 6d65 203d 206f 7574 7075  tputName = outpu
-00023920: 744e 616d 652c 0d0a 2020 2020 2020 6f72  tName,..      or
-00023930: 6967 696e 203d 206f 7269 6769 6e2c 0d0a  igin = origin,..
-00023940: 2020 2020 2020 7374 7564 7941 7265 6120        studyArea 
-00023950: 3d20 7374 7564 7941 7265 612c 0d0a 2020  = studyArea,..  
-00023960: 2020 2020 6372 7320 3d20 6372 732c 0d0a      crs = crs,..
-00023970: 2020 2020 2020 7472 616e 7366 6f72 6d20        transform 
-00023980: 3d20 7472 616e 7366 6f72 6d2c 0d0a 2020  = transform,..  
-00023990: 2020 2020 7363 616c 6520 3d20 7363 616c      scale = scal
-000239a0: 652c 0d0a 2020 2020 2020 7374 6172 7459  e,..      startY
-000239b0: 6561 7220 3d20 7374 6172 7459 6561 722c  ear = startYear,
-000239c0: 0d0a 2020 2020 2020 656e 6459 6561 7220  ..      endYear 
-000239d0: 3d20 656e 6459 6561 722c 0d0a 2020 2020  = endYear,..    
-000239e0: 2020 7374 6172 744a 756c 6961 6e20 3d20    startJulian = 
-000239f0: 7374 6172 744a 756c 6961 6e2c 0d0a 2020  startJulian,..  
-00023a00: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
-00023a10: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
-00023a20: 2020 636f 6d70 6f73 6974 696e 674d 6574    compositingMet
-00023a30: 686f 6420 3d20 636f 6d70 6f73 6974 696e  hod = compositin
-00023a40: 674d 6574 686f 642c 0d0a 2020 2020 2020  gMethod,..      
-00023a50: 7469 6d65 6275 6666 6572 203d 2074 696d  timebuffer = tim
-00023a60: 6562 7566 6665 722c 0d0a 2020 2020 2020  ebuffer,..      
-00023a70: 746f 614f 7253 5220 3d20 746f 614f 7253  toaOrSR = toaOrS
-00023a80: 522c 0d0a 2020 2020 2020 6e6f 6e44 6976  R,..      nonDiv
-00023a90: 6964 6542 616e 6473 203d 206e 6f6e 4469  ideBands = nonDi
-00023aa0: 7669 6465 4261 6e64 732c 0d0a 2020 2020  videBands,..    
-00023ab0: 2020 6578 706f 7274 4261 6e64 7320 3d20    exportBands = 
-00023ac0: 6578 706f 7274 4261 6e64 732c 0d0a 2020  exportBands,..  
-00023ad0: 2020 2020 6164 6469 7469 6f6e 616c 5072      additionalPr
-00023ae0: 6f70 6572 7479 4469 6374 203d 2061 7267  opertyDict = arg
-00023af0: 732c 0d0a 2020 2020 2020 6f76 6572 7772  s,..      overwr
-00023b00: 6974 6520 3d20 6f76 6572 7772 6974 6529  ite = overwrite)
-00023b10: 0d0a 0d0a 2020 6172 6773 5b27 7072 6f63  ....  args['proc
-00023b20: 6573 7365 6453 6365 6e65 7327 5d20 3d20  essedScenes'] = 
-00023b30: 6d65 7267 6564 0d0a 2020 6172 6773 5b27  merged..  args['
-00023b40: 7072 6f63 6573 7365 6443 6f6d 706f 7369  processedComposi
-00023b50: 7465 7327 5d20 3d20 636f 6d70 6f73 6974  tes'] = composit
-00023b60: 6573 0d0a 0d0a 2020 7265 7475 726e 2061  es....  return a
-00023b70: 7267 730d 0a0d 0a23 2323 2323 2323 2323  rgs....#########
-00023b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023bc0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00023bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c00: 2323 2323 2323 2323 2323 230d 0a23 4861  ###########..#Ha
-00023c10: 726d 6f6e 6963 2072 6567 7265 7373 696f  rmonic regressio
-00023c20: 6e0d 0a23 2323 2323 2323 2323 2323 2323  n..#############
-00023c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c60: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
-00023c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023cb0: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
-00023cc0: 6f6e 2074 6f20 6769 7665 2079 6561 722e  on to give year.
-00023cd0: 6464 2069 6d61 6765 2061 6e64 2068 6172  dd image and har
-00023ce0: 6d6f 6e69 6373 206c 6973 7420 2865 2e67  monics list (e.g
-00023cf0: 2e20 5b31 2c32 2c33 2c2e 2e2e 5d29 0d0a  . [1,2,3,...])..
-00023d00: 6465 6620 6765 7448 6172 6d6f 6e69 634c  def getHarmonicL
-00023d10: 6973 7428 7965 6172 4461 7465 496d 672c  ist(yearDateImg,
-00023d20: 7472 616e 7366 6f72 6d42 616e 644e 616d  transformBandNam
-00023d30: 652c 6861 726d 6f6e 6963 4c69 7374 293a  e,harmonicList):
-00023d40: 0d0a 2020 743d 2079 6561 7244 6174 6549  ..  t= yearDateI
-00023d50: 6d67 2e73 656c 6563 7428 5b74 7261 6e73  mg.select([trans
-00023d60: 666f 726d 4261 6e64 4e61 6d65 5d29 0d0a  formBandName])..
-00023d70: 2020 7365 6c65 6374 4261 6e64 7320 3d20    selectBands = 
-00023d80: 6565 2e4c 6973 742e 7365 7175 656e 6365  ee.List.sequence
-00023d90: 2830 2c6c 656e 2868 6172 6d6f 6e69 634c  (0,len(harmonicL
-00023da0: 6973 7429 2d31 290d 0a0d 0a20 2064 6566  ist)-1)....  def
-00023db0: 2073 696e 4361 7428 6829 3a0d 0a20 2020   sinCat(h):..   
-00023dc0: 2068 7420 3d20 682a 3130 300d 0a20 2020   ht = h*100..   
-00023dd0: 2072 6574 7572 6e20 6565 2e53 7472 696e   return ee.Strin
-00023de0: 6728 2773 696e 5f27 292e 6361 7428 7374  g('sin_').cat(st
-00023df0: 7228 6874 2929 2e63 6174 2827 5f27 292e  r(ht)).cat('_').
-00023e00: 6361 7428 7472 616e 7366 6f72 6d42 616e  cat(transformBan
-00023e10: 644e 616d 6529 0d0a 2020 7369 6e4e 616d  dName)..  sinNam
-00023e20: 6573 203d 206c 6973 7428 6d61 7028 6c61  es = list(map(la
-00023e30: 6d62 6461 2069 3a73 696e 4361 7428 6929  mbda i:sinCat(i)
-00023e40: 2c68 6172 6d6f 6e69 634c 6973 7429 290d  ,harmonicList)).
-00023e50: 0a0d 0a20 2064 6566 2063 6f73 4361 7428  ...  def cosCat(
-00023e60: 6829 3a0d 0a20 2020 2068 7420 3d68 2a31  h):..    ht =h*1
-00023e70: 3030 3b0d 0a20 2020 2072 6574 7572 6e20  00;..    return 
-00023e80: 6565 2e53 7472 696e 6728 2763 6f73 5f27  ee.String('cos_'
-00023e90: 292e 6361 7428 7374 7228 6874 2929 2e63  ).cat(str(ht)).c
-00023ea0: 6174 2827 5f27 292e 6361 7428 7472 616e  at('_').cat(tran
-00023eb0: 7366 6f72 6d42 616e 644e 616d 6529 0d0a  sformBandName)..
-00023ec0: 0d0a 2020 636f 734e 616d 6573 203d 206c  ..  cosNames = l
-00023ed0: 6973 7428 6d61 7028 6c61 6d62 6461 2069  ist(map(lambda i
-00023ee0: 203a 2063 6f73 4361 7428 6929 2c68 6172   : cosCat(i),har
-00023ef0: 6d6f 6e69 634c 6973 7429 290d 0a0d 0a0d  monicList)).....
-00023f00: 0a0d 0a20 206d 756c 7469 706c 6965 7273  ...  multipliers
-00023f10: 203d 2065 652e 496d 6167 6528 6861 726d   = ee.Image(harm
-00023f20: 6f6e 6963 4c69 7374 292e 6d75 6c74 6970  onicList).multip
-00023f30: 6c79 2865 652e 4e75 6d62 6572 286d 6174  ly(ee.Number(mat
-00023f40: 682e 7069 292e 666c 6f61 7428 2929 0d0a  h.pi).float())..
-00023f50: 2020 7369 6e49 6e64 203d 2028 742e 6d75    sinInd = (t.mu
-00023f60: 6c74 6970 6c79 2865 652e 496d 6167 6528  ltiply(ee.Image(
-00023f70: 6d75 6c74 6970 6c69 6572 7329 2929 2e73  multipliers))).s
-00023f80: 696e 2829 2e73 656c 6563 7428 7365 6c65  in().select(sele
-00023f90: 6374 4261 6e64 732c 7369 6e4e 616d 6573  ctBands,sinNames
-00023fa0: 292e 666c 6f61 7428 290d 0a20 2063 6f73  ).float()..  cos
-00023fb0: 496e 6420 3d20 2874 2e6d 756c 7469 706c  Ind = (t.multipl
-00023fc0: 7928 6565 2e49 6d61 6765 286d 756c 7469  y(ee.Image(multi
-00023fd0: 706c 6965 7273 2929 292e 636f 7328 292e  pliers))).cos().
-00023fe0: 7365 6c65 6374 2873 656c 6563 7442 616e  select(selectBan
-00023ff0: 6473 2c63 6f73 4e61 6d65 7329 2e66 6c6f  ds,cosNames).flo
-00024000: 6174 2829 0d0a 0d0a 2020 7265 7475 726e  at()....  return
-00024010: 2079 6561 7244 6174 6549 6d67 2e61 6464   yearDateImg.add
-00024020: 4261 6e64 7328 7369 6e49 6e64 2e61 6464  Bands(sinInd.add
-00024030: 4261 6e64 7328 636f 7349 6e64 2929 0d0a  Bands(cosInd))..
-00024040: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00024050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024080: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
-00024090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000240a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000240b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000240c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000240d0: 2323 2323 2323 0d0a 2354 616b 6573 2061  ######..#Takes a
-000240e0: 2064 6570 656e 6465 6e74 2061 6e64 2069   dependent and i
-000240f0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00024100: 626c 6520 616e 6420 7265 7475 726e 7320  ble and returns 
-00024110: 7468 6520 6465 7065 6e64 656e 742c 0d0a  the dependent,..
-00024120: 2320 7369 6e20 6f66 2069 6e64 2c20 616e  # sin of ind, an
-00024130: 6420 636f 7320 6f66 2069 6e64 0d0a 2349  d cos of ind..#I
-00024140: 6e74 656e 6465 6420 666f 7220 6861 726d  ntended for harm
-00024150: 6f6e 6963 2072 6567 7265 7373 696f 6e0d  onic regression.
-00024160: 0a64 6566 2067 6574 4861 726d 6f6e 6963  .def getHarmonic
-00024170: 7332 2863 6f6c 6c65 6374 696f 6e2c 7472  s2(collection,tr
-00024180: 616e 7366 6f72 6d42 616e 644e 616d 652c  ansformBandName,
-00024190: 6861 726d 6f6e 6963 4c69 7374 2c64 6574  harmonicList,det
-000241a0: 7265 6e64 203d 2046 616c 7365 293a 0d0a  rend = False):..
-000241b0: 0d0a 2020 6465 7042 616e 644e 616d 6573  ..  depBandNames
-000241c0: 203d 2065 652e 496d 6167 6528 636f 6c6c   = ee.Image(coll
-000241d0: 6563 7469 6f6e 2e66 6972 7374 2829 292e  ection.first()).
-000241e0: 6261 6e64 4e61 6d65 7328 292e 7265 6d6f  bandNames().remo
-000241f0: 7665 2874 7261 6e73 666f 726d 4261 6e64  ve(transformBand
-00024200: 4e61 6d65 290d 0a20 2064 6570 4261 6e64  Name)..  depBand
-00024210: 4e75 6d62 6572 7320 3d20 6465 7042 616e  Numbers = depBan
-00024220: 644e 616d 6573 2e6d 6170 286c 616d 6264  dNames.map(lambd
-00024230: 6120 6462 6e3a 6465 7042 616e 644e 616d  a dbn:depBandNam
-00024240: 6573 2e69 6e64 6578 4f66 2864 626e 2929  es.indexOf(dbn))
-00024250: 0d0a 0d0a 2020 6465 6620 6861 726d 5772  ....  def harmWr
-00024260: 6170 2869 6d67 293a 0d0a 2020 2020 6f75  ap(img):..    ou
-00024270: 7454 203d 2067 6574 4861 726d 6f6e 6963  tT = getHarmonic
-00024280: 4c69 7374 2869 6d67 2c74 7261 6e73 666f  List(img,transfo
-00024290: 726d 4261 6e64 4e61 6d65 2c68 6172 6d6f  rmBandName,harmo
-000242a0: 6e69 634c 6973 7429 5c0d 0a20 2020 202e  nicList)\..    .
-000242b0: 636f 7079 5072 6f70 6572 7469 6573 2869  copyProperties(i
-000242c0: 6d67 2c5b 2773 7973 7465 6d3a 7469 6d65  mg,['system:time
-000242d0: 5f73 7461 7274 272c 2773 7973 7465 6d3a  _start','system:
-000242e0: 7469 6d65 5f65 6e64 275d 290d 0a20 2020  time_end'])..   
-000242f0: 2072 6574 7572 6e20 6f75 7454 0d0a 2020   return outT..  
-00024300: 6f75 7420 3d20 636f 6c6c 6563 7469 6f6e  out = collection
-00024310: 2e6d 6170 2868 6172 6d57 7261 7029 0d0a  .map(harmWrap)..
-00024320: 0d0a 2020 6966 206e 6f74 2064 6574 7265  ..  if not detre
-00024330: 6e64 3a0d 0a20 2020 206f 7574 4261 6e64  nd:..    outBand
-00024340: 4e61 6d65 7320 3d20 6565 2e49 6d61 6765  Names = ee.Image
-00024350: 286f 7574 2e66 6972 7374 2829 292e 6261  (out.first()).ba
-00024360: 6e64 4e61 6d65 7328 292e 7265 6d6f 7665  ndNames().remove
-00024370: 416c 6c28 5b27 7965 6172 275d 290d 0a20  All(['year']).. 
-00024380: 2020 206f 7574 203d 206f 7574 2e73 656c     out = out.sel
-00024390: 6563 7428 6f75 7442 616e 644e 616d 6573  ect(outBandNames
-000243a0: 290d 0a0d 0a0d 0a20 2069 6e64 4261 6e64  )......  indBand
-000243b0: 4e61 6d65 7320 3d20 6565 2e49 6d61 6765  Names = ee.Image
-000243c0: 286f 7574 2e66 6972 7374 2829 292e 6261  (out.first()).ba
-000243d0: 6e64 4e61 6d65 7328 292e 7265 6d6f 7665  ndNames().remove
-000243e0: 416c 6c28 6465 7042 616e 644e 616d 6573  All(depBandNames
-000243f0: 290d 0a20 2069 6e64 4261 6e64 4e75 6d62  )..  indBandNumb
-00024400: 6572 7320 3d20 696e 6442 616e 644e 616d  ers = indBandNam
-00024410: 6573 2e6d 6170 286c 616d 6264 6120 696e  es.map(lambda in
-00024420: 643a 2065 652e 496d 6167 6528 6f75 742e  d: ee.Image(out.
-00024430: 6669 7273 7428 2929 2e62 616e 644e 616d  first()).bandNam
-00024440: 6573 2829 2e69 6e64 6578 4f66 2869 6e64  es().indexOf(ind
-00024450: 2929 0d0a 0d0a 0d0a 2020 6f75 7420 3d20  ))......  out = 
-00024460: 6f75 742e 7365 7428 7b27 696e 6442 616e  out.set({'indBan
-00024470: 644e 616d 6573 273a 696e 6442 616e 644e  dNames':indBandN
-00024480: 616d 6573 2c27 6465 7042 616e 644e 616d  ames,'depBandNam
-00024490: 6573 273a 6465 7042 616e 644e 616d 6573  es':depBandNames
-000244a0: 2c5c 0d0a 2020 2020 2020 2020 2020 2020  ,\..            
-000244b0: 2020 2020 2769 6e64 4261 6e64 4e75 6d62      'indBandNumb
-000244c0: 6572 7327 3a69 6e64 4261 6e64 4e75 6d62  ers':indBandNumb
-000244d0: 6572 732c 2764 6570 4261 6e64 4e75 6d62  ers,'depBandNumb
-000244e0: 6572 7327 3a64 6570 4261 6e64 4e75 6d62  ers':depBandNumb
-000244f0: 6572 737d 290d 0a0d 0a20 2072 6574 7572  ers})....  retur
-00024500: 6e20 6f75 740d 0a0d 0a23 2323 2323 2323  n out....#######
-00024510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024550: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
-00024560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024590: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-000245a0: 5369 6d70 6c69 6669 6573 2074 6865 2075  Simplifies the u
-000245b0: 7365 206f 6620 7468 6520 726f 6275 7374  se of the robust
-000245c0: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
-000245d0: 6f6e 2072 6564 7563 6572 0d0a 2341 7373  on reducer..#Ass
-000245e0: 756d 6573 2074 6865 2064 6570 656e 6465  umes the depende
-000245f0: 6e74 2069 7320 7468 6520 6669 7273 7420  nt is the first 
-00024600: 6261 6e64 2061 6e64 2061 6c6c 2073 7562  band and all sub
-00024610: 7365 7175 656e 7420 6261 6e64 7320 6172  sequent bands ar
-00024620: 6520 696e 6465 7065 6e64 656e 7473 0d0a  e independents..
-00024630: 6465 6620 6e65 7752 6f62 7573 744d 756c  def newRobustMul
-00024640: 7469 706c 654c 696e 6561 7232 2864 6570  tipleLinear2(dep
-00024650: 656e 6465 6e74 7349 6e64 6570 656e 6465  endentsIndepende
-00024660: 6e74 7329 3a0d 0a20 2023 5365 7420 7570  nts):..  #Set up
-00024670: 2074 6865 2062 616e 6420 6e61 6d65 730d   the band names.
-00024680: 0a0d 0a20 2064 6570 656e 6465 6e74 4261  ...  dependentBa
-00024690: 6e64 7320 3d20 6565 2e4c 6973 7428 6465  nds = ee.List(de
-000246a0: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
-000246b0: 656e 7473 2e67 6574 2827 6465 7042 616e  ents.get('depBan
-000246c0: 644e 756d 6265 7273 2729 290d 0a20 2069  dNumbers'))..  i
-000246d0: 6e64 6570 656e 6465 6e74 4261 6e64 7320  ndependentBands 
-000246e0: 3d20 6565 2e4c 6973 7428 6465 7065 6e64  = ee.List(depend
-000246f0: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
-00024700: 2e67 6574 2827 696e 6442 616e 644e 756d  .get('indBandNum
-00024710: 6265 7273 2729 290d 0a20 2062 6e73 203d  bers'))..  bns =
-00024720: 2065 652e 496d 6167 6528 6465 7065 6e64   ee.Image(depend
-00024730: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
-00024740: 2e66 6972 7374 2829 292e 6261 6e64 4e61  .first()).bandNa
-00024750: 6d65 7328 290d 0a20 2064 6570 656e 6465  mes()..  depende
-00024760: 6e74 7320 3d20 6565 2e4c 6973 7428 6465  nts = ee.List(de
-00024770: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
-00024780: 656e 7473 2e67 6574 2827 6465 7042 616e  ents.get('depBan
-00024790: 644e 616d 6573 2729 290d 0a20 2069 6e64  dNames'))..  ind
-000247a0: 6570 656e 6465 6e74 7320 3d20 6565 2e4c  ependents = ee.L
-000247b0: 6973 7428 6465 7065 6e64 656e 7473 496e  ist(dependentsIn
-000247c0: 6465 7065 6e64 656e 7473 2e67 6574 2827  dependents.get('
-000247d0: 696e 6442 616e 644e 616d 6573 2729 290d  indBandNames')).
-000247e0: 0a0d 0a20 2023 6465 7065 6e64 656e 7420  ...  #dependent 
-000247f0: 3d20 626e 732e 736c 6963 6528 302c 3129  = bns.slice(0,1)
-00024800: 0d0a 2020 2369 6e64 6570 656e 6465 6e74  ..  #independent
-00024810: 7320 3d20 626e 732e 736c 6963 6528 312c  s = bns.slice(1,
-00024820: 6e75 6c6c 290d 0a20 206e 6f49 6e64 6570  null)..  noIndep
-00024830: 656e 6465 6e74 7320 3d20 696e 6465 7065  endents = indepe
-00024840: 6e64 656e 7473 2e6c 656e 6774 6828 292e  ndents.length().
-00024850: 6164 6428 3129 0d0a 2020 6e6f 4465 7065  add(1)..  noDepe
-00024860: 6e64 656e 7473 203d 2064 6570 656e 6465  ndents = depende
-00024870: 6e74 732e 6c65 6e67 7468 2829 0d0a 0d0a  nts.length()....
-00024880: 2020 6f75 744e 616d 6573 203d 2065 652e    outNames = ee.
-00024890: 4c69 7374 285b 2769 6e74 6572 6365 7074  List(['intercept
-000248a0: 275d 292e 6361 7428 696e 6465 7065 6e64  ']).cat(independ
-000248b0: 656e 7473 290d 0a0d 0a20 2023 4164 6420  ents)....  #Add 
-000248c0: 636f 6e73 7461 6e74 2062 616e 6420 666f  constant band fo
-000248d0: 7220 696e 7465 7263 6570 7420 616e 6420  r intercept and 
-000248e0: 7265 6f72 6465 7220 666f 720d 0a20 2023  reorder for..  #
-000248f0: 7379 6e74 6178 3a20 636f 6e73 7461 6e74  syntax: constant
-00024900: 2c20 696e 6431 2c69 6e64 322c 696e 6433  , ind1,ind2,ind3
-00024910: 2c69 6e64 6e2c 6465 7065 6e64 656e 740d  ,indn,dependent.
-00024920: 0a20 2064 6566 2066 6f72 4669 7446 756e  .  def forFitFun
-00024930: 2869 6d67 293a 0d0a 2020 2020 6f75 7420  (img):..    out 
-00024940: 3d20 696d 672e 6164 6442 616e 6473 2865  = img.addBands(e
-00024950: 652e 496d 6167 6528 3129 2e73 656c 6563  e.Image(1).selec
-00024960: 7428 5b30 5d2c 5b27 636f 6e73 7461 6e74  t([0],['constant
-00024970: 275d 2929 0d0a 2020 2020 6f75 7420 3d20  ']))..    out = 
-00024980: 6f75 742e 7365 6c65 6374 2865 652e 4c69  out.select(ee.Li
-00024990: 7374 285b 2763 6f6e 7374 616e 7427 2c69  st(['constant',i
-000249a0: 6e64 6570 656e 6465 6e74 735d 292e 666c  ndependents]).fl
-000249b0: 6174 7465 6e28 2929 0d0a 2020 2020 7265  atten())..    re
-000249c0: 7475 726e 206f 7574 2e61 6464 4261 6e64  turn out.addBand
-000249d0: 7328 696d 672e 7365 6c65 6374 2864 6570  s(img.select(dep
-000249e0: 656e 6465 6e74 7329 290d 0a0d 0a0d 0a20  endents))...... 
-000249f0: 2066 6f72 4669 7420 3d20 6465 7065 6e64   forFit = depend
-00024a00: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
-00024a10: 2e6d 6170 2866 6f72 4669 7446 756e 290d  .map(forFitFun).
-00024a20: 0a0d 0a20 2023 4170 706c 7920 7265 6475  ...  #Apply redu
-00024a30: 6365 722c 2061 6e64 2063 6f6e 7665 7274  cer, and convert
-00024a40: 2062 6163 6b20 746f 2069 6d61 6765 2077   back to image w
-00024a50: 6974 6820 7265 7370 6563 7469 7665 2062  ith respective b
-00024a60: 616e 644e 616d 6573 0d0a 2020 7265 6475  andNames..  redu
-00024a70: 6365 724f 7574 203d 2066 6f72 4669 742e  cerOut = forFit.
-00024a80: 7265 6475 6365 2865 652e 5265 6475 6365  reduce(ee.Reduce
-00024a90: 722e 6c69 6e65 6172 5265 6772 6573 7369  r.linearRegressi
-00024aa0: 6f6e 286e 6f49 6e64 6570 656e 6465 6e74  on(noIndependent
-00024ab0: 732c 6e6f 4465 7065 6e64 656e 7473 2929  s,noDependents))
-00024ac0: 0d0a 2020 2320 2f2f 2074 6573 7420 3d20  ..  # // test = 
-00024ad0: 666f 7246 6974 2e72 6564 7563 6528 6565  forFit.reduce(ee
-00024ae0: 2e52 6564 7563 6572 2e72 6f62 7573 744c  .Reducer.robustL
-00024af0: 696e 6561 7252 6567 7265 7373 696f 6e28  inearRegression(
-00024b00: 6e6f 496e 6465 7065 6e64 656e 7473 2c6e  noIndependents,n
-00024b10: 6f44 6570 656e 6465 6e74 732c 302e 3229  oDependents,0.2)
-00024b20: 290d 0a20 2023 202f 2f20 7265 7369 6473  )..  # // resids
-00024b30: 203d 2074 6573 740d 0a20 2023 202f 2f20   = test..  # // 
-00024b40: 2e73 656c 6563 7428 5b31 5d2c 5b27 7265  .select([1],['re
-00024b50: 7369 6475 616c 7327 5d29 2e61 7272 6179  siduals']).array
-00024b60: 466c 6174 7465 6e28 5b64 6570 656e 6465  Flatten([depende
-00024b70: 6e74 735d 293b 0d0a 2020 2320 2f2f 204d  nts]);..  # // M
-00024b80: 6170 2e61 6464 4c61 7965 7228 7265 7369  ap.addLayer(resi
-00024b90: 6473 2c7b 7d2c 2772 6573 6964 7349 6d61  ds,{},'residsIma
-00024ba0: 6765 2729 3b0d 0a20 2023 202f 2f20 4d61  ge');..  # // Ma
-00024bb0: 702e 6164 644c 6179 6572 2872 6564 7563  p.addLayer(reduc
-00024bc0: 6572 4f75 742e 7365 6c65 6374 285b 305d  erOut.select([0]
-00024bd0: 292c 7b7d 2c27 636f 6566 6669 6369 656e  ),{},'coefficien
-00024be0: 7473 2729 3b0d 0a20 2023 202f 2f20 4d61  ts');..  # // Ma
-00024bf0: 702e 6164 644c 6179 6572 2874 6573 742e  p.addLayer(test.
-00024c00: 7365 6c65 6374 285b 315d 292c 7b7d 2c27  select([1]),{},'
-00024c10: 7472 6573 6964 7561 6c73 2729 3b0d 0a20  tresiduals');.. 
-00024c20: 2023 202f 2f20 4d61 702e 6164 644c 6179   # // Map.addLay
-00024c30: 6572 2872 6564 7563 6572 4f75 742e 7365  er(reducerOut.se
-00024c40: 6c65 6374 285b 315d 292c 7b7d 2c27 726f  lect([1]),{},'ro
-00024c50: 7265 7369 6475 616c 7327 293b 0d0a 2020  residuals');..  
-00024c60: 7265 6475 6365 724f 7574 203d 2072 6564  reducerOut = red
-00024c70: 7563 6572 4f75 742e 7365 6c65 6374 285b  ucerOut.select([
-00024c80: 305d 2c5b 2763 6f65 6666 6963 6965 6e74  0],['coefficient
-00024c90: 7327 5d29 2e61 7272 6179 5472 616e 7370  s']).arrayTransp
-00024ca0: 6f73 6528 292e 6172 7261 7946 6c61 7474  ose().arrayFlatt
-00024cb0: 656e 285b 6465 7065 6e64 656e 7473 2c6f  en([dependents,o
-00024cc0: 7574 4e61 6d65 735d 290d 0a20 2072 6564  utNames])..  red
-00024cd0: 7563 6572 4f75 7420 3d20 7265 6475 6365  ucerOut = reduce
-00024ce0: 724f 7574 2e73 6574 287b 276e 6f44 6570  rOut.set({'noDep
-00024cf0: 656e 6465 6e74 7327 3a65 652e 4e75 6d62  endents':ee.Numb
-00024d00: 6572 286e 6f44 6570 656e 6465 6e74 7329  er(noDependents)
-00024d10: 2c5c 0d0a 2020 276d 6f64 656c 4c65 6e67  ,\..  'modelLeng
-00024d20: 7468 273a 6565 2e4e 756d 6265 7228 6e6f  th':ee.Number(no
-00024d30: 496e 6465 7065 6e64 656e 7473 295c 0d0a  Independents)\..
-00024d40: 2020 7d29 0d0a 0d0a 2020 7265 7475 726e    })....  return
-00024d50: 2072 6564 7563 6572 4f75 740d 0a23 2323   reducerOut..###
-00024d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024da0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
-00024db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024dd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024de0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024df0: 230d 0a23 436f 6465 2066 6f72 2066 696e  #..#Code for fin
-00024e00: 6469 6e67 2074 6865 2064 6174 6520 6f66  ding the date of
-00024e10: 2070 6561 6b20 6f66 2067 7265 656e 0d0a   peak of green..
-00024e20: 2320 416c 736f 2063 6f6e 7665 7274 7320  # Also converts 
-00024e30: 6974 2074 6f20 4a75 6c69 616e 2064 6179  it to Julian day
-00024e40: 2c20 6d6f 6e74 682c 2061 6e64 2064 6179  , month, and day
-00024e50: 206f 6620 6d6f 6e74 680d 0a6d 6f6e 7468   of month..month
-00024e60: 5265 6d61 7020 3d5b 312c 2031 2c20 312c  Remap =[1, 1, 1,
-00024e70: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
-00024e80: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
-00024e90: 2c20 312c 2031 2c20 312c 2031 2c20 312c  , 1, 1, 1, 1, 1,
-00024ea0: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
-00024eb0: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
-00024ec0: 2c20 312c 2032 2c20 322c 2032 2c20 322c  , 1, 2, 2, 2, 2,
-00024ed0: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
-00024ee0: 322c 2032 2c20 322c 2032 2c20 322c 2032  2, 2, 2, 2, 2, 2
-00024ef0: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
-00024f00: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
-00024f10: 322c 2032 2c20 322c 2033 2c20 332c 2033  2, 2, 2, 3, 3, 3
-00024f20: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
-00024f30: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
-00024f40: 332c 2033 2c20 332c 2033 2c20 332c 2033  3, 3, 3, 3, 3, 3
-00024f50: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
-00024f60: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
-00024f70: 332c 2033 2c20 342c 2034 2c20 342c 2034  3, 3, 4, 4, 4, 4
-00024f80: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
-00024f90: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
-00024fa0: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
-00024fb0: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
-00024fc0: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
-00024fd0: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
-00024fe0: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
-00024ff0: 2035 2c20 352c 2035 2c20 352c 2035 2c20   5, 5, 5, 5, 5, 
-00025000: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
-00025010: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
-00025020: 2035 2c20 352c 2035 2c20 352c 2036 2c20   5, 5, 5, 5, 6, 
-00025030: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
-00025040: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
-00025050: 2036 2c20 362c 2036 2c20 362c 2036 2c20   6, 6, 6, 6, 6, 
-00025060: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
-00025070: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
-00025080: 2036 2c20 362c 2037 2c20 372c 2037 2c20   6, 6, 7, 7, 7, 
-00025090: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
-000250a0: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
-000250b0: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
-000250c0: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
-000250d0: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
-000250e0: 2037 2c20 382c 2038 2c20 382c 2038 2c20   7, 8, 8, 8, 8, 
-000250f0: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
-00025100: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
-00025110: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
-00025120: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
-00025130: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
-00025140: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
-00025150: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
-00025160: 2c20 392c 2039 2c20 392c 2039 2c20 392c  , 9, 9, 9, 9, 9,
-00025170: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
-00025180: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
-00025190: 2c20 392c 2039 2c20 392c 2031 302c 2031  , 9, 9, 9, 10, 1
-000251a0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-000251b0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-000251c0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-000251d0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-000251e0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-000251f0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025200: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025210: 302c 2031 302c 2031 312c 2031 312c 2031  0, 10, 11, 11, 1
-00025220: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025230: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025240: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025250: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025260: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025270: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025280: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025290: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252a0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252b0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252c0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252d0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252e0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-000252f0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025300: 322c 2031 322c 2031 3220 5d0d 0a6d 6f6e  2, 12, 12 ]..mon
-00025310: 7468 4461 7952 656d 6170 203d 205b 312c  thDayRemap = [1,
-00025320: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
-00025330: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
-00025340: 2031 322c 2031 332c 2031 342c 2031 352c   12, 13, 14, 15,
-00025350: 2031 362c 2031 372c 2031 382c 2031 392c   16, 17, 18, 19,
-00025360: 2032 302c 2032 312c 2032 322c 2032 332c   20, 21, 22, 23,
-00025370: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
-00025380: 2032 382c 2032 392c 2033 302c 2033 312c   28, 29, 30, 31,
-00025390: 2031 2c20 322c 2033 2c20 342c 2035 2c20   1, 2, 3, 4, 5, 
-000253a0: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
-000253b0: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
-000253c0: 3135 2c20 3136 2c20 3137 2c20 3138 2c20  15, 16, 17, 18, 
-000253d0: 3139 2c20 3230 2c20 3231 2c20 3232 2c20  19, 20, 21, 22, 
-000253e0: 3233 2c20 3234 2c20 3235 2c20 3236 2c20  23, 24, 25, 26, 
-000253f0: 3237 2c20 3238 2c20 312c 2032 2c20 332c  27, 28, 1, 2, 3,
-00025400: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
-00025410: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
-00025420: 332c 2031 342c 2031 352c 2031 362c 2031  3, 14, 15, 16, 1
-00025430: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
-00025440: 312c 2032 322c 2032 332c 2032 342c 2032  1, 22, 23, 24, 2
-00025450: 352c 2032 362c 2032 372c 2032 382c 2032  5, 26, 27, 28, 2
-00025460: 392c 2033 302c 2033 312c 2031 2c20 322c  9, 30, 31, 1, 2,
-00025470: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
-00025480: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
-00025490: 2c20 3133 2c20 3134 2c20 3135 2c20 3136  , 13, 14, 15, 16
-000254a0: 2c20 3137 2c20 3138 2c20 3139 2c20 3230  , 17, 18, 19, 20
-000254b0: 2c20 3231 2c20 3232 2c20 3233 2c20 3234  , 21, 22, 23, 24
-000254c0: 2c20 3235 2c20 3236 2c20 3237 2c20 3238  , 25, 26, 27, 28
-000254d0: 2c20 3239 2c20 3330 2c20 312c 2032 2c20  , 29, 30, 1, 2, 
-000254e0: 332c 2034 2c20 352c 2036 2c20 372c 2038  3, 4, 5, 6, 7, 8
-000254f0: 2c20 392c 2031 302c 2031 312c 2031 322c  , 9, 10, 11, 12,
-00025500: 2031 332c 2031 342c 2031 352c 2031 362c   13, 14, 15, 16,
-00025510: 2031 372c 2031 382c 2031 392c 2032 302c   17, 18, 19, 20,
-00025520: 2032 312c 2032 322c 2032 332c 2032 342c   21, 22, 23, 24,
-00025530: 2032 352c 2032 362c 2032 372c 2032 382c   25, 26, 27, 28,
-00025540: 2032 392c 2033 302c 2033 312c 2031 2c20   29, 30, 31, 1, 
-00025550: 322c 2033 2c20 342c 2035 2c20 362c 2037  2, 3, 4, 5, 6, 7
-00025560: 2c20 382c 2039 2c20 3130 2c20 3131 2c20  , 8, 9, 10, 11, 
-00025570: 3132 2c20 3133 2c20 3134 2c20 3135 2c20  12, 13, 14, 15, 
-00025580: 3136 2c20 3137 2c20 3138 2c20 3139 2c20  16, 17, 18, 19, 
-00025590: 3230 2c20 3231 2c20 3232 2c20 3233 2c20  20, 21, 22, 23, 
-000255a0: 3234 2c20 3235 2c20 3236 2c20 3237 2c20  24, 25, 26, 27, 
-000255b0: 3238 2c20 3239 2c20 3330 2c20 312c 2032  28, 29, 30, 1, 2
-000255c0: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-000255d0: 2038 2c20 392c 2031 302c 2031 312c 2031   8, 9, 10, 11, 1
-000255e0: 322c 2031 332c 2031 342c 2031 352c 2031  2, 13, 14, 15, 1
-000255f0: 362c 2031 372c 2031 382c 2031 392c 2032  6, 17, 18, 19, 2
-00025600: 302c 2032 312c 2032 322c 2032 332c 2032  0, 21, 22, 23, 2
-00025610: 342c 2032 352c 2032 362c 2032 372c 2032  4, 25, 26, 27, 2
-00025620: 382c 2032 392c 2033 302c 2033 312c 2031  8, 29, 30, 31, 1
-00025630: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
-00025640: 2037 2c20 382c 2039 2c20 3130 2c20 3131   7, 8, 9, 10, 11
-00025650: 2c20 3132 2c20 3133 2c20 3134 2c20 3135  , 12, 13, 14, 15
-00025660: 2c20 3136 2c20 3137 2c20 3138 2c20 3139  , 16, 17, 18, 19
-00025670: 2c20 3230 2c20 3231 2c20 3232 2c20 3233  , 20, 21, 22, 23
-00025680: 2c20 3234 2c20 3235 2c20 3236 2c20 3237  , 24, 25, 26, 27
-00025690: 2c20 3238 2c20 3239 2c20 3330 2c20 3331  , 28, 29, 30, 31
-000256a0: 2c20 312c 2032 2c20 332c 2034 2c20 352c  , 1, 2, 3, 4, 5,
-000256b0: 2036 2c20 372c 2038 2c20 392c 2031 302c   6, 7, 8, 9, 10,
-000256c0: 2031 312c 2031 322c 2031 332c 2031 342c   11, 12, 13, 14,
-000256d0: 2031 352c 2031 362c 2031 372c 2031 382c   15, 16, 17, 18,
-000256e0: 2031 392c 2032 302c 2032 312c 2032 322c   19, 20, 21, 22,
-000256f0: 2032 332c 2032 342c 2032 352c 2032 362c   23, 24, 25, 26,
-00025700: 2032 372c 2032 382c 2032 392c 2033 302c   27, 28, 29, 30,
-00025710: 2031 2c20 322c 2033 2c20 342c 2035 2c20   1, 2, 3, 4, 5, 
-00025720: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
-00025730: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
-00025740: 3135 2c20 3136 2c20 3137 2c20 3138 2c20  15, 16, 17, 18, 
-00025750: 3139 2c20 3230 2c20 3231 2c20 3232 2c20  19, 20, 21, 22, 
-00025760: 3233 2c20 3234 2c20 3235 2c20 3236 2c20  23, 24, 25, 26, 
-00025770: 3237 2c20 3238 2c20 3239 2c20 3330 2c20  27, 28, 29, 30, 
-00025780: 3331 2c20 312c 2032 2c20 332c 2034 2c20  31, 1, 2, 3, 4, 
-00025790: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
-000257a0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
-000257b0: 342c 2031 352c 2031 362c 2031 372c 2031  4, 15, 16, 17, 1
-000257c0: 382c 2031 392c 2032 302c 2032 312c 2032  8, 19, 20, 21, 2
-000257d0: 322c 2032 332c 2032 342c 2032 352c 2032  2, 23, 24, 25, 2
-000257e0: 362c 2032 372c 2032 382c 2032 392c 2033  6, 27, 28, 29, 3
-000257f0: 302c 2031 2c20 322c 2033 2c20 342c 2035  0, 1, 2, 3, 4, 5
-00025800: 2c20 362c 2037 2c20 382c 2039 2c20 3130  , 6, 7, 8, 9, 10
-00025810: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
-00025820: 2c20 3135 2c20 3136 2c20 3137 2c20 3138  , 15, 16, 17, 18
-00025830: 2c20 3139 2c20 3230 2c20 3231 2c20 3232  , 19, 20, 21, 22
-00025840: 2c20 3233 2c20 3234 2c20 3235 2c20 3236  , 23, 24, 25, 26
-00025850: 2c20 3237 2c20 3238 2c20 3239 2c20 3330  , 27, 28, 29, 30
-00025860: 2c20 3331 205d 0d0a 6a75 6c69 616e 4461  , 31 ]..julianDa
-00025870: 7920 3d20 5b31 2c20 322c 2033 2c20 342c  y = [1, 2, 3, 4,
-00025880: 2035 2c20 362c 2037 2c20 382c 2039 2c20   5, 6, 7, 8, 9, 
-00025890: 3130 2c20 3131 2c20 3132 2c20 3133 2c20  10, 11, 12, 13, 
-000258a0: 3134 2c20 3135 2c20 3136 2c20 3137 2c20  14, 15, 16, 17, 
-000258b0: 3138 2c20 3139 2c20 3230 2c20 3231 2c20  18, 19, 20, 21, 
-000258c0: 3232 2c20 3233 2c20 3234 2c20 3235 2c20  22, 23, 24, 25, 
-000258d0: 3236 2c20 3237 2c20 3238 2c20 3239 2c20  26, 27, 28, 29, 
-000258e0: 3330 2c20 3331 2c20 3332 2c20 3333 2c20  30, 31, 32, 33, 
-000258f0: 3334 2c20 3335 2c20 3336 2c20 3337 2c20  34, 35, 36, 37, 
-00025900: 3338 2c20 3339 2c20 3430 2c20 3431 2c20  38, 39, 40, 41, 
-00025910: 3432 2c20 3433 2c20 3434 2c20 3435 2c20  42, 43, 44, 45, 
-00025920: 3436 2c20 3437 2c20 3438 2c20 3439 2c20  46, 47, 48, 49, 
-00025930: 3530 2c20 3531 2c20 3532 2c20 3533 2c20  50, 51, 52, 53, 
-00025940: 3534 2c20 3535 2c20 3536 2c20 3537 2c20  54, 55, 56, 57, 
-00025950: 3538 2c20 3539 2c20 3630 2c20 3631 2c20  58, 59, 60, 61, 
-00025960: 3632 2c20 3633 2c20 3634 2c20 3635 2c20  62, 63, 64, 65, 
-00025970: 3636 2c20 3637 2c20 3638 2c20 3639 2c20  66, 67, 68, 69, 
-00025980: 3730 2c20 3731 2c20 3732 2c20 3733 2c20  70, 71, 72, 73, 
-00025990: 3734 2c20 3735 2c20 3736 2c20 3737 2c20  74, 75, 76, 77, 
-000259a0: 3738 2c20 3739 2c20 3830 2c20 3831 2c20  78, 79, 80, 81, 
-000259b0: 3832 2c20 3833 2c20 3834 2c20 3835 2c20  82, 83, 84, 85, 
-000259c0: 3836 2c20 3837 2c20 3838 2c20 3839 2c20  86, 87, 88, 89, 
-000259d0: 3930 2c20 3931 2c20 3932 2c20 3933 2c20  90, 91, 92, 93, 
-000259e0: 3934 2c20 3935 2c20 3936 2c20 3937 2c20  94, 95, 96, 97, 
-000259f0: 3938 2c20 3939 2c20 3130 302c 2031 3031  98, 99, 100, 101
-00025a00: 2c20 3130 322c 2031 3033 2c20 3130 342c  , 102, 103, 104,
-00025a10: 2031 3035 2c20 3130 362c 2031 3037 2c20   105, 106, 107, 
-00025a20: 3130 382c 2031 3039 2c20 3131 302c 2031  108, 109, 110, 1
-00025a30: 3131 2c20 3131 322c 2031 3133 2c20 3131  11, 112, 113, 11
-00025a40: 342c 2031 3135 2c20 3131 362c 2031 3137  4, 115, 116, 117
-00025a50: 2c20 3131 382c 2031 3139 2c20 3132 302c  , 118, 119, 120,
-00025a60: 2031 3231 2c20 3132 322c 2031 3233 2c20   121, 122, 123, 
-00025a70: 3132 342c 2031 3235 2c20 3132 362c 2031  124, 125, 126, 1
-00025a80: 3237 2c20 3132 382c 2031 3239 2c20 3133  27, 128, 129, 13
-00025a90: 302c 2031 3331 2c20 3133 322c 2031 3333  0, 131, 132, 133
-00025aa0: 2c20 3133 342c 2031 3335 2c20 3133 362c  , 134, 135, 136,
-00025ab0: 2031 3337 2c20 3133 382c 2031 3339 2c20   137, 138, 139, 
-00025ac0: 3134 302c 2031 3431 2c20 3134 322c 2031  140, 141, 142, 1
-00025ad0: 3433 2c20 3134 342c 2031 3435 2c20 3134  43, 144, 145, 14
-00025ae0: 362c 2031 3437 2c20 3134 382c 2031 3439  6, 147, 148, 149
-00025af0: 2c20 3135 302c 2031 3531 2c20 3135 322c  , 150, 151, 152,
-00025b00: 2031 3533 2c20 3135 342c 2031 3535 2c20   153, 154, 155, 
-00025b10: 3135 362c 2031 3537 2c20 3135 382c 2031  156, 157, 158, 1
-00025b20: 3539 2c20 3136 302c 2031 3631 2c20 3136  59, 160, 161, 16
-00025b30: 322c 2031 3633 2c20 3136 342c 2031 3635  2, 163, 164, 165
-00025b40: 2c20 3136 362c 2031 3637 2c20 3136 382c  , 166, 167, 168,
-00025b50: 2031 3639 2c20 3137 302c 2031 3731 2c20   169, 170, 171, 
-00025b60: 3137 322c 2031 3733 2c20 3137 342c 2031  172, 173, 174, 1
-00025b70: 3735 2c20 3137 362c 2031 3737 2c20 3137  75, 176, 177, 17
-00025b80: 382c 2031 3739 2c20 3138 302c 2031 3831  8, 179, 180, 181
-00025b90: 2c20 3138 322c 2031 3833 2c20 3138 342c  , 182, 183, 184,
-00025ba0: 2031 3835 2c20 3138 362c 2031 3837 2c20   185, 186, 187, 
-00025bb0: 3138 382c 2031 3839 2c20 3139 302c 2031  188, 189, 190, 1
-00025bc0: 3931 2c20 3139 322c 2031 3933 2c20 3139  91, 192, 193, 19
-00025bd0: 342c 2031 3935 2c20 3139 362c 2031 3937  4, 195, 196, 197
-00025be0: 2c20 3139 382c 2031 3939 2c20 3230 302c  , 198, 199, 200,
-00025bf0: 2032 3031 2c20 3230 322c 2032 3033 2c20   201, 202, 203, 
-00025c00: 3230 342c 2032 3035 2c20 3230 362c 2032  204, 205, 206, 2
-00025c10: 3037 2c20 3230 382c 2032 3039 2c20 3231  07, 208, 209, 21
-00025c20: 302c 2032 3131 2c20 3231 322c 2032 3133  0, 211, 212, 213
-00025c30: 2c20 3231 342c 2032 3135 2c20 3231 362c  , 214, 215, 216,
-00025c40: 2032 3137 2c20 3231 382c 2032 3139 2c20   217, 218, 219, 
-00025c50: 3232 302c 2032 3231 2c20 3232 322c 2032  220, 221, 222, 2
-00025c60: 3233 2c20 3232 342c 2032 3235 2c20 3232  23, 224, 225, 22
-00025c70: 362c 2032 3237 2c20 3232 382c 2032 3239  6, 227, 228, 229
-00025c80: 2c20 3233 302c 2032 3331 2c20 3233 322c  , 230, 231, 232,
-00025c90: 2032 3333 2c20 3233 342c 2032 3335 2c20   233, 234, 235, 
-00025ca0: 3233 362c 2032 3337 2c20 3233 382c 2032  236, 237, 238, 2
-00025cb0: 3339 2c20 3234 302c 2032 3431 2c20 3234  39, 240, 241, 24
-00025cc0: 322c 2032 3433 2c20 3234 342c 2032 3435  2, 243, 244, 245
-00025cd0: 2c20 3234 362c 2032 3437 2c20 3234 382c  , 246, 247, 248,
-00025ce0: 2032 3439 2c20 3235 302c 2032 3531 2c20   249, 250, 251, 
-00025cf0: 3235 322c 2032 3533 2c20 3235 342c 2032  252, 253, 254, 2
-00025d00: 3535 2c20 3235 362c 2032 3537 2c20 3235  55, 256, 257, 25
-00025d10: 382c 2032 3539 2c20 3236 302c 2032 3631  8, 259, 260, 261
-00025d20: 2c20 3236 322c 2032 3633 2c20 3236 342c  , 262, 263, 264,
-00025d30: 2032 3635 2c20 3236 362c 2032 3637 2c20   265, 266, 267, 
-00025d40: 3236 382c 2032 3639 2c20 3237 302c 2032  268, 269, 270, 2
-00025d50: 3731 2c20 3237 322c 2032 3733 2c20 3237  71, 272, 273, 27
-00025d60: 342c 2032 3735 2c20 3237 362c 2032 3737  4, 275, 276, 277
-00025d70: 2c20 3237 382c 2032 3739 2c20 3238 302c  , 278, 279, 280,
-00025d80: 2032 3831 2c20 3238 322c 2032 3833 2c20   281, 282, 283, 
-00025d90: 3238 342c 2032 3835 2c20 3238 362c 2032  284, 285, 286, 2
-00025da0: 3837 2c20 3238 382c 2032 3839 2c20 3239  87, 288, 289, 29
-00025db0: 302c 2032 3931 2c20 3239 322c 2032 3933  0, 291, 292, 293
-00025dc0: 2c20 3239 342c 2032 3935 2c20 3239 362c  , 294, 295, 296,
-00025dd0: 2032 3937 2c20 3239 382c 2032 3939 2c20   297, 298, 299, 
-00025de0: 3330 302c 2033 3031 2c20 3330 322c 2033  300, 301, 302, 3
-00025df0: 3033 2c20 3330 342c 2033 3035 2c20 3330  03, 304, 305, 30
-00025e00: 362c 2033 3037 2c20 3330 382c 2033 3039  6, 307, 308, 309
-00025e10: 2c20 3331 302c 2033 3131 2c20 3331 322c  , 310, 311, 312,
-00025e20: 2033 3133 2c20 3331 342c 2033 3135 2c20   313, 314, 315, 
-00025e30: 3331 362c 2033 3137 2c20 3331 382c 2033  316, 317, 318, 3
-00025e40: 3139 2c20 3332 302c 2033 3231 2c20 3332  19, 320, 321, 32
-00025e50: 322c 2033 3233 2c20 3332 342c 2033 3235  2, 323, 324, 325
-00025e60: 2c20 3332 362c 2033 3237 2c20 3332 382c  , 326, 327, 328,
-00025e70: 2033 3239 2c20 3333 302c 2033 3331 2c20   329, 330, 331, 
-00025e80: 3333 322c 2033 3333 2c20 3333 342c 2033  332, 333, 334, 3
-00025e90: 3335 2c20 3333 362c 2033 3337 2c20 3333  35, 336, 337, 33
-00025ea0: 382c 2033 3339 2c20 3334 302c 2033 3431  8, 339, 340, 341
-00025eb0: 2c20 3334 322c 2033 3433 2c20 3334 342c  , 342, 343, 344,
-00025ec0: 2033 3435 2c20 3334 362c 2033 3437 2c20   345, 346, 347, 
-00025ed0: 3334 382c 2033 3439 2c20 3335 302c 2033  348, 349, 350, 3
-00025ee0: 3531 2c20 3335 322c 2033 3533 2c20 3335  51, 352, 353, 35
-00025ef0: 342c 2033 3535 2c20 3335 362c 2033 3537  4, 355, 356, 357
-00025f00: 2c20 3335 382c 2033 3539 2c20 3336 302c  , 358, 359, 360,
-00025f10: 2033 3631 2c20 3336 322c 2033 3633 2c20   361, 362, 363, 
-00025f20: 3336 342c 2033 3635 205d 0d0a 0d0a 2323  364, 365 ]....##
-00025f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f70: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
-00025f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025fa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025fc0: 2323 0d0a 2346 756e 6374 696f 6e20 666f  ##..#Function fo
-00025fd0: 7220 6765 7474 696e 6720 7468 6520 6461  r getting the da
-00025fe0: 7465 206f 6620 7468 6520 7065 616b 206f  te of the peak o
-00025ff0: 6620 7665 6720 7669 676f 722d 2063 616e  f veg vigor- can
-00026000: 2068 616e 646c 6520 6261 6e64 7320 6e65   handle bands ne
-00026010: 6761 7469 7665 6c79 2063 6f72 7265 6c61  gatively correla
-00026020: 7465 6420 746f 2076 6567 2069 6e0d 0a23  ted to veg in..#
-00026030: 6368 616e 6765 4469 7244 6963 7420 6469  changeDirDict di
-00026040: 6374 696f 6e61 7279 2061 626f 7665 0d0a  ctionary above..
-00026050: 6465 6620 6765 7450 6561 6b44 6174 6528  def getPeakDate(
-00026060: 636f 6566 6673 2c70 6561 6b44 6972 6563  coeffs,peakDirec
-00026070: 7469 6f6e 203d 2031 293a 0d0a 0d0a 2020  tion = 1):....  
-00026080: 7369 6e20 3d20 636f 6566 6673 2e73 656c  sin = coeffs.sel
-00026090: 6563 7428 5b30 5d29 0d0a 2020 636f 7320  ect([0])..  cos 
-000260a0: 3d20 636f 6566 6673 2e73 656c 6563 7428  = coeffs.select(
-000260b0: 5b31 5d29 0d0a 0d0a 2020 2346 696e 6420  [1])....  #Find 
-000260c0: 7768 6572 6520 696e 2063 7963 6c65 2073  where in cycle s
-000260d0: 6c6f 7065 2069 7320 7a65 726f 0d0a 2020  lope is zero..  
-000260e0: 6772 6565 6e44 6174 6520 3d20 2828 7369  greenDate = ((si
-000260f0: 6e2e 6469 7669 6465 2863 6f73 2929 2e61  n.divide(cos)).a
-00026100: 7461 6e28 2929 2e64 6976 6964 6528 322a  tan()).divide(2*
-00026110: 6d61 7468 2e70 6929 2e72 656e 616d 6528  math.pi).rename(
-00026120: 5b27 7065 616b 4461 7465 275d 290d 0a20  ['peakDate']).. 
-00026130: 2067 7265 656e 4461 7465 4c61 7465 7220   greenDateLater 
-00026140: 3d20 6772 6565 6e44 6174 652e 6164 6428  = greenDate.add(
-00026150: 302e 3529 0d0a 2020 2343 6865 636b 2077  0.5)..  #Check w
-00026160: 6869 6368 2064 3120 736c 6f70 6520 3d20  hich d1 slope = 
-00026170: 3020 6973 2074 6865 206d 6178 2062 7920  0 is the max by 
-00026180: 7072 6564 6963 7469 6e67 206f 7574 2074  predicting out t
-00026190: 6865 2076 616c 7565 0d0a 2020 7072 6564  he value..  pred
-000261a0: 6963 7465 6431 203d 2063 6f65 6666 732e  icted1 = coeffs.
-000261b0: 7365 6c65 6374 285b 305d 295c 0d0a 2020  select([0])\..  
-000261c0: 2020 2020 2020 2020 2020 2020 2e61 6464              .add
-000261d0: 2873 696e 2e6d 756c 7469 706c 7928 6772  (sin.multiply(gr
-000261e0: 6565 6e44 6174 652e 6d75 6c74 6970 6c79  eenDate.multiply
-000261f0: 2832 2a6d 6174 682e 7069 292e 7369 6e28  (2*math.pi).sin(
-00026200: 2929 295c 0d0a 2020 2020 2020 2020 2020  )))\..          
-00026210: 2020 2020 2e61 6464 2863 6f73 2e6d 756c      .add(cos.mul
-00026220: 7469 706c 7928 6772 6565 6e44 6174 652e  tiply(greenDate.
-00026230: 6d75 6c74 6970 6c79 2832 2a6d 6174 682e  multiply(2*math.
-00026240: 7069 292e 636f 7328 2929 295c 0d0a 2020  pi).cos()))\..  
-00026250: 2020 2020 2020 2020 2020 2020 2e72 656e              .ren
-00026260: 616d 6528 5b27 7072 6564 6963 7465 6427  ame(['predicted'
-00026270: 5d29 5c0d 0a20 2020 2020 2020 2020 2020  ])\..           
-00026280: 2020 202e 6d75 6c74 6970 6c79 2865 652e     .multiply(ee.
-00026290: 496d 6167 652e 636f 6e73 7461 6e74 2870  Image.constant(p
-000262a0: 6561 6b44 6972 6563 7469 6f6e 2929 5c0d  eakDirection))\.
-000262b0: 0a20 2020 2020 2020 2020 2020 2020 202e  .              .
-000262c0: 6164 6442 616e 6473 2867 7265 656e 4461  addBands(greenDa
-000262d0: 7465 290d 0a20 2070 7265 6469 6374 6564  te)..  predicted
-000262e0: 3220 3d20 636f 6566 6673 2e73 656c 6563  2 = coeffs.selec
-000262f0: 7428 5b30 5d29 5c0d 0a20 2020 2020 2020  t([0])\..       
-00026300: 2020 2020 2020 202e 6164 6428 7369 6e2e         .add(sin.
-00026310: 6d75 6c74 6970 6c79 2867 7265 656e 4461  multiply(greenDa
-00026320: 7465 4c61 7465 722e 6d75 6c74 6970 6c79  teLater.multiply
-00026330: 2832 2a6d 6174 682e 7069 292e 7369 6e28  (2*math.pi).sin(
-00026340: 2929 295c 0d0a 2020 2020 2020 2020 2020  )))\..          
-00026350: 2020 2020 2e61 6464 2863 6f73 2e6d 756c      .add(cos.mul
-00026360: 7469 706c 7928 6772 6565 6e44 6174 654c  tiply(greenDateL
-00026370: 6174 6572 2e6d 756c 7469 706c 7928 322a  ater.multiply(2*
-00026380: 6d61 7468 2e70 6929 2e63 6f73 2829 2929  math.pi).cos()))
-00026390: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-000263a0: 202e 7265 6e61 6d65 285b 2770 7265 6469   .rename(['predi
-000263b0: 6374 6564 275d 295c 0d0a 2020 2020 2020  cted'])\..      
-000263c0: 2020 2020 2020 2020 2e6d 756c 7469 706c          .multipl
-000263d0: 7928 6565 2e49 6d61 6765 2e63 6f6e 7374  y(ee.Image.const
-000263e0: 616e 7428 7065 616b 4469 7265 6374 696f  ant(peakDirectio
-000263f0: 6e29 295c 0d0a 2020 2020 2020 2020 2020  n))\..          
-00026400: 2020 2020 2e61 6464 4261 6e64 7328 6772      .addBands(gr
-00026410: 6565 6e44 6174 654c 6174 6572 290d 0a20  eenDateLater).. 
-00026420: 2066 696e 616c 4772 6565 6e44 6174 6520   finalGreenDate 
-00026430: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
-00026440: 7469 6f6e 285b 7072 6564 6963 7465 6431  tion([predicted1
-00026450: 2c70 7265 6469 6374 6564 325d 292e 7175  ,predicted2]).qu
-00026460: 616c 6974 794d 6f73 6169 6328 2770 7265  alityMosaic('pre
-00026470: 6469 6374 6564 2729 2e73 656c 6563 7428  dicted').select(
-00026480: 5b27 7065 616b 4461 7465 275d 292e 7265  ['peakDate']).re
-00026490: 6e61 6d65 285b 2770 6561 6b4a 756c 6961  name(['peakJulia
-000264a0: 6e44 6179 275d 290d 0a0d 0a20 2066 696e  nDay'])....  fin
-000264b0: 616c 4772 6565 6e44 6174 6520 3d20 6669  alGreenDate = fi
-000264c0: 6e61 6c47 7265 656e 4461 7465 2e77 6865  nalGreenDate.whe
-000264d0: 7265 2866 696e 616c 4772 6565 6e44 6174  re(finalGreenDat
-000264e0: 652e 6c74 2830 292c 2067 7265 656e 4461  e.lt(0), greenDa
-000264f0: 7465 2e61 6464 2831 2929 2e6d 756c 7469  te.add(1)).multi
-00026500: 706c 7928 3336 3529 2e69 6e74 3136 2829  ply(365).int16()
-00026510: 3b0d 0a0d 0a20 2023 436f 6e76 6572 7420  ;....  #Convert 
-00026520: 746f 206d 6f6e 7468 2061 6e64 2064 6179  to month and day
-00026530: 206f 6620 6d6f 6e74 680d 0a20 2067 7265   of month..  gre
-00026540: 656e 4d6f 6e74 6820 3d20 6669 6e61 6c47  enMonth = finalG
-00026550: 7265 656e 4461 7465 2e72 656d 6170 286a  reenDate.remap(j
-00026560: 756c 6961 6e44 6179 2c6d 6f6e 7468 5265  ulianDay,monthRe
-00026570: 6d61 7029 2e72 656e 616d 6528 5b27 7065  map).rename(['pe
-00026580: 616b 4d6f 6e74 6827 5d29 0d0a 2020 6772  akMonth'])..  gr
-00026590: 6565 6e4d 6f6e 7468 4461 7920 3d20 6669  eenMonthDay = fi
-000265a0: 6e61 6c47 7265 656e 4461 7465 2e72 656d  nalGreenDate.rem
-000265b0: 6170 286a 756c 6961 6e44 6179 2c6d 6f6e  ap(julianDay,mon
-000265c0: 7468 4461 7952 656d 6170 292e 7265 6e61  thDayRemap).rena
-000265d0: 6d65 285b 2770 6561 6b44 6179 4f66 4d6f  me(['peakDayOfMo
-000265e0: 6e74 6827 5d29 0d0a 2020 6772 6565 6e53  nth'])..  greenS
-000265f0: 7461 636b 203d 2066 696e 616c 4772 6565  tack = finalGree
-00026600: 6e44 6174 652e 6164 6442 616e 6473 2867  nDate.addBands(g
-00026610: 7265 656e 4d6f 6e74 6829 2e61 6464 4261  reenMonth).addBa
-00026620: 6e64 7328 6772 6565 6e4d 6f6e 7468 4461  nds(greenMonthDa
-00026630: 7929 0d0a 2020 7265 7475 726e 2067 7265  y)..  return gre
-00026640: 656e 5374 6163 6b0d 0a20 2023 4d61 702e  enStack..  #Map.
-00026650: 6164 644c 6179 6572 2867 7265 656e 5374  addLayer(greenSt
-00026660: 6163 6b2c 7b27 6d69 6e27 3a31 2c27 6d61  ack,{'min':1,'ma
-00026670: 7827 3a31 327d 2c27 6772 6565 6e4d 6f6e  x':12},'greenMon
-00026680: 7468 272c 4661 6c73 6529 0d0a 0d0a 2323  th',False)....##
-00026690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000266a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000266b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000266c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000266d0: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
-000266e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000266f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026720: 2323 0d0a 2346 756e 6374 696f 6e20 666f  ##..#Function fo
-00026730: 7220 6765 7474 696e 6720 6c65 6674 2073  r getting left s
-00026740: 756d 2075 6e64 6572 2074 6865 2063 7572  um under the cur
-00026750: 7665 2066 6f72 2061 2073 696e 676c 6520  ve for a single 
-00026760: 6772 6f77 696e 6720 7365 6173 6f6e 0d0a  growing season..
-00026770: 2354 616b 6573 2063 6172 6520 6f66 206e  #Takes care of n
-00026780: 6f72 6d61 6c69 7a61 7469 6f6e 2062 7920  ormalization by 
-00026790: 666f 7263 696e 6720 7468 6520 6d69 6e20  forcing the min 
-000267a0: 7661 6c75 6520 616c 6f6e 6720 7468 6520  value along the 
-000267b0: 6375 7276 6520 300d 0a23 6279 2074 616b  curve 0..#by tak
-000267c0: 696e 6720 7468 6520 616d 706c 6974 7564  ing the amplitud
-000267d0: 6520 6173 2074 6865 2069 6e74 6572 6365  e as the interce
-000267e0: 7074 0d0a 2341 7373 756d 6573 2074 6865  pt..#Assumes the
-000267f0: 2073 696e 2061 6e64 2063 6f73 2063 6f65   sin and cos coe
-00026800: 6666 7320 6172 6520 7468 6520 6861 726d  ffs are the harm
-00026810: 436f 6566 6673 0d0a 2374 3020 6973 2074  Coeffs..#t0 is t
-00026820: 6865 2073 7461 7274 2074 696d 6520 2864  he start time (d
-00026830: 6566 6175 6c74 7320 746f 2030 2928 6d69  efaults to 0)(mi
-00026840: 6e20 7661 6c75 6520 7368 6f75 6c64 2062  n value should b
-00026850: 6520 6275 7420 646f 6573 6e27 7420 6861  e but doesn't ha
-00026860: 7665 2074 6f20 6265 2030 290d 0a23 7431  ve to be 0)..#t1
-00026870: 2069 7320 7468 6520 656e 6420 7469 6d65   is the end time
-00026880: 2028 6465 6661 756c 7473 2074 6f20 3129   (defaults to 1)
-00026890: 286d 6178 2076 616c 7565 2073 686f 756c  (max value shoul
-000268a0: 6420 6265 2062 7574 2064 6f65 736e 2774  d be but doesn't
-000268b0: 2068 6176 6520 746f 2062 6520 3129 0d0a   have to be 1)..
-000268c0: 0d0a 2345 7861 6d70 6c65 206f 6620 7768  ..#Example of wh
-000268d0: 6174 2074 6869 7320 636f 6465 2069 7320  at this code is 
-000268e0: 646f 696e 6720 6361 6e20 6265 2066 6f75  doing can be fou
-000268f0: 6e64 2068 6572 653a 0d0a 2320 2068 7474  nd here:..#  htt
-00026900: 703a 2f2f 7777 772e 776f 6c66 7261 6d61  p://www.wolframa
-00026910: 6c70 6861 2e63 6f6d 2f69 6e70 7574 2f3f  lpha.com/input/?
-00026920: 693d 696e 7465 6772 6174 652b 302e 3135  i=integrate+0.15
-00026930: 3934 3930 3734 3932 3339 3932 3135 372b  949074923992157+
-00026940: 2532 422b 2d30 2e30 3832 3837 3539 392a  %2B+-0.08287599*
-00026950: 7369 6e28 322b 5049 2b54 292b 2532 422b  sin(2+PI+T)+%2B+
-00026960: 2d30 2e31 3132 3532 3031 3036 3133 2a63  -0.11252010613*c
-00026970: 6f73 2832 2b50 492b 5429 2b2b 6672 6f6d  os(2+PI+T)++from
-00026980: 2b30 2b74 6f2b 310d 0a64 6566 2067 6574  +0+to+1..def get
-00026990: 4172 6561 556e 6465 7243 7572 7665 2868  AreaUnderCurve(h
-000269a0: 6172 6d43 6f65 6666 732c 7430 3d20 302c  armCoeffs,t0= 0,
-000269b0: 7431 203d 2031 293a 0d0a 0d0a 2020 2350  t1 = 1):....  #P
-000269c0: 756c 6c20 6170 6172 7420 7468 6520 6d6f  ull apart the mo
-000269d0: 6465 6c0d 0a20 2061 6d70 6c69 7475 6465  del..  amplitude
-000269e0: 203d 2068 6172 6d43 6f65 6666 732e 7365   = harmCoeffs.se
-000269f0: 6c65 6374 285b 315d 292e 6879 706f 7428  lect([1]).hypot(
-00026a00: 6861 726d 436f 6566 6673 2e73 656c 6563  harmCoeffs.selec
-00026a10: 7428 5b30 5d29 290d 0a20 2069 6e74 6572  t([0]))..  inter
-00026a20: 6563 6570 744e 6f72 6d61 6c69 7a65 6420  eceptNormalized 
-00026a30: 3d20 616d 706c 6974 7564 6523 5768 656e  = amplitude#When
-00026a40: 206d 616b 696e 6720 7468 6520 6d69 6e20   making the min 
-00026a50: 302c 2074 6865 2069 6e74 6572 6365 7074  0, the intercept
-00026a60: 2062 6563 6f6d 6573 2074 6865 2061 6d70   becomes the amp
-00026a70: 6c69 7475 6465 2028 7468 6520 6879 706f  litude (the hypo
-00026a80: 7465 6e75 7365 290d 0a20 2073 696e 203d  tenuse)..  sin =
-00026a90: 2068 6172 6d43 6f65 6666 732e 7365 6c65   harmCoeffs.sele
-00026aa0: 6374 285b 305d 290d 0a20 2063 6f73 203d  ct([0])..  cos =
-00026ab0: 2068 6172 6d43 6f65 6666 732e 7365 6c65   harmCoeffs.sele
-00026ac0: 6374 285b 315d 290d 0a0d 0a20 2023 4669  ct([1])....  #Fi
-00026ad0: 6e64 2074 6865 2073 756d 2066 726f 6d20  nd the sum from 
-00026ae0: 2d20 696e 6669 6e69 7479 2074 6f20 300d  - infinity to 0.
-00026af0: 0a20 2073 756d 3020 3d20 696e 7465 7265  .  sum0 = intere
-00026b00: 6365 7074 4e6f 726d 616c 697a 6564 2e6d  ceptNormalized.m
-00026b10: 756c 7469 706c 7928 7430 295c 0d0a 2020  ultiply(t0)\..  
-00026b20: 2020 2020 2020 2020 2020 2e73 7562 7472            .subtr
-00026b30: 6163 7428 7369 6e2e 6469 7669 6465 2832  act(sin.divide(2
-00026b40: 2a6d 6174 682e 7069 292e 6d75 6c74 6970  *math.pi).multip
-00026b50: 6c79 286d 6174 682e 7369 6e28 322a 6d61  ly(math.sin(2*ma
-00026b60: 7468 2e70 692a 7430 2929 295c 0d0a 2020  th.pi*t0)))\..  
-00026b70: 2020 2020 2020 2020 2020 2e61 6464 2863            .add(c
-00026b80: 6f73 2e64 6976 6964 6528 322a 6d61 7468  os.divide(2*math
-00026b90: 2e70 6929 2e6d 756c 7469 706c 7928 6d61  .pi).multiply(ma
-00026ba0: 7468 2e63 6f73 2832 2a6d 6174 682e 7069  th.cos(2*math.pi
-00026bb0: 2a74 3029 2929 0d0a 2020 2346 696e 6420  *t0)))..  #Find 
-00026bc0: 7468 6520 7375 6d20 6672 6f6d 202d 2069  the sum from - i
-00026bd0: 6e66 696e 6974 7920 746f 2031 0d0a 2020  nfinity to 1..  
-00026be0: 7375 6d31 203d 2069 6e74 6572 6563 6570  sum1 = interecep
-00026bf0: 744e 6f72 6d61 6c69 7a65 642e 6d75 6c74  tNormalized.mult
-00026c00: 6970 6c79 2874 3129 5c0d 0a20 2020 2020  iply(t1)\..     
-00026c10: 2020 202e 7375 6274 7261 6374 2873 696e     .subtract(sin
-00026c20: 2e64 6976 6964 6528 322a 6d61 7468 2e70  .divide(2*math.p
-00026c30: 6929 2e6d 756c 7469 706c 7928 6d61 7468  i).multiply(math
-00026c40: 2e73 696e 2832 2a6d 6174 682e 7069 2a74  .sin(2*math.pi*t
-00026c50: 3129 2929 5c0d 0a20 2020 2020 2020 202e  1)))\..        .
-00026c60: 6164 6428 636f 732e 6469 7669 6465 2832  add(cos.divide(2
-00026c70: 2a6d 6174 682e 7069 292e 6d75 6c74 6970  *math.pi).multip
-00026c80: 6c79 286d 6174 682e 636f 7328 322a 6d61  ly(math.cos(2*ma
-00026c90: 7468 2e70 692a 7431 2929 290d 0a20 2023  th.pi*t1)))..  #
-00026ca0: 4669 6e64 2074 6865 2064 6966 6665 7265  Find the differe
-00026cb0: 6e63 650d 0a20 206c 6566 7453 756d 203d  nce..  leftSum =
-00026cc0: 2073 756d 312e 7375 6274 7261 6374 2873   sum1.subtract(s
-00026cd0: 756d 3029 2e72 656e 616d 6528 5b27 4155  um0).rename(['AU
-00026ce0: 4327 5d29 0d0a 2020 7265 7475 726e 206c  C'])..  return l
-00026cf0: 6566 7453 756d 0d0a 0d0a 2323 2323 2323  eftSum....######
-00026d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d40: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
-00026d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026d80: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00026d90: 6465 6620 6765 7450 6861 7365 416d 706c  def getPhaseAmpl
-00026da0: 6974 7564 6550 6561 6b28 636f 6566 6673  itudePeak(coeffs
-00026db0: 2c74 3020 3d20 302c 7431 203d 2031 293a  ,t0 = 0,t1 = 1):
-00026dc0: 0d0a 2020 2350 6172 7365 2074 6865 206d  ..  #Parse the m
-00026dd0: 6f64 656c 0d0a 2020 6261 6e64 4e61 6d65  odel..  bandName
-00026de0: 7320 3d20 636f 6566 6673 2e62 616e 644e  s = coeffs.bandN
-00026df0: 616d 6573 2829 0d0a 2020 6261 6e64 4e75  ames()..  bandNu
-00026e00: 6d62 6572 203d 2062 616e 644e 616d 6573  mber = bandNames
-00026e10: 2e6c 656e 6774 6828 290d 0a20 206e 6f44  .length()..  noD
-00026e20: 6570 656e 6465 6e74 7320 3d20 6565 2e4e  ependents = ee.N
-00026e30: 756d 6265 7228 636f 6566 6673 2e67 6574  umber(coeffs.get
-00026e40: 2827 6e6f 4465 7065 6e64 656e 7473 2729  ('noDependents')
-00026e50: 290d 0a20 206d 6f64 656c 4c65 6e67 7468  )..  modelLength
-00026e60: 203d 2065 652e 4e75 6d62 6572 2863 6f65   = ee.Number(coe
-00026e70: 6666 732e 6765 7428 276d 6f64 656c 4c65  ffs.get('modelLe
-00026e80: 6e67 7468 2729 290d 0a20 2069 6e74 6572  ngth'))..  inter
-00026e90: 6365 7074 4261 6e64 7320 3d20 6565 2e4c  ceptBands = ee.L
-00026ea0: 6973 742e 7365 7175 656e 6365 2830 2c62  ist.sequence(0,b
-00026eb0: 616e 644e 756d 6265 722e 7375 6274 7261  andNumber.subtra
-00026ec0: 6374 2831 292c 6d6f 6465 6c4c 656e 6774  ct(1),modelLengt
-00026ed0: 6829 0d0a 0d0a 2020 6d6f 6465 6c73 203d  h)....  models =
-00026ee0: 2065 652e 4c69 7374 2e73 6571 7565 6e63   ee.List.sequenc
-00026ef0: 6528 302c 6e6f 4465 7065 6e64 656e 7473  e(0,noDependents
-00026f00: 2e73 7562 7472 6163 7428 3129 290d 0a0d  .subtract(1))...
-00026f10: 0a20 2064 6566 206d 6f64 656c 4765 7474  .  def modelGett
-00026f20: 6572 286d 6e29 3a0d 0a20 2020 206d 6e20  er(mn):..    mn 
-00026f30: 3d20 6565 2e4e 756d 6265 7228 6d6e 290d  = ee.Number(mn).
-00026f40: 0a20 2020 2072 6574 7572 6e20 6261 6e64  .    return band
-00026f50: 4e61 6d65 732e 736c 6963 6528 6d6e 2e6d  Names.slice(mn.m
-00026f60: 756c 7469 706c 7928 6d6f 6465 6c4c 656e  ultiply(modelLen
-00026f70: 6774 6829 2c6d 6e2e 6d75 6c74 6970 6c79  gth),mn.multiply
-00026f80: 286d 6f64 656c 4c65 6e67 7468 292e 6164  (modelLength).ad
-00026f90: 6428 6d6f 6465 6c4c 656e 6774 6829 290d  d(modelLength)).
-00026fa0: 0a0d 0a20 2070 6172 7365 644d 6f64 656c  ...  parsedModel
-00026fb0: 203d 6d6f 6465 6c73 2e6d 6170 286d 6f64   =models.map(mod
-00026fc0: 656c 4765 7474 6572 290d 0a0d 0a0d 0a20  elGetter)...... 
-00026fd0: 2023 7072 696e 7428 2750 6172 7365 6420   #print('Parsed 
-00026fe0: 6861 726d 6f6e 6963 2072 6567 7265 7373  harmonic regress
-00026ff0: 696f 6e20 6d6f 6465 6c27 2c70 6172 7365  ion model',parse
-00027000: 644d 6f64 656c 290d 0a0d 0a20 2023 4974  dModel)....  #It
-00027010: 6572 6174 6520 6163 726f 7373 206d 6f64  erate across mod
-00027020: 656c 7320 746f 2063 6f6e 7665 7274 2074  els to convert t
-00027030: 6f20 7068 6173 652c 2061 6d70 6c69 7475  o phase, amplitu
-00027040: 6465 2c20 616e 6420 7065 616b 0d0a 2020  de, and peak..  
-00027050: 6465 6620 7061 7047 6574 7465 7228 706d  def papGetter(pm
-00027060: 293a 0d0a 2020 2020 706d 203d 2065 652e  ):..    pm = ee.
-00027070: 4c69 7374 2870 6d29 3b0d 0a20 2020 206d  List(pm);..    m
-00027080: 6f64 656c 436f 6566 6673 203d 2063 6f65  odelCoeffs = coe
-00027090: 6666 732e 7365 6c65 6374 2870 6d29 0d0a  ffs.select(pm)..
-000270a0: 0d0a 2020 2020 696e 7465 7263 6570 7420  ..    intercept 
-000270b0: 3d20 6d6f 6465 6c43 6f65 6666 732e 7365  = modelCoeffs.se
-000270c0: 6c65 6374 2827 2e2a 5f69 6e74 6572 6365  lect('.*_interce
-000270d0: 7074 2729 0d0a 2020 2020 6861 726d 436f  pt')..    harmCo
-000270e0: 6566 6673 203d 206d 6f64 656c 436f 6566  effs = modelCoef
-000270f0: 6673 2e73 656c 6563 7428 272e 2a5f 3230  fs.select('.*_20
-00027100: 305f 7965 6172 2729 0d0a 2020 2020 6f75  0_year')..    ou
-00027110: 744e 616d 6520 3d20 6565 2e53 7472 696e  tName = ee.Strin
-00027120: 6728 6565 2e53 7472 696e 6728 706d 2e67  g(ee.String(pm.g
-00027130: 6574 2831 2929 2e73 706c 6974 2827 5f27  et(1)).split('_'
-00027140: 292e 6765 7428 3029 290d 0a20 2020 2073  ).get(0))..    s
-00027150: 6967 6e20 3d20 6565 2e4e 756d 6265 7228  ign = ee.Number(
-00027160: 6565 2e44 6963 7469 6f6e 6172 7928 6368  ee.Dictionary(ch
-00027170: 616e 6765 4469 7244 6963 7429 2e67 6574  angeDirDict).get
-00027180: 286f 7574 4e61 6d65 2929 2e6d 756c 7469  (outName)).multi
-00027190: 706c 7928 2d31 290d 0a0d 0a20 2020 2061  ply(-1)....    a
-000271a0: 6d70 6c69 7475 6465 203d 2068 6172 6d43  mplitude = harmC
-000271b0: 6f65 6666 732e 7365 6c65 6374 285b 315d  oeffs.select([1]
-000271c0: 292e 6879 706f 7428 6861 726d 436f 6566  ).hypot(harmCoef
-000271d0: 6673 2e73 656c 6563 7428 5b30 5d29 295c  fs.select([0]))\
-000271e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000271f0: 2e6d 756c 7469 706c 7928 3229 5c0d 0a20  .multiply(2)\.. 
-00027200: 2020 2020 2020 2020 2020 2020 202e 7265               .re
-00027210: 6e61 6d65 285b 6f75 744e 616d 652e 6361  name([outName.ca
-00027220: 7428 275f 616d 706c 6974 7564 6527 295d  t('_amplitude')]
-00027230: 290d 0a20 2020 2070 6861 7365 203d 2068  )..    phase = h
-00027240: 6172 6d43 6f65 6666 732e 7365 6c65 6374  armCoeffs.select
-00027250: 285b 305d 292e 6174 616e 3228 6861 726d  ([0]).atan2(harm
-00027260: 436f 6566 6673 2e73 656c 6563 7428 5b31  Coeffs.select([1
-00027270: 5d29 295c 0d0a 2020 2020 2020 2020 2020  ]))\..          
-00027280: 2020 2020 2e75 6e69 7453 6361 6c65 282d      .unitScale(-
-00027290: 6d61 7468 2e70 692c 206d 6174 682e 7069  math.pi, math.pi
-000272a0: 295c 0d0a 2020 2020 2020 2020 2020 2020  )\..            
-000272b0: 2020 2e72 656e 616d 6528 5b6f 7574 4e61    .rename([outNa
-000272c0: 6d65 2e63 6174 2827 5f70 6861 7365 2729  me.cat('_phase')
-000272d0: 5d29 0d0a 0d0a 2020 2020 2347 6574 2070  ])....    #Get p
-000272e0: 6561 6b20 6461 7465 2069 6e66 6f0d 0a20  eak date info.. 
-000272f0: 2020 2070 6561 6b44 6174 6520 3d20 6765     peakDate = ge
-00027300: 7450 6561 6b44 6174 6528 6861 726d 436f  tPeakDate(harmCo
-00027310: 6566 6673 2c73 6967 6e29 0d0a 2020 2020  effs,sign)..    
-00027320: 7065 616b 4461 7465 4261 6e64 4e61 6d65  peakDateBandName
-00027330: 7320 3d20 7065 616b 4461 7465 2e62 616e  s = peakDate.ban
-00027340: 644e 616d 6573 2829 0d0a 2020 2020 7065  dNames()..    pe
-00027350: 616b 4461 7465 4261 6e64 4e61 6d65 7320  akDateBandNames 
-00027360: 3d20 7065 616b 4461 7465 4261 6e64 4e61  = peakDateBandNa
-00027370: 6d65 732e 6d61 7028 6c61 6d62 6461 2062  mes.map(lambda b
-00027380: 6e3a 206f 7574 4e61 6d65 2e63 6174 2865  n: outName.cat(e
-00027390: 652e 5374 7269 6e67 2827 5f27 292e 6361  e.String('_').ca
-000273a0: 7428 6565 2e53 7472 696e 6728 626e 2929  t(ee.String(bn))
-000273b0: 2929 0d0a 0d0a 2020 2020 2347 6574 2074  ))....    #Get t
-000273c0: 6865 206c 6566 7420 7375 6d0d 0a20 2020  he left sum..   
-000273d0: 206c 6566 7453 756d 203d 2067 6574 4172   leftSum = getAr
-000273e0: 6561 556e 6465 7243 7572 7665 2868 6172  eaUnderCurve(har
-000273f0: 6d43 6f65 6666 732c 7430 2c74 3129 0d0a  mCoeffs,t0,t1)..
-00027400: 2020 2020 6c65 6674 5375 6d42 616e 644e      leftSumBandN
-00027410: 616d 6573 203d 206c 6566 7453 756d 2e62  ames = leftSum.b
-00027420: 616e 644e 616d 6573 2829 0d0a 2020 2020  andNames()..    
-00027430: 6c65 6674 5375 6d42 616e 644e 616d 6573  leftSumBandNames
-00027440: 203d 206c 6566 7453 756d 4261 6e64 4e61   = leftSumBandNa
-00027450: 6d65 732e 6d61 7028 6c61 6d62 6461 2062  mes.map(lambda b
-00027460: 6e3a 206f 7574 4e61 6d65 2e63 6174 2865  n: outName.cat(e
-00027470: 652e 5374 7269 6e67 2827 5f27 292e 6361  e.String('_').ca
-00027480: 7428 6565 2e53 7472 696e 6728 626e 2929  t(ee.String(bn))
-00027490: 2929 0d0a 0d0a 2020 2020 7265 7475 726e  ))....    return
-000274a0: 2061 6d70 6c69 7475 6465 5c0d 0a20 2020   amplitude\..   
-000274b0: 2020 2020 2020 2020 202e 6164 6442 616e           .addBan
-000274c0: 6473 2870 6861 7365 295c 0d0a 2020 2020  ds(phase)\..    
-000274d0: 2020 2020 2020 2020 2e61 6464 4261 6e64          .addBand
-000274e0: 7328 7065 616b 4461 7465 2e72 656e 616d  s(peakDate.renam
-000274f0: 6528 7065 616b 4461 7465 4261 6e64 4e61  e(peakDateBandNa
-00027500: 6d65 7329 295c 0d0a 2020 2020 2020 2020  mes))\..        
-00027510: 2020 2020 2e61 6464 4261 6e64 7328 6c65      .addBands(le
-00027520: 6674 5375 6d2e 7265 6e61 6d65 286c 6566  ftSum.rename(lef
-00027530: 7453 756d 4261 6e64 4e61 6d65 7329 290d  tSumBandNames)).
-00027540: 0a0d 0a0d 0a0d 0a20 2023 436f 6e76 6572  .......  #Conver
-00027550: 7420 746f 2061 6e20 696d 6167 650d 0a20  t to an image.. 
-00027560: 2070 6861 7365 416d 706c 6974 7564 6520   phaseAmplitude 
-00027570: 3d70 6172 7365 644d 6f64 656c 2e6d 6170  =parsedModel.map
-00027580: 2870 6170 4765 7474 6572 290d 0a0d 0a20  (papGetter).... 
-00027590: 2070 6861 7365 416d 706c 6974 7564 6520   phaseAmplitude 
-000275a0: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
-000275b0: 7469 6f6e 2e66 726f 6d49 6d61 6765 7328  tion.fromImages(
-000275c0: 7068 6173 6541 6d70 6c69 7475 6465 290d  phaseAmplitude).
-000275d0: 0a0d 0a20 2070 6861 7365 416d 706c 6974  ...  phaseAmplit
-000275e0: 7564 6520 3d20 6565 2e49 6d61 6765 2863  ude = ee.Image(c
-000275f0: 6f6c 6c65 6374 696f 6e54 6f49 6d61 6765  ollectionToImage
-00027600: 2870 6861 7365 416d 706c 6974 7564 6529  (phaseAmplitude)
-00027610: 292e 666c 6f61 7428 295c 0d0a 2020 2020  ).float()\..    
-00027620: 2020 2020 2e63 6f70 7950 726f 7065 7274      .copyPropert
-00027630: 6965 7328 636f 6566 6673 2c5b 2773 7973  ies(coeffs,['sys
-00027640: 7465 6d3a 7469 6d65 5f73 7461 7274 275d  tem:time_start']
-00027650: 290d 0a20 2023 7072 696e 7428 2770 6127  )..  #print('pa'
-00027660: 2c70 6861 7365 416d 706c 6974 7564 6529  ,phaseAmplitude)
-00027670: 3b0d 0a20 2072 6574 7572 6e20 7068 6173  ;..  return phas
-00027680: 6541 6d70 6c69 7475 6465 3b0d 0a0d 0a23  eAmplitude;....#
-00027690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276d0: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
-000276e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027720: 2323 230d 0a23 4675 6e63 7469 6f6e 2066  ###..#Function f
-00027730: 6f72 2061 7070 6c79 696e 6720 6861 726d  or applying harm
-00027740: 6f6e 6963 2072 6567 7265 7373 696f 6e20  onic regression 
-00027750: 6d6f 6465 6c20 746f 2073 6574 206f 6620  model to set of 
-00027760: 7072 6564 6963 746f 7220 7365 7473 0d0a  predictor sets..
-00027770: 6465 6620 6e65 7750 7265 6469 6374 2863  def newPredict(c
-00027780: 6f65 6666 732c 6861 726d 6f6e 6963 7329  oeffs,harmonics)
-00027790: 3a0d 0a20 2023 5061 7273 6520 7468 6520  :..  #Parse the 
-000277a0: 6d6f 6465 6c0d 0a20 2062 616e 644e 616d  model..  bandNam
-000277b0: 6573 203d 2063 6f65 6666 732e 6261 6e64  es = coeffs.band
-000277c0: 4e61 6d65 7328 290d 0a20 2062 616e 644e  Names()..  bandN
-000277d0: 756d 6265 7220 3d20 6261 6e64 4e61 6d65  umber = bandName
-000277e0: 732e 6c65 6e67 7468 2829 0d0a 2020 6e6f  s.length()..  no
-000277f0: 4465 7065 6e64 656e 7473 203d 2065 652e  Dependents = ee.
-00027800: 4e75 6d62 6572 2863 6f65 6666 732e 6765  Number(coeffs.ge
-00027810: 7428 276e 6f44 6570 656e 6465 6e74 7327  t('noDependents'
-00027820: 2929 0d0a 2020 6d6f 6465 6c4c 656e 6774  ))..  modelLengt
-00027830: 6820 3d20 6565 2e4e 756d 6265 7228 636f  h = ee.Number(co
-00027840: 6566 6673 2e67 6574 2827 6d6f 6465 6c4c  effs.get('modelL
-00027850: 656e 6774 6827 2929 0d0a 2020 696e 7465  ength'))..  inte
-00027860: 7263 6570 7442 616e 6473 203d 2065 652e  rceptBands = ee.
-00027870: 4c69 7374 2e73 6571 7565 6e63 6528 302c  List.sequence(0,
-00027880: 6261 6e64 4e75 6d62 6572 2e73 7562 7472  bandNumber.subtr
-00027890: 6163 7428 3129 2c6d 6f64 656c 4c65 6e67  act(1),modelLeng
-000278a0: 7468 290d 0a20 2074 696d 6542 616e 6420  th)..  timeBand 
-000278b0: 3d20 6565 2e4c 6973 7428 6861 726d 6f6e  = ee.List(harmon
-000278c0: 6963 732e 6765 7428 2769 6e64 4261 6e64  ics.get('indBand
-000278d0: 4e61 6d65 7327 2929 2e67 6574 2830 290d  Names')).get(0).
-000278e0: 0a20 2061 6374 7561 6c42 616e 6473 203d  .  actualBands =
-000278f0: 2068 6172 6d6f 6e69 6373 2e67 6574 2827   harmonics.get('
-00027900: 6465 7042 616e 644e 756d 6265 7273 2729  depBandNumbers')
-00027910: 0d0a 2020 696e 6442 616e 6473 203d 2068  ..  indBands = h
-00027920: 6172 6d6f 6e69 6373 2e67 6574 2827 696e  armonics.get('in
-00027930: 6442 616e 644e 756d 6265 7273 2729 0d0a  dBandNumbers')..
-00027940: 2020 696e 6442 616e 644e 616d 6573 203d    indBandNames =
-00027950: 2065 652e 4c69 7374 2868 6172 6d6f 6e69   ee.List(harmoni
-00027960: 6373 2e67 6574 2827 696e 6442 616e 644e  cs.get('indBandN
-00027970: 616d 6573 2729 290d 0a20 2064 6570 4261  ames'))..  depBa
-00027980: 6e64 4e61 6d65 7320 3d20 6565 2e4c 6973  ndNames = ee.Lis
-00027990: 7428 6861 726d 6f6e 6963 732e 6765 7428  t(harmonics.get(
-000279a0: 2764 6570 4261 6e64 4e61 6d65 7327 2929  'depBandNames'))
-000279b0: 0d0a 2020 7072 6564 6963 7465 6442 616e  ..  predictedBan
-000279c0: 644e 616d 6573 203d 2064 6570 4261 6e64  dNames = depBand
-000279d0: 4e61 6d65 732e 6d61 7028 6c61 6d62 6461  Names.map(lambda
-000279e0: 2064 6570 626e 6d73 3a65 652e 5374 7269   depbnms:ee.Stri
-000279f0: 6e67 2864 6570 626e 6d73 292e 6361 7428  ng(depbnms).cat(
-00027a00: 275f 7072 6564 6963 7465 6427 2929 0d0a  '_predicted'))..
-00027a10: 2020 7072 6564 6963 7465 6442 616e 644e    predictedBandN
-00027a20: 756d 6265 7273 203d 2065 652e 4c69 7374  umbers = ee.List
-00027a30: 2e73 6571 7565 6e63 6528 302c 7072 6564  .sequence(0,pred
-00027a40: 6963 7465 6442 616e 644e 616d 6573 2e6c  ictedBandNames.l
-00027a50: 656e 6774 6828 292e 7375 6274 7261 6374  ength().subtract
-00027a60: 2831 2929 0d0a 0d0a 2020 6d6f 6465 6c73  (1))....  models
-00027a70: 203d 2065 652e 4c69 7374 2e73 6571 7565   = ee.List.seque
-00027a80: 6e63 6528 302c 6e6f 4465 7065 6e64 656e  nce(0,noDependen
-00027a90: 7473 2e73 7562 7472 6163 7428 3129 290d  ts.subtract(1)).
-00027aa0: 0a20 2064 6566 206d 6e47 6574 7465 7228  .  def mnGetter(
-00027ab0: 6d6e 293a 0d0a 2020 2020 6d6e 203d 2065  mn):..    mn = e
-00027ac0: 652e 4e75 6d62 6572 286d 6e29 0d0a 2020  e.Number(mn)..  
-00027ad0: 2020 7265 7475 726e 2062 616e 644e 616d    return bandNam
-00027ae0: 6573 2e73 6c69 6365 286d 6e2e 6d75 6c74  es.slice(mn.mult
-00027af0: 6970 6c79 286d 6f64 656c 4c65 6e67 7468  iply(modelLength
-00027b00: 292c 6d6e 2e6d 756c 7469 706c 7928 6d6f  ),mn.multiply(mo
-00027b10: 6465 6c4c 656e 6774 6829 2e61 6464 286d  delLength).add(m
-00027b20: 6f64 656c 4c65 6e67 7468 2929 0d0a 0d0a  odelLength))....
-00027b30: 2020 7061 7273 6564 4d6f 6465 6c20 3d6d    parsedModel =m
-00027b40: 6f64 656c 732e 6d61 7028 6d6e 4765 7474  odels.map(mnGett
-00027b50: 6572 290d 0a0d 0a20 2023 7072 696e 7428  er)....  #print(
-00027b60: 2750 6172 7365 6420 6861 726d 6f6e 6963  'Parsed harmonic
-00027b70: 2072 6567 7265 7373 696f 6e20 6d6f 6465   regression mode
-00027b80: 6c27 2c70 6172 7365 644d 6f64 656c 2c70  l',parsedModel,p
-00027b90: 7265 6469 6374 6564 4261 6e64 4e61 6d65  redictedBandName
-00027ba0: 7329 0d0a 0d0a 2020 2341 7070 6c79 2070  s)....  #Apply p
-00027bb0: 6172 7365 6420 6d6f 6465 6c0d 0a20 2064  arsed model..  d
-00027bc0: 6566 2070 7265 6447 6574 7465 7228 696d  ef predGetter(im
-00027bd0: 6729 3a0d 0a20 2020 2074 696d 6520 3d20  g):..    time = 
-00027be0: 696d 672e 7365 6c65 6374 2874 696d 6542  img.select(timeB
-00027bf0: 616e 6429 0d0a 2020 2020 6163 7475 616c  and)..    actual
-00027c00: 203d 2069 6d67 2e73 656c 6563 7428 6163   = img.select(ac
-00027c10: 7475 616c 4261 6e64 7329 2e66 6c6f 6174  tualBands).float
-00027c20: 2829 0d0a 2020 2020 7072 6564 6963 746f  ()..    predicto
-00027c30: 7242 616e 6473 203d 2069 6d67 2e73 656c  rBands = img.sel
-00027c40: 6563 7428 696e 6442 616e 644e 616d 6573  ect(indBandNames
-00027c50: 290d 0a0d 0a20 2020 2023 4974 6572 6174  )....    #Iterat
-00027c60: 6520 6163 726f 7373 2065 6163 6820 6d6f  e across each mo
-00027c70: 6465 6c20 666f 7220 6561 6368 2064 6570  del for each dep
-00027c80: 656e 6465 6e74 2076 6172 6961 626c 650d  endent variable.
-00027c90: 0a20 2020 2064 6566 2070 6d47 6574 7465  .    def pmGette
-00027ca0: 7228 706d 293a 0d0a 2020 2020 2020 706d  r(pm):..      pm
-00027cb0: 203d 2065 652e 4c69 7374 2870 6d29 0d0a   = ee.List(pm)..
-00027cc0: 2020 2020 2020 6d6f 6465 6c43 6f65 6666        modelCoeff
-00027cd0: 7320 3d20 636f 6566 6673 2e73 656c 6563  s = coeffs.selec
-00027ce0: 7428 706d 290d 0a20 2020 2020 206f 7574  t(pm)..      out
-00027cf0: 4e61 6d65 203d 2065 652e 5374 7269 6e67  Name = ee.String
-00027d00: 2870 6d2e 6765 7428 3129 292e 6361 7428  (pm.get(1)).cat(
-00027d10: 275f 7072 6564 6963 7465 6427 290d 0a20  '_predicted').. 
-00027d20: 2020 2020 2069 6e74 6572 6365 7074 203d       intercept =
-00027d30: 206d 6f64 656c 436f 6566 6673 2e73 656c   modelCoeffs.sel
-00027d40: 6563 7428 6d6f 6465 6c43 6f65 6666 732e  ect(modelCoeffs.
-00027d50: 6261 6e64 4e61 6d65 7328 292e 736c 6963  bandNames().slic
-00027d60: 6528 302c 3129 290d 0a20 2020 2020 206f  e(0,1))..      o
-00027d70: 7468 6572 7320 3d20 6d6f 6465 6c43 6f65  thers = modelCoe
-00027d80: 6666 732e 7365 6c65 6374 286d 6f64 656c  ffs.select(model
-00027d90: 436f 6566 6673 2e62 616e 644e 616d 6573  Coeffs.bandNames
-00027da0: 2829 2e73 6c69 6365 2831 2c4e 6f6e 6529  ().slice(1,None)
-00027db0: 290d 0a0d 0a20 2020 2020 2070 7265 6469  )....      predi
-00027dc0: 6374 6564 203d 2070 7265 6469 6374 6f72  cted = predictor
-00027dd0: 4261 6e64 732e 6d75 6c74 6970 6c79 286f  Bands.multiply(o
-00027de0: 7468 6572 7329 2e72 6564 7563 6528 6565  thers).reduce(ee
-00027df0: 2e52 6564 7563 6572 2e73 756d 2829 292e  .Reducer.sum()).
-00027e00: 6164 6428 696e 7465 7263 6570 7429 2e66  add(intercept).f
-00027e10: 6c6f 6174 2829 0d0a 2020 2020 2020 7265  loat()..      re
-00027e20: 7475 726e 2070 7265 6469 6374 6564 2e66  turn predicted.f
-00027e30: 6c6f 6174 2829 0d0a 0d0a 0d0a 2020 2020  loat()......    
-00027e40: 7072 6564 6963 7465 644c 6973 7420 3d70  predictedList =p
-00027e50: 6172 7365 644d 6f64 656c 2e6d 6170 2870  arsedModel.map(p
-00027e60: 6d47 6574 7465 7229 0d0a 0d0a 2020 2020  mGetter)....    
-00027e70: 2343 6f6e 7665 7274 2074 6f20 616e 2069  #Convert to an i
-00027e80: 6d61 6765 0d0a 2020 2020 7072 6564 6963  mage..    predic
-00027e90: 7465 644c 6973 7420 3d20 6565 2e49 6d61  tedList = ee.Ima
-00027ea0: 6765 436f 6c6c 6563 7469 6f6e 2e66 726f  geCollection.fro
-00027eb0: 6d49 6d61 6765 7328 7072 6564 6963 7465  mImages(predicte
-00027ec0: 644c 6973 7429 0d0a 2020 2020 7072 6564  dList)..    pred
-00027ed0: 6963 7465 6449 6d61 6765 203d 2063 6f6c  ictedImage = col
-00027ee0: 6c65 6374 696f 6e54 6f49 6d61 6765 2870  lectionToImage(p
-00027ef0: 7265 6469 6374 6564 4c69 7374 292e 7365  redictedList).se
-00027f00: 6c65 6374 2870 7265 6469 6374 6564 4261  lect(predictedBa
-00027f10: 6e64 4e75 6d62 6572 732c 7072 6564 6963  ndNumbers,predic
-00027f20: 7465 6442 616e 644e 616d 6573 290d 0a0d  tedBandNames)...
-00027f30: 0a20 2020 2023 5365 7420 736f 6d65 206d  .    #Set some m
-00027f40: 6574 6164 6174 610d 0a20 2020 206f 7574  etadata..    out
-00027f50: 203d 2061 6374 7561 6c2e 6164 6442 616e   = actual.addBan
-00027f60: 6473 2870 7265 6469 6374 6564 496d 6167  ds(predictedImag
-00027f70: 652e 666c 6f61 7428 2929 5c0d 0a20 2020  e.float())\..   
-00027f80: 202e 636f 7079 5072 6f70 6572 7469 6573   .copyProperties
-00027f90: 2869 6d67 2c5b 2773 7973 7465 6d3a 7469  (img,['system:ti
-00027fa0: 6d65 5f73 7461 7274 272c 2773 7973 7465  me_start','syste
-00027fb0: 6d3a 7469 6d65 5f65 6e64 275d 290d 0a20  m:time_end']).. 
-00027fc0: 2020 2072 6574 7572 6e20 6f75 740d 0a0d     return out...
-00027fd0: 0a20 2070 7265 6469 6374 6564 203d 6861  .  predicted =ha
-00027fe0: 726d 6f6e 6963 732e 6d61 7028 7072 6564  rmonics.map(pred
-00027ff0: 4765 7474 6572 290d 0a0d 0a20 2070 7265  Getter)....  pre
-00028000: 6469 6374 6564 203d 2065 652e 496d 6167  dicted = ee.Imag
-00028010: 6543 6f6c 6c65 6374 696f 6e28 7072 6564  eCollection(pred
-00028020: 6963 7465 6429 0d0a 0d0a 2020 234d 6170  icted)....  #Map
-00028030: 2e61 6464 4c61 7965 7228 7072 6564 6963  .addLayer(predic
-00028040: 7465 642c 7b7d 2c27 7072 6564 6963 7465  ted,{},'predicte
-00028050: 6427 2c46 616c 7365 290d 0a0d 0a20 2072  d',False)....  r
-00028060: 6574 7572 6e20 7072 6564 6963 7465 640d  eturn predicted.
-00028070: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
-00028080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000280a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000280b0: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
-000280c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000280d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000280e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000280f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028100: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
-00028110: 6f6e 2074 6f20 6765 7420 6120 6475 6d6d  on to get a dumm
-00028120: 7920 696d 6167 6520 7374 6163 6b20 666f  y image stack fo
-00028130: 7220 7379 6e74 6865 7469 6320 7469 6d65  r synthetic time
-00028140: 2073 6572 6965 730d 0a64 6566 2067 6574   series..def get
-00028150: 4461 7465 5374 6163 6b28 7374 6172 7459  DateStack(startY
-00028160: 6561 722c 656e 6459 6561 722c 7374 6172  ear,endYear,star
-00028170: 744a 756c 6961 6e2c 656e 644a 756c 6961  tJulian,endJulia
-00028180: 6e2c 6672 6571 7565 6e63 7929 3a0d 0a20  n,frequency):.. 
-00028190: 2079 6561 7273 203d 2065 652e 4c69 7374   years = ee.List
-000281a0: 2e73 6571 7565 6e63 6528 7374 6172 7459  .sequence(startY
-000281b0: 6561 722c 656e 6459 6561 7229 0d0a 2020  ear,endYear)..  
-000281c0: 6461 7465 7320 3d20 6565 2e4c 6973 742e  dates = ee.List.
-000281d0: 7365 7175 656e 6365 2873 7461 7274 4a75  sequence(startJu
-000281e0: 6c69 616e 2c65 6e64 4a75 6c69 616e 2c66  lian,endJulian,f
-000281f0: 7265 7175 656e 6379 290d 0a0d 0a20 2064  requency)....  d
-00028200: 6566 2079 7247 6574 7465 7228 7972 293a  ef yrGetter(yr):
-00028210: 0d0a 2020 2020 6465 6620 6447 6574 7465  ..    def dGette
-00028220: 7228 6429 3a0d 0a20 2020 2020 2072 6574  r(d):..      ret
-00028230: 7572 6e20 6565 2e44 6174 652e 6672 6f6d  urn ee.Date.from
-00028240: 594d 4428 7972 2c31 2c31 292e 6164 7661  YMD(yr,1,1).adva
-00028250: 6e63 6528 642c 2764 6179 2729 0d0a 2020  nce(d,'day')..  
-00028260: 2020 6473 203d 2064 6174 6573 2e6d 6170    ds = dates.map
-00028270: 2864 4765 7474 6572 290d 0a20 2020 2072  (dGetter)..    r
-00028280: 6574 7572 6e20 6473 0d0a 0d0a 2020 6461  eturn ds....  da
-00028290: 7465 5365 7473 203d 2079 6561 7273 2e6d  teSets = years.m
-000282a0: 6170 2879 7247 6574 7465 7229 0d0a 0d0a  ap(yrGetter)....
-000282b0: 2020 6c20 3d20 7261 6e67 6528 312c 6c65    l = range(1,le
-000282c0: 6e28 696e 6465 784e 616d 6573 292b 3129  n(indexNames)+1)
-000282d0: 0d0a 2020 6c20 3d20 5b69 2569 2066 6f72  ..  l = [i%i for
-000282e0: 2069 2069 6e20 6c5d 0d0a 2020 6320 3d20   i in l]..  c = 
-000282f0: 6565 2e49 6d61 6765 286c 292e 7265 6e61  ee.Image(l).rena
-00028300: 6d65 2869 6e64 6578 4e61 6d65 7329 0d0a  me(indexNames)..
-00028310: 2020 6320 3d20 632e 6469 7669 6465 2863    c = c.divide(c
-00028320: 290d 0a0d 0a20 2064 6174 6553 6574 7320  )....  dateSets 
-00028330: 3d20 6461 7465 5365 7473 2e66 6c61 7474  = dateSets.flatt
-00028340: 656e 2829 0d0a 0d0a 2020 6465 6620 6474  en()....  def dt
-00028350: 4765 7474 6572 2864 7429 3a0d 0a20 2020  Getter(dt):..   
-00028360: 2064 7420 3d20 6565 2e44 6174 6528 6474   dt = ee.Date(dt
-00028370: 290d 0a20 2020 2079 203d 2064 742e 6765  )..    y = dt.ge
-00028380: 7428 2779 6561 7227 290d 0a20 2020 2064  t('year')..    d
-00028390: 203d 2064 742e 6765 7446 7261 6374 696f   = dt.getFractio
-000283a0: 6e28 2779 6561 7227 290d 0a20 2020 2069  n('year')..    i
-000283b0: 203d 2065 652e 496d 6167 6528 792e 6164   = ee.Image(y.ad
-000283c0: 6428 6429 292e 666c 6f61 7428 292e 7365  d(d)).float().se
-000283d0: 6c65 6374 285b 305d 2c5b 2779 6561 7227  lect([0],['year'
-000283e0: 5d29 0d0a 0d0a 2020 2020 6920 3d20 632e  ])....    i = c.
-000283f0: 6164 6442 616e 6473 2869 292e 666c 6f61  addBands(i).floa
-00028400: 7428 295c 0d0a 2020 2020 2020 2e73 6574  t()\..      .set
-00028410: 2827 7379 7374 656d 3a74 696d 655f 7374  ('system:time_st
-00028420: 6172 7427 2c64 742e 6d69 6c6c 6973 2829  art',dt.millis()
-00028430: 295c 0d0a 2020 2020 2020 2e73 6574 2827  )\..      .set('
-00028440: 7379 7374 656d 3a74 696d 655f 656e 6427  system:time_end'
-00028450: 2c64 742e 6164 7661 6e63 6528 6672 6571  ,dt.advance(freq
-00028460: 7565 6e63 792c 2764 6179 2729 2e6d 696c  uency,'day').mil
-00028470: 6c69 7328 2929 0d0a 2020 2020 7265 7475  lis())..    retu
-00028480: 726e 2069 0d0a 2020 7374 6163 6b20 3d20  rn i..  stack = 
-00028490: 6461 7465 5365 7473 2e6d 6170 2864 7447  dateSets.map(dtG
-000284a0: 6574 7465 7229 0d0a 2020 7374 6163 6b20  etter)..  stack 
-000284b0: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
-000284c0: 7469 6f6e 2e66 726f 6d49 6d61 6765 7328  tion.fromImages(
-000284d0: 7374 6163 6b29 0d0a 2020 7265 7475 726e  stack)..  return
-000284e0: 2073 7461 636b 0d0a 0d0a 2323 2323 2323   stack....######
-000284f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028530: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
-00028540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028570: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00028580: 6465 6620 6765 7448 6172 6d6f 6e69 6343  def getHarmonicC
-00028590: 6f65 6666 6963 6965 6e74 7341 6e64 4669  oefficientsAndFi
-000285a0: 7428 616c 6c49 6d61 6765 732c 696e 6465  t(allImages,inde
-000285b0: 784e 616d 6573 2c77 6869 6368 4861 726d  xNames,whichHarm
-000285c0: 6f6e 6963 7320 3d20 5b32 5d2c 6465 7472  onics = [2],detr
-000285d0: 656e 6420 3d20 4661 6c73 6529 3a0d 0a0d  end = False):...
-000285e0: 0a20 2023 5365 6c65 6374 2064 6573 6972  .  #Select desir
-000285f0: 6564 2062 616e 6473 0d0a 2020 616c 6c49  ed bands..  allI
-00028600: 6e64 6963 6573 203d 2061 6c6c 496d 6167  ndices = allImag
-00028610: 6573 2e73 656c 6563 7428 696e 6465 784e  es.select(indexN
-00028620: 616d 6573 290d 0a0d 0a20 2023 4164 6420  ames)....  #Add 
-00028630: 6461 7465 2062 616e 640d 0a20 2069 6620  date band..  if 
-00028640: 6465 7472 656e 643a 0d0a 2020 2020 616c  detrend:..    al
-00028650: 6c49 6e64 6963 6573 203d 2061 6c6c 496e  lIndices = allIn
-00028660: 6469 6365 732e 6d61 7028 6164 6444 6174  dices.map(addDat
-00028670: 6542 616e 6429 0d0a 2020 656c 7365 3a0d  eBand)..  else:.
-00028680: 0a20 2020 2061 6c6c 496e 6469 6365 7320  .    allIndices 
-00028690: 3d20 616c 6c49 6e64 6963 6573 2e6d 6170  = allIndices.map
-000286a0: 2861 6464 5965 6172 4672 6163 7469 6f6e  (addYearFraction
-000286b0: 4261 6e64 290d 0a0d 0a0d 0a20 2023 4164  Band)......  #Ad
-000286c0: 6420 696e 6465 7065 6e64 656e 7420 7072  d independent pr
-000286d0: 6564 6963 746f 7273 2028 6861 726d 6f6e  edictors (harmon
-000286e0: 6963 7329 0d0a 2020 7769 7468 4861 726d  ics)..  withHarm
-000286f0: 6f6e 6963 7320 3d20 6765 7448 6172 6d6f  onics = getHarmo
-00028700: 6e69 6373 3228 616c 6c49 6e64 6963 6573  nics2(allIndices
-00028710: 2c27 7965 6172 272c 7768 6963 6848 6172  ,'year',whichHar
-00028720: 6d6f 6e69 6373 2c64 6574 7265 6e64 290d  monics,detrend).
-00028730: 0a20 2077 6974 6848 6172 6d6f 6e69 6373  .  withHarmonics
-00028740: 426e 7320 3d20 6565 2e49 6d61 6765 2877  Bns = ee.Image(w
-00028750: 6974 6848 6172 6d6f 6e69 6373 2e66 6972  ithHarmonics.fir
-00028760: 7374 2829 292e 6261 6e64 4e61 6d65 7328  st()).bandNames(
-00028770: 292e 736c 6963 6528 6c65 6e28 696e 6465  ).slice(len(inde
-00028780: 784e 616d 6573 292b 312c 4e6f 6e65 290d  xNames)+1,None).
-00028790: 0a0d 0a20 2023 4f70 7469 6f6e 616c 6c79  ...  #Optionally
-000287a0: 2063 6861 7274 2074 6865 2063 6f6c 6c65   chart the colle
-000287b0: 6374 696f 6e20 7769 7468 2068 6172 6d6f  ction with harmo
-000287c0: 6e69 6373 0d0a 0d0a 2020 2346 6974 2061  nics....  #Fit a
-000287d0: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
-000287e0: 6f6e 206d 6f64 656c 0d0a 2020 636f 6566  on model..  coef
-000287f0: 6673 203d 206e 6577 526f 6275 7374 4d75  fs = newRobustMu
-00028800: 6c74 6970 6c65 4c69 6e65 6172 3228 7769  ltipleLinear2(wi
-00028810: 7468 4861 726d 6f6e 6963 7329 0d0a 0d0a  thHarmonics)....
-00028820: 2020 2343 616e 2076 6973 7561 6c69 7a65    #Can visualize
-00028830: 2074 6865 2070 6861 7365 2061 6e64 2061   the phase and a
-00028840: 6d70 6c69 7475 6465 2069 6620 6f6e 6c79  mplitude if only
-00028850: 2074 6865 2066 6972 7374 2028 5b32 5d29   the first ([2])
-00028860: 2068 6172 6d6f 6e69 6320 6973 2063 686f   harmonic is cho
-00028870: 7365 6e0d 0a20 2023 2069 6620 7768 6963  sen..  # if whic
-00028880: 6848 6172 6d6f 6e69 6373 203d 3d20 327b  hHarmonics == 2{
-00028890: 0d0a 2020 2320 2020 2070 6120 3d20 6765  ..  #    pa = ge
-000288a0: 7450 6861 7365 416d 706c 6974 7564 6528  tPhaseAmplitude(
-000288b0: 636f 6566 6673 293b 0d0a 2020 2320 202f  coeffs);..  #  /
-000288c0: 2f20 5475 726e 2074 6865 2048 5356 2064  / Turn the HSV d
-000288d0: 6174 6120 696e 746f 2061 6e20 5247 4220  ata into an RGB 
-000288e0: 696d 6167 6520 616e 6420 6164 6420 6974  image and add it
-000288f0: 2074 6f20 7468 6520 6d61 702e 0d0a 2020   to the map...  
-00028900: 2320 2073 6561 736f 6e61 6c69 7479 203d  #  seasonality =
-00028910: 2070 612e 7365 6c65 6374 285b 312c 305d   pa.select([1,0]
-00028920: 292e 6164 6442 616e 6473 2861 6c6c 496e  ).addBands(allIn
-00028930: 6469 6365 732e 7365 6c65 6374 285b 696e  dices.select([in
-00028940: 6465 784e 616d 6573 5b30 5d5d 292e 6d65  dexNames[0]]).me
-00028950: 616e 2829 292e 6873 7654 6f52 6762 2829  an()).hsvToRgb()
-00028960: 3b0d 0a20 2023 2020 2f2f 204d 6170 2e61  ;..  #  // Map.a
-00028970: 6464 4c61 7965 7228 7365 6173 6f6e 616c  ddLayer(seasonal
-00028980: 6974 792c 207b 7d2c 2027 5365 6173 6f6e  ity, {}, 'Season
-00028990: 616c 6974 7927 293b 0d0a 2020 2320 207d  ality');..  #  }
-000289a0: 0d0a 0d0a 0d0a 0d0a 2020 234d 6170 2e61  ........  #Map.a
-000289b0: 6464 4c61 7965 7228 636f 6566 6673 2c7b  ddLayer(coeffs,{
-000289c0: 7d2c 2748 6172 6d6f 6e69 6320 5265 6772  },'Harmonic Regr
-000289d0: 6573 7369 6f6e 2043 6f65 6666 6963 6965  ession Coefficie
-000289e0: 6e74 7327 2c46 616c 7365 290d 0a20 2070  nts',False)..  p
-000289f0: 7265 6469 6374 6564 203d 206e 6577 5072  redicted = newPr
-00028a00: 6564 6963 7428 636f 6566 6673 2c77 6974  edict(coeffs,wit
-00028a10: 6848 6172 6d6f 6e69 6373 290d 0a20 2072  hHarmonics)..  r
-00028a20: 6574 7572 6e20 5b63 6f65 6666 732c 7072  eturn [coeffs,pr
-00028a30: 6564 6963 7465 645d 0d0a 2323 2323 2323  edicted]..######
-00028a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a80: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
-00028a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028ac0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00028ad0: 2353 696d 706c 6520 7072 6564 6963 7420  #Simple predict 
-00028ae0: 6675 6e63 7469 6f6e 2066 6f72 2068 6172  function for har
-00028af0: 6d6f 6e69 6320 636f 6566 6669 6369 656e  monic coefficien
-00028b00: 7473 0d0a 2345 7870 6563 7473 2063 6f65  ts..#Expects coe
-00028b10: 6666 7320 6672 6f6d 2067 6574 4861 726d  ffs from getHarm
-00028b20: 6f6e 6963 436f 6566 6669 6369 656e 7473  onicCoefficients
-00028b30: 416e 6446 6974 2066 756e 6374 696f 6e0d  AndFit function.
-00028b40: 0a23 4461 7465 2069 6d61 6765 2069 7320  .#Date image is 
-00028b50: 6578 7065 6374 6564 2074 6f20 6265 2079  expected to be y
-00028b60: 7979 792e 6464 2077 6865 7265 2064 6420  yyy.dd where dd 
-00028b70: 6973 2074 6865 2064 6179 206f 6620 7965  is the day of ye
-00028b80: 6172 202f 2033 3635 2028 7072 6f70 6f72  ar / 365 (propor
-00028b90: 7469 6f6e 206f 6620 7965 6172 290d 0a23  tion of year)..#
-00028ba0: 6578 2e20 7379 6e74 6849 6d61 6765 2863  ex. synthImage(c
-00028bb0: 6f65 6666 732c 6565 2e49 6d61 6765 285b  oeffs,ee.Image([
-00028bc0: 3230 3139 2e36 5d29 2c5b 2762 6c75 6527  2019.6]),['blue'
-00028bd0: 2c27 6772 6565 6e27 2c27 7265 6427 2c27  ,'green','red','
-00028be0: 6e69 7227 2c27 7377 6972 3127 2c27 7377  nir','swir1','sw
-00028bf0: 6972 3227 2c27 4e42 5227 2c27 4e44 5649  ir2','NBR','NDVI
-00028c00: 275d 2c5b 322c 345d 2c74 7275 6529 0d0a  '],[2,4],true)..
-00028c10: 6465 6620 7379 6e74 6849 6d61 6765 2863  def synthImage(c
-00028c20: 6f65 6666 732c 6461 7465 496d 6167 652c  oeffs,dateImage,
-00028c30: 696e 6465 784e 616d 6573 2c68 6172 6d6f  indexNames,harmo
-00028c40: 6e69 6373 2c64 6574 7265 6e64 293a 0d0a  nics,detrend):..
-00028c50: 2020 2353 6574 2075 7020 636f 6e73 7461    #Set up consta
-00028c60: 6e74 2069 6d61 6765 2074 6f20 6d75 6c74  nt image to mult
-00028c70: 6970 6c79 2063 6f65 6666 7320 6279 0d0a  iply coeffs by..
-00028c80: 2020 636f 6e73 7449 6d61 6765 203d 2065    constImage = e
-00028c90: 652e 496d 6167 6528 3129 0d0a 2020 6966  e.Image(1)..  if
-00028ca0: 2064 6574 7265 6e64 3a63 6f6e 7374 496d   detrend:constIm
-00028cb0: 6167 6520 3d20 636f 6e73 7449 6d61 6765  age = constImage
-00028cc0: 2e61 6464 4261 6e64 7328 6461 7465 496d  .addBands(dateIm
-00028cd0: 6167 6529 0d0a 2020 666f 7220 6861 726d  age)..  for harm
-00028ce0: 2069 6e20 6861 726d 6f6e 6963 733a 0d0a   in harmonics:..
-00028cf0: 2020 2020 636f 6e73 7449 6d61 6765 203d      constImage =
-00028d00: 2063 6f6e 7374 496d 6167 652e 6164 6442   constImage.addB
-00028d10: 616e 6473 2865 652e 496d 6167 6528 5b64  ands(ee.Image([d
-00028d20: 6174 6549 6d61 6765 2e6d 756c 7469 706c  ateImage.multipl
-00028d30: 7928 6861 726d 2a6d 6174 682e 7069 292e  y(harm*math.pi).
-00028d40: 7369 6e28 295d 292e 7265 6e61 6d65 285b  sin()]).rename([
-00028d50: 277b 7d5f 7369 6e27 2e66 6f72 6d61 7428  '{}_sin'.format(
-00028d60: 6861 726d 2a31 3030 295d 2929 2020 2020  harm*100)]))    
-00028d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028d80: 2020 200d 0a20 2066 6f72 2068 6172 6d20     ..  for harm 
-00028d90: 696e 2068 6172 6d6f 6e69 6373 3a0d 0a20  in harmonics:.. 
-00028da0: 2020 2063 6f6e 7374 496d 6167 6520 3d20     constImage = 
-00028db0: 636f 6e73 7449 6d61 6765 2e61 6464 4261  constImage.addBa
-00028dc0: 6e64 7328 6565 2e49 6d61 6765 285b 6461  nds(ee.Image([da
-00028dd0: 7465 496d 6167 652e 6d75 6c74 6970 6c79  teImage.multiply
-00028de0: 2868 6172 6d2a 6d61 7468 2e70 6929 2e63  (harm*math.pi).c
-00028df0: 6f73 2829 5d29 2e72 656e 616d 6528 5b27  os()]).rename(['
-00028e00: 7b7d 5f63 6f73 272e 666f 726d 6174 2868  {}_cos'.format(h
-00028e10: 6172 6d2a 3130 3029 5d29 290d 0a20 200d  arm*100)]))..  .
-00028e20: 0a20 2023 2063 6f65 6666 7373 426e 203d  .  # coeffssBn =
-00028e30: 2063 6f65 6666 732e 7365 6c65 6374 2865   coeffs.select(e
-00028e40: 652e 5374 7269 6e67 2869 6e64 6578 4e61  e.String(indexNa
-00028e50: 6d65 735b 305d 292e 6361 7428 275f 2e2a  mes[0]).cat('_.*
-00028e60: 2729 290d 0a20 2023 2070 7269 6e74 2863  '))..  # print(c
-00028e70: 6f6e 7374 496d 6167 652e 6261 6e64 4e61  onstImage.bandNa
-00028e80: 6d65 7328 292e 6765 7449 6e66 6f28 292c  mes().getInfo(),
-00028e90: 636f 6566 6673 7342 6e2e 6261 6e64 4e61  coeffssBn.bandNa
-00028ea0: 6d65 7328 292e 6765 7449 6e66 6f28 2929  mes().getInfo())
-00028eb0: 0d0a 2020 2350 7265 6469 6374 2076 616c  ..  #Predict val
-00028ec0: 7565 7320 666f 7220 6561 6368 2062 616e  ues for each ban
-00028ed0: 640d 0a20 206f 7574 203d 2065 652e 496d  d..  out = ee.Im
-00028ee0: 6167 6528 3129 3b0d 0a20 2064 6566 2070  age(1);..  def p
-00028ef0: 7265 6469 6374 5772 6170 7065 7228 626e  redictWrapper(bn
-00028f00: 2c6f 7574 293a 0d0a 2020 2020 626e 203d  ,out):..    bn =
-00028f10: 2065 652e 5374 7269 6e67 2862 6e29 0d0a   ee.String(bn)..
-00028f20: 2020 2020 2353 656c 6563 7420 636f 6566      #Select coef
-00028f30: 6673 2066 6f72 2074 6861 7420 6261 6e64  fs for that band
-00028f40: 0d0a 2020 2020 636f 6566 6673 7342 6e20  ..    coeffssBn 
-00028f50: 3d20 636f 6566 6673 2e73 656c 6563 7428  = coeffs.select(
-00028f60: 6565 2e53 7472 696e 6728 626e 292e 6361  ee.String(bn).ca
-00028f70: 7428 275f 2e2a 2729 290d 0a20 2020 2070  t('_.*'))..    p
-00028f80: 7265 6469 6374 6564 203d 2063 6f6e 7374  redicted = const
-00028f90: 496d 6167 652e 6d75 6c74 6970 6c79 2863  Image.multiply(c
-00028fa0: 6f65 6666 7373 426e 292e 7265 6475 6365  oeffssBn).reduce
-00028fb0: 2827 7375 6d27 292e 7265 6e61 6d65 2862  ('sum').rename(b
-00028fc0: 6e29 0d0a 2020 2020 7265 7475 726e 2065  n)..    return e
-00028fd0: 652e 496d 6167 6528 6f75 7429 2e61 6464  e.Image(out).add
-00028fe0: 4261 6e64 7328 7072 6564 6963 7465 6429  Bands(predicted)
-00028ff0: 0d0a 0d0a 2020 6f75 7420 3d20 6565 2e49  ....  out = ee.I
-00029000: 6d61 6765 2865 652e 4c69 7374 2869 6e64  mage(ee.List(ind
-00029010: 6578 4e61 6d65 7329 2e69 7465 7261 7465  exNames).iterate
-00029020: 2870 7265 6469 6374 5772 6170 7065 722c  (predictWrapper,
-00029030: 6f75 7429 293b 0d0a 0d0a 2020 6f75 7420  out));....  out 
-00029040: 3d20 6f75 742e 7365 6c65 6374 2865 652e  = out.select(ee.
-00029050: 4c69 7374 2e73 6571 7565 6e63 6528 312c  List.sequence(1,
-00029060: 206f 7574 2e62 616e 644e 616d 6573 2829   out.bandNames()
-00029070: 2e73 697a 6528 292e 7375 6274 7261 6374  .size().subtract
-00029080: 2831 2929 290d 0a0d 0a20 2072 6574 7572  (1)))....  retur
-00029090: 6e20 6f75 740d 0a23 2323 2323 2323 2323  n out..#########
-000290a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000290b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000290c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000290d0: 2323 2323 2323 2323 2323 2323 0d0a 2357  ############..#W
-000290e0: 7261 7070 6572 2066 756e 6374 696f 6e20  rapper function 
-000290f0: 746f 2067 6574 2063 6c69 6d61 7465 2064  to get climate d
-00029100: 6174 610d 0a23 2053 7570 706f 7274 733a  ata..# Supports:
-00029110: 0d0a 2320 4e41 5341 2f4f 524e 4c2f 4441  ..# NASA/ORNL/DA
-00029120: 594d 4554 5f56 330d 0a23 204e 4153 412f  YMET_V3..# NASA/
-00029130: 4f52 4e4c 2f44 4159 4d45 545f 5634 0d0a  ORNL/DAYMET_V4..
-00029140: 2320 5543 5342 2d43 4847 2f43 4849 5250  # UCSB-CHG/CHIRP
-00029150: 532f 4441 494c 5920 2870 7265 6369 7069  S/DAILY (precipi
-00029160: 7461 7469 6f6e 206f 6e6c 7929 0d0a 2361  tation only)..#a
-00029170: 6e64 2070 6f73 7369 626c 7920 6f74 6865  nd possibly othe
-00029180: 7273 0d0a 6465 6620 6765 7443 6c69 6d61  rs..def getClima
-00029190: 7465 5772 6170 7065 7228 636f 6c6c 6563  teWrapper(collec
-000291a0: 7469 6f6e 4e61 6d65 2c73 7475 6479 4172  tionName,studyAr
-000291b0: 6561 2c73 7461 7274 5965 6172 2c65 6e64  ea,startYear,end
-000291c0: 5965 6172 2c73 7461 7274 4a75 6c69 616e  Year,startJulian
-000291d0: 2c65 6e64 4a75 6c69 616e 2c74 696d 6562  ,endJulian,timeb
-000291e0: 7566 6665 722c 7765 6967 6874 732c 636f  uffer,weights,co
-000291f0: 6d70 6f73 6974 696e 6752 6564 7563 6572  mpositingReducer
-00029200: 2c65 7870 6f72 7443 6f6d 706f 7369 7465  ,exportComposite
-00029210: 7320 3d20 4661 6c73 652c 6578 706f 7274  s = False,export
-00029220: 5061 7468 526f 6f74 203d 204e 6f6e 652c  PathRoot = None,
-00029230: 6372 7320 3d20 4e6f 6e65 2c74 7261 6e73  crs = None,trans
-00029240: 666f 726d 203d 204e 6f6e 652c 7363 616c  form = None,scal
-00029250: 6520 3d20 4e6f 6e65 2c65 7870 6f72 7442  e = None,exportB
-00029260: 616e 6473 203d 204e 6f6e 6529 3a0d 0a20  ands = None):.. 
-00029270: 2061 7267 7320 3d20 666f 726d 6174 4172   args = formatAr
-00029280: 6773 286c 6f63 616c 7328 2929 0d0a 2020  gs(locals())..  
-00029290: 6966 2027 6172 6773 2720 696e 2061 7267  if 'args' in arg
-000292a0: 732e 6b65 7973 2829 3a0d 0a20 2020 2064  s.keys():..    d
-000292b0: 656c 2061 7267 735b 2761 7267 7327 5d0d  el args['args'].
-000292c0: 0a20 2070 7269 6e74 2861 7267 7329 0d0a  .  print(args)..
-000292d0: 0d0a 2020 2350 7265 7061 7265 2064 6174  ..  #Prepare dat
-000292e0: 6573 0d0a 2020 2357 7261 7020 7468 6520  es..  #Wrap the 
-000292f0: 6461 7465 7320 6966 206e 6565 6465 640d  dates if needed.
-00029300: 0a20 2077 7261 704f 6666 7365 7420 3d20  .  wrapOffset = 
-00029310: 300d 0a20 2069 6620 7374 6172 744a 756c  0..  if startJul
-00029320: 6961 6e20 3e20 656e 644a 756c 6961 6e3a  ian > endJulian:
-00029330: 0d0a 2020 2020 7772 6170 4f66 6673 6574  ..    wrapOffset
-00029340: 203d 2033 3635 0d0a 0d0a 2020 7374 6172   = 365....  star
-00029350: 7444 6174 6520 3d20 6565 2e44 6174 652e  tDate = ee.Date.
-00029360: 6672 6f6d 594d 4428 7374 6172 7459 6561  fromYMD(startYea
-00029370: 722c 312c 3129 2e61 6476 616e 6365 2873  r,1,1).advance(s
-00029380: 7461 7274 4a75 6c69 616e 2d31 2c27 6461  tartJulian-1,'da
-00029390: 7927 290d 0a20 2065 6e64 4461 7465 203d  y')..  endDate =
-000293a0: 2065 652e 4461 7465 2e66 726f 6d59 4d44   ee.Date.fromYMD
-000293b0: 2865 6e64 5965 6172 2c31 2c31 292e 6164  (endYear,1,1).ad
-000293c0: 7661 6e63 6528 656e 644a 756c 6961 6e2d  vance(endJulian-
-000293d0: 312b 7772 6170 4f66 6673 6574 2c27 6461  1+wrapOffset,'da
-000293e0: 7927 290d 0a20 2070 7269 6e74 2827 5374  y')..  print('St
-000293f0: 6172 7420 616e 6420 656e 6420 6461 7465  art and end date
-00029400: 733a 272c 2073 7461 7274 4461 7465 2e66  s:', startDate.f
-00029410: 6f72 6d61 7428 2759 5959 592d 4d4d 2d64  ormat('YYYY-MM-d
-00029420: 6427 292e 6765 7449 6e66 6f28 292c 2065  d').getInfo(), e
-00029430: 6e64 4461 7465 2e66 6f72 6d61 7428 2759  ndDate.format('Y
-00029440: 5959 592d 4d4d 2d64 6427 292e 6765 7449  YYY-MM-dd').getI
-00029450: 6e66 6f28 2929 0d0a 2020 7072 696e 7428  nfo())..  print(
-00029460: 274a 756c 6961 6e20 6461 7973 2061 7265  'Julian days are
-00029470: 3a27 2c73 7461 7274 4a75 6c69 616e 2c65  :',startJulian,e
-00029480: 6e64 4a75 6c69 616e 290d 0a0d 0a20 2023  ndJulian)....  #
-00029490: 4765 7420 636c 696d 6174 6520 6461 7461  Get climate data
-000294a0: 0d0a 2020 6320 3d20 6565 2e49 6d61 6765  ..  c = ee.Image
-000294b0: 436f 6c6c 6563 7469 6f6e 2863 6f6c 6c65  Collection(colle
-000294c0: 6374 696f 6e4e 616d 6529 5c0d 0a20 2020  ctionName)\..   
-000294d0: 2020 2020 2020 2020 2e66 696c 7465 7242          .filterB
-000294e0: 6f75 6e64 7328 7374 7564 7941 7265 6129  ounds(studyArea)
-000294f0: 5c0d 0a20 2020 2020 2020 2020 2020 2e66  \..           .f
-00029500: 696c 7465 7244 6174 6528 7374 6172 7444  ilterDate(startD
-00029510: 6174 652c 656e 6444 6174 652e 6164 7661  ate,endDate.adva
-00029520: 6e63 6528 312c 2764 6179 2729 295c 0d0a  nce(1,'day'))\..
-00029530: 2020 2020 2020 2020 2020 202e 6669 6c74             .filt
-00029540: 6572 2865 652e 4669 6c74 6572 2e63 616c  er(ee.Filter.cal
-00029550: 656e 6461 7252 616e 6765 2873 7461 7274  endarRange(start
-00029560: 4a75 6c69 616e 2c65 6e64 4a75 6c69 616e  Julian,endJulian
-00029570: 2929 0d0a 0d0a 2020 2353 6574 2074 6f20  ))....  #Set to 
-00029580: 6170 7072 6f70 7269 6174 6520 7265 7361  appropriate resa
-00029590: 6d70 6c69 6e67 206d 6574 686f 640d 0a20  mpling method.. 
-000295a0: 2063 203d 2063 2e6d 6170 286c 616d 6264   c = c.map(lambd
-000295b0: 6120 696d 673a 2069 6d67 2e72 6573 616d  a img: img.resam
-000295c0: 706c 6528 2762 6963 7562 6963 2729 290d  ple('bicubic')).
-000295d0: 0a20 204d 6170 2e61 6464 4c61 7965 7228  .  Map.addLayer(
-000295e0: 632c 7b7d 2c27 5261 7720 436c 696d 6174  c,{},'Raw Climat
-000295f0: 6527 2c46 616c 7365 290d 0a0d 0a20 2023  e',False)....  #
-00029600: 4372 6561 7465 2063 6f6d 706f 7369 7465  Create composite
-00029610: 2074 696d 6520 7365 7269 6573 0d0a 2020   time series..  
-00029620: 7473 203d 2063 6f6d 706f 7369 7465 5469  ts = compositeTi
-00029630: 6d65 5365 7269 6573 2863 2c73 7461 7274  meSeries(c,start
-00029640: 5965 6172 2c65 6e64 5965 6172 2c73 7461  Year,endYear,sta
-00029650: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
-00029660: 616e 2c74 696d 6562 7566 6665 722c 7765  an,timebuffer,we
-00029670: 6967 6874 732c 4e6f 6e65 2c63 6f6d 706f  ights,None,compo
-00029680: 7369 7469 6e67 5265 6475 6365 7229 0d0a  sitingReducer)..
-00029690: 2020 7473 203d 2065 652e 496d 6167 6543    ts = ee.ImageC
-000296a0: 6f6c 6c65 6374 696f 6e28 7473 2e6d 6170  ollection(ts.map
-000296b0: 286c 616d 6264 6120 6920 3a20 692e 666c  (lambda i : i.fl
-000296c0: 6f61 7428 2929 290d 0a0d 0a20 2023 4578  oat()))....  #Ex
-000296d0: 706f 7274 2063 6f6d 706f 7369 7465 2063  port composite c
-000296e0: 6f6c 6c65 6374 696f 6e0d 0a20 2069 6620  ollection..  if 
-000296f0: 6578 706f 7274 436f 6d70 6f73 6974 6573  exportComposites
-00029700: 3a0d 0a20 2020 2023 5365 7420 7570 2065  :..    #Set up e
-00029710: 7870 6f72 7420 6261 6e64 7320 6966 206e  xport bands if n
-00029720: 6f74 2073 7065 6369 6669 6564 0d0a 2020  ot specified..  
-00029730: 2020 6966 2065 7870 6f72 7442 616e 6473    if exportBands
-00029740: 203d 3d20 4e6f 6e65 3a0d 0a20 2020 2020   == None:..     
-00029750: 2065 7870 6f72 7442 616e 6473 203d 2065   exportBands = e
-00029760: 652e 4c69 7374 2865 652e 496d 6167 6528  e.List(ee.Image(
-00029770: 7473 2e66 6972 7374 2829 292e 6261 6e64  ts.first()).band
-00029780: 4e61 6d65 7328 2929 0d0a 0d0a 2020 2020  Names())....    
-00029790: 6578 706f 7274 436f 6c6c 6563 7469 6f6e  exportCollection
-000297a0: 2865 7870 6f72 7450 6174 6852 6f6f 742c  (exportPathRoot,
-000297b0: 636f 6c6c 6563 7469 6f6e 4e61 6d65 2e73  collectionName.s
-000297c0: 706c 6974 2827 2f27 295b 2d31 5d2c 7374  plit('/')[-1],st
-000297d0: 7564 7941 7265 612c 2063 7273 2c74 7261  udyArea, crs,tra
-000297e0: 6e73 666f 726d 2c73 6361 6c65 2c74 732c  nsform,scale,ts,
-000297f0: 7374 6172 7459 6561 722c 656e 6459 6561  startYear,endYea
-00029800: 722c 7374 6172 744a 756c 6961 6e2c 656e  r,startJulian,en
-00029810: 644a 756c 6961 6e2c 636f 6d70 6f73 6974  dJulian,composit
-00029820: 696e 6752 6564 7563 6572 2c74 696d 6562  ingReducer,timeb
-00029830: 7566 6665 722c 6578 706f 7274 4261 6e64  uffer,exportBand
-00029840: 7329 0d0a 0d0a 2020 7265 7475 726e 2074  s)....  return t
-00029850: 7323 2323 230d 0a23 2323 2323 2323 2323  s####..#########
-00029860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029890: 2323 2323 2323 2323 2323 2323 0d0a 2341  ############..#A
-000298a0: 6464 7320 6162 736f 6c75 7465 2064 6966  dds absolute dif
-000298b0: 6665 7265 6e63 6520 6672 6f6d 2061 2073  ference from a s
-000298c0: 7065 6369 6669 6564 2062 616e 6420 7375  pecified band su
-000298d0: 6d6d 6172 697a 6564 2062 7920 6120 7072  mmarized by a pr
-000298e0: 6f76 6964 6564 2070 6572 6365 6e74 696c  ovided percentil
-000298f0: 650d 0a23 496e 7465 6e64 6564 2066 6f72  e..#Intended for
-00029900: 2063 7573 746f 6d20 736f 7274 696e 6720   custom sorting 
-00029910: 6163 726f 7373 2063 6f6c 6c65 6374 696f  across collectio
-00029920: 6e73 0d0a 6465 6620 6164 6441 6273 4469  ns..def addAbsDi
-00029930: 6666 2869 6e43 6f6c 6c65 6374 696f 6e2c  ff(inCollection,
-00029940: 2071 7561 6c69 7479 4261 6e64 2c20 7065   qualityBand, pe
-00029950: 7263 656e 7469 6c65 2c73 6967 6e29 3a0d  rcentile,sign):.
-00029960: 0a20 2062 6573 7451 7561 6c69 7479 203d  .  bestQuality =
-00029970: 2069 6e43 6f6c 6c65 6374 696f 6e2e 7365   inCollection.se
-00029980: 6c65 6374 285b 7175 616c 6974 7942 616e  lect([qualityBan
-00029990: 645d 292e 7265 6475 6365 2865 652e 5265  d]).reduce(ee.Re
-000299a0: 6475 6365 722e 7065 7263 656e 7469 6c65  ducer.percentile
-000299b0: 285b 7065 7263 656e 7469 6c65 5d29 290d  ([percentile])).
-000299c0: 0a20 2064 6566 2077 2869 6d61 6765 293a  .  def w(image):
-000299d0: 0d0a 2020 2020 6465 6c74 6120 3d20 696d  ..    delta = im
-000299e0: 6167 652e 7365 6c65 6374 285b 7175 616c  age.select([qual
-000299f0: 6974 7942 616e 645d 292e 7375 6274 7261  ityBand]).subtra
-00029a00: 6374 2862 6573 7451 7561 6c69 7479 292e  ct(bestQuality).
-00029a10: 6162 7328 292e 6d75 6c74 6970 6c79 2873  abs().multiply(s
-00029a20: 6967 6e29 0d0a 2020 2020 7265 7475 726e  ign)..    return
-00029a30: 2069 6d61 6765 2e61 6464 4261 6e64 7328   image.addBands(
-00029a40: 6465 6c74 612e 7365 6c65 6374 285b 305d  delta.select([0]
-00029a50: 2c20 5b27 6465 6c74 6127 5d29 290d 0a20  , ['delta'])).. 
-00029a60: 206f 7574 203d 2069 6e43 6f6c 6c65 6374   out = inCollect
-00029a70: 696f 6e2e 6d61 7028 7729 0d0a 2020 7265  ion.map(w)..  re
-00029a80: 7475 726e 206f 7574 0d0a 0d0a 2323 2323  turn out....####
-00029a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029ad0: 230d 0a23 4d65 7468 6f64 2066 6f72 2061  #..#Method for a
-00029ae0: 7070 6c79 696e 6720 7468 6520 7175 616c  pplying the qual
-00029af0: 6974 794d 6f73 6169 6320 6675 6e63 7469  ityMosaic functi
-00029b00: 6f6e 2075 7369 6e67 2061 2073 7065 6369  on using a speci
-00029b10: 6669 6564 2070 6572 6365 6e74 696c 650d  fied percentile.
-00029b20: 0a23 5573 6566 756c 2077 6865 6e20 7468  .#Useful when th
-00029b30: 6520 6d61 7820 6f66 2074 6865 2071 7561  e max of the qua
-00029b40: 6c69 7479 2062 616e 6420 6973 206e 6f74  lity band is not
-00029b50: 2077 6861 7420 6973 2077 616e 7465 640d   what is wanted.
-00029b60: 0a64 6566 2063 7573 746f 6d51 7561 6c69  .def customQuali
-00029b70: 7479 4d6f 7361 6963 2869 6e43 6f6c 6c65  tyMosaic(inColle
-00029b80: 6374 696f 6e2c 7175 616c 6974 7942 616e  ction,qualityBan
-00029b90: 642c 7065 7263 656e 7469 6c65 293a 0d0a  d,percentile):..
-00029ba0: 2020 2341 6464 2061 6e20 6162 736f 6c75    #Add an absolu
-00029bb0: 7465 2064 6966 6665 7265 6e63 6520 6672  te difference fr
-00029bc0: 6f6d 2074 6865 2073 7065 6369 6669 6564  om the specified
-00029bd0: 2070 6572 6365 6e74 696c 650d 0a20 2023   percentile..  #
-00029be0: 5468 6973 2069 7320 696e 7665 7274 6564  This is inverted
-00029bf0: 2066 6f72 2074 6865 2071 7561 6c69 7479   for the quality
-00029c00: 4d6f 7361 6963 2066 756e 6374 696f 6e20  Mosaic function 
-00029c10: 746f 2070 726f 7065 726c 7920 7072 696f  to properly prio
-00029c20: 7269 7469 7a65 0d0a 2020 696e 436f 6c6c  ritize..  inColl
-00029c30: 6563 7469 6f6e 4465 6c74 6120 3d20 6164  ectionDelta = ad
-00029c40: 6441 6273 4469 6666 2869 6e43 6f6c 6c65  dAbsDiff(inColle
-00029c50: 6374 696f 6e2c 2071 7561 6c69 7479 4261  ction, qualityBa
-00029c60: 6e64 2c20 7065 7263 656e 7469 6c65 2c2d  nd, percentile,-
-00029c70: 3129 0d0a 0d0a 2020 2341 7070 6c79 2074  1)....  #Apply t
-00029c80: 6865 2071 7561 6c69 7479 4d6f 7361 6963  he qualityMosaic
-00029c90: 2066 756e 6374 696f 6e0d 0a20 2072 6574   function..  ret
-00029ca0: 7572 6e20 696e 436f 6c6c 6563 7469 6f6e  urn inCollection
-00029cb0: 4465 6c74 612e 7175 616c 6974 794d 6f73  Delta.qualityMos
-00029cc0: 6169 6328 2764 656c 7461 2729 0d0a 0d0a  aic('delta')....
-00029cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029d10: 2323 2323 230d 0a23 4f6e 2d74 6865 2d66  #####..#On-the-f
-00029d20: 6c79 2062 6173 6963 2077 6174 6572 206d  ly basic water m
-00029d30: 6173 6b69 6e67 206d 6574 686f 640d 0a23  asking method..#
-00029d40: 5468 6973 206d 6574 686f 6420 6973 2075  This method is u
-00029d50: 7365 6420 746f 2070 726f 7669 6465 2061  sed to provide a
-00029d60: 2074 696d 652d 7365 6e73 6974 6976 6520   time-sensitive 
-00029d70: 7761 7465 7220 6d61 736b 0d0a 2354 6869  water mask..#Thi
-00029d80: 7320 6d65 7468 6f64 2074 656e 6473 2074  s method tends t
-00029d90: 6f20 776f 726b 2077 656c 6c20 6966 2074  o work well if t
-00029da0: 6865 7265 2069 7320 6e6f 2077 6574 2073  here is no wet s
-00029db0: 6e6f 7720 7072 6573 656e 740d 0a23 5765  now present..#We
-00029dc0: 7420 736e 6f77 206f 7665 7220 666c 6174  t snow over flat
-00029dd0: 2061 7265 6173 2063 616e 2072 6573 756c   areas can resul
-00029de0: 7420 696e 2066 616c 7365 2070 6f73 6974  t in false posit
-00029df0: 6976 6573 0d0a 2344 6573 6967 6e65 6420  ives..#Designed 
-00029e00: 746f 2077 6f72 6b20 7769 7468 2054 4f41  to work with TOA
-00029e10: 2064 6174 612e 2053 5220 6461 7461 2077   data. SR data w
-00029e20: 696c 6c20 7265 7375 6c74 2069 6e20 6661  ill result in fa
-00029e30: 6c73 6520 6e65 6761 7469 7665 7320 286f  lse negatives (o
-00029e40: 6d69 7373 696f 6e29 0d0a 6465 6620 7369  mission)..def si
-00029e50: 6d70 6c65 5761 7465 724d 6173 6b28 696d  mpleWaterMask(im
-00029e60: 672c 636f 6e74 7261 6374 5069 7865 6c73  g,contractPixels
-00029e70: 203d 2030 2c73 6c6f 7065 5f74 6872 6573   = 0,slope_thres
-00029e80: 6820 3d20 3130 2c65 6c65 7661 7469 6f6e  h = 10,elevation
-00029e90: 496d 6167 6550 6174 6820 3d20 2255 5347  ImagePath = "USG
-00029ea0: 532f 3344 4550 2f31 306d 222c 656c 6576  S/3DEP/10m",elev
-00029eb0: 6174 696f 6e46 6f63 616c 4d65 616e 5261  ationFocalMeanRa
-00029ec0: 6469 7573 203d 2035 2e35 293a 0d0a 2020  dius = 5.5):..  
-00029ed0: 696d 6720 3d20 6164 6454 4341 6e67 6c65  img = addTCAngle
-00029ee0: 7328 696d 6729 0d0a 2020 6e65 6420 3d20  s(img)..  ned = 
-00029ef0: 6565 2e49 6d61 6765 2865 6c65 7661 7469  ee.Image(elevati
-00029f00: 6f6e 496d 6167 6550 6174 6829 2e72 6573  onImagePath).res
-00029f10: 616d 706c 6528 2762 6963 7562 6963 2729  ample('bicubic')
-00029f20: 0d0a 2020 736c 6f70 6520 3d20 6565 2e54  ..  slope = ee.T
-00029f30: 6572 7261 696e 2e73 6c6f 7065 286e 6564  errain.slope(ned
-00029f40: 2e66 6f63 616c 5f6d 6561 6e28 656c 6576  .focal_mean(elev
-00029f50: 6174 696f 6e46 6f63 616c 4d65 616e 5261  ationFocalMeanRa
-00029f60: 6469 7573 2929 0d0a 2020 666c 6174 203d  dius))..  flat =
-00029f70: 2073 6c6f 7065 2e6c 7465 2873 6c6f 7065   slope.lte(slope
-00029f80: 5f74 6872 6573 6829 0d0a 0d0a 2020 7761  _thresh)....  wa
-00029f90: 7465 724d 6173 6b20 3d20 696d 672e 7365  terMask = img.se
-00029fa0: 6c65 6374 285b 2774 6341 6e67 6c65 4257  lect(['tcAngleBW
-00029fb0: 275d 292e 6774 6528 2d30 2e30 3529 5c0d  ']).gte(-0.05)\.
-00029fc0: 0a20 2020 202e 416e 6428 696d 672e 7365  .    .And(img.se
-00029fd0: 6c65 6374 285b 2774 6341 6e67 6c65 4247  lect(['tcAngleBG
-00029fe0: 275d 292e 6c74 6528 302e 3035 2929 5c0d  ']).lte(0.05))\.
-00029ff0: 0a20 2020 202e 416e 6428 696d 672e 7365  .    .And(img.se
-0002a000: 6c65 6374 285b 2762 7269 6768 746e 6573  lect(['brightnes
-0002a010: 7327 5d29 2e6c 7428 302e 3329 295c 0d0a  s']).lt(0.3))\..
-0002a020: 2020 2020 2e41 6e64 2866 6c61 7429 2e66      .And(flat).f
-0002a030: 6f63 616c 5f6d 696e 2863 6f6e 7472 6163  ocal_min(contrac
-0002a040: 7450 6978 656c 7329 0d0a 0d0a 2020 7265  tPixels)....  re
-0002a050: 7475 726e 2077 6174 6572 4d61 736b 2e72  turn waterMask.r
-0002a060: 656e 616d 6528 5b27 7761 7465 724d 6173  ename(['waterMas
-0002a070: 6b27 5d29 0d0a 2323 2323 2323 2323 2323  k'])..##########
-0002a080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0002a090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0002a0a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0002a0b0: 2323 2323 2323 2323 2323 230d 0a23 4a65  ###########..#Je
-0002a0c0: 6666 2048 6f20 4d65 7468 6f64 2066 6f72  ff Ho Method for
-0002a0d0: 2061 6c67 616c 2062 6c6f 6f6d 2064 6574   algal bloom det
-0002a0e0: 6563 7469 6f6e 0d0a 2368 7474 7073 3a2f  ection..#https:/
-0002a0f0: 2f77 7777 2e6e 6174 7572 652e 636f 6d2f  /www.nature.com/
-0002a100: 6172 7469 636c 6573 2f73 3431 3538 362d  articles/s41586-
-0002a110: 3031 392d 3136 3438 2d37 0d0a 0d0a 2320  019-1648-7....# 
-0002a120: 5369 6d70 6c69 6669 6564 2053 6372 6970  Simplified Scrip
-0002a130: 7420 666f 7220 4c61 6e64 7361 7420 5761  t for Landsat Wa
-0002a140: 7465 7220 5175 616c 6974 790d 0a23 2050  ter Quality..# P
-0002a150: 726f 6475 6365 7320 6120 6d61 7020 6f66  roduces a map of
-0002a160: 2061 6e20 616c 6761 6c20 626c 6f6f 6d20   an algal bloom 
-0002a170: 696e 204c 616b 6520 4572 6965 206f 6e20  in Lake Erie on 
-0002a180: 3230 3131 2f39 2f33 0d0a 2320 4372 6561  2011/9/3..# Crea
-0002a190: 7465 6420 6f6e 2031 322f 372f 3230 3135  ted on 12/7/2015
-0002a1a0: 2062 7920 4a65 6666 2048 6f0d 0a0d 0a23   by Jeff Ho....#
-0002a1b0: 2053 7065 6369 6669 6573 2061 2074 6872   Specifies a thr
-0002a1c0: 6573 686f 6c64 2066 6f72 2068 7565 2074  eshold for hue t
-0002a1d0: 6f20 6573 7469 6d61 7465 2022 6772 6565  o estimate "gree
-0002a1e0: 6e22 2070 6978 656c 730d 0a23 2074 6869  n" pixels..# thi
-0002a1f0: 7320 6973 2075 7365 6420 6173 2061 6e20  s is used as an 
-0002a200: 6164 6469 7469 6f6e 616c 2066 696c 7465  additional filte
-0002a210: 7220 746f 2072 6566 696e 6520 7468 6520  r to refine the 
-0002a220: 616c 676f 7269 7468 6d20 6162 6f76 650d  algorithm above.
-0002a230: 0a64 6566 2048 6f43 616c 6347 7265 656e  .def HoCalcGreen
-0002a240: 6e65 7373 2869 6d67 293a 0d0a 2020 236d  ness(img):..  #m
-0002a250: 6170 2072 2c20 672c 2061 6e64 2062 2066  ap r, g, and b f
-0002a260: 6f72 206d 6f72 6520 7265 6164 6162 6c65  or more readable
-0002a270: 2061 6c67 6562 7261 2062 656c 6f77 0d0a   algebra below..
-0002a280: 2020 7220 3d20 696d 672e 7365 6c65 6374    r = img.select
-0002a290: 285b 2772 6564 275d 290d 0a20 2067 203d  (['red'])..  g =
-0002a2a0: 2069 6d67 2e73 656c 6563 7428 5b27 6772   img.select(['gr
-0002a2b0: 6565 6e27 5d29 0d0a 2020 6220 3d20 696d  een'])..  b = im
-0002a2c0: 672e 7365 6c65 6374 285b 2762 6c75 6527  g.select(['blue'
-0002a2d0: 5d29 0d0a 0d0a 2020 2363 616c 6375 6c61  ])....  #calcula
-0002a2e0: 7465 2069 6e74 656e 7369 7479 2c20 6875  te intensity, hu
-0002a2f0: 650d 0a20 2049 203d 2072 2e61 6464 2867  e..  I = r.add(g
-0002a300: 292e 6164 6428 6229 2e72 656e 616d 6528  ).add(b).rename(
-0002a310: 5b27 4927 5d29 0d0a 2020 6d69 6e73 203d  ['I'])..  mins =
-0002a320: 2072 2e6d 696e 2867 292e 6d69 6e28 6229   r.min(g).min(b)
-0002a330: 2e72 656e 616d 6528 5b27 6d69 6e73 275d  .rename(['mins']
-0002a340: 290d 0a20 2048 203d 206d 696e 732e 7768  )..  H = mins.wh
-0002a350: 6572 6528 6d69 6e73 2e65 7128 7229 2c28  ere(mins.eq(r),(
-0002a360: 622e 7375 6274 7261 6374 2872 2929 2e64  b.subtract(r)).d
-0002a370: 6976 6964 6528 492e 7375 6274 7261 6374  ivide(I.subtract
-0002a380: 2872 2e6d 756c 7469 706c 7928 3329 2929  (r.multiply(3)))
-0002a390: 2e61 6464 2831 2920 290d 0a20 2048 203d  .add(1) )..  H =
-0002a3a0: 2048 2e77 6865 7265 286d 696e 732e 6571   H.where(mins.eq
-0002a3b0: 2867 292c 2872 2e73 7562 7472 6163 7428  (g),(r.subtract(
-0002a3c0: 6729 292e 6469 7669 6465 2849 2e73 7562  g)).divide(I.sub
-0002a3d0: 7472 6163 7428 672e 6d75 6c74 6970 6c79  tract(g.multiply
-0002a3e0: 2833 2929 292e 6164 6428 3229 2029 0d0a  (3))).add(2) )..
-0002a3f0: 2020 4820 3d20 482e 7768 6572 6528 6d69    H = H.where(mi
-0002a400: 6e73 2e65 7128 6229 2c28 672e 7375 6274  ns.eq(b),(g.subt
-0002a410: 7261 6374 2862 2929 2e64 6976 6964 6528  ract(b)).divide(
-0002a420: 492e 7375 6274 7261 6374 2862 2e6d 756c  I.subtract(b.mul
-0002a430: 7469 706c 7928 3329 2929 2029 0d0a 0d0a  tiply(3))) )....
-0002a440: 2020 2370 6978 656c 7320 7769 7468 2068    #pixels with h
-0002a450: 7565 2062 656c 6f77 2031 2e36 206d 6f72  ue below 1.6 mor
-0002a460: 6520 6c69 6b65 6c79 2074 6f20 6265 2062  e likely to be b
-0002a470: 6c6f 6f6d 2061 6e64 206e 6f74 2073 7573  loom and not sus
-0002a480: 7065 6e64 6564 2073 6564 696d 656e 740d  pended sediment.
-0002a490: 0a20 2048 7468 7265 7368 203d 2048 2e6c  .  Hthresh = H.l
-0002a4a0: 7465 2831 2e36 290d 0a0d 0a20 2072 6574  te(1.6)....  ret
-0002a4b0: 7572 6e20 482e 7265 6e61 6d65 2827 4827  urn H.rename('H'
-0002a4c0: 290d 0a0d 0a0d 0a23 4170 706c 7920 626c  )......#Apply bl
-0002a4d0: 6f6f 6d20 6465 7465 6374 696f 6e20 616c  oom detection al
-0002a4e0: 676f 7269 7468 6d0d 0a64 6566 2048 6f43  gorithm..def HoC
-0002a4f0: 616c 6341 6c67 6f72 6974 686d 3128 696d  alcAlgorithm1(im
-0002a500: 6167 6529 3a0d 0a20 2074 7275 6563 6f6c  age):..  truecol
-0002a510: 6f72 203d 2031 2023 7368 6f77 2074 7275  or = 1 #show tru
-0002a520: 6520 636f 6c6f 7220 696d 6167 6520 6173  e color image as
-0002a530: 2077 656c 6c0d 0a20 2074 6573 7454 6872   well..  testThr
-0002a540: 6573 6820 3d20 4661 6c73 6520 2320 6164  esh = False # ad
-0002a550: 6420 6120 6269 6e61 7279 2069 6d61 6765  d a binary image
-0002a560: 2063 6c61 7373 6966 7969 6e67 2069 6e74   classifying int
-0002a570: 6f20 2262 6c6f 6f6d 2261 6e64 2022 6e6f  o "bloom"and "no
-0002a580: 6e2d 626c 6f6f 6d0d 0a20 2062 6c6f 6f6d  n-bloom..  bloom
-0002a590: 5468 7265 7368 6f6c 6420 3d20 302e 3032  Threshold = 0.02
-0002a5a0: 3334 3620 2374 6872 6573 686f 6c64 2066  346 #threshold f
-0002a5b0: 6f72 2063 6c61 7373 6966 6963 6174 696f  or classificatio
-0002a5c0: 6e20 6669 7420 6261 7365 6420 6f6e 206f  n fit based on o
-0002a5d0: 7468 6572 2064 6174 610d 0a20 2067 7265  ther data..  gre
-0002a5e0: 656e 6573 7354 6872 6573 686f 6c64 203d  enessThreshold =
-0002a5f0: 2031 2e36 0d0a 0d0a 2020 2320 416c 676f   1.6....  # Algo
-0002a600: 7269 7468 6d20 3120 6261 7365 6420 6f6e  rithm 1 based on
-0002a610: 3a0d 0a20 2023 2057 616e 672c 204d 2e2c  :..  # Wang, M.,
-0002a620: 2026 2053 6869 2c20 572e 2028 3230 3037   & Shi, W. (2007
-0002a630: 292e 2054 6865 204e 4952 2d53 5749 5220  ). The NIR-SWIR 
-0002a640: 636f 6d62 696e 6564 2061 746d 6f73 7068  combined atmosph
-0002a650: 6572 6963 0d0a 2020 2320 2063 6f72 7265  eric..  #  corre
-0002a660: 6374 696f 6e20 6170 7072 6f61 6368 2066  ction approach f
-0002a670: 6f72 204d 4f44 4953 206f 6365 616e 2063  or MODIS ocean c
-0002a680: 6f6c 6f72 2064 6174 6120 7072 6f63 6573  olor data proces
-0002a690: 7369 6e67 2e0d 0a20 2023 2020 4f70 7469  sing...  #  Opti
-0002a6a0: 6373 2045 7870 7265 7373 2c20 3135 2832  cs Express, 15(2
-0002a6b0: 3429 2c20 3135 3732 32e2 8093 3135 3733  4), 15722...1573
-0002a6c0: 332e 0d0a 0d0a 2020 2320 4164 6420 7365  3.....  # Add se
-0002a6d0: 636f 6e64 6172 7920 6669 6c74 6572 2075  condary filter u
-0002a6e0: 7369 6e67 2067 7265 656e 6e65 7373 2066  sing greenness f
-0002a6f0: 756e 6374 696f 6e20 6265 6c6f 770d 0a20  unction below.. 
-0002a700: 2069 6d61 6765 203d 2069 6d61 6765 2e61   image = image.a
-0002a710: 6464 4261 6e64 7328 486f 4361 6c63 4772  ddBands(HoCalcGr
-0002a720: 6565 6e6e 6573 7328 696d 6167 6529 290d  eenness(image)).
-0002a730: 0a0d 0a20 2023 2041 7070 6c79 2061 6c67  ...  # Apply alg
-0002a740: 6f72 6974 686d 2031 3a20 4234 202d 2031  orithm 1: B4 - 1
-0002a750: 2e30 332a 4235 0d0a 2020 2362 6c6f 6f6d  .03*B5..  #bloom
-0002a760: 3120 3d20 696d 6167 652e 7365 6c65 6374  1 = image.select
-0002a770: 2827 6e69 7227 292e 7375 6274 7261 6374  ('nir').subtract
-0002a780: 2869 6d61 6765 2e73 656c 6563 7428 2773  (image.select('s
-0002a790: 7769 7231 2729 2e6d 756c 7469 706c 7928  wir1').multiply(
-0002a7a0: 312e 3033 2929 2e72 656e 616d 6528 2762  1.03)).rename('b
-0002a7b0: 6c6f 6f6d 3127 290d 0a0d 0a20 2023 2047  loom1')....  # G
-0002a7c0: 6574 2062 696e 6172 7920 696d 6167 6520  et binary image 
-0002a7d0: 6279 2061 7070 6c79 696e 6720 7468 6520  by applying the 
-0002a7e0: 7468 7265 7368 6f6c 640d 0a20 2062 6c6f  threshold..  blo
-0002a7f0: 6f6d 315f 6d61 736b 203d 2069 6d61 6765  om1_mask = image
-0002a800: 2e73 656c 6563 7428 2248 2229 2e6c 7465  .select("H").lte
-0002a810: 2867 7265 656e 6573 7354 6872 6573 686f  (greenessThresho
-0002a820: 6c64 292e 7265 6e61 6d65 285b 2262 6c6f  ld).rename(["blo
-0002a830: 6f6d 315f 6d61 736b 225d 290d 0a0d 0a0d  om1_mask"]).....
-0002a840: 0a20 2072 6574 7572 6e20 696d 6167 655c  .  return image\
-0002a850: 0d0a 2020 2020 2020 2020 2020 2e61 6464  ..          .add
-0002a860: 4261 6e64 7328 626c 6f6f 6d31 295c 0d0a  Bands(bloom1)\..
-0002a870: 2020 2020 2020 2020 2020 2e61 6464 4261            .addBa
-0002a880: 6e64 7328 626c 6f6f 6d31 5f6d 6173 6b29  nds(bloom1_mask)
-0002a890: 0d0a 0d0a 0d0a 0d0a 0d0a 2320 2f2f 2f2f  ..........# ////
-0002a8a0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a8b0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a8c0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a8d0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a8e0: 2f2f 2f2f 2f2f 0d0a 2320 2f2f 2045 4e44  //////..# // END
-0002a8f0: 2046 554e 4354 494f 4e53 0d0a 2320 2f2f   FUNCTIONS..# //
-0002a900: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a910: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a920: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a930: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a940: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 0d0a  //////////////..
-0002a950: 0d0a 0d0a 7465 7374 4172 6561 7320 3d20  ....testAreas = 
-0002a960: 7b7d 3b0d 0a74 6573 7441 7265 6173 5b27  {};..testAreas['
-0002a970: 434f 275d 203d 2065 652e 4765 6f6d 6574  CO'] = ee.Geomet
-0002a980: 7279 2e50 6f6c 7967 6f6e 280d 0a20 2020  ry.Polygon(..   
-0002a990: 2020 2020 205b 5b5b 2d31 3038 2e32 3836       [[[-108.286
-0002a9a0: 3330 3530 3930 3634 3735 392c 2033 382e  30509064759, 38.
-0002a9b0: 3038 3533 3433 3633 3831 3230 3932 355d  085343638120925]
-0002a9c0: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
-0002a9d0: 3038 2e32 3836 3330 3530 3930 3634 3735  08.2863050906475
-0002a9e0: 392c 2033 372e 3138 3035 3132 3230 3039  9, 37.1805122009
-0002a9f0: 3239 3435 5d2c 0d0a 2020 2020 2020 2020  2945],..        
-0002aa00: 2020 5b2d 3130 362e 3734 3832 3139 3135    [-106.74821915
-0002aa10: 3331 3437 3539 2c20 3337 2e31 3830 3531  314759, 37.18051
-0002aa20: 3232 3030 3932 3934 355d 2c0d 0a20 2020  220092945],..   
-0002aa30: 2020 2020 2020 205b 2d31 3036 2e37 3438         [-106.748
-0002aa40: 3231 3931 3533 3134 3735 392c 2033 382e  21915314759, 38.
-0002aa50: 3038 3533 3433 3633 3831 3230 3932 355d  085343638120925]
-0002aa60: 5d5d 2c20 4e6f 6e65 2c20 4661 6c73 6529  ]], None, False)
-0002aa70: 0d0a 7465 7374 4172 6561 735b 2743 4f5f  ..testAreas['CO_
-0002aa80: 4e6f 7274 6827 5d20 3d20 6565 2e47 656f  North'] = ee.Geo
-0002aa90: 6d65 7472 792e 506f 6c79 676f 6e28 0d0a  metry.Polygon(..
-0002aaa0: 2020 2020 2020 2020 5b5b 5b2d 3130 362e          [[[-106.
-0002aab0: 3431 3937 3738 3639 3333 3935 3234 2c20  41977869339524, 
-0002aac0: 3430 2e39 3739 3437 3730 3233 3933 3233  40.9794770239323
-0002aad0: 345d 2c0d 0a20 2020 2020 2020 2020 205b  4],..          [
-0002aae0: 2d31 3036 2e34 3139 3737 3836 3933 3339  -106.41977869339
-0002aaf0: 3532 342c 2033 392e 3936 3430 3633 3231  524, 39.96406321
-0002ab00: 3831 3430 3031 5d2c 0d0a 2020 2020 2020  814001],..      
-0002ab10: 2020 2020 5b2d 3130 352e 3230 3537 3839      [-105.205789
-0002ab20: 3433 3535 3832 3734 2c20 3339 2e39 3634  43558274, 39.964
-0002ab30: 3036 3332 3138 3134 3030 315d 2c0d 0a20  06321814001],.. 
-0002ab40: 2020 2020 2020 2020 205b 2d31 3035 2e32           [-105.2
-0002ab50: 3035 3738 3934 3335 3538 3237 342c 2034  0578943558274, 4
-0002ab60: 302e 3937 3934 3737 3032 3339 3332 3334  0.97947702393234
-0002ab70: 5d5d 5d2c 204e 6f6e 652c 2046 616c 7365  ]]], None, False
-0002ab80: 290d 0a74 6573 7441 7265 6173 5b27 4341  )..testAreas['CA
-0002ab90: 275d 203d 6565 2e47 656f 6d65 7472 792e  '] =ee.Geometry.
-0002aba0: 506f 6c79 676f 6e28 0d0a 2020 2020 2020  Polygon(..      
-0002abb0: 2020 5b5b 5b2d 3131 392e 3936 3338 3337    [[[-119.963837
-0002abc0: 3630 3238 3735 3036 2c20 3337 2e31 3338  60287506, 37.138
-0002abd0: 3135 3035 3734 3130 3837 3134 5d2c 0d0a  150574108714],..
-0002abe0: 2020 2020 2020 2020 2020 5b2d 3131 392e            [-119.
-0002abf0: 3936 3338 3337 3630 3238 3735 3036 2c20  96383760287506, 
-0002ac00: 3336 2e34 3037 3734 3431 3231 3036 3432  36.4077441210642
-0002ac10: 345d 2c0d 0a20 2020 2020 2020 2020 205b  4],..          [
-0002ac20: 2d31 3137 2e39 3533 3333 3935 3536 3030  -117.95333955600
-0002ac30: 3030 362c 2033 362e 3430 3737 3434 3132  006, 36.40774412
-0002ac40: 3130 3634 3234 5d2c 0d0a 2020 2020 2020  106424],..      
-0002ac50: 2020 2020 5b2d 3131 372e 3935 3333 3339      [-117.953339
-0002ac60: 3535 3630 3030 3036 2c20 3337 2e31 3338  55600006, 37.138
-0002ac70: 3135 3035 3734 3130 3837 3134 5d5d 5d2c  150574108714]]],
-0002ac80: 204e 6f6e 652c 2046 616c 7365 290d 0a0d   None, False)...
-0002ac90: 0a74 6573 7441 7265 6173 5b27 4341 5f53  .testAreas['CA_S
-0002aca0: 6d61 6c6c 275d 203d 2065 652e 4765 6f6d  mall'] = ee.Geom
-0002acb0: 6574 7279 2e50 6f6c 7967 6f6e 280d 0a20  etry.Polygon(.. 
-0002acc0: 2020 2020 2020 205b 5b5b 2d31 3233 2e32         [[[-123.2
-0002acd0: 3235 3636 3936 3833 3734 3632 352c 2033  2566968374625, 3
-0002ace0: 392e 3637 3732 3039 3539 3932 3639 3135  9.67720959926915
-0002acf0: 355d 2c0d 0a20 2020 2020 2020 2020 205b  5],..          [
-0002ad00: 2d31 3233 2e32 3235 3636 3936 3833 3734  -123.22566968374
-0002ad10: 3632 352c 2033 382e 3939 3331 3739 3530  625, 38.99317950
-0002ad20: 3436 3937 3538 365d 2c0d 0a20 2020 2020  4697586],..     
-0002ad30: 2020 2020 205b 2d31 3232 2e36 3034 3934       [-122.60494
-0002ad40: 3231 3434 3638 3337 352c 2033 382e 3939  214468375, 38.99
-0002ad50: 3331 3739 3530 3436 3937 3538 365d 2c0d  3179504697586],.
-0002ad60: 0a20 2020 2020 2020 2020 205b 2d31 3232  .          [-122
-0002ad70: 2e36 3034 3934 3231 3434 3638 3337 352c  .60494214468375,
-0002ad80: 2033 392e 3637 3732 3039 3539 3932 3639   39.677209599269
-0002ad90: 3135 355d 5d5d 2c20 4e6f 6e65 2c20 4661  155]]], None, Fa
-0002ada0: 6c73 6529 0d0a 0d0a 7465 7374 4172 6561  lse)....testArea
-0002adb0: 735b 2748 4927 5d20 3d20 6565 2e47 656f  s['HI'] = ee.Geo
-0002adc0: 6d65 7472 792e 506f 6c79 676f 6e28 0d0a  metry.Polygon(..
-0002add0: 2020 2020 2020 2020 5b5b 5b2d 3136 302e          [[[-160.
-0002ade0: 3530 3832 3438 3734 3435 3035 3434 2c20  50824874450544, 
-0002adf0: 3232 2e36 3539 3831 3435 3133 3930 3934  22.6598145139094
-0002ae00: 3734 5d2c 0d0a 2020 2020 2020 2020 2020  74],..          
-0002ae10: 5b2d 3136 302e 3530 3832 3438 3734 3435  [-160.5082487445
-0002ae20: 3035 3434 2c20 3138 2e35 3437 3530 3330  0544, 18.5475030
-0002ae30: 3939 3539 3832 375d 2c0d 0a20 2020 2020  9959827],..     
-0002ae40: 2020 2020 205b 2d31 3534 2e33 3535 3930       [-154.35590
-0002ae50: 3439 3934 3530 3534 342c 2031 382e 3534  499450544, 18.54
-0002ae60: 3735 3033 3039 3935 3938 3237 5d2c 0d0a  750309959827],..
-0002ae70: 2020 2020 2020 2020 2020 5b2d 3135 342e            [-154.
-0002ae80: 3335 3539 3034 3939 3435 3035 3434 2c20  35590499450544, 
-0002ae90: 3232 2e36 3539 3831 3435 3133 3930 3934  22.6598145139094
-0002aea0: 3734 5d5d 5d2c 204e 6f6e 652c 2046 616c  74]]], None, Fal
-0002aeb0: 7365 290d 0a                             se)..
+0001f220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f250: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
+0001f260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f270: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f280: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f290: 2323 2323 2323 2323 2323 2323 0d0a 2320  ############..# 
+0001f2a0: 5772 6170 7065 7220 6675 6e63 7469 6f6e  Wrapper function
+0001f2b0: 2066 6f72 2067 6574 7469 6e67 2053 656e   for getting Sen
+0001f2c0: 7469 6e65 6c20 3220 696d 6167 6572 790d  tinel 2 imagery.
+0001f2d0: 0a64 6566 2067 6574 5365 6e74 696e 656c  .def getSentinel
+0001f2e0: 3257 7261 7070 6572 285c 0d0a 2020 7374  2Wrapper(\..  st
+0001f2f0: 7564 7941 7265 612c 0d0a 2020 7374 6172  udyArea,..  star
+0001f300: 7459 6561 722c 0d0a 2020 656e 6459 6561  tYear,..  endYea
+0001f310: 722c 0d0a 2020 7374 6172 744a 756c 6961  r,..  startJulia
+0001f320: 6e2c 0d0a 2020 656e 644a 756c 6961 6e2c  n,..  endJulian,
+0001f330: 0d0a 2020 7469 6d65 6275 6666 6572 203d  ..  timebuffer =
+0001f340: 2030 2c0d 0a20 2077 6569 6768 7473 203d   0,..  weights =
+0001f350: 205b 315d 2c0d 0a20 2063 6f6d 706f 7369   [1],..  composi
+0001f360: 7469 6e67 4d65 7468 6f64 203d 2027 6d65  tingMethod = 'me
+0001f370: 646f 6964 272c 0d0a 2020 6170 706c 7951  doid',..  applyQ
+0001f380: 4142 616e 6420 3d20 4661 6c73 652c 0d0a  ABand = False,..
+0001f390: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
+0001f3a0: 6520 3d20 4661 6c73 652c 0d0a 2020 6170  e = False,..  ap
+0001f3b0: 706c 7953 6861 646f 7753 6869 6674 203d  plyShadowShift =
+0001f3c0: 2046 616c 7365 2c0d 0a20 2061 7070 6c79   False,..  apply
+0001f3d0: 5444 4f4d 203d 2054 7275 652c 0d0a 2020  TDOM = True,..  
+0001f3e0: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
+0001f3f0: 203d 2032 302c 0d0a 2020 7065 7266 6f72   = 20,..  perfor
+0001f400: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
+0001f410: 7420 3d20 5472 7565 2c0d 0a20 2063 6c6f  t = True,..  clo
+0001f420: 7564 5363 6f72 6550 6374 6c20 3d20 3130  udScorePctl = 10
+0001f430: 2c0d 0a20 2063 6c6f 7564 4865 6967 6874  ,..  cloudHeight
+0001f440: 7320 3d65 652e 4c69 7374 2e73 6571 7565  s =ee.List.seque
+0001f450: 6e63 6528 3530 302c 3130 3030 302c 3530  nce(500,10000,50
+0001f460: 3029 2c0d 0a20 207a 5363 6f72 6554 6872  0),..  zScoreThr
+0001f470: 6573 6820 3d20 2d31 2c0d 0a20 2073 6861  esh = -1,..  sha
+0001f480: 646f 7753 756d 5468 7265 7368 203d 2030  dowSumThresh = 0
+0001f490: 2e33 352c 0d0a 2020 636f 6e74 7261 6374  .35,..  contract
+0001f4a0: 5069 7865 6c73 203d 2031 2e35 2c0d 0a20  Pixels = 1.5,.. 
+0001f4b0: 2064 696c 6174 6550 6978 656c 7320 3d20   dilatePixels = 
+0001f4c0: 332e 352c 0d0a 2020 7368 6164 6f77 5375  3.5,..  shadowSu
+0001f4d0: 6d42 616e 6473 203d 205b 276e 6972 272c  mBands = ['nir',
+0001f4e0: 2773 7769 7231 275d 2c0d 0a20 2063 6f72  'swir1'],..  cor
+0001f4f0: 7265 6374 496c 6c75 6d69 6e61 7469 6f6e  rectIllumination
+0001f500: 203d 2046 616c 7365 2c0d 0a20 2063 6f72   = False,..  cor
+0001f510: 7265 6374 5363 616c 6520 3d20 3235 302c  rectScale = 250,
+0001f520: 0d0a 2020 6578 706f 7274 436f 6d70 6f73  ..  exportCompos
+0001f530: 6974 6573 203d 2046 616c 7365 2c0d 0a20  ites = False,.. 
+0001f540: 206f 7574 7075 744e 616d 6520 3d20 2753   outputName = 'S
+0001f550: 656e 7469 6e65 6c32 2d43 6f6d 706f 7369  entinel2-Composi
+0001f560: 7465 272c 0d0a 2020 6578 706f 7274 5061  te',..  exportPa
+0001f570: 7468 526f 6f74 203d 2027 7573 6572 732f  thRoot = 'users/
+0001f580: 6961 6e68 6f75 736d 616e 2f74 6573 7427  ianhousman/test'
+0001f590: 2c0d 0a20 2063 7273 203d 2027 4550 5347  ,..  crs = 'EPSG
+0001f5a0: 3a35 3037 3027 2c0d 0a20 2074 7261 6e73  :5070',..  trans
+0001f5b0: 666f 726d 203d 205b 3130 2c30 2c2d 3233  form = [10,0,-23
+0001f5c0: 3631 3931 352e 302c 302c 2d31 302c 3331  61915.0,0,-10,31
+0001f5d0: 3737 3733 352e 305d 2c0d 0a20 2073 6361  77735.0],..  sca
+0001f5e0: 6c65 203d 204e 6f6e 652c 0d0a 2020 7265  le = None,..  re
+0001f5f0: 7361 6d70 6c65 4d65 7468 6f64 203d 2027  sampleMethod = '
+0001f600: 6167 6772 6567 6174 6527 2c0d 0a20 2074  aggregate',..  t
+0001f610: 6f61 4f72 5352 203d 2027 544f 4127 2c0d  oaOrSR = 'TOA',.
+0001f620: 0a20 2063 6f6e 7665 7274 546f 4461 696c  .  convertToDail
+0001f630: 794d 6f73 6169 6373 203d 2054 7275 652c  yMosaics = True,
+0001f640: 0d0a 2020 6170 706c 7943 6c6f 7564 5072  ..  applyCloudPr
+0001f650: 6f62 6162 696c 6974 7920 3d20 5472 7565  obability = True
+0001f660: 2c0d 0a20 2070 7265 436f 6d70 7574 6564  ,..  preComputed
+0001f670: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+0001f680: 203d 204e 6f6e 652c 0d0a 2020 7072 6543   = None,..  preC
+0001f690: 6f6d 7075 7465 6454 444f 4d49 524d 6561  omputedTDOMIRMea
+0001f6a0: 6e20 3d20 4e6f 6e65 2c0d 0a20 2070 7265  n = None,..  pre
+0001f6b0: 436f 6d70 7574 6564 5444 4f4d 4952 5374  ComputedTDOMIRSt
+0001f6c0: 6444 6576 203d 204e 6f6e 652c 0d0a 2020  dDev = None,..  
+0001f6d0: 636c 6f75 6450 726f 6254 6872 6573 6820  cloudProbThresh 
+0001f6e0: 3d20 3430 2c0d 0a20 206f 7665 7277 7269  = 40,..  overwri
+0001f6f0: 7465 203d 2046 616c 7365 2c0d 0a20 2076  te = False,..  v
+0001f700: 6572 626f 7365 203d 2046 616c 7365 293a  erbose = False):
+0001f710: 0d0a 0d0a 2020 6f72 6967 696e 203d 2027  ....  origin = '
+0001f720: 5365 6e74 696e 656c 3227 0d0a 2020 746f  Sentinel2'..  to
+0001f730: 614f 7253 5220 3d20 746f 614f 7253 522e  aOrSR = toaOrSR.
+0001f740: 7570 7065 7228 290d 0a0d 0a20 2061 7267  upper()....  arg
+0001f750: 7320 3d20 666f 726d 6174 4172 6773 286c  s = formatArgs(l
+0001f760: 6f63 616c 7328 2929 0d0a 2020 6966 2027  ocals())..  if '
+0001f770: 6172 6773 2720 696e 2061 7267 732e 6b65  args' in args.ke
+0001f780: 7973 2829 3a0d 0a20 2020 2064 656c 2061  ys():..    del a
+0001f790: 7267 735b 2761 7267 7327 5d0d 0a0d 0a20  rgs['args'].... 
+0001f7a0: 2073 3273 203d 2067 6574 5072 6f63 6573   s2s = getProces
+0001f7b0: 7365 6453 656e 7469 6e65 6c32 5363 656e  sedSentinel2Scen
+0001f7c0: 6573 285c 0d0a 2020 2020 7374 7564 7941  es(\..    studyA
+0001f7d0: 7265 6120 3d20 7374 7564 7941 7265 612c  rea = studyArea,
+0001f7e0: 0d0a 2020 2020 7374 6172 7459 6561 7220  ..    startYear 
+0001f7f0: 3d20 7374 6172 7459 6561 722c 0d0a 2020  = startYear,..  
+0001f800: 2020 656e 6459 6561 7220 3d20 656e 6459    endYear = endY
+0001f810: 6561 722c 0d0a 2020 2020 7374 6172 744a  ear,..    startJ
+0001f820: 756c 6961 6e20 3d20 7374 6172 744a 756c  ulian = startJul
+0001f830: 6961 6e2c 0d0a 2020 2020 656e 644a 756c  ian,..    endJul
+0001f840: 6961 6e20 3d20 656e 644a 756c 6961 6e2c  ian = endJulian,
+0001f850: 0d0a 2020 2020 6170 706c 7951 4142 616e  ..    applyQABan
+0001f860: 6420 3d20 6170 706c 7951 4142 616e 642c  d = applyQABand,
+0001f870: 0d0a 2020 2020 6170 706c 7943 6c6f 7564  ..    applyCloud
+0001f880: 5363 6f72 6520 3d20 6170 706c 7943 6c6f  Score = applyClo
+0001f890: 7564 5363 6f72 652c 0d0a 2020 2020 6170  udScore,..    ap
+0001f8a0: 706c 7953 6861 646f 7753 6869 6674 203d  plyShadowShift =
+0001f8b0: 2061 7070 6c79 5368 6164 6f77 5368 6966   applyShadowShif
+0001f8c0: 742c 0d0a 2020 2020 6170 706c 7954 444f  t,..    applyTDO
+0001f8d0: 4d20 3d20 6170 706c 7954 444f 4d2c 0d0a  M = applyTDOM,..
+0001f8e0: 2020 2020 636c 6f75 6453 636f 7265 5468      cloudScoreTh
+0001f8f0: 7265 7368 203d 2063 6c6f 7564 5363 6f72  resh = cloudScor
+0001f900: 6554 6872 6573 682c 0d0a 2020 2020 7065  eThresh,..    pe
+0001f910: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
+0001f920: 6666 7365 7420 3d20 7065 7266 6f72 6d43  ffset = performC
+0001f930: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+0001f940: 0d0a 2020 2020 636c 6f75 6453 636f 7265  ..    cloudScore
+0001f950: 5063 746c 203d 2063 6c6f 7564 5363 6f72  Pctl = cloudScor
+0001f960: 6550 6374 6c2c 0d0a 2020 2020 636c 6f75  ePctl,..    clou
+0001f970: 6448 6569 6768 7473 203d 2063 6c6f 7564  dHeights = cloud
+0001f980: 4865 6967 6874 732c 0d0a 2020 2020 7a53  Heights,..    zS
+0001f990: 636f 7265 5468 7265 7368 203d 207a 5363  coreThresh = zSc
+0001f9a0: 6f72 6554 6872 6573 682c 0d0a 2020 2020  oreThresh,..    
+0001f9b0: 7368 6164 6f77 5375 6d54 6872 6573 6820  shadowSumThresh 
+0001f9c0: 3d20 7368 6164 6f77 5375 6d54 6872 6573  = shadowSumThres
+0001f9d0: 682c 0d0a 2020 2020 636f 6e74 7261 6374  h,..    contract
+0001f9e0: 5069 7865 6c73 203d 2063 6f6e 7472 6163  Pixels = contrac
+0001f9f0: 7450 6978 656c 732c 0d0a 2020 2020 6469  tPixels,..    di
+0001fa00: 6c61 7465 5069 7865 6c73 203d 2064 696c  latePixels = dil
+0001fa10: 6174 6550 6978 656c 732c 0d0a 2020 2020  atePixels,..    
+0001fa20: 7368 6164 6f77 5375 6d42 616e 6473 203d  shadowSumBands =
+0001fa30: 2073 6861 646f 7753 756d 4261 6e64 732c   shadowSumBands,
+0001fa40: 0d0a 2020 2020 7265 7361 6d70 6c65 4d65  ..    resampleMe
+0001fa50: 7468 6f64 203d 2072 6573 616d 706c 654d  thod = resampleM
+0001fa60: 6574 686f 642c 0d0a 2020 2020 746f 614f  ethod,..    toaO
+0001fa70: 7253 5220 3d20 746f 614f 7253 522c 0d0a  rSR = toaOrSR,..
+0001fa80: 2020 2020 636f 6e76 6572 7454 6f44 6169      convertToDai
+0001fa90: 6c79 4d6f 7361 6963 7320 3d20 636f 6e76  lyMosaics = conv
+0001faa0: 6572 7454 6f44 6169 6c79 4d6f 7361 6963  ertToDailyMosaic
+0001fab0: 732c 0d0a 2020 2020 6170 706c 7943 6c6f  s,..    applyClo
+0001fac0: 7564 5072 6f62 6162 696c 6974 7920 3d20  udProbability = 
+0001fad0: 6170 706c 7943 6c6f 7564 5072 6f62 6162  applyCloudProbab
+0001fae0: 696c 6974 792c 0d0a 2020 2020 7072 6543  ility,..    preC
+0001faf0: 6f6d 7075 7465 6443 6c6f 7564 5363 6f72  omputedCloudScor
+0001fb00: 654f 6666 7365 7420 3d20 7072 6543 6f6d  eOffset = preCom
+0001fb10: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
+0001fb20: 6666 7365 742c 0d0a 2020 2020 7072 6543  ffset,..    preC
+0001fb30: 6f6d 7075 7465 6454 444f 4d49 524d 6561  omputedTDOMIRMea
+0001fb40: 6e20 3d20 7072 6543 6f6d 7075 7465 6454  n = preComputedT
+0001fb50: 444f 4d49 524d 6561 6e2c 0d0a 2020 2020  DOMIRMean,..    
+0001fb60: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
+0001fb70: 5253 7464 4465 7620 3d20 7072 6543 6f6d  RStdDev = preCom
+0001fb80: 7075 7465 6454 444f 4d49 5253 7464 4465  putedTDOMIRStdDe
+0001fb90: 762c 0d0a 2020 2020 636c 6f75 6450 726f  v,..    cloudPro
+0001fba0: 6254 6872 6573 6820 3d20 636c 6f75 6450  bThresh = cloudP
+0001fbb0: 726f 6254 6872 6573 682c 0d0a 2020 2020  robThresh,..    
+0001fbc0: 7665 7262 6f73 6520 3d20 7665 7262 6f73  verbose = verbos
+0001fbd0: 6529 0d0a 0d0a 2020 2341 6464 207a 656e  e)....  #Add zen
+0001fbe0: 6974 6820 616e 6420 617a 696d 7574 680d  ith and azimuth.
+0001fbf0: 0a20 2023 6966 2063 6f72 7265 6374 496c  .  #if correctIl
+0001fc00: 6c75 6d69 6e61 7469 6f6e 3a0d 0a20 2023  lumination:..  #
+0001fc10: 2020 7332 7320 3d20 7332 732e 6d61 7028    s2s = s2s.map(
+0001fc20: 6675 6e63 7469 6f6e 2869 6d67 297b 0d0a  function(img){..
+0001fc30: 2020 2320 2020 2072 6574 7572 6e20 6164    #    return ad
+0001fc40: 645a 656e 6974 6841 7a69 6d75 7468 2869  dZenithAzimuth(i
+0001fc50: 6d67 2c27 544f 4127 2c7b 2754 4f41 273a  mg,'TOA',{'TOA':
+0001fc60: 274d 4541 4e5f 534f 4c41 525f 5a45 4e49  'MEAN_SOLAR_ZENI
+0001fc70: 5448 5f41 4e47 4c45 277d 2c7b 2754 4f41  TH_ANGLE'},{'TOA
+0001fc80: 273a 274d 4541 4e5f 534f 4c41 525f 415a  ':'MEAN_SOLAR_AZ
+0001fc90: 494d 5554 485f 414e 474c 4527 7d29 3b0d  IMUTH_ANGLE'});.
+0001fca0: 0a20 2023 2020 7d29 3b0d 0a20 2023 7d0d  .  #  });..  #}.
+0001fcb0: 0a0d 0a20 2023 4372 6561 7465 2063 6f6d  ...  #Create com
+0001fcc0: 706f 7369 7465 2074 696d 6520 7365 7269  posite time seri
+0001fcd0: 6573 0d0a 2020 7473 203d 2063 6f6d 706f  es..  ts = compo
+0001fce0: 7369 7465 5469 6d65 5365 7269 6573 285c  siteTimeSeries(\
+0001fcf0: 0d0a 2020 2020 6c73 203d 2073 3273 2c0d  ..    ls = s2s,.
+0001fd00: 0a20 2020 2073 7461 7274 5965 6172 203d  .    startYear =
+0001fd10: 2073 7461 7274 5965 6172 2c0d 0a20 2020   startYear,..   
+0001fd20: 2065 6e64 5965 6172 203d 2065 6e64 5965   endYear = endYe
+0001fd30: 6172 2c0d 0a20 2020 2073 7461 7274 4a75  ar,..    startJu
+0001fd40: 6c69 616e 203d 2073 7461 7274 4a75 6c69  lian = startJuli
+0001fd50: 616e 2c0d 0a20 2020 2065 6e64 4a75 6c69  an,..    endJuli
+0001fd60: 616e 203d 2065 6e64 4a75 6c69 616e 2c0d  an = endJulian,.
+0001fd70: 0a20 2020 2074 696d 6562 7566 6665 7220  .    timebuffer 
+0001fd80: 3d20 7469 6d65 6275 6666 6572 2c0d 0a20  = timebuffer,.. 
+0001fd90: 2020 2077 6569 6768 7473 203d 2077 6569     weights = wei
+0001fda0: 6768 7473 2c0d 0a20 2020 2063 6f6d 706f  ghts,..    compo
+0001fdb0: 7369 7469 6e67 4d65 7468 6f64 203d 2063  sitingMethod = c
+0001fdc0: 6f6d 706f 7369 7469 6e67 4d65 7468 6f64  ompositingMethod
+0001fdd0: 290d 0a0d 0a20 2023 436f 7272 6563 7420  )....  #Correct 
+0001fde0: 696c 6c75 6d69 6e61 7469 6f6e 0d0a 2020  illumination..  
+0001fdf0: 2320 6966 2028 636f 7272 6563 7449 6c6c  # if (correctIll
+0001fe00: 756d 696e 6174 696f 6e29 7b0d 0a20 2023  umination){..  #
+0001fe10: 2020 2066 203d 2065 652e 496d 6167 6528     f = ee.Image(
+0001fe20: 7473 2e66 6972 7374 2829 293b 0d0a 2020  ts.first());..  
+0001fe30: 2320 2020 4d61 702e 6164 644c 6179 6572  #   Map.addLayer
+0001fe40: 2866 2c76 697a 5061 7261 6d73 4661 6c73  (f,vizParamsFals
+0001fe50: 652c 2746 6972 7374 2d6e 6f6e 2d69 6c6c  e,'First-non-ill
+0001fe60: 756d 696e 6174 6564 272c 6661 6c73 6529  uminated',false)
+0001fe70: 3b0d 0a0d 0a20 2023 2020 2070 7269 6e74  ;....  #   print
+0001fe80: 2827 436f 7272 6563 7469 6e67 2069 6c6c  ('Correcting ill
+0001fe90: 756d 696e 6174 696f 6e27 293b 0d0a 2020  umination');..  
+0001fea0: 2320 2020 7473 203d 2074 732e 6d61 7028  #   ts = ts.map(
+0001feb0: 696c 6c75 6d69 6e61 7469 6f6e 436f 6e64  illuminationCond
+0001fec0: 6974 696f 6e29 0d0a 2020 2320 2020 2020  ition)..  #     
+0001fed0: 2e6d 6170 2866 756e 6374 696f 6e28 696d  .map(function(im
+0001fee0: 6729 7b0d 0a20 2023 2020 2020 2020 2072  g){..  #       r
+0001fef0: 6574 7572 6e20 696c 6c75 6d69 6e61 7469  eturn illuminati
+0001ff00: 6f6e 436f 7272 6563 7469 6f6e 2869 6d67  onCorrection(img
+0001ff10: 2c20 636f 7272 6563 7453 6361 6c65 2c73  , correctScale,s
+0001ff20: 7475 6479 4172 6561 2c5b 2027 626c 7565  tudyArea,[ 'blue
+0001ff30: 272c 2027 6772 6565 6e27 2c20 2772 6564  ', 'green', 'red
+0001ff40: 272c 276e 6972 272c 2773 7769 7231 272c  ','nir','swir1',
+0001ff50: 2027 7377 6972 3227 5d29 3b0d 0a20 2023   'swir2']);..  #
+0001ff60: 2020 2020 207d 293b 0d0a 2020 2320 2020       });..  #   
+0001ff70: 6620 3d20 6565 2e49 6d61 6765 2874 732e  f = ee.Image(ts.
+0001ff80: 6669 7273 7428 2929 3b0d 0a20 2023 2020  first());..  #  
+0001ff90: 204d 6170 2e61 6464 4c61 7965 7228 662c   Map.addLayer(f,
+0001ffa0: 7669 7a50 6172 616d 7346 616c 7365 2c27  vizParamsFalse,'
+0001ffb0: 4669 7273 742d 696c 6c75 6d69 6e61 7465  First-illuminate
+0001ffc0: 6427 2c66 616c 7365 293b 0d0a 0d0a 2020  d',false);....  
+0001ffd0: 2320 4578 706f 7274 2063 6f6d 706f 7369  # Export composi
+0001ffe0: 7465 730d 0a20 2069 6620 6578 706f 7274  tes..  if export
+0001fff0: 436f 6d70 6f73 6974 6573 3a0d 0a20 2020  Composites:..   
+00020000: 2065 7870 6f72 7442 616e 6444 6963 7420   exportBandDict 
+00020010: 3d20 7b5c 0d0a 2020 2020 2020 2753 525f  = {\..      'SR_
+00020020: 6d65 646f 6964 273a 5b27 6362 272c 2027  medoid':['cb', '
+00020030: 626c 7565 272c 2027 6772 6565 6e27 2c20  blue', 'green', 
+00020040: 2772 6564 272c 2027 7265 3127 2c27 7265  'red', 're1','re
+00020050: 3227 2c27 7265 3327 2c27 6e69 7227 2c20  2','re3','nir', 
+00020060: 276e 6972 3227 2c20 2777 6174 6572 5661  'nir2', 'waterVa
+00020070: 706f 7227 2c20 2773 7769 7231 272c 2027  por', 'swir1', '
+00020080: 7377 6972 3227 2c27 636f 6d70 6f73 6974  swir2','composit
+00020090: 654f 6273 436f 756e 7427 2c27 7365 6e73  eObsCount','sens
+000200a0: 6f72 272c 2779 6561 7227 2c27 6a75 6c69  or','year','juli
+000200b0: 616e 4461 7927 5d2c 0d0a 2020 2020 2020  anDay'],..      
+000200c0: 2753 525f 6d65 6469 616e 273a 5b27 6362  'SR_median':['cb
+000200d0: 272c 2027 626c 7565 272c 2027 6772 6565  ', 'blue', 'gree
+000200e0: 6e27 2c20 2772 6564 272c 2027 7265 3127  n', 'red', 're1'
+000200f0: 2c27 7265 3227 2c27 7265 3327 2c27 6e69  ,'re2','re3','ni
+00020100: 7227 2c20 276e 6972 3227 2c20 2777 6174  r', 'nir2', 'wat
+00020110: 6572 5661 706f 7227 2c20 2773 7769 7231  erVapor', 'swir1
+00020120: 272c 2027 7377 6972 3227 2c27 636f 6d70  ', 'swir2','comp
+00020130: 6f73 6974 654f 6273 436f 756e 7427 5d2c  ositeObsCount'],
+00020140: 0d0a 2020 2020 2020 2754 4f41 5f6d 6564  ..      'TOA_med
+00020150: 6f69 6427 3a5b 2763 6227 2c20 2762 6c75  oid':['cb', 'blu
+00020160: 6527 2c20 2767 7265 656e 272c 2027 7265  e', 'green', 're
+00020170: 6427 2c20 2772 6531 272c 2772 6532 272c  d', 're1','re2',
+00020180: 2772 6533 272c 276e 6972 272c 2027 6e69  're3','nir', 'ni
+00020190: 7232 272c 2027 7761 7465 7256 6170 6f72  r2', 'waterVapor
+000201a0: 272c 2027 6369 7272 7573 272c 2027 7377  ', 'cirrus', 'sw
+000201b0: 6972 3127 2c20 2773 7769 7232 272c 2763  ir1', 'swir2','c
+000201c0: 6f6d 706f 7369 7465 4f62 7343 6f75 6e74  ompositeObsCount
+000201d0: 272c 2773 656e 736f 7227 2c27 7965 6172  ','sensor','year
+000201e0: 272c 276a 756c 6961 6e44 6179 275d 2c0d  ','julianDay'],.
+000201f0: 0a20 2020 2020 2027 544f 415f 6d65 6469  .      'TOA_medi
+00020200: 616e 273a 5b27 6362 272c 2027 626c 7565  an':['cb', 'blue
+00020210: 272c 2027 6772 6565 6e27 2c20 2772 6564  ', 'green', 'red
+00020220: 272c 2027 7265 3127 2c27 7265 3227 2c27  ', 're1','re2','
+00020230: 7265 3327 2c27 6e69 7227 2c20 276e 6972  re3','nir', 'nir
+00020240: 3227 2c20 2777 6174 6572 5661 706f 7227  2', 'waterVapor'
+00020250: 2c20 2763 6972 7275 7327 2c20 2773 7769  , 'cirrus', 'swi
+00020260: 7231 272c 2027 7377 6972 3227 2c27 636f  r1', 'swir2','co
+00020270: 6d70 6f73 6974 654f 6273 436f 756e 7427  mpositeObsCount'
+00020280: 5d5c 0d0a 2020 2020 7d0d 0a20 2020 206e  ]\..    }..    n
+00020290: 6f6e 4469 7669 6465 4261 6e64 4469 6374  onDivideBandDict
+000202a0: 203d 207b 5c0d 0a20 2020 2020 2027 6d65   = {\..      'me
+000202b0: 646f 6964 273a 5b27 636f 6d70 6f73 6974  doid':['composit
+000202c0: 654f 6273 436f 756e 7427 2c27 7365 6e73  eObsCount','sens
+000202d0: 6f72 272c 2779 6561 7227 2c27 6a75 6c69  or','year','juli
+000202e0: 616e 4461 7927 5d2c 0d0a 2020 2020 2020  anDay'],..      
+000202f0: 276d 6564 6961 6e27 3a5b 2763 6f6d 706f  'median':['compo
+00020300: 7369 7465 4f62 7343 6f75 6e74 275d 5c0d  siteObsCount']\.
+00020310: 0a20 2020 207d 0d0a 2020 2020 6578 706f  .    }..    expo
+00020320: 7274 4261 6e64 7320 3d20 6578 706f 7274  rtBands = export
+00020330: 4261 6e64 4469 6374 5b74 6f61 4f72 5352  BandDict[toaOrSR
+00020340: 202b 2027 5f27 202b 2063 6f6d 706f 7369   + '_' + composi
+00020350: 7469 6e67 4d65 7468 6f64 5d0d 0a20 2020  tingMethod]..   
+00020360: 206e 6f6e 4469 7669 6465 4261 6e64 7320   nonDivideBands 
+00020370: 3d20 6e6f 6e44 6976 6964 6542 616e 6444  = nonDivideBandD
+00020380: 6963 745b 636f 6d70 6f73 6974 696e 674d  ict[compositingM
+00020390: 6574 686f 645d 0d0a 0d0a 2020 2020 6578  ethod]....    ex
+000203a0: 706f 7274 436f 6d70 6f73 6974 6543 6f6c  portCompositeCol
+000203b0: 6c65 6374 696f 6e28 5c0d 0a20 2020 2020  lection(\..     
+000203c0: 2063 6f6c 6c65 6374 696f 6e20 3d20 7473   collection = ts
+000203d0: 2c0d 0a20 2020 2020 2065 7870 6f72 7450  ,..      exportP
+000203e0: 6174 6852 6f6f 7420 3d20 6578 706f 7274  athRoot = export
+000203f0: 5061 7468 526f 6f74 2c0d 0a20 2020 2020  PathRoot,..     
+00020400: 206f 7574 7075 744e 616d 6520 3d20 6f75   outputName = ou
+00020410: 7470 7574 4e61 6d65 2c0d 0a20 2020 2020  tputName,..     
+00020420: 206f 7269 6769 6e20 3d20 6f72 6967 696e   origin = origin
+00020430: 2c0d 0a20 2020 2020 2073 7475 6479 4172  ,..      studyAr
+00020440: 6561 203d 2073 7475 6479 4172 6561 2c0d  ea = studyArea,.
+00020450: 0a20 2020 2020 2063 7273 203d 2063 7273  .      crs = crs
+00020460: 2c0d 0a20 2020 2020 2074 7261 6e73 666f  ,..      transfo
+00020470: 726d 203d 2074 7261 6e73 666f 726d 2c0d  rm = transform,.
+00020480: 0a20 2020 2020 2073 6361 6c65 203d 2073  .      scale = s
+00020490: 6361 6c65 2c0d 0a20 2020 2020 2073 7461  cale,..      sta
+000204a0: 7274 5965 6172 203d 2073 7461 7274 5965  rtYear = startYe
+000204b0: 6172 2c0d 0a20 2020 2020 2065 6e64 5965  ar,..      endYe
+000204c0: 6172 203d 2065 6e64 5965 6172 2c0d 0a20  ar = endYear,.. 
+000204d0: 2020 2020 2073 7461 7274 4a75 6c69 616e       startJulian
+000204e0: 203d 2073 7461 7274 4a75 6c69 616e 2c0d   = startJulian,.
+000204f0: 0a20 2020 2020 2065 6e64 4a75 6c69 616e  .      endJulian
+00020500: 203d 2065 6e64 4a75 6c69 616e 2c0d 0a20   = endJulian,.. 
+00020510: 2020 2020 2063 6f6d 706f 7369 7469 6e67       compositing
+00020520: 4d65 7468 6f64 203d 2063 6f6d 706f 7369  Method = composi
+00020530: 7469 6e67 4d65 7468 6f64 2c0d 0a20 2020  tingMethod,..   
+00020540: 2020 2074 696d 6562 7566 6665 7220 3d20     timebuffer = 
+00020550: 7469 6d65 6275 6666 6572 2c0d 0a20 2020  timebuffer,..   
+00020560: 2020 2074 6f61 4f72 5352 203d 2074 6f61     toaOrSR = toa
+00020570: 4f72 5352 2c0d 0a20 2020 2020 206e 6f6e  OrSR,..      non
+00020580: 4469 7669 6465 4261 6e64 7320 3d20 6e6f  DivideBands = no
+00020590: 6e44 6976 6964 6542 616e 6473 2c0d 0a20  nDivideBands,.. 
+000205a0: 2020 2020 2065 7870 6f72 7442 616e 6473       exportBands
+000205b0: 203d 2065 7870 6f72 7442 616e 6473 2c0d   = exportBands,.
+000205c0: 0a20 2020 2020 2061 6464 6974 696f 6e61  .      additiona
+000205d0: 6c50 726f 7065 7274 7944 6963 7420 3d20  lPropertyDict = 
+000205e0: 6172 6773 2c0d 0a20 2020 2020 206f 7665  args,..      ove
+000205f0: 7277 7269 7465 203d 206f 7665 7277 7269  rwrite = overwri
+00020600: 7465 290d 0a0d 0a20 2061 7267 735b 2770  te)....  args['p
+00020610: 726f 6365 7373 6564 5363 656e 6573 275d  rocessedScenes']
+00020620: 203d 2073 3273 0d0a 2020 6172 6773 5b27   = s2s..  args['
+00020630: 7072 6f63 6573 7365 6443 6f6d 706f 7369  processedComposi
+00020640: 7465 7327 5d20 3d20 7473 0d0a 0d0a 2020  tes'] = ts....  
+00020650: 7265 7475 726e 2061 7267 730d 0a0d 0a23  return args....#
+00020660: 2048 7962 7269 6420 6765 7420 4c61 6e64   Hybrid get Land
+00020670: 7361 7420 616e 6420 5365 6e74 696e 656c  sat and Sentinel
+00020680: 2032 2070 726f 6365 7373 6564 2073 6365   2 processed sce
+00020690: 6e65 730d 0a23 2048 616e 646c 6573 2067  nes..# Handles g
+000206a0: 6574 7469 6e67 2070 726f 6365 7373 6564  etting processed
+000206b0: 2073 6365 6e65 7320 2077 6974 6820 4c61   scenes  with La
+000206c0: 6e64 7361 7420 616e 6420 5365 6e74 696e  ndsat and Sentin
+000206d0: 656c 2032 0d0a 6465 6620 6765 7450 726f  el 2..def getPro
+000206e0: 6365 7373 6564 4c61 6e64 7361 7441 6e64  cessedLandsatAnd
+000206f0: 5365 6e74 696e 656c 3253 6365 6e65 7328  Sentinel2Scenes(
+00020700: 0d0a 2020 2020 2020 7374 7564 7941 7265  ..      studyAre
+00020710: 612c 0d0a 2020 2020 2020 7374 6172 7459  a,..      startY
+00020720: 6561 722c 0d0a 2020 2020 2020 656e 6459  ear,..      endY
+00020730: 6561 722c 0d0a 2020 2020 2020 7374 6172  ear,..      star
+00020740: 744a 756c 6961 6e2c 0d0a 2020 2020 2020  tJulian,..      
+00020750: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
+00020760: 2020 746f 614f 7253 5220 3d20 2754 4f41    toaOrSR = 'TOA
+00020770: 272c 0d0a 2020 2020 2020 696e 636c 7564  ',..      includ
+00020780: 6553 4c43 4f66 664c 3720 3d20 4661 6c73  eSLCOffL7 = Fals
+00020790: 652c 0d0a 2020 2020 2020 6465 6672 696e  e,..      defrin
+000207a0: 6765 4c35 203d 2046 616c 7365 2c0d 0a20  geL5 = False,.. 
+000207b0: 2020 2020 2061 7070 6c79 5141 4261 6e64       applyQABand
+000207c0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+000207d0: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
+000207e0: 6269 6c69 7479 203d 2054 7275 652c 0d0a  bility = True,..
+000207f0: 2020 2020 2020 6170 706c 7953 6861 646f        applyShado
+00020800: 7753 6869 6674 203d 2046 616c 7365 2c0d  wShift = False,.
+00020810: 0a20 2020 2020 2061 7070 6c79 436c 6f75  .      applyClou
+00020820: 6453 636f 7265 4c61 6e64 7361 7420 3d20  dScoreLandsat = 
+00020830: 4661 6c73 652c 0d0a 2020 2020 2020 6170  False,..      ap
+00020840: 706c 7943 6c6f 7564 5363 6f72 6553 656e  plyCloudScoreSen
+00020850: 7469 6e65 6c32 203d 2046 616c 7365 2c0d  tinel2 = False,.
+00020860: 0a20 2020 2020 2061 7070 6c79 5444 4f4d  .      applyTDOM
+00020870: 4c61 6e64 7361 7420 3d20 5472 7565 2c0d  Landsat = True,.
+00020880: 0a20 2020 2020 2061 7070 6c79 5444 4f4d  .      applyTDOM
+00020890: 5365 6e74 696e 656c 3220 3d20 5472 7565  Sentinel2 = True
+000208a0: 2c0d 0a20 2020 2020 2061 7070 6c79 466d  ,..      applyFm
+000208b0: 6173 6b43 6c6f 7564 4d61 736b 203d 2054  askCloudMask = T
+000208c0: 7275 652c 0d0a 2020 2020 2020 6170 706c  rue,..      appl
+000208d0: 7946 6d61 736b 436c 6f75 6453 6861 646f  yFmaskCloudShado
+000208e0: 774d 6173 6b20 3d20 5472 7565 2c0d 0a20  wMask = True,.. 
+000208f0: 2020 2020 2061 7070 6c79 466d 6173 6b53       applyFmaskS
+00020900: 6e6f 774d 6173 6b20 3d20 4661 6c73 652c  nowMask = False,
+00020910: 0d0a 2020 2020 2020 636c 6f75 6448 6569  ..      cloudHei
+00020920: 6768 7473 203d 2065 652e 4c69 7374 2e73  ghts = ee.List.s
+00020930: 6571 7565 6e63 6528 3530 302c 3130 3030  equence(500,1000
+00020940: 302c 3530 3029 2c0d 0a20 2020 2020 2063  0,500),..      c
+00020950: 6c6f 7564 5363 6f72 6554 6872 6573 6820  loudScoreThresh 
+00020960: 3d20 3230 2c0d 0a20 2020 2020 2070 6572  = 20,..      per
+00020970: 666f 726d 436c 6f75 6453 636f 7265 4f66  formCloudScoreOf
+00020980: 6673 6574 203d 2054 7275 652c 0d0a 2020  fset = True,..  
+00020990: 2020 2020 636c 6f75 6453 636f 7265 5063      cloudScorePc
+000209a0: 746c 203d 2031 302c 0d0a 2020 2020 2020  tl = 10,..      
+000209b0: 7a53 636f 7265 5468 7265 7368 203d 202d  zScoreThresh = -
+000209c0: 312c 0d0a 2020 2020 2020 7368 6164 6f77  1,..      shadow
+000209d0: 5375 6d54 6872 6573 6820 3d20 302e 3335  SumThresh = 0.35
+000209e0: 2c0d 0a20 2020 2020 2063 6f6e 7472 6163  ,..      contrac
+000209f0: 7450 6978 656c 7320 3d20 312e 352c 0d0a  tPixels = 1.5,..
+00020a00: 2020 2020 2020 6469 6c61 7465 5069 7865        dilatePixe
+00020a10: 6c73 203d 2033 2e35 2c0d 0a20 2020 2020  ls = 3.5,..     
+00020a20: 2073 6861 646f 7753 756d 4261 6e64 7320   shadowSumBands 
+00020a30: 3d20 5b27 6e69 7227 2c27 7377 6972 3127  = ['nir','swir1'
+00020a40: 5d2c 0d0a 2020 2020 2020 6c61 6e64 7361  ],..      landsa
+00020a50: 7452 6573 616d 706c 654d 6574 686f 6420  tResampleMethod 
+00020a60: 3d20 276e 6561 7227 2c0d 0a20 2020 2020  = 'near',..     
+00020a70: 2073 656e 7469 6e65 6c32 5265 7361 6d70   sentinel2Resamp
+00020a80: 6c65 4d65 7468 6f64 203d 2027 6167 6772  leMethod = 'aggr
+00020a90: 6567 6174 6527 2c0d 0a20 2020 2020 2063  egate',..      c
+00020aa0: 6f6e 7665 7274 546f 4461 696c 794d 6f73  onvertToDailyMos
+00020ab0: 6169 6373 203d 2054 7275 652c 0d0a 2020  aics = True,..  
+00020ac0: 2020 2020 7275 6e43 6861 7374 6169 6e48      runChastainH
+00020ad0: 6172 6d6f 6e69 7a61 7469 6f6e 203d 2054  armonization = T
+00020ae0: 7275 652c 0d0a 2020 2020 2020 636f 7272  rue,..      corr
+00020af0: 6563 7449 6c6c 756d 696e 6174 696f 6e20  ectIllumination 
+00020b00: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00020b10: 636f 7272 6563 7453 6361 6c65 203d 2032  correctScale = 2
+00020b20: 3530 2c0d 0a20 2020 2020 2070 7265 436f  50,..      preCo
+00020b30: 6d70 7574 6564 4c61 6e64 7361 7443 6c6f  mputedLandsatClo
+00020b40: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+00020b50: 4e6f 6e65 2c0d 0a20 2020 2020 2070 7265  None,..      pre
+00020b60: 436f 6d70 7574 6564 4c61 6e64 7361 7454  ComputedLandsatT
+00020b70: 444f 4d49 524d 6561 6e20 3d20 4e6f 6e65  DOMIRMean = None
+00020b80: 2c0d 0a20 2020 2020 2070 7265 436f 6d70  ,..      preComp
+00020b90: 7574 6564 4c61 6e64 7361 7454 444f 4d49  utedLandsatTDOMI
+00020ba0: 5253 7464 4465 7620 3d20 4e6f 6e65 2c0d  RStdDev = None,.
+00020bb0: 0a20 2020 2020 2070 7265 436f 6d70 7574  .      preComput
+00020bc0: 6564 5365 6e74 696e 656c 3243 6c6f 7564  edSentinel2Cloud
+00020bd0: 5363 6f72 654f 6666 7365 7420 3d20 4e6f  ScoreOffset = No
+00020be0: 6e65 2c0d 0a20 2020 2020 2070 7265 436f  ne,..      preCo
+00020bf0: 6d70 7574 6564 5365 6e74 696e 656c 3254  mputedSentinel2T
+00020c00: 444f 4d49 524d 6561 6e20 3d20 4e6f 6e65  DOMIRMean = None
+00020c10: 2c0d 0a20 2020 2020 2070 7265 436f 6d70  ,..      preComp
+00020c20: 7574 6564 5365 6e74 696e 656c 3254 444f  utedSentinel2TDO
+00020c30: 4d49 5253 7464 4465 7620 3d20 4e6f 6e65  MIRStdDev = None
+00020c40: 2c0d 0a20 2020 2020 2063 6c6f 7564 5072  ,..      cloudPr
+00020c50: 6f62 5468 7265 7368 203d 2034 302c 0d0a  obThresh = 40,..
+00020c60: 2020 2020 2020 6c61 6e64 7361 7443 6f6c        landsatCol
+00020c70: 6c65 6374 696f 6e56 6572 7369 6f6e 203d  lectionVersion =
+00020c80: 2027 4332 272c 0d0a 2020 2020 2020 7665   'C2',..      ve
+00020c90: 7262 6f73 6520 3d20 4661 6c73 6529 3a0d  rbose = False):.
+00020ca0: 0a0d 0a20 2069 6620 746f 614f 7253 5220  ...  if toaOrSR 
+00020cb0: 3d3d 2027 5352 273a 0d0a 2020 2020 7275  == 'SR':..    ru
+00020cc0: 6e43 6861 7374 6169 6e48 6172 6d6f 6e69  nChastainHarmoni
+00020cd0: 7a61 7469 6f6e 203d 2046 616c 7365 0d0a  zation = False..
+00020ce0: 0d0a 2020 6f72 6967 696e 203d 2027 4c61  ..  origin = 'La
+00020cf0: 6e64 7361 742d 5365 6e74 696e 656c 322d  ndsat-Sentinel2-
+00020d00: 4879 6272 6964 270d 0a20 2074 6f61 4f72  Hybrid'..  toaOr
+00020d10: 5352 203d 2074 6f61 4f72 5352 2e75 7070  SR = toaOrSR.upp
+00020d20: 6572 2829 0d0a 0d0a 2020 2350 7265 7061  er()....  #Prepa
+00020d30: 7265 2064 6174 6573 0d0a 2020 2357 7261  re dates..  #Wra
+00020d40: 7020 7468 6520 6461 7465 7320 6966 206e  p the dates if n
+00020d50: 6565 6465 640d 0a20 2077 7261 704f 6666  eeded..  wrapOff
+00020d60: 7365 7420 3d20 300d 0a20 2069 6620 7374  set = 0..  if st
+00020d70: 6172 744a 756c 6961 6e20 3e20 656e 644a  artJulian > endJ
+00020d80: 756c 6961 6e3a 0d0a 2020 2020 7772 6170  ulian:..    wrap
+00020d90: 4f66 6673 6574 203d 2033 3635 0d0a 2020  Offset = 365..  
+00020da0: 7374 6172 7444 6174 6520 3d20 6565 2e44  startDate = ee.D
+00020db0: 6174 652e 6672 6f6d 594d 4428 7374 6172  ate.fromYMD(star
+00020dc0: 7459 6561 722c 312c 3129 2e61 6476 616e  tYear,1,1).advan
+00020dd0: 6365 2873 7461 7274 4a75 6c69 616e 2d31  ce(startJulian-1
+00020de0: 2c27 6461 7927 290d 0a20 2065 6e64 4461  ,'day')..  endDa
+00020df0: 7465 203d 2065 652e 4461 7465 2e66 726f  te = ee.Date.fro
+00020e00: 6d59 4d44 2865 6e64 5965 6172 2c31 2c31  mYMD(endYear,1,1
+00020e10: 292e 6164 7661 6e63 6528 656e 644a 756c  ).advance(endJul
+00020e20: 6961 6e2d 312b 7772 6170 4f66 6673 6574  ian-1+wrapOffset
+00020e30: 2c27 6461 7927 290d 0a0d 0a20 2061 7267  ,'day')....  arg
+00020e40: 7320 3d20 666f 726d 6174 4172 6773 286c  s = formatArgs(l
+00020e50: 6f63 616c 7328 2929 0d0a 2020 6966 2027  ocals())..  if '
+00020e60: 6172 6773 2720 696e 2061 7267 732e 6b65  args' in args.ke
+00020e70: 7973 2829 3a0d 0a20 2020 2064 656c 2061  ys():..    del a
+00020e80: 7267 735b 2761 7267 7327 5d0d 0a0d 0a20  rgs['args'].... 
+00020e90: 2070 7269 6e74 2827 4765 7420 5072 6f63   print('Get Proc
+00020ea0: 6573 7365 6420 4c61 6e64 7361 7420 616e  essed Landsat an
+00020eb0: 6420 5365 6e74 696e 656c 3220 5363 656e  d Sentinel2 Scen
+00020ec0: 6573 3a20 2729 0d0a 2020 7072 696e 7428  es: ')..  print(
+00020ed0: 2753 7461 7274 2064 6174 653a 272c 2073  'Start date:', s
+00020ee0: 7461 7274 4461 7465 2e66 6f72 6d61 7428  tartDate.format(
+00020ef0: 274d 4d4d 2064 6420 7979 7979 2729 2e67  'MMM dd yyyy').g
+00020f00: 6574 496e 666f 2829 2c27 2c20 456e 6420  etInfo(),', End 
+00020f10: 6461 7465 3a27 2c20 656e 6444 6174 652e  date:', endDate.
+00020f20: 666f 726d 6174 2827 4d4d 4d20 6464 2079  format('MMM dd y
+00020f30: 7979 7927 292e 6765 7449 6e66 6f28 2929  yyy').getInfo())
+00020f40: 0d0a 2020 6966 2076 6572 626f 7365 3a0d  ..  if verbose:.
+00020f50: 0a20 2020 2066 6f72 2061 7267 2069 6e20  .    for arg in 
+00020f60: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
+00020f70: 2020 2020 7072 696e 7428 6172 672c 2027      print(arg, '
+00020f80: 3a20 272c 2061 7267 735b 6172 675d 290d  : ', args[arg]).
+00020f90: 0a0d 0a20 2023 4765 7420 4c61 6e64 7361  ...  #Get Landsa
+00020fa0: 740d 0a20 206c 7320 3d20 6765 7450 726f  t..  ls = getPro
+00020fb0: 6365 7373 6564 4c61 6e64 7361 7453 6365  cessedLandsatSce
+00020fc0: 6e65 7328 5c0d 0a20 2020 2073 7475 6479  nes(\..    study
+00020fd0: 4172 6561 203d 2073 7475 6479 4172 6561  Area = studyArea
+00020fe0: 2c0d 0a20 2020 2073 7461 7274 5965 6172  ,..    startYear
+00020ff0: 203d 2073 7461 7274 5965 6172 2c0d 0a20   = startYear,.. 
+00021000: 2020 2065 6e64 5965 6172 203d 2065 6e64     endYear = end
+00021010: 5965 6172 2c0d 0a20 2020 2073 7461 7274  Year,..    start
+00021020: 4a75 6c69 616e 203d 2073 7461 7274 4a75  Julian = startJu
+00021030: 6c69 616e 2c0d 0a20 2020 2065 6e64 4a75  lian,..    endJu
+00021040: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
+00021050: 2c0d 0a20 2020 2074 6f61 4f72 5352 203d  ,..    toaOrSR =
+00021060: 2074 6f61 4f72 5352 2c0d 0a20 2020 2069   toaOrSR,..    i
+00021070: 6e63 6c75 6465 534c 434f 6666 4c37 203d  ncludeSLCOffL7 =
+00021080: 2069 6e63 6c75 6465 534c 434f 6666 4c37   includeSLCOffL7
+00021090: 2c0d 0a20 2020 2064 6566 7269 6e67 654c  ,..    defringeL
+000210a0: 3520 3d20 6465 6672 696e 6765 4c35 2c0d  5 = defringeL5,.
+000210b0: 0a20 2020 2061 7070 6c79 436c 6f75 6453  .    applyCloudS
+000210c0: 636f 7265 203d 2061 7070 6c79 436c 6f75  core = applyClou
+000210d0: 6453 636f 7265 4c61 6e64 7361 742c 0d0a  dScoreLandsat,..
+000210e0: 2020 2020 6170 706c 7946 6d61 736b 436c      applyFmaskCl
+000210f0: 6f75 644d 6173 6b20 3d20 6170 706c 7946  oudMask = applyF
+00021100: 6d61 736b 436c 6f75 644d 6173 6b2c 0d0a  maskCloudMask,..
+00021110: 2020 2020 6170 706c 7954 444f 4d20 3d20      applyTDOM = 
+00021120: 6170 706c 7954 444f 4d4c 616e 6473 6174  applyTDOMLandsat
+00021130: 2c0d 0a20 2020 2061 7070 6c79 466d 6173  ,..    applyFmas
+00021140: 6b43 6c6f 7564 5368 6164 6f77 4d61 736b  kCloudShadowMask
+00021150: 203d 2061 7070 6c79 466d 6173 6b43 6c6f   = applyFmaskClo
+00021160: 7564 5368 6164 6f77 4d61 736b 2c0d 0a20  udShadowMask,.. 
+00021170: 2020 2061 7070 6c79 466d 6173 6b53 6e6f     applyFmaskSno
+00021180: 774d 6173 6b20 3d20 6170 706c 7946 6d61  wMask = applyFma
+00021190: 736b 536e 6f77 4d61 736b 2c0d 0a20 2020  skSnowMask,..   
+000211a0: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
+000211b0: 6820 3d20 636c 6f75 6453 636f 7265 5468  h = cloudScoreTh
+000211c0: 7265 7368 2c0d 0a20 2020 2070 6572 666f  resh,..    perfo
+000211d0: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
+000211e0: 6574 203d 2070 6572 666f 726d 436c 6f75  et = performClou
+000211f0: 6453 636f 7265 4f66 6673 6574 2c0d 0a20  dScoreOffset,.. 
+00021200: 2020 2063 6c6f 7564 5363 6f72 6550 6374     cloudScorePct
+00021210: 6c20 3d20 636c 6f75 6453 636f 7265 5063  l = cloudScorePc
+00021220: 746c 2c0d 0a20 2020 207a 5363 6f72 6554  tl,..    zScoreT
+00021230: 6872 6573 6820 3d20 7a53 636f 7265 5468  hresh = zScoreTh
+00021240: 7265 7368 2c0d 0a20 2020 2073 6861 646f  resh,..    shado
+00021250: 7753 756d 5468 7265 7368 203d 2073 6861  wSumThresh = sha
+00021260: 646f 7753 756d 5468 7265 7368 2c0d 0a20  dowSumThresh,.. 
+00021270: 2020 2063 6f6e 7472 6163 7450 6978 656c     contractPixel
+00021280: 7320 3d20 636f 6e74 7261 6374 5069 7865  s = contractPixe
+00021290: 6c73 2c0d 0a20 2020 2064 696c 6174 6550  ls,..    dilateP
+000212a0: 6978 656c 7320 3d20 6469 6c61 7465 5069  ixels = dilatePi
+000212b0: 7865 6c73 2c0d 0a20 2020 2073 6861 646f  xels,..    shado
+000212c0: 7753 756d 4261 6e64 7320 3d20 7368 6164  wSumBands = shad
+000212d0: 6f77 5375 6d42 616e 6473 2c0d 0a20 2020  owSumBands,..   
+000212e0: 2072 6573 616d 706c 654d 6574 686f 6420   resampleMethod 
+000212f0: 3d20 6c61 6e64 7361 7452 6573 616d 706c  = landsatResampl
+00021300: 654d 6574 686f 642c 0d0a 2020 2020 2368  eMethod,..    #h
+00021310: 6172 6d6f 6e69 7a65 4f4c 4920 3d20 6861  armonizeOLI = ha
+00021320: 726d 6f6e 697a 654f 4c49 2c0d 0a20 2020  rmonizeOLI,..   
+00021330: 2070 7265 436f 6d70 7574 6564 436c 6f75   preComputedClou
+00021340: 6453 636f 7265 4f66 6673 6574 203d 2070  dScoreOffset = p
+00021350: 7265 436f 6d70 7574 6564 4c61 6e64 7361  reComputedLandsa
+00021360: 7443 6c6f 7564 5363 6f72 654f 6666 7365  tCloudScoreOffse
+00021370: 742c 0d0a 2020 2020 7072 6543 6f6d 7075  t,..    preCompu
+00021380: 7465 6454 444f 4d49 524d 6561 6e20 3d20  tedTDOMIRMean = 
+00021390: 7072 6543 6f6d 7075 7465 644c 616e 6473  preComputedLands
+000213a0: 6174 5444 4f4d 4952 4d65 616e 2c0d 0a20  atTDOMIRMean,.. 
+000213b0: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
+000213c0: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
+000213d0: 436f 6d70 7574 6564 5365 6e74 696e 656c  ComputedSentinel
+000213e0: 3254 444f 4d49 5253 7464 4465 762c 0d0a  2TDOMIRStdDev,..
+000213f0: 2020 2020 6c61 6e64 7361 7443 6f6c 6c65      landsatColle
+00021400: 6374 696f 6e56 6572 7369 6f6e 203d 206c  ctionVersion = l
+00021410: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
+00021420: 5665 7273 696f 6e2c 0d0a 2020 2020 7665  Version,..    ve
+00021430: 7262 6f73 6520 3d20 4661 6c73 6529 0d0a  rbose = False)..
+00021440: 0d0a 2020 2347 6574 2053 656e 7469 6e65  ..  #Get Sentine
+00021450: 6c20 320d 0a20 2073 3273 203d 2067 6574  l 2..  s2s = get
+00021460: 5072 6f63 6573 7365 6453 656e 7469 6e65  ProcessedSentine
+00021470: 6c32 5363 656e 6573 285c 0d0a 2020 2020  l2Scenes(\..    
+00021480: 7374 7564 7941 7265 6120 3d20 7374 7564  studyArea = stud
+00021490: 7941 7265 612c 0d0a 2020 2020 7374 6172  yArea,..    star
+000214a0: 7459 6561 7220 3d20 7374 6172 7459 6561  tYear = startYea
+000214b0: 722c 0d0a 2020 2020 656e 6459 6561 7220  r,..    endYear 
+000214c0: 3d20 656e 6459 6561 722c 0d0a 2020 2020  = endYear,..    
+000214d0: 7374 6172 744a 756c 6961 6e20 3d20 7374  startJulian = st
+000214e0: 6172 744a 756c 6961 6e2c 0d0a 2020 2020  artJulian,..    
+000214f0: 656e 644a 756c 6961 6e20 3d20 656e 644a  endJulian = endJ
+00021500: 756c 6961 6e2c 0d0a 2020 2020 6170 706c  ulian,..    appl
+00021510: 7951 4142 616e 6420 3d20 6170 706c 7951  yQABand = applyQ
+00021520: 4142 616e 642c 0d0a 2020 2020 6170 706c  ABand,..    appl
+00021530: 7943 6c6f 7564 5363 6f72 6520 3d20 6170  yCloudScore = ap
+00021540: 706c 7943 6c6f 7564 5363 6f72 6553 656e  plyCloudScoreSen
+00021550: 7469 6e65 6c32 2c0d 0a20 2020 2061 7070  tinel2,..    app
+00021560: 6c79 5368 6164 6f77 5368 6966 7420 3d20  lyShadowShift = 
+00021570: 6170 706c 7953 6861 646f 7753 6869 6674  applyShadowShift
+00021580: 2c0d 0a20 2020 2061 7070 6c79 5444 4f4d  ,..    applyTDOM
+00021590: 203d 2061 7070 6c79 5444 4f4d 5365 6e74   = applyTDOMSent
+000215a0: 696e 656c 322c 0d0a 2020 2020 636c 6f75  inel2,..    clou
+000215b0: 6453 636f 7265 5468 7265 7368 203d 2063  dScoreThresh = c
+000215c0: 6c6f 7564 5363 6f72 6554 6872 6573 682c  loudScoreThresh,
+000215d0: 0d0a 2020 2020 7065 7266 6f72 6d43 6c6f  ..    performClo
+000215e0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+000215f0: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
+00021600: 654f 6666 7365 742c 0d0a 2020 2020 636c  eOffset,..    cl
+00021610: 6f75 6453 636f 7265 5063 746c 203d 2063  oudScorePctl = c
+00021620: 6c6f 7564 5363 6f72 6550 6374 6c2c 0d0a  loudScorePctl,..
+00021630: 2020 2020 636c 6f75 6448 6569 6768 7473      cloudHeights
+00021640: 203d 2063 6c6f 7564 4865 6967 6874 732c   = cloudHeights,
+00021650: 0d0a 2020 2020 7a53 636f 7265 5468 7265  ..    zScoreThre
+00021660: 7368 203d 207a 5363 6f72 6554 6872 6573  sh = zScoreThres
+00021670: 682c 0d0a 2020 2020 7368 6164 6f77 5375  h,..    shadowSu
+00021680: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
+00021690: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
+000216a0: 636f 6e74 7261 6374 5069 7865 6c73 203d  contractPixels =
+000216b0: 2063 6f6e 7472 6163 7450 6978 656c 732c   contractPixels,
+000216c0: 0d0a 2020 2020 6469 6c61 7465 5069 7865  ..    dilatePixe
+000216d0: 6c73 203d 2064 696c 6174 6550 6978 656c  ls = dilatePixel
+000216e0: 732c 0d0a 2020 2020 7368 6164 6f77 5375  s,..    shadowSu
+000216f0: 6d42 616e 6473 203d 2073 6861 646f 7753  mBands = shadowS
+00021700: 756d 4261 6e64 732c 0d0a 2020 2020 7265  umBands,..    re
+00021710: 7361 6d70 6c65 4d65 7468 6f64 203d 2073  sampleMethod = s
+00021720: 656e 7469 6e65 6c32 5265 7361 6d70 6c65  entinel2Resample
+00021730: 4d65 7468 6f64 2c0d 0a20 2020 2074 6f61  Method,..    toa
+00021740: 4f72 5352 203d 2074 6f61 4f72 5352 2c0d  OrSR = toaOrSR,.
+00021750: 0a20 2020 2063 6f6e 7665 7274 546f 4461  .    convertToDa
+00021760: 696c 794d 6f73 6169 6373 203d 2063 6f6e  ilyMosaics = con
+00021770: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
+00021780: 6373 2c0d 0a20 2020 2061 7070 6c79 436c  cs,..    applyCl
+00021790: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
+000217a0: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
+000217b0: 6269 6c69 7479 2c0d 0a20 2020 2070 7265  bility,..    pre
+000217c0: 436f 6d70 7574 6564 436c 6f75 6453 636f  ComputedCloudSco
+000217d0: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
+000217e0: 6d70 7574 6564 5365 6e74 696e 656c 3243  mputedSentinel2C
+000217f0: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+00021800: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
+00021810: 6454 444f 4d49 524d 6561 6e20 3d20 7072  dTDOMIRMean = pr
+00021820: 6543 6f6d 7075 7465 6453 656e 7469 6e65  eComputedSentine
+00021830: 6c32 5444 4f4d 4952 4d65 616e 2c0d 0a20  l2TDOMIRMean,.. 
+00021840: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
+00021850: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
+00021860: 436f 6d70 7574 6564 5365 6e74 696e 656c  ComputedSentinel
+00021870: 3254 444f 4d49 5253 7464 4465 762c 0d0a  2TDOMIRStdDev,..
+00021880: 2020 2020 636c 6f75 6450 726f 6254 6872      cloudProbThr
+00021890: 6573 6820 3d20 636c 6f75 6450 726f 6254  esh = cloudProbT
+000218a0: 6872 6573 682c 0d0a 2020 2020 7665 7262  hresh,..    verb
+000218b0: 6f73 6520 3d20 4661 6c73 6529 0d0a 0d0a  ose = False)....
+000218c0: 0d0a 2020 2353 656c 6563 7420 6f66 6620  ..  #Select off 
+000218d0: 636f 6d6d 6f6e 2062 616e 6473 2062 6574  common bands bet
+000218e0: 7765 656e 204c 616e 6473 6174 2061 6e64  ween Landsat and
+000218f0: 2053 656e 7469 6e65 6c20 320d 0a20 2063   Sentinel 2..  c
+00021900: 6f6d 6d6f 6e42 616e 6473 203d 2020 5b27  ommonBands =  ['
+00021910: 626c 7565 272c 2027 6772 6565 6e27 2c20  blue', 'green', 
+00021920: 2772 6564 272c 2027 6e69 7227 2c20 2773  'red', 'nir', 's
+00021930: 7769 7231 272c 2027 7377 6972 3227 2c20  wir1', 'swir2', 
+00021940: 2773 656e 736f 7227 5d0d 0a20 206c 7320  'sensor']..  ls 
+00021950: 3d20 6c73 2e73 656c 6563 7428 636f 6d6d  = ls.select(comm
+00021960: 6f6e 4261 6e64 7329 0d0a 2020 7332 7320  onBands)..  s2s 
+00021970: 3d20 7332 732e 7365 6c65 6374 2863 6f6d  = s2s.select(com
+00021980: 6d6f 6e42 616e 6473 290d 0a20 2023 4669  monBands)..  #Fi
+00021990: 6c6c 2069 6e20 616e 7920 656d 7074 7920  ll in any empty 
+000219a0: 636f 6c6c 6563 7469 6f6e 730d 0a20 2023  collections..  #
+000219b0: 4966 2074 6865 7927 7265 2062 6f74 6820  If they're both 
+000219c0: 656d 7074 792c 2074 6869 7320 7769 6c6c  empty, this will
+000219d0: 206e 6f74 2077 6f72 6b0d 0a20 2064 756d   not work..  dum
+000219e0: 6d79 496d 6167 6520 3d65 652e 496d 6167  myImage =ee.Imag
+000219f0: 6528 6565 2e49 6d61 6765 436f 6c6c 6563  e(ee.ImageCollec
+00021a00: 7469 6f6e 2865 652e 416c 676f 7269 7468  tion(ee.Algorith
+00021a10: 6d73 2e49 6628 6c73 2e74 6f4c 6973 7428  ms.If(ls.toList(
+00021a20: 3129 2e6c 656e 6774 6828 292e 6774 2830  1).length().gt(0
+00021a30: 292c 6c73 2c73 3273 2929 2e66 6972 7374  ),ls,s2s)).first
+00021a40: 2829 290d 0a20 206c 7320 3d20 6669 6c6c  ())..  ls = fill
+00021a50: 456d 7074 7943 6f6c 6c65 6374 696f 6e73  EmptyCollections
+00021a60: 286c 732c 6475 6d6d 7949 6d61 6765 290d  (ls,dummyImage).
+00021a70: 0a20 2073 3273 203d 2066 696c 6c45 6d70  .  s2s = fillEmp
+00021a80: 7479 436f 6c6c 6563 7469 6f6e 7328 7332  tyCollections(s2
+00021a90: 732c 6475 6d6d 7949 6d61 6765 290d 0a0d  s,dummyImage)...
+00021aa0: 0a0d 0a20 2069 6620 7275 6e43 6861 7374  ...  if runChast
+00021ab0: 6169 6e48 6172 6d6f 6e69 7a61 7469 6f6e  ainHarmonization
+00021ac0: 2061 6e64 2074 6f61 4f72 5352 203d 3d20   and toaOrSR == 
+00021ad0: 2754 4f41 273a 0d0a 0d0a 2020 2020 2320  'TOA':....    # 
+00021ae0: 5365 7061 7261 7465 2065 6163 6820 7365  Separate each se
+00021af0: 6e73 6f72 0d0a 0d0a 2020 2020 746d 203d  nsor....    tm =
+00021b00: 206c 732e 6669 6c74 6572 2865 652e 4669   ls.filter(ee.Fi
+00021b10: 6c74 6572 2e69 6e4c 6973 7428 2753 454e  lter.inList('SEN
+00021b20: 534f 525f 4944 272c 5b27 544d 272c 2745  SOR_ID',['TM','E
+00021b30: 544d 275d 2929 0d0a 2020 2020 6f6c 6920  TM']))..    oli 
+00021b40: 3d20 6c73 2e66 696c 7465 7228 6565 2e46  = ls.filter(ee.F
+00021b50: 696c 7465 722e 6571 2827 5345 4e53 4f52  ilter.eq('SENSOR
+00021b60: 5f49 4427 2c27 4f4c 495f 5449 5253 2729  _ID','OLI_TIRS')
+00021b70: 290d 0a20 2020 2023 2065 6c73 653a 0d0a  )..    # else:..
+00021b80: 2020 2020 2320 2020 746d 203d 206c 732e      #   tm = ls.
+00021b90: 6669 6c74 6572 2865 652e 4669 6c74 6572  filter(ee.Filter
+00021ba0: 2e69 6e4c 6973 7428 2773 656e 736f 7227  .inList('sensor'
+00021bb0: 2c5b 274c 414e 4453 4154 5f34 272c 274c  ,['LANDSAT_4','L
+00021bc0: 414e 4453 4154 5f35 272c 274c 414e 4453  ANDSAT_5','LANDS
+00021bd0: 4154 5f37 275d 2929 0d0a 2020 2020 2320  AT_7']))..    # 
+00021be0: 2020 6f6c 6920 3d20 6c73 2e66 696c 7465    oli = ls.filte
+00021bf0: 7228 6565 2e46 696c 7465 722e 6571 2827  r(ee.Filter.eq('
+00021c00: 7365 6e73 6f72 272c 274c 414e 4453 4154  sensor','LANDSAT
+00021c10: 5f38 2729 290d 0a20 2020 206d 7369 203d  _8'))..    msi =
+00021c20: 2073 3273 0d0a 0d0a 2020 2020 2320 4669   s2s....    # Fi
+00021c30: 6c6c 2069 6620 6e6f 2069 6d61 6765 7320  ll if no images 
+00021c40: 6578 6973 7420 666f 7220 7061 7274 6963  exist for partic
+00021c50: 756c 6172 204c 616e 6473 6174 2073 656e  ular Landsat sen
+00021c60: 736f 720d 0a20 2020 2023 2041 6c6c 6f77  sor..    # Allow
+00021c70: 2069 7420 746f 2066 6169 6c20 6f66 206e   it to fail of n
+00021c80: 6f20 696d 6167 6573 2065 7869 7374 2066  o images exist f
+00021c90: 6f72 2053 656e 7469 6e65 6c20 3220 7369  or Sentinel 2 si
+00021ca0: 6e63 6520 7468 6520 706f 696e 740d 0a20  nce the point.. 
+00021cb0: 2020 2023 206f 6620 7468 6973 206d 6574     # of this met
+00021cc0: 686f 6420 6973 2074 6f20 696e 636c 7564  hod is to includ
+00021cd0: 6520 5332 0d0a 2020 2020 746d 203d 2066  e S2..    tm = f
+00021ce0: 696c 6c45 6d70 7479 436f 6c6c 6563 7469  illEmptyCollecti
+00021cf0: 6f6e 7328 746d 2c20 6565 2e49 6d61 6765  ons(tm, ee.Image
+00021d00: 286c 732e 6669 7273 7428 2929 290d 0a20  (ls.first())).. 
+00021d10: 2020 206f 6c69 203d 2066 696c 6c45 6d70     oli = fillEmp
+00021d20: 7479 436f 6c6c 6563 7469 6f6e 7328 6f6c  tyCollections(ol
+00021d30: 692c 2065 652e 496d 6167 6528 6c73 2e66  i, ee.Image(ls.f
+00021d40: 6972 7374 2829 2929 0d0a 0d0a 2020 2020  irst()))....    
+00021d50: 7072 696e 7428 2752 756e 6e69 6e67 2043  print('Running C
+00021d60: 6861 7374 6169 6e20 6574 2061 6c20 3230  hastain et al 20
+00021d70: 3139 2068 6172 6d6f 6e69 7a61 7469 6f6e  19 harmonization
+00021d80: 2729 0d0a 0d0a 2020 2020 2341 7070 6c79  ')....    #Apply
+00021d90: 2063 6f72 7265 6374 696f 6e0d 0a20 2020   correction..   
+00021da0: 2023 4375 7272 656e 746c 7920 636f 6465   #Currently code
+00021db0: 6420 746f 2067 6f20 746f 2045 544d 2b0d  d to go to ETM+.
+00021dc0: 0a0d 0a20 2020 2023 4e6f 206e 6565 6420  ...    #No need 
+00021dd0: 746f 2063 6f72 7265 6374 2045 544d 2074  to correct ETM t
+00021de0: 6f20 4554 4d0d 0a20 2020 2023 2074 6d20  o ETM..    # tm 
+00021df0: 3d20 746d 2e6d 6170 2866 756e 6374 696f  = tm.map(functio
+00021e00: 6e28 696d 6729 7b72 6574 7572 6e20 6765  n(img){return ge
+00021e10: 7449 6d61 6765 734c 6962 2e68 6172 6d6f  tImagesLib.harmo
+00021e20: 6e69 7a61 7469 6f6e 4368 6173 7461 696e  nizationChastain
+00021e30: 2869 6d67 2c20 2745 544d 272c 2745 544d  (img, 'ETM','ETM
+00021e40: 2729 7d29 0d0a 2020 2020 2320 6574 6d20  ')})..    # etm 
+00021e50: 3d20 6574 6d2e 6d61 7028 6675 6e63 7469  = etm.map(functi
+00021e60: 6f6e 2869 6d67 297b 7265 7475 726e 2067  on(img){return g
+00021e70: 6574 496d 6167 6573 4c69 622e 6861 726d  etImagesLib.harm
+00021e80: 6f6e 697a 6174 696f 6e43 6861 7374 6169  onizationChastai
+00021e90: 6e28 696d 672c 2027 4554 4d27 2c27 4554  n(img, 'ETM','ET
+00021ea0: 4d27 297d 290d 0a0d 0a20 2020 2023 4861  M')})....    #Ha
+00021eb0: 726d 6f6e 697a 6520 7468 6520 6f74 6865  rmonize the othe
+00021ec0: 7220 7477 6f0d 0a20 2020 206f 6c69 203d  r two..    oli =
+00021ed0: 206f 6c69 2e6d 6170 286c 616d 6264 6120   oli.map(lambda 
+00021ee0: 696d 673a 2068 6172 6d6f 6e69 7a61 7469  img: harmonizati
+00021ef0: 6f6e 4368 6173 7461 696e 2869 6d67 2c20  onChastain(img, 
+00021f00: 274f 4c49 272c 2745 544d 2729 290d 0a20  'OLI','ETM')).. 
+00021f10: 2020 206d 7369 203d 206d 7369 2e6d 6170     msi = msi.map
+00021f20: 286c 616d 6264 6120 696d 673a 2068 6172  (lambda img: har
+00021f30: 6d6f 6e69 7a61 7469 6f6e 4368 6173 7461  monizationChasta
+00021f40: 696e 2869 6d67 2c20 274d 5349 272c 2745  in(img, 'MSI','E
+00021f50: 544d 2729 290d 0a0d 0a20 2020 2073 3273  TM'))....    s2s
+00021f60: 203d 206d 7369 0d0a 0d0a 2020 2020 234d   = msi....    #M
+00021f70: 6572 6765 204c 616e 6473 6174 2062 6163  erge Landsat bac
+00021f80: 6b20 746f 6765 7468 6572 0d0a 2020 2020  k together..    
+00021f90: 6c73 203d 2065 652e 496d 6167 6543 6f6c  ls = ee.ImageCol
+00021fa0: 6c65 6374 696f 6e28 746d 2e6d 6572 6765  lection(tm.merge
+00021fb0: 286f 6c69 2929 0d0a 0d0a 0d0a 2020 2320  (oli))......  # 
+00021fc0: 4d65 7267 6520 4c61 6e64 7361 7420 616e  Merge Landsat an
+00021fd0: 6420 5332 0d0a 2020 6d65 7267 6564 203d  d S2..  merged =
+00021fe0: 2065 652e 496d 6167 6543 6f6c 6c65 6374   ee.ImageCollect
+00021ff0: 696f 6e28 6c73 2e6d 6572 6765 2873 3273  ion(ls.merge(s2s
+00022000: 2929 0d0a 2020 6d65 7267 6564 203d 206d  ))..  merged = m
+00022010: 6572 6765 642e 6d61 7028 7369 6d70 6c65  erged.map(simple
+00022020: 4164 6449 6e64 6963 6573 295c 0d0a 2020  AddIndices)\..  
+00022030: 2020 2020 2020 2020 2020 2e6d 6170 2867            .map(g
+00022040: 6574 5461 7373 656c 6564 4361 7029 5c0d  etTasseledCap)\.
+00022050: 0a20 2020 2020 2020 2020 2020 202e 6d61  .            .ma
+00022060: 7028 7369 6d70 6c65 4164 6454 4341 6e67  p(simpleAddTCAng
+00022070: 6c65 7329 0d0a 0d0a 2020 6d65 7267 6564  les)....  merged
+00022080: 203d 206d 6572 6765 642e 7365 7428 6172   = merged.set(ar
+00022090: 6773 290d 0a0d 0a0d 0a20 2072 6574 7572  gs)......  retur
+000220a0: 6e20 6d65 7267 6564 0d0a 2323 2323 2323  n merged..######
+000220b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000220c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000220d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000220e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000220f0: 2323 2323 2323 2323 2323 230d 0a23 4675  ###########..#Fu
+00022100: 6e63 7469 6f6e 2074 6f20 7265 6769 7374  nction to regist
+00022110: 6572 2061 6e20 696d 6167 6543 6f6c 6c65  er an imageColle
+00022120: 6374 696f 6e20 746f 2069 6d61 6765 7320  ction to images 
+00022130: 7769 7468 696e 2069 740d 0a23 416c 7761  within it..#Alwa
+00022140: 7973 2075 7365 7320 7468 6520 6669 7273  ys uses the firs
+00022150: 7420 696d 6167 6520 6173 2074 6865 2072  t image as the r
+00022160: 6566 6572 656e 6365 2069 6d61 6765 0d0a  eference image..
+00022170: 6465 6620 636f 5265 6769 7374 6572 436f  def coRegisterCo
+00022180: 6c6c 6563 7469 6f6e 2869 6d61 6765 732c  llection(images,
+00022190: 7265 6665 7265 6e63 6542 616e 6473 203d  referenceBands =
+000221a0: 205b 276e 6972 275d 293a 0d0a 2020 2020   ['nir']):..    
+000221b0: 7265 6665 7265 6e63 6549 6d61 6765 496e  referenceImageIn
+000221c0: 6465 7820 3d20 300d 0a20 2020 2072 6566  dex = 0..    ref
+000221d0: 6572 656e 6365 496d 6167 6520 3d20 6565  erenceImage = ee
+000221e0: 2e49 6d61 6765 2869 6d61 6765 732e 746f  .Image(images.to
+000221f0: 4c69 7374 2872 6566 6572 656e 6365 496d  List(referenceIm
+00022200: 6167 6549 6e64 6578 2b31 292e 6765 7428  ageIndex+1).get(
+00022210: 7265 6665 7265 6e63 6549 6d61 6765 496e  referenceImageIn
+00022220: 6465 7829 292e 7365 6c65 6374 2872 6566  dex)).select(ref
+00022230: 6572 656e 6365 4261 6e64 7329 0d0a 0d0a  erenceBands)....
+00022240: 2020 2020 6465 6620 7265 6769 7374 6572      def register
+00022250: 496d 6167 6528 696d 6167 6529 3a0d 0a20  Image(image):.. 
+00022260: 2020 2020 2020 2023 4465 7465 726d 696e         #Determin
+00022270: 6520 7468 6520 6469 7370 6c61 6365 6d65  e the displaceme
+00022280: 6e74 2062 7920 6d61 7463 6869 6e67 206f  nt by matching o
+00022290: 6e6c 7920 7468 6520 7265 6665 7265 6e63  nly the referenc
+000222a0: 6542 616e 6420 6261 6e64 732e 0d0a 2020  eBand bands...  
+000222b0: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
+000222c0: 6e74 5f70 6172 616d 7320 3d20 7b0d 0a20  nt_params = {.. 
+000222d0: 2020 2020 2020 2020 2020 2027 7265 6665             'refe
+000222e0: 7265 6e63 6549 6d61 6765 273a 2072 6566  renceImage': ref
+000222f0: 6572 656e 6365 496d 6167 652c 0d0a 2020  erenceImage,..  
+00022300: 2020 2020 2020 2020 2020 276d 6178 4f66            'maxOf
+00022310: 6673 6574 273a 2032 302e 302c 0d0a 2020  fset': 20.0,..  
+00022320: 2020 2020 2020 2020 2020 2770 726f 6a65            'proje
+00022330: 6374 696f 6e27 3a20 4e6f 6e65 2c0d 0a20  ction': None,.. 
+00022340: 2020 2020 2020 2020 2020 2027 7061 7463             'patc
+00022350: 6857 6964 7468 273a 2032 302e 302c 0d0a  hWidth': 20.0,..
+00022360: 2020 2020 2020 2020 2020 2020 2773 7469              'sti
+00022370: 6666 6e65 7373 273a 2035 0d0a 2020 2020  ffness': 5..    
+00022380: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+00022390: 2020 2064 6973 706c 6163 656d 656e 7420     displacement 
+000223a0: 3d20 696d 6167 652e 7365 6c65 6374 2872  = image.select(r
+000223b0: 6566 6572 656e 6365 4261 6e64 7329 2e64  eferenceBands).d
+000223c0: 6973 706c 6163 656d 656e 7428 2a2a 6469  isplacement(**di
+000223d0: 7370 6c61 6365 6d65 6e74 5f70 6172 616d  splacement_param
+000223e0: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
+000223f0: 726e 2069 6d61 6765 2e64 6973 706c 6163  rn image.displac
+00022400: 6528 6469 7370 6c61 6365 6d65 6e74 290d  e(displacement).
+00022410: 0a0d 0a20 2020 206f 7574 203d 2065 652e  ...    out = ee.
+00022420: 496d 6167 6543 6f6c 6c65 6374 696f 6e28  ImageCollection(
+00022430: 6565 2e49 6d61 6765 436f 6c6c 6563 7469  ee.ImageCollecti
+00022440: 6f6e 2869 6d61 6765 732e 746f 4c69 7374  on(images.toList
+00022450: 2831 3030 3030 2c31 2929 2e6d 6170 2872  (10000,1)).map(r
+00022460: 6567 6973 7465 7249 6d61 6765 2929 2328  egisterImage))#(
+00022470: 6565 2e49 6d61 6765 2869 6d61 6765 732e  ee.Image(images.
+00022480: 746f 4c69 7374 2831 3030 3030 2c30 292e  toList(10000,0).
+00022490: 6765 7428 3129 292c 7265 6665 7265 6e63  get(1)),referenc
+000224a0: 6549 6d61 6765 290d 0a20 2020 206f 7574  eImage)..    out
+000224b0: 203d 2065 652e 496d 6167 6543 6f6c 6c65   = ee.ImageColle
+000224c0: 6374 696f 6e28 696d 6167 6573 2e6c 696d  ction(images.lim
+000224d0: 6974 2831 292e 6d65 7267 6528 6f75 7429  it(1).merge(out)
+000224e0: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
+000224f0: 6f75 740d 0a23 2323 2323 2323 2323 2323  out..###########
+00022500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022540: 2323 2323 2323 0d0a 2346 756e 6374 696f  ######..#Functio
+00022550: 6e20 746f 2066 696e 6420 6120 7375 6273  n to find a subs
+00022560: 6574 206f 6620 6120 636f 6c6c 6563 7469  et of a collecti
+00022570: 6f6e 0d0a 2346 6f72 2065 6163 6820 6772  on..#For each gr
+00022580: 6f75 7020 2865 2e67 2e20 7469 6c65 206f  oup (e.g. tile o
+00022590: 7220 6f72 6269 7420 6f72 2070 6174 6829  r orbit or path)
+000225a0: 2c20 616c 6c20 696d 6167 6573 2077 6974  , all images wit
+000225b0: 6869 6e20 7468 6174 2067 726f 7570 2077  hin that group w
+000225c0: 696c 6c20 6265 2072 6567 6973 7465 7265  ill be registere
+000225d0: 640d 0a23 4173 2073 696e 676c 6520 636f  d..#As single co
+000225e0: 6c6c 6563 7469 6f6e 2069 7320 7265 7475  llection is retu
+000225f0: 726e 6564 0d0a 6465 6620 636f 5265 6769  rned..def coRegi
+00022600: 7374 6572 4772 6f75 7073 2869 6d67 732c  sterGroups(imgs,
+00022610: 6669 656c 644e 616d 6520 3d20 2753 454e  fieldName = 'SEN
+00022620: 5349 4e47 5f4f 5242 4954 5f4e 554d 4245  SING_ORBIT_NUMBE
+00022630: 5227 2c66 6965 6c64 4973 4e75 6d65 7269  R',fieldIsNumeri
+00022640: 6320 3d20 5472 7565 293a 0d0a 2020 2020  c = True):..    
+00022650: 6772 6f75 7073 203d 2065 652e 4469 6374  groups = ee.Dict
+00022660: 696f 6e61 7279 2869 6d67 732e 6167 6772  ionary(imgs.aggr
+00022670: 6567 6174 655f 6869 7374 6f67 7261 6d28  egate_histogram(
+00022680: 6669 656c 644e 616d 6529 292e 6b65 7973  fieldName)).keys
+00022690: 2829 0d0a 2020 2020 6966 2066 6965 6c64  ()..    if field
+000226a0: 4973 4e75 6d65 7269 633a 0d0a 2020 2020  IsNumeric:..    
+000226b0: 2020 2020 6772 6f75 7073 203d 2067 726f      groups = gro
+000226c0: 7570 732e 6d61 7028 6c61 6d62 6461 206e  ups.map(lambda n
+000226d0: 3a20 6565 2e4e 756d 6265 722e 7061 7273  : ee.Number.pars
+000226e0: 6528 6e29 290d 0a0d 0a20 2020 206f 7574  e(n))....    out
+000226f0: 203d 6565 2e49 6d61 6765 436f 6c6c 6563   =ee.ImageCollec
+00022700: 7469 6f6e 2865 652e 4665 6174 7572 6543  tion(ee.FeatureC
+00022710: 6f6c 6c65 6374 696f 6e28 6772 6f75 7073  ollection(groups
+00022720: 2e6d 6170 286c 616d 6264 6120 6772 6f75  .map(lambda grou
+00022730: 703a 636f 5265 6769 7374 6572 436f 6c6c  p:coRegisterColl
+00022740: 6563 7469 6f6e 2869 6d67 732e 6669 6c74  ection(imgs.filt
+00022750: 6572 2865 652e 4669 6c74 6572 2e65 7128  er(ee.Filter.eq(
+00022760: 6669 656c 644e 616d 652c 6772 6f75 7029  fieldName,group)
+00022770: 2929 2929 2e66 6c61 7474 656e 2829 290d  )))).flatten()).
+00022780: 0a0d 0a20 2020 2072 6574 7572 6e20 6f75  ...    return ou
+00022790: 740d 0a23 2323 2323 2323 2323 2323 2323  t..#############
+000227a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000227b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000227c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000227d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000227e0: 2323 2323 0d0a 6465 6620 6765 744c 616e  ####..def getLan
+000227f0: 6473 6174 416e 6453 656e 7469 6e65 6c32  dsatAndSentinel2
+00022800: 4879 6272 6964 5772 6170 7065 7228 5c0d  HybridWrapper(\.
+00022810: 0a20 2073 7475 6479 4172 6561 2c0d 0a20  .  studyArea,.. 
+00022820: 2073 7461 7274 5965 6172 2c0d 0a20 2065   startYear,..  e
+00022830: 6e64 5965 6172 2c0d 0a20 2073 7461 7274  ndYear,..  start
+00022840: 4a75 6c69 616e 2c0d 0a20 2065 6e64 4a75  Julian,..  endJu
+00022850: 6c69 616e 2c0d 0a20 2074 696d 6562 7566  lian,..  timebuf
+00022860: 6665 7220 3d20 2030 2c0d 0a20 2077 6569  fer =  0,..  wei
+00022870: 6768 7473 203d 2020 5b31 5d2c 0d0a 2020  ghts =  [1],..  
+00022880: 636f 6d70 6f73 6974 696e 674d 6574 686f  compositingMetho
+00022890: 6420 3d20 276d 6564 6f69 6427 2c0d 0a20  d = 'medoid',.. 
+000228a0: 2074 6f61 4f72 5352 203d 2027 544f 4127   toaOrSR = 'TOA'
+000228b0: 2c0d 0a20 2069 6e63 6c75 6465 534c 434f  ,..  includeSLCO
+000228c0: 6666 4c37 203d 2046 616c 7365 2c0d 0a20  ffL7 = False,.. 
+000228d0: 2064 6566 7269 6e67 654c 3520 3d20 4661   defringeL5 = Fa
+000228e0: 6c73 652c 0d0a 2020 6170 706c 7951 4142  lse,..  applyQAB
+000228f0: 616e 6420 3d20 4661 6c73 652c 0d0a 2020  and = False,..  
+00022900: 6170 706c 7943 6c6f 7564 5072 6f62 6162  applyCloudProbab
+00022910: 696c 6974 7920 3d20 5472 7565 2c0d 0a20  ility = True,.. 
+00022920: 2061 7070 6c79 5368 6164 6f77 5368 6966   applyShadowShif
+00022930: 7420 3d20 4661 6c73 652c 0d0a 2020 6170  t = False,..  ap
+00022940: 706c 7943 6c6f 7564 5363 6f72 654c 616e  plyCloudScoreLan
+00022950: 6473 6174 203d 2046 616c 7365 2c0d 0a20  dsat = False,.. 
+00022960: 2061 7070 6c79 436c 6f75 6453 636f 7265   applyCloudScore
+00022970: 5365 6e74 696e 656c 3220 3d20 4661 6c73  Sentinel2 = Fals
+00022980: 652c 0d0a 2020 6170 706c 7954 444f 4d4c  e,..  applyTDOML
+00022990: 616e 6473 6174 203d 2054 7275 652c 0d0a  andsat = True,..
+000229a0: 2020 6170 706c 7954 444f 4d53 656e 7469    applyTDOMSenti
+000229b0: 6e65 6c32 203d 2054 7275 652c 0d0a 2020  nel2 = True,..  
+000229c0: 6170 706c 7946 6d61 736b 436c 6f75 644d  applyFmaskCloudM
+000229d0: 6173 6b20 3d20 5472 7565 2c0d 0a20 2061  ask = True,..  a
+000229e0: 7070 6c79 466d 6173 6b43 6c6f 7564 5368  pplyFmaskCloudSh
+000229f0: 6164 6f77 4d61 736b 203d 2054 7275 652c  adowMask = True,
+00022a00: 0d0a 2020 6170 706c 7946 6d61 736b 536e  ..  applyFmaskSn
+00022a10: 6f77 4d61 736b 203d 2046 616c 7365 2c0d  owMask = False,.
+00022a20: 0a20 2063 6c6f 7564 4865 6967 6874 7320  .  cloudHeights 
+00022a30: 3d20 6565 2e4c 6973 742e 7365 7175 656e  = ee.List.sequen
+00022a40: 6365 2835 3030 2c31 3030 3030 2c35 3030  ce(500,10000,500
+00022a50: 292c 0d0a 2020 636c 6f75 6453 636f 7265  ),..  cloudScore
+00022a60: 5468 7265 7368 203d 2032 302c 0d0a 2020  Thresh = 20,..  
+00022a70: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
+00022a80: 654f 6666 7365 7420 3d20 5472 7565 2c0d  eOffset = True,.
+00022a90: 0a20 2063 6c6f 7564 5363 6f72 6550 6374  .  cloudScorePct
+00022aa0: 6c20 3d20 3130 2c0d 0a20 207a 5363 6f72  l = 10,..  zScor
+00022ab0: 6554 6872 6573 6820 3d20 2d31 2c0d 0a20  eThresh = -1,.. 
+00022ac0: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
+00022ad0: 203d 2030 2e33 352c 0d0a 2020 636f 6e74   = 0.35,..  cont
+00022ae0: 7261 6374 5069 7865 6c73 203d 2031 2e35  ractPixels = 1.5
+00022af0: 2c0d 0a20 2064 696c 6174 6550 6978 656c  ,..  dilatePixel
+00022b00: 7320 3d20 332e 352c 0d0a 2020 7368 6164  s = 3.5,..  shad
+00022b10: 6f77 5375 6d42 616e 6473 203d 205b 276e  owSumBands = ['n
+00022b20: 6972 272c 2773 7769 7231 275d 2c0d 0a20  ir','swir1'],.. 
+00022b30: 206c 616e 6473 6174 5265 7361 6d70 6c65   landsatResample
+00022b40: 4d65 7468 6f64 203d 2027 6e65 6172 272c  Method = 'near',
+00022b50: 0d0a 2020 7365 6e74 696e 656c 3252 6573  ..  sentinel2Res
+00022b60: 616d 706c 654d 6574 686f 6420 3d20 2761  ampleMethod = 'a
+00022b70: 6767 7265 6761 7465 272c 0d0a 2020 636f  ggregate',..  co
+00022b80: 6e76 6572 7454 6f44 6169 6c79 4d6f 7361  nvertToDailyMosa
+00022b90: 6963 7320 3d20 5472 7565 2c0d 0a20 2072  ics = True,..  r
+00022ba0: 756e 4368 6173 7461 696e 4861 726d 6f6e  unChastainHarmon
+00022bb0: 697a 6174 696f 6e20 3d20 5472 7565 2c0d  ization = True,.
+00022bc0: 0a20 2063 6f72 7265 6374 496c 6c75 6d69  .  correctIllumi
+00022bd0: 6e61 7469 6f6e 203d 2046 616c 7365 2c0d  nation = False,.
+00022be0: 0a20 2063 6f72 7265 6374 5363 616c 6520  .  correctScale 
+00022bf0: 3d20 3235 302c 0d0a 2020 6578 706f 7274  = 250,..  export
+00022c00: 436f 6d70 6f73 6974 6573 203d 2046 616c  Composites = Fal
+00022c10: 7365 2c0d 0a20 206f 7574 7075 744e 616d  se,..  outputNam
+00022c20: 6520 3d20 274c 616e 6473 6174 2d53 656e  e = 'Landsat-Sen
+00022c30: 7469 6e65 6c32 2d48 7962 7269 6427 2c0d  tinel2-Hybrid',.
+00022c40: 0a20 2065 7870 6f72 7450 6174 6852 6f6f  .  exportPathRoo
+00022c50: 7420 3d20 4e6f 6e65 2c0d 0a20 2063 7273  t = None,..  crs
+00022c60: 203d 2027 4550 5347 3a35 3037 3027 2c0d   = 'EPSG:5070',.
+00022c70: 0a20 2074 7261 6e73 666f 726d 203d 205b  .  transform = [
+00022c80: 3330 2c30 2c2d 3233 3631 3931 352e 302c  30,0,-2361915.0,
+00022c90: 302c 2d33 302c 3331 3737 3733 352e 305d  0,-30,3177735.0]
+00022ca0: 2c0d 0a20 2073 6361 6c65 203d 204e 6f6e  ,..  scale = Non
+00022cb0: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
+00022cc0: 644c 616e 6473 6174 436c 6f75 6453 636f  dLandsatCloudSco
+00022cd0: 7265 4f66 6673 6574 203d 204e 6f6e 652c  reOffset = None,
+00022ce0: 0d0a 2020 7072 6543 6f6d 7075 7465 644c  ..  preComputedL
+00022cf0: 616e 6473 6174 5444 4f4d 4952 4d65 616e  andsatTDOMIRMean
+00022d00: 203d 204e 6f6e 652c 0d0a 2020 7072 6543   = None,..  preC
+00022d10: 6f6d 7075 7465 644c 616e 6473 6174 5444  omputedLandsatTD
+00022d20: 4f4d 4952 5374 6444 6576 203d 204e 6f6e  OMIRStdDev = Non
+00022d30: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
+00022d40: 6453 656e 7469 6e65 6c32 436c 6f75 6453  dSentinel2CloudS
+00022d50: 636f 7265 4f66 6673 6574 203d 204e 6f6e  coreOffset = Non
+00022d60: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
+00022d70: 6453 656e 7469 6e65 6c32 5444 4f4d 4952  dSentinel2TDOMIR
+00022d80: 4d65 616e 203d 204e 6f6e 652c 0d0a 2020  Mean = None,..  
+00022d90: 7072 6543 6f6d 7075 7465 6453 656e 7469  preComputedSenti
+00022da0: 6e65 6c32 5444 4f4d 4952 5374 6444 6576  nel2TDOMIRStdDev
+00022db0: 203d 204e 6f6e 652c 0d0a 2020 636c 6f75   = None,..  clou
+00022dc0: 6450 726f 6254 6872 6573 6820 3d20 3430  dProbThresh = 40
+00022dd0: 2c0d 0a20 206c 616e 6473 6174 436f 6c6c  ,..  landsatColl
+00022de0: 6563 7469 6f6e 5665 7273 696f 6e20 3d20  ectionVersion = 
+00022df0: 2743 3227 2c0d 0a20 206f 7665 7277 7269  'C2',..  overwri
+00022e00: 7465 203d 2046 616c 7365 2c0d 0a20 2076  te = False,..  v
+00022e10: 6572 626f 7365 203d 2046 616c 7365 293a  erbose = False):
+00022e20: 0d0a 0d0a 2020 6f72 6967 696e 203d 2027  ....  origin = '
+00022e30: 4c61 6e64 7361 742d 5365 6e74 696e 656c  Landsat-Sentinel
+00022e40: 322d 4879 6272 6964 270d 0a20 2074 6f61  2-Hybrid'..  toa
+00022e50: 4f72 5352 203d 2074 6f61 4f72 5352 2e75  OrSR = toaOrSR.u
+00022e60: 7070 6572 2829 0d0a 0d0a 2020 6172 6773  pper()....  args
+00022e70: 203d 2066 6f72 6d61 7441 7267 7328 6c6f   = formatArgs(lo
+00022e80: 6361 6c73 2829 290d 0a20 2069 6620 2761  cals())..  if 'a
+00022e90: 7267 7327 2069 6e20 6172 6773 2e6b 6579  rgs' in args.key
+00022ea0: 7328 293a 0d0a 2020 2020 6465 6c20 6172  s():..    del ar
+00022eb0: 6773 5b27 6172 6773 275d 0d0a 0d0a 2020  gs['args']....  
+00022ec0: 6d65 7267 6564 203d 2067 6574 5072 6f63  merged = getProc
+00022ed0: 6573 7365 644c 616e 6473 6174 416e 6453  essedLandsatAndS
+00022ee0: 656e 7469 6e65 6c32 5363 656e 6573 285c  entinel2Scenes(\
+00022ef0: 0d0a 2020 2020 7374 7564 7941 7265 6120  ..    studyArea 
+00022f00: 3d20 7374 7564 7941 7265 612c 0d0a 2020  = studyArea,..  
+00022f10: 2020 7374 6172 7459 6561 7220 3d20 7374    startYear = st
+00022f20: 6172 7459 6561 722c 0d0a 2020 2020 656e  artYear,..    en
+00022f30: 6459 6561 7220 3d20 656e 6459 6561 722c  dYear = endYear,
+00022f40: 0d0a 2020 2020 7374 6172 744a 756c 6961  ..    startJulia
+00022f50: 6e20 3d20 7374 6172 744a 756c 6961 6e2c  n = startJulian,
+00022f60: 0d0a 2020 2020 656e 644a 756c 6961 6e20  ..    endJulian 
+00022f70: 3d20 656e 644a 756c 6961 6e2c 0d0a 2020  = endJulian,..  
+00022f80: 2020 746f 614f 7253 5220 3d20 746f 614f    toaOrSR = toaO
+00022f90: 7253 522c 0d0a 2020 2020 696e 636c 7564  rSR,..    includ
+00022fa0: 6553 4c43 4f66 664c 3720 3d20 696e 636c  eSLCOffL7 = incl
+00022fb0: 7564 6553 4c43 4f66 664c 372c 0d0a 2020  udeSLCOffL7,..  
+00022fc0: 2020 6465 6672 696e 6765 4c35 203d 2064    defringeL5 = d
+00022fd0: 6566 7269 6e67 654c 352c 0d0a 2020 2020  efringeL5,..    
+00022fe0: 6170 706c 7951 4142 616e 6420 3d20 6170  applyQABand = ap
+00022ff0: 706c 7951 4142 616e 642c 0d0a 2020 2020  plyQABand,..    
+00023000: 6170 706c 7943 6c6f 7564 5072 6f62 6162  applyCloudProbab
+00023010: 696c 6974 7920 3d20 6170 706c 7943 6c6f  ility = applyClo
+00023020: 7564 5072 6f62 6162 696c 6974 792c 0d0a  udProbability,..
+00023030: 2020 2020 6170 706c 7953 6861 646f 7753      applyShadowS
+00023040: 6869 6674 203d 2061 7070 6c79 5368 6164  hift = applyShad
+00023050: 6f77 5368 6966 742c 0d0a 2020 2020 6170  owShift,..    ap
+00023060: 706c 7943 6c6f 7564 5363 6f72 654c 616e  plyCloudScoreLan
+00023070: 6473 6174 203d 2061 7070 6c79 436c 6f75  dsat = applyClou
+00023080: 6453 636f 7265 4c61 6e64 7361 742c 0d0a  dScoreLandsat,..
+00023090: 2020 2020 6170 706c 7943 6c6f 7564 5363      applyCloudSc
+000230a0: 6f72 6553 656e 7469 6e65 6c32 203d 2061  oreSentinel2 = a
+000230b0: 7070 6c79 436c 6f75 6453 636f 7265 5365  pplyCloudScoreSe
+000230c0: 6e74 696e 656c 322c 0d0a 2020 2020 6170  ntinel2,..    ap
+000230d0: 706c 7954 444f 4d4c 616e 6473 6174 203d  plyTDOMLandsat =
+000230e0: 2061 7070 6c79 5444 4f4d 4c61 6e64 7361   applyTDOMLandsa
+000230f0: 742c 0d0a 2020 2020 6170 706c 7954 444f  t,..    applyTDO
+00023100: 4d53 656e 7469 6e65 6c32 203d 2061 7070  MSentinel2 = app
+00023110: 6c79 5444 4f4d 5365 6e74 696e 656c 322c  lyTDOMSentinel2,
+00023120: 0d0a 2020 2020 6170 706c 7946 6d61 736b  ..    applyFmask
+00023130: 436c 6f75 644d 6173 6b20 3d20 6170 706c  CloudMask = appl
+00023140: 7946 6d61 736b 436c 6f75 644d 6173 6b2c  yFmaskCloudMask,
+00023150: 0d0a 2020 2020 6170 706c 7946 6d61 736b  ..    applyFmask
+00023160: 436c 6f75 6453 6861 646f 774d 6173 6b20  CloudShadowMask 
+00023170: 3d20 6170 706c 7946 6d61 736b 436c 6f75  = applyFmaskClou
+00023180: 6453 6861 646f 774d 6173 6b2c 0d0a 2020  dShadowMask,..  
+00023190: 2020 6170 706c 7946 6d61 736b 536e 6f77    applyFmaskSnow
+000231a0: 4d61 736b 203d 2061 7070 6c79 466d 6173  Mask = applyFmas
+000231b0: 6b53 6e6f 774d 6173 6b2c 0d0a 2020 2020  kSnowMask,..    
+000231c0: 636c 6f75 6448 6569 6768 7473 203d 2063  cloudHeights = c
+000231d0: 6c6f 7564 4865 6967 6874 732c 0d0a 2020  loudHeights,..  
+000231e0: 2020 636c 6f75 6453 636f 7265 5468 7265    cloudScoreThre
+000231f0: 7368 203d 2063 6c6f 7564 5363 6f72 6554  sh = cloudScoreT
+00023200: 6872 6573 682c 0d0a 2020 2020 7065 7266  hresh,..    perf
+00023210: 6f72 6d43 6c6f 7564 5363 6f72 654f 6666  ormCloudScoreOff
+00023220: 7365 7420 3d20 7065 7266 6f72 6d43 6c6f  set = performClo
+00023230: 7564 5363 6f72 654f 6666 7365 742c 0d0a  udScoreOffset,..
+00023240: 2020 2020 636c 6f75 6453 636f 7265 5063      cloudScorePc
+00023250: 746c 203d 2063 6c6f 7564 5363 6f72 6550  tl = cloudScoreP
+00023260: 6374 6c2c 0d0a 2020 2020 7a53 636f 7265  ctl,..    zScore
+00023270: 5468 7265 7368 203d 207a 5363 6f72 6554  Thresh = zScoreT
+00023280: 6872 6573 682c 0d0a 2020 2020 7368 6164  hresh,..    shad
+00023290: 6f77 5375 6d54 6872 6573 6820 3d20 7368  owSumThresh = sh
+000232a0: 6164 6f77 5375 6d54 6872 6573 682c 0d0a  adowSumThresh,..
+000232b0: 2020 2020 636f 6e74 7261 6374 5069 7865      contractPixe
+000232c0: 6c73 203d 2063 6f6e 7472 6163 7450 6978  ls = contractPix
+000232d0: 656c 732c 0d0a 2020 2020 6469 6c61 7465  els,..    dilate
+000232e0: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
+000232f0: 6978 656c 732c 0d0a 2020 2020 7368 6164  ixels,..    shad
+00023300: 6f77 5375 6d42 616e 6473 203d 2073 6861  owSumBands = sha
+00023310: 646f 7753 756d 4261 6e64 732c 0d0a 2020  dowSumBands,..  
+00023320: 2020 6c61 6e64 7361 7452 6573 616d 706c    landsatResampl
+00023330: 654d 6574 686f 6420 3d20 6c61 6e64 7361  eMethod = landsa
+00023340: 7452 6573 616d 706c 654d 6574 686f 642c  tResampleMethod,
+00023350: 0d0a 2020 2020 7365 6e74 696e 656c 3252  ..    sentinel2R
+00023360: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+00023370: 7365 6e74 696e 656c 3252 6573 616d 706c  sentinel2Resampl
+00023380: 654d 6574 686f 642c 0d0a 2020 2020 636f  eMethod,..    co
+00023390: 6e76 6572 7454 6f44 6169 6c79 4d6f 7361  nvertToDailyMosa
+000233a0: 6963 7320 3d20 636f 6e76 6572 7454 6f44  ics = convertToD
+000233b0: 6169 6c79 4d6f 7361 6963 732c 0d0a 2020  ailyMosaics,..  
+000233c0: 2020 7275 6e43 6861 7374 6169 6e48 6172    runChastainHar
+000233d0: 6d6f 6e69 7a61 7469 6f6e 203d 2072 756e  monization = run
+000233e0: 4368 6173 7461 696e 4861 726d 6f6e 697a  ChastainHarmoniz
+000233f0: 6174 696f 6e2c 0d0a 2020 2020 636f 7272  ation,..    corr
+00023400: 6563 7449 6c6c 756d 696e 6174 696f 6e20  ectIllumination 
+00023410: 3d20 636f 7272 6563 7449 6c6c 756d 696e  = correctIllumin
+00023420: 6174 696f 6e2c 0d0a 2020 2020 636f 7272  ation,..    corr
+00023430: 6563 7453 6361 6c65 203d 2063 6f72 7265  ectScale = corre
+00023440: 6374 5363 616c 652c 0d0a 2020 2020 7072  ctScale,..    pr
+00023450: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
+00023460: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+00023470: 203d 2070 7265 436f 6d70 7574 6564 4c61   = preComputedLa
+00023480: 6e64 7361 7443 6c6f 7564 5363 6f72 654f  ndsatCloudScoreO
+00023490: 6666 7365 742c 0d0a 2020 2020 7072 6543  ffset,..    preC
+000234a0: 6f6d 7075 7465 644c 616e 6473 6174 5444  omputedLandsatTD
+000234b0: 4f4d 4952 4d65 616e 203d 2070 7265 436f  OMIRMean = preCo
+000234c0: 6d70 7574 6564 4c61 6e64 7361 7454 444f  mputedLandsatTDO
+000234d0: 4d49 524d 6561 6e2c 0d0a 2020 2020 7072  MIRMean,..    pr
+000234e0: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
+000234f0: 5444 4f4d 4952 5374 6444 6576 203d 2070  TDOMIRStdDev = p
+00023500: 7265 436f 6d70 7574 6564 4c61 6e64 7361  reComputedLandsa
+00023510: 7454 444f 4d49 5253 7464 4465 762c 0d0a  tTDOMIRStdDev,..
+00023520: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
+00023530: 656e 7469 6e65 6c32 436c 6f75 6453 636f  entinel2CloudSco
+00023540: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
+00023550: 6d70 7574 6564 5365 6e74 696e 656c 3243  mputedSentinel2C
+00023560: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+00023570: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
+00023580: 6453 656e 7469 6e65 6c32 5444 4f4d 4952  dSentinel2TDOMIR
+00023590: 4d65 616e 203d 2070 7265 436f 6d70 7574  Mean = preComput
+000235a0: 6564 5365 6e74 696e 656c 3254 444f 4d49  edSentinel2TDOMI
+000235b0: 524d 6561 6e2c 0d0a 2020 2020 7072 6543  RMean,..    preC
+000235c0: 6f6d 7075 7465 6453 656e 7469 6e65 6c32  omputedSentinel2
+000235d0: 5444 4f4d 4952 5374 6444 6576 203d 2070  TDOMIRStdDev = p
+000235e0: 7265 436f 6d70 7574 6564 5365 6e74 696e  reComputedSentin
+000235f0: 656c 3254 444f 4d49 5253 7464 4465 762c  el2TDOMIRStdDev,
+00023600: 0d0a 2020 2020 636c 6f75 6450 726f 6254  ..    cloudProbT
+00023610: 6872 6573 6820 3d20 636c 6f75 6450 726f  hresh = cloudPro
+00023620: 6254 6872 6573 682c 0d0a 2020 2020 6c61  bThresh,..    la
+00023630: 6e64 7361 7443 6f6c 6c65 6374 696f 6e56  ndsatCollectionV
+00023640: 6572 7369 6f6e 203d 206c 616e 6473 6174  ersion = landsat
+00023650: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
+00023660: 6e2c 0d0a 2020 2020 7665 7262 6f73 6520  n,..    verbose 
+00023670: 3d20 7665 7262 6f73 6529 0d0a 0d0a 2020  = verbose)....  
+00023680: 2343 7265 6174 6520 6879 6272 6964 2063  #Create hybrid c
+00023690: 6f6d 706f 7369 7465 730d 0a20 2063 6f6d  omposites..  com
+000236a0: 706f 7369 7465 7320 3d20 636f 6d70 6f73  posites = compos
+000236b0: 6974 6554 696d 6553 6572 6965 7328 5c0d  iteTimeSeries(\.
+000236c0: 0a20 2020 206c 7320 3d20 6d65 7267 6564  .    ls = merged
+000236d0: 2c0d 0a20 2020 2073 7461 7274 5965 6172  ,..    startYear
+000236e0: 203d 2073 7461 7274 5965 6172 2c0d 0a20   = startYear,.. 
+000236f0: 2020 2065 6e64 5965 6172 203d 2065 6e64     endYear = end
+00023700: 5965 6172 2c0d 0a20 2020 2073 7461 7274  Year,..    start
+00023710: 4a75 6c69 616e 203d 2073 7461 7274 4a75  Julian = startJu
+00023720: 6c69 616e 2c0d 0a20 2020 2065 6e64 4a75  lian,..    endJu
+00023730: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
+00023740: 2c0d 0a20 2020 2074 696d 6562 7566 6665  ,..    timebuffe
+00023750: 7220 3d20 7469 6d65 6275 6666 6572 2c0d  r = timebuffer,.
+00023760: 0a20 2020 2077 6569 6768 7473 203d 2077  .    weights = w
+00023770: 6569 6768 7473 2c0d 0a20 2020 2063 6f6d  eights,..    com
+00023780: 706f 7369 7469 6e67 4d65 7468 6f64 203d  positingMethod =
+00023790: 2063 6f6d 706f 7369 7469 6e67 4d65 7468   compositingMeth
+000237a0: 6f64 290d 0a0d 0a20 2023 2045 7870 6f72  od)....  # Expor
+000237b0: 7420 636f 6d70 6f73 6974 6520 636f 6c6c  t composite coll
+000237c0: 6563 7469 6f6e 0d0a 2020 6966 2065 7870  ection..  if exp
+000237d0: 6f72 7443 6f6d 706f 7369 7465 733a 0d0a  ortComposites:..
+000237e0: 0d0a 2020 2020 6578 706f 7274 4261 6e64  ..    exportBand
+000237f0: 4469 6374 203d 207b 5c0d 0a20 2020 2020  Dict = {\..     
+00023800: 2027 6d65 646f 6964 273a 5b27 626c 7565   'medoid':['blue
+00023810: 272c 2027 6772 6565 6e27 2c20 2772 6564  ', 'green', 'red
+00023820: 272c 276e 6972 272c 2773 7769 7231 272c  ','nir','swir1',
+00023830: 2027 7377 6972 3227 2c27 636f 6d70 6f73   'swir2','compos
+00023840: 6974 654f 6273 436f 756e 7427 2c27 7365  iteObsCount','se
+00023850: 6e73 6f72 272c 2779 6561 7227 2c27 6a75  nsor','year','ju
+00023860: 6c69 616e 4461 7927 5d2c 0d0a 2020 2020  lianDay'],..    
+00023870: 2020 276d 6564 6961 6e27 3a5b 2762 6c75    'median':['blu
+00023880: 6527 2c20 2767 7265 656e 272c 2027 7265  e', 'green', 're
+00023890: 6427 2c27 6e69 7227 2c27 7377 6972 3127  d','nir','swir1'
+000238a0: 2c20 2773 7769 7232 272c 2763 6f6d 706f  , 'swir2','compo
+000238b0: 7369 7465 4f62 7343 6f75 6e74 275d 5c0d  siteObsCount']\.
+000238c0: 0a20 2020 207d 3b0d 0a20 2020 206e 6f6e  .    };..    non
+000238d0: 4469 7669 6465 4261 6e64 4469 6374 203d  DivideBandDict =
+000238e0: 207b 5c0d 0a20 2020 2020 2027 6d65 646f   {\..      'medo
+000238f0: 6964 273a 5b27 636f 6d70 6f73 6974 654f  id':['compositeO
+00023900: 6273 436f 756e 7427 2c27 7365 6e73 6f72  bsCount','sensor
+00023910: 272c 2779 6561 7227 2c27 6a75 6c69 616e  ','year','julian
+00023920: 4461 7927 5d2c 0d0a 2020 2020 2020 276d  Day'],..      'm
+00023930: 6564 6961 6e27 3a5b 2763 6f6d 706f 7369  edian':['composi
+00023940: 7465 4f62 7343 6f75 6e74 275d 5c0d 0a20  teObsCount']\.. 
+00023950: 2020 207d 3b0d 0a20 2020 2065 7870 6f72     };..    expor
+00023960: 7442 616e 6473 203d 2065 7870 6f72 7442  tBands = exportB
+00023970: 616e 6444 6963 745b 636f 6d70 6f73 6974  andDict[composit
+00023980: 696e 674d 6574 686f 645d 0d0a 2020 2020  ingMethod]..    
+00023990: 6e6f 6e44 6976 6964 6542 616e 6473 203d  nonDivideBands =
+000239a0: 206e 6f6e 4469 7669 6465 4261 6e64 4469   nonDivideBandDi
+000239b0: 6374 5b63 6f6d 706f 7369 7469 6e67 4d65  ct[compositingMe
+000239c0: 7468 6f64 5d0d 0a0d 0a20 2020 2065 7870  thod]....    exp
+000239d0: 6f72 7443 6f6d 706f 7369 7465 436f 6c6c  ortCompositeColl
+000239e0: 6563 7469 6f6e 285c 0d0a 2020 2020 2020  ection(\..      
+000239f0: 636f 6c6c 6563 7469 6f6e 203d 2063 6f6d  collection = com
+00023a00: 706f 7369 7465 732c 0d0a 2020 2020 2020  posites,..      
+00023a10: 6578 706f 7274 5061 7468 526f 6f74 203d  exportPathRoot =
+00023a20: 2065 7870 6f72 7450 6174 6852 6f6f 742c   exportPathRoot,
+00023a30: 0d0a 2020 2020 2020 6f75 7470 7574 4e61  ..      outputNa
+00023a40: 6d65 203d 206f 7574 7075 744e 616d 652c  me = outputName,
+00023a50: 0d0a 2020 2020 2020 6f72 6967 696e 203d  ..      origin =
+00023a60: 206f 7269 6769 6e2c 0d0a 2020 2020 2020   origin,..      
+00023a70: 7374 7564 7941 7265 6120 3d20 7374 7564  studyArea = stud
+00023a80: 7941 7265 612c 0d0a 2020 2020 2020 6372  yArea,..      cr
+00023a90: 7320 3d20 6372 732c 0d0a 2020 2020 2020  s = crs,..      
+00023aa0: 7472 616e 7366 6f72 6d20 3d20 7472 616e  transform = tran
+00023ab0: 7366 6f72 6d2c 0d0a 2020 2020 2020 7363  sform,..      sc
+00023ac0: 616c 6520 3d20 7363 616c 652c 0d0a 2020  ale = scale,..  
+00023ad0: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
+00023ae0: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
+00023af0: 2020 656e 6459 6561 7220 3d20 656e 6459    endYear = endY
+00023b00: 6561 722c 0d0a 2020 2020 2020 7374 6172  ear,..      star
+00023b10: 744a 756c 6961 6e20 3d20 7374 6172 744a  tJulian = startJ
+00023b20: 756c 6961 6e2c 0d0a 2020 2020 2020 656e  ulian,..      en
+00023b30: 644a 756c 6961 6e20 3d20 656e 644a 756c  dJulian = endJul
+00023b40: 6961 6e2c 0d0a 2020 2020 2020 636f 6d70  ian,..      comp
+00023b50: 6f73 6974 696e 674d 6574 686f 6420 3d20  ositingMethod = 
+00023b60: 636f 6d70 6f73 6974 696e 674d 6574 686f  compositingMetho
+00023b70: 642c 0d0a 2020 2020 2020 7469 6d65 6275  d,..      timebu
+00023b80: 6666 6572 203d 2074 696d 6562 7566 6665  ffer = timebuffe
+00023b90: 722c 0d0a 2020 2020 2020 746f 614f 7253  r,..      toaOrS
+00023ba0: 5220 3d20 746f 614f 7253 522c 0d0a 2020  R = toaOrSR,..  
+00023bb0: 2020 2020 6e6f 6e44 6976 6964 6542 616e      nonDivideBan
+00023bc0: 6473 203d 206e 6f6e 4469 7669 6465 4261  ds = nonDivideBa
+00023bd0: 6e64 732c 0d0a 2020 2020 2020 6578 706f  nds,..      expo
+00023be0: 7274 4261 6e64 7320 3d20 6578 706f 7274  rtBands = export
+00023bf0: 4261 6e64 732c 0d0a 2020 2020 2020 6164  Bands,..      ad
+00023c00: 6469 7469 6f6e 616c 5072 6f70 6572 7479  ditionalProperty
+00023c10: 4469 6374 203d 2061 7267 732c 0d0a 2020  Dict = args,..  
+00023c20: 2020 2020 6f76 6572 7772 6974 6520 3d20      overwrite = 
+00023c30: 6f76 6572 7772 6974 6529 0d0a 0d0a 2020  overwrite)....  
+00023c40: 6172 6773 5b27 7072 6f63 6573 7365 6453  args['processedS
+00023c50: 6365 6e65 7327 5d20 3d20 6d65 7267 6564  cenes'] = merged
+00023c60: 0d0a 2020 6172 6773 5b27 7072 6f63 6573  ..  args['proces
+00023c70: 7365 6443 6f6d 706f 7369 7465 7327 5d20  sedComposites'] 
+00023c80: 3d20 636f 6d70 6f73 6974 6573 0d0a 0d0a  = composites....
+00023c90: 2020 7265 7475 726e 2061 7267 730d 0a0d    return args...
+00023ca0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00023cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023ce0: 2323 2323 2323 2323 2323 0d0a 2323 2323  ##########..####
+00023cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d30: 2323 2323 230d 0a23 4861 726d 6f6e 6963  #####..#Harmonic
+00023d40: 2072 6567 7265 7373 696f 6e0d 0a23 2323   regression..###
+00023d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d90: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
+00023da0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023dd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023de0: 230d 0a23 4675 6e63 7469 6f6e 2074 6f20  #..#Function to 
+00023df0: 6769 7665 2079 6561 722e 6464 2069 6d61  give year.dd ima
+00023e00: 6765 2061 6e64 2068 6172 6d6f 6e69 6373  ge and harmonics
+00023e10: 206c 6973 7420 2865 2e67 2e20 5b31 2c32   list (e.g. [1,2
+00023e20: 2c33 2c2e 2e2e 5d29 0d0a 6465 6620 6765  ,3,...])..def ge
+00023e30: 7448 6172 6d6f 6e69 634c 6973 7428 7965  tHarmonicList(ye
+00023e40: 6172 4461 7465 496d 672c 7472 616e 7366  arDateImg,transf
+00023e50: 6f72 6d42 616e 644e 616d 652c 6861 726d  ormBandName,harm
+00023e60: 6f6e 6963 4c69 7374 293a 0d0a 2020 743d  onicList):..  t=
+00023e70: 2079 6561 7244 6174 6549 6d67 2e73 656c   yearDateImg.sel
+00023e80: 6563 7428 5b74 7261 6e73 666f 726d 4261  ect([transformBa
+00023e90: 6e64 4e61 6d65 5d29 0d0a 2020 7365 6c65  ndName])..  sele
+00023ea0: 6374 4261 6e64 7320 3d20 6565 2e4c 6973  ctBands = ee.Lis
+00023eb0: 742e 7365 7175 656e 6365 2830 2c6c 656e  t.sequence(0,len
+00023ec0: 2868 6172 6d6f 6e69 634c 6973 7429 2d31  (harmonicList)-1
+00023ed0: 290d 0a0d 0a20 2064 6566 2073 696e 4361  )....  def sinCa
+00023ee0: 7428 6829 3a0d 0a20 2020 2068 7420 3d20  t(h):..    ht = 
+00023ef0: 682a 3130 300d 0a20 2020 2072 6574 7572  h*100..    retur
+00023f00: 6e20 6565 2e53 7472 696e 6728 2773 696e  n ee.String('sin
+00023f10: 5f27 292e 6361 7428 7374 7228 6874 2929  _').cat(str(ht))
+00023f20: 2e63 6174 2827 5f27 292e 6361 7428 7472  .cat('_').cat(tr
+00023f30: 616e 7366 6f72 6d42 616e 644e 616d 6529  ansformBandName)
+00023f40: 0d0a 2020 7369 6e4e 616d 6573 203d 206c  ..  sinNames = l
+00023f50: 6973 7428 6d61 7028 6c61 6d62 6461 2069  ist(map(lambda i
+00023f60: 3a73 696e 4361 7428 6929 2c68 6172 6d6f  :sinCat(i),harmo
+00023f70: 6e69 634c 6973 7429 290d 0a0d 0a20 2064  nicList))....  d
+00023f80: 6566 2063 6f73 4361 7428 6829 3a0d 0a20  ef cosCat(h):.. 
+00023f90: 2020 2068 7420 3d68 2a31 3030 3b0d 0a20     ht =h*100;.. 
+00023fa0: 2020 2072 6574 7572 6e20 6565 2e53 7472     return ee.Str
+00023fb0: 696e 6728 2763 6f73 5f27 292e 6361 7428  ing('cos_').cat(
+00023fc0: 7374 7228 6874 2929 2e63 6174 2827 5f27  str(ht)).cat('_'
+00023fd0: 292e 6361 7428 7472 616e 7366 6f72 6d42  ).cat(transformB
+00023fe0: 616e 644e 616d 6529 0d0a 0d0a 2020 636f  andName)....  co
+00023ff0: 734e 616d 6573 203d 206c 6973 7428 6d61  sNames = list(ma
+00024000: 7028 6c61 6d62 6461 2069 203a 2063 6f73  p(lambda i : cos
+00024010: 4361 7428 6929 2c68 6172 6d6f 6e69 634c  Cat(i),harmonicL
+00024020: 6973 7429 290d 0a0d 0a0d 0a0d 0a20 206d  ist))........  m
+00024030: 756c 7469 706c 6965 7273 203d 2065 652e  ultipliers = ee.
+00024040: 496d 6167 6528 6861 726d 6f6e 6963 4c69  Image(harmonicLi
+00024050: 7374 292e 6d75 6c74 6970 6c79 2865 652e  st).multiply(ee.
+00024060: 4e75 6d62 6572 286d 6174 682e 7069 292e  Number(math.pi).
+00024070: 666c 6f61 7428 2929 0d0a 2020 7369 6e49  float())..  sinI
+00024080: 6e64 203d 2028 742e 6d75 6c74 6970 6c79  nd = (t.multiply
+00024090: 2865 652e 496d 6167 6528 6d75 6c74 6970  (ee.Image(multip
+000240a0: 6c69 6572 7329 2929 2e73 696e 2829 2e73  liers))).sin().s
+000240b0: 656c 6563 7428 7365 6c65 6374 4261 6e64  elect(selectBand
+000240c0: 732c 7369 6e4e 616d 6573 292e 666c 6f61  s,sinNames).floa
+000240d0: 7428 290d 0a20 2063 6f73 496e 6420 3d20  t()..  cosInd = 
+000240e0: 2874 2e6d 756c 7469 706c 7928 6565 2e49  (t.multiply(ee.I
+000240f0: 6d61 6765 286d 756c 7469 706c 6965 7273  mage(multipliers
+00024100: 2929 292e 636f 7328 292e 7365 6c65 6374  ))).cos().select
+00024110: 2873 656c 6563 7442 616e 6473 2c63 6f73  (selectBands,cos
+00024120: 4e61 6d65 7329 2e66 6c6f 6174 2829 0d0a  Names).float()..
+00024130: 0d0a 2020 7265 7475 726e 2079 6561 7244  ..  return yearD
+00024140: 6174 6549 6d67 2e61 6464 4261 6e64 7328  ateImg.addBands(
+00024150: 7369 6e49 6e64 2e61 6464 4261 6e64 7328  sinInd.addBands(
+00024160: 636f 7349 6e64 2929 0d0a 0d0a 2323 2323  cosInd))....####
+00024170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000241a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000241b0: 2323 2323 230d 0a23 2323 2323 2323 2323  #####..#########
+000241c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000241d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000241e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000241f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024200: 0d0a 2354 616b 6573 2061 2064 6570 656e  ..#Takes a depen
+00024210: 6465 6e74 2061 6e64 2069 6e64 6570 656e  dent and indepen
+00024220: 6465 6e74 2076 6172 6961 626c 6520 616e  dent variable an
+00024230: 6420 7265 7475 726e 7320 7468 6520 6465  d returns the de
+00024240: 7065 6e64 656e 742c 0d0a 2320 7369 6e20  pendent,..# sin 
+00024250: 6f66 2069 6e64 2c20 616e 6420 636f 7320  of ind, and cos 
+00024260: 6f66 2069 6e64 0d0a 2349 6e74 656e 6465  of ind..#Intende
+00024270: 6420 666f 7220 6861 726d 6f6e 6963 2072  d for harmonic r
+00024280: 6567 7265 7373 696f 6e0d 0a64 6566 2067  egression..def g
+00024290: 6574 4861 726d 6f6e 6963 7332 2863 6f6c  etHarmonics2(col
+000242a0: 6c65 6374 696f 6e2c 7472 616e 7366 6f72  lection,transfor
+000242b0: 6d42 616e 644e 616d 652c 6861 726d 6f6e  mBandName,harmon
+000242c0: 6963 4c69 7374 2c64 6574 7265 6e64 203d  icList,detrend =
+000242d0: 2046 616c 7365 293a 0d0a 0d0a 2020 6465   False):....  de
+000242e0: 7042 616e 644e 616d 6573 203d 2065 652e  pBandNames = ee.
+000242f0: 496d 6167 6528 636f 6c6c 6563 7469 6f6e  Image(collection
+00024300: 2e66 6972 7374 2829 292e 6261 6e64 4e61  .first()).bandNa
+00024310: 6d65 7328 292e 7265 6d6f 7665 2874 7261  mes().remove(tra
+00024320: 6e73 666f 726d 4261 6e64 4e61 6d65 290d  nsformBandName).
+00024330: 0a20 2064 6570 4261 6e64 4e75 6d62 6572  .  depBandNumber
+00024340: 7320 3d20 6465 7042 616e 644e 616d 6573  s = depBandNames
+00024350: 2e6d 6170 286c 616d 6264 6120 6462 6e3a  .map(lambda dbn:
+00024360: 6465 7042 616e 644e 616d 6573 2e69 6e64  depBandNames.ind
+00024370: 6578 4f66 2864 626e 2929 0d0a 0d0a 2020  exOf(dbn))....  
+00024380: 6465 6620 6861 726d 5772 6170 2869 6d67  def harmWrap(img
+00024390: 293a 0d0a 2020 2020 6f75 7454 203d 2067  ):..    outT = g
+000243a0: 6574 4861 726d 6f6e 6963 4c69 7374 2869  etHarmonicList(i
+000243b0: 6d67 2c74 7261 6e73 666f 726d 4261 6e64  mg,transformBand
+000243c0: 4e61 6d65 2c68 6172 6d6f 6e69 634c 6973  Name,harmonicLis
+000243d0: 7429 5c0d 0a20 2020 202e 636f 7079 5072  t)\..    .copyPr
+000243e0: 6f70 6572 7469 6573 2869 6d67 2c5b 2773  operties(img,['s
+000243f0: 7973 7465 6d3a 7469 6d65 5f73 7461 7274  ystem:time_start
+00024400: 272c 2773 7973 7465 6d3a 7469 6d65 5f65  ','system:time_e
+00024410: 6e64 275d 290d 0a20 2020 2072 6574 7572  nd'])..    retur
+00024420: 6e20 6f75 7454 0d0a 2020 6f75 7420 3d20  n outT..  out = 
+00024430: 636f 6c6c 6563 7469 6f6e 2e6d 6170 2868  collection.map(h
+00024440: 6172 6d57 7261 7029 0d0a 0d0a 2020 6966  armWrap)....  if
+00024450: 206e 6f74 2064 6574 7265 6e64 3a0d 0a20   not detrend:.. 
+00024460: 2020 206f 7574 4261 6e64 4e61 6d65 7320     outBandNames 
+00024470: 3d20 6565 2e49 6d61 6765 286f 7574 2e66  = ee.Image(out.f
+00024480: 6972 7374 2829 292e 6261 6e64 4e61 6d65  irst()).bandName
+00024490: 7328 292e 7265 6d6f 7665 416c 6c28 5b27  s().removeAll(['
+000244a0: 7965 6172 275d 290d 0a20 2020 206f 7574  year'])..    out
+000244b0: 203d 206f 7574 2e73 656c 6563 7428 6f75   = out.select(ou
+000244c0: 7442 616e 644e 616d 6573 290d 0a0d 0a0d  tBandNames).....
+000244d0: 0a20 2069 6e64 4261 6e64 4e61 6d65 7320  .  indBandNames 
+000244e0: 3d20 6565 2e49 6d61 6765 286f 7574 2e66  = ee.Image(out.f
+000244f0: 6972 7374 2829 292e 6261 6e64 4e61 6d65  irst()).bandName
+00024500: 7328 292e 7265 6d6f 7665 416c 6c28 6465  s().removeAll(de
+00024510: 7042 616e 644e 616d 6573 290d 0a20 2069  pBandNames)..  i
+00024520: 6e64 4261 6e64 4e75 6d62 6572 7320 3d20  ndBandNumbers = 
+00024530: 696e 6442 616e 644e 616d 6573 2e6d 6170  indBandNames.map
+00024540: 286c 616d 6264 6120 696e 643a 2065 652e  (lambda ind: ee.
+00024550: 496d 6167 6528 6f75 742e 6669 7273 7428  Image(out.first(
+00024560: 2929 2e62 616e 644e 616d 6573 2829 2e69  )).bandNames().i
+00024570: 6e64 6578 4f66 2869 6e64 2929 0d0a 0d0a  ndexOf(ind))....
+00024580: 0d0a 2020 6f75 7420 3d20 6f75 742e 7365  ..  out = out.se
+00024590: 7428 7b27 696e 6442 616e 644e 616d 6573  t({'indBandNames
+000245a0: 273a 696e 6442 616e 644e 616d 6573 2c27  ':indBandNames,'
+000245b0: 6465 7042 616e 644e 616d 6573 273a 6465  depBandNames':de
+000245c0: 7042 616e 644e 616d 6573 2c5c 0d0a 2020  pBandNames,\..  
+000245d0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+000245e0: 6e64 4261 6e64 4e75 6d62 6572 7327 3a69  ndBandNumbers':i
+000245f0: 6e64 4261 6e64 4e75 6d62 6572 732c 2764  ndBandNumbers,'d
+00024600: 6570 4261 6e64 4e75 6d62 6572 7327 3a64  epBandNumbers':d
+00024610: 6570 4261 6e64 4e75 6d62 6572 737d 290d  epBandNumbers}).
+00024620: 0a0d 0a20 2072 6574 7572 6e20 6f75 740d  ...  return out.
+00024630: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00024640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024670: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+00024680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000246a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000246b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000246c0: 2323 2323 2323 230d 0a23 5369 6d70 6c69  #######..#Simpli
+000246d0: 6669 6573 2074 6865 2075 7365 206f 6620  fies the use of 
+000246e0: 7468 6520 726f 6275 7374 206c 696e 6561  the robust linea
+000246f0: 7220 7265 6772 6573 7369 6f6e 2072 6564  r regression red
+00024700: 7563 6572 0d0a 2341 7373 756d 6573 2074  ucer..#Assumes t
+00024710: 6865 2064 6570 656e 6465 6e74 2069 7320  he dependent is 
+00024720: 7468 6520 6669 7273 7420 6261 6e64 2061  the first band a
+00024730: 6e64 2061 6c6c 2073 7562 7365 7175 656e  nd all subsequen
+00024740: 7420 6261 6e64 7320 6172 6520 696e 6465  t bands are inde
+00024750: 7065 6e64 656e 7473 0d0a 6465 6620 6e65  pendents..def ne
+00024760: 7752 6f62 7573 744d 756c 7469 706c 654c  wRobustMultipleL
+00024770: 696e 6561 7232 2864 6570 656e 6465 6e74  inear2(dependent
+00024780: 7349 6e64 6570 656e 6465 6e74 7329 3a0d  sIndependents):.
+00024790: 0a20 2023 5365 7420 7570 2074 6865 2062  .  #Set up the b
+000247a0: 616e 6420 6e61 6d65 730d 0a0d 0a20 2064  and names....  d
+000247b0: 6570 656e 6465 6e74 4261 6e64 7320 3d20  ependentBands = 
+000247c0: 6565 2e4c 6973 7428 6465 7065 6e64 656e  ee.List(dependen
+000247d0: 7473 496e 6465 7065 6e64 656e 7473 2e67  tsIndependents.g
+000247e0: 6574 2827 6465 7042 616e 644e 756d 6265  et('depBandNumbe
+000247f0: 7273 2729 290d 0a20 2069 6e64 6570 656e  rs'))..  indepen
+00024800: 6465 6e74 4261 6e64 7320 3d20 6565 2e4c  dentBands = ee.L
+00024810: 6973 7428 6465 7065 6e64 656e 7473 496e  ist(dependentsIn
+00024820: 6465 7065 6e64 656e 7473 2e67 6574 2827  dependents.get('
+00024830: 696e 6442 616e 644e 756d 6265 7273 2729  indBandNumbers')
+00024840: 290d 0a20 2062 6e73 203d 2065 652e 496d  )..  bns = ee.Im
+00024850: 6167 6528 6465 7065 6e64 656e 7473 496e  age(dependentsIn
+00024860: 6465 7065 6e64 656e 7473 2e66 6972 7374  dependents.first
+00024870: 2829 292e 6261 6e64 4e61 6d65 7328 290d  ()).bandNames().
+00024880: 0a20 2064 6570 656e 6465 6e74 7320 3d20  .  dependents = 
+00024890: 6565 2e4c 6973 7428 6465 7065 6e64 656e  ee.List(dependen
+000248a0: 7473 496e 6465 7065 6e64 656e 7473 2e67  tsIndependents.g
+000248b0: 6574 2827 6465 7042 616e 644e 616d 6573  et('depBandNames
+000248c0: 2729 290d 0a20 2069 6e64 6570 656e 6465  '))..  independe
+000248d0: 6e74 7320 3d20 6565 2e4c 6973 7428 6465  nts = ee.List(de
+000248e0: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
+000248f0: 656e 7473 2e67 6574 2827 696e 6442 616e  ents.get('indBan
+00024900: 644e 616d 6573 2729 290d 0a0d 0a20 2023  dNames'))....  #
+00024910: 6465 7065 6e64 656e 7420 3d20 626e 732e  dependent = bns.
+00024920: 736c 6963 6528 302c 3129 0d0a 2020 2369  slice(0,1)..  #i
+00024930: 6e64 6570 656e 6465 6e74 7320 3d20 626e  ndependents = bn
+00024940: 732e 736c 6963 6528 312c 6e75 6c6c 290d  s.slice(1,null).
+00024950: 0a20 206e 6f49 6e64 6570 656e 6465 6e74  .  noIndependent
+00024960: 7320 3d20 696e 6465 7065 6e64 656e 7473  s = independents
+00024970: 2e6c 656e 6774 6828 292e 6164 6428 3129  .length().add(1)
+00024980: 0d0a 2020 6e6f 4465 7065 6e64 656e 7473  ..  noDependents
+00024990: 203d 2064 6570 656e 6465 6e74 732e 6c65   = dependents.le
+000249a0: 6e67 7468 2829 0d0a 0d0a 2020 6f75 744e  ngth()....  outN
+000249b0: 616d 6573 203d 2065 652e 4c69 7374 285b  ames = ee.List([
+000249c0: 2769 6e74 6572 6365 7074 275d 292e 6361  'intercept']).ca
+000249d0: 7428 696e 6465 7065 6e64 656e 7473 290d  t(independents).
+000249e0: 0a0d 0a20 2023 4164 6420 636f 6e73 7461  ...  #Add consta
+000249f0: 6e74 2062 616e 6420 666f 7220 696e 7465  nt band for inte
+00024a00: 7263 6570 7420 616e 6420 7265 6f72 6465  rcept and reorde
+00024a10: 7220 666f 720d 0a20 2023 7379 6e74 6178  r for..  #syntax
+00024a20: 3a20 636f 6e73 7461 6e74 2c20 696e 6431  : constant, ind1
+00024a30: 2c69 6e64 322c 696e 6433 2c69 6e64 6e2c  ,ind2,ind3,indn,
+00024a40: 6465 7065 6e64 656e 740d 0a20 2064 6566  dependent..  def
+00024a50: 2066 6f72 4669 7446 756e 2869 6d67 293a   forFitFun(img):
+00024a60: 0d0a 2020 2020 6f75 7420 3d20 696d 672e  ..    out = img.
+00024a70: 6164 6442 616e 6473 2865 652e 496d 6167  addBands(ee.Imag
+00024a80: 6528 3129 2e73 656c 6563 7428 5b30 5d2c  e(1).select([0],
+00024a90: 5b27 636f 6e73 7461 6e74 275d 2929 0d0a  ['constant']))..
+00024aa0: 2020 2020 6f75 7420 3d20 6f75 742e 7365      out = out.se
+00024ab0: 6c65 6374 2865 652e 4c69 7374 285b 2763  lect(ee.List(['c
+00024ac0: 6f6e 7374 616e 7427 2c69 6e64 6570 656e  onstant',indepen
+00024ad0: 6465 6e74 735d 292e 666c 6174 7465 6e28  dents]).flatten(
+00024ae0: 2929 0d0a 2020 2020 7265 7475 726e 206f  ))..    return o
+00024af0: 7574 2e61 6464 4261 6e64 7328 696d 672e  ut.addBands(img.
+00024b00: 7365 6c65 6374 2864 6570 656e 6465 6e74  select(dependent
+00024b10: 7329 290d 0a0d 0a0d 0a20 2066 6f72 4669  s))......  forFi
+00024b20: 7420 3d20 6465 7065 6e64 656e 7473 496e  t = dependentsIn
+00024b30: 6465 7065 6e64 656e 7473 2e6d 6170 2866  dependents.map(f
+00024b40: 6f72 4669 7446 756e 290d 0a0d 0a20 2023  orFitFun)....  #
+00024b50: 4170 706c 7920 7265 6475 6365 722c 2061  Apply reducer, a
+00024b60: 6e64 2063 6f6e 7665 7274 2062 6163 6b20  nd convert back 
+00024b70: 746f 2069 6d61 6765 2077 6974 6820 7265  to image with re
+00024b80: 7370 6563 7469 7665 2062 616e 644e 616d  spective bandNam
+00024b90: 6573 0d0a 2020 7265 6475 6365 724f 7574  es..  reducerOut
+00024ba0: 203d 2066 6f72 4669 742e 7265 6475 6365   = forFit.reduce
+00024bb0: 2865 652e 5265 6475 6365 722e 6c69 6e65  (ee.Reducer.line
+00024bc0: 6172 5265 6772 6573 7369 6f6e 286e 6f49  arRegression(noI
+00024bd0: 6e64 6570 656e 6465 6e74 732c 6e6f 4465  ndependents,noDe
+00024be0: 7065 6e64 656e 7473 2929 0d0a 2020 2320  pendents))..  # 
+00024bf0: 2f2f 2074 6573 7420 3d20 666f 7246 6974  // test = forFit
+00024c00: 2e72 6564 7563 6528 6565 2e52 6564 7563  .reduce(ee.Reduc
+00024c10: 6572 2e72 6f62 7573 744c 696e 6561 7252  er.robustLinearR
+00024c20: 6567 7265 7373 696f 6e28 6e6f 496e 6465  egression(noInde
+00024c30: 7065 6e64 656e 7473 2c6e 6f44 6570 656e  pendents,noDepen
+00024c40: 6465 6e74 732c 302e 3229 290d 0a20 2023  dents,0.2))..  #
+00024c50: 202f 2f20 7265 7369 6473 203d 2074 6573   // resids = tes
+00024c60: 740d 0a20 2023 202f 2f20 2e73 656c 6563  t..  # // .selec
+00024c70: 7428 5b31 5d2c 5b27 7265 7369 6475 616c  t([1],['residual
+00024c80: 7327 5d29 2e61 7272 6179 466c 6174 7465  s']).arrayFlatte
+00024c90: 6e28 5b64 6570 656e 6465 6e74 735d 293b  n([dependents]);
+00024ca0: 0d0a 2020 2320 2f2f 204d 6170 2e61 6464  ..  # // Map.add
+00024cb0: 4c61 7965 7228 7265 7369 6473 2c7b 7d2c  Layer(resids,{},
+00024cc0: 2772 6573 6964 7349 6d61 6765 2729 3b0d  'residsImage');.
+00024cd0: 0a20 2023 202f 2f20 4d61 702e 6164 644c  .  # // Map.addL
+00024ce0: 6179 6572 2872 6564 7563 6572 4f75 742e  ayer(reducerOut.
+00024cf0: 7365 6c65 6374 285b 305d 292c 7b7d 2c27  select([0]),{},'
+00024d00: 636f 6566 6669 6369 656e 7473 2729 3b0d  coefficients');.
+00024d10: 0a20 2023 202f 2f20 4d61 702e 6164 644c  .  # // Map.addL
+00024d20: 6179 6572 2874 6573 742e 7365 6c65 6374  ayer(test.select
+00024d30: 285b 315d 292c 7b7d 2c27 7472 6573 6964  ([1]),{},'tresid
+00024d40: 7561 6c73 2729 3b0d 0a20 2023 202f 2f20  uals');..  # // 
+00024d50: 4d61 702e 6164 644c 6179 6572 2872 6564  Map.addLayer(red
+00024d60: 7563 6572 4f75 742e 7365 6c65 6374 285b  ucerOut.select([
+00024d70: 315d 292c 7b7d 2c27 726f 7265 7369 6475  1]),{},'roresidu
+00024d80: 616c 7327 293b 0d0a 2020 7265 6475 6365  als');..  reduce
+00024d90: 724f 7574 203d 2072 6564 7563 6572 4f75  rOut = reducerOu
+00024da0: 742e 7365 6c65 6374 285b 305d 2c5b 2763  t.select([0],['c
+00024db0: 6f65 6666 6963 6965 6e74 7327 5d29 2e61  oefficients']).a
+00024dc0: 7272 6179 5472 616e 7370 6f73 6528 292e  rrayTranspose().
+00024dd0: 6172 7261 7946 6c61 7474 656e 285b 6465  arrayFlatten([de
+00024de0: 7065 6e64 656e 7473 2c6f 7574 4e61 6d65  pendents,outName
+00024df0: 735d 290d 0a20 2072 6564 7563 6572 4f75  s])..  reducerOu
+00024e00: 7420 3d20 7265 6475 6365 724f 7574 2e73  t = reducerOut.s
+00024e10: 6574 287b 276e 6f44 6570 656e 6465 6e74  et({'noDependent
+00024e20: 7327 3a65 652e 4e75 6d62 6572 286e 6f44  s':ee.Number(noD
+00024e30: 6570 656e 6465 6e74 7329 2c5c 0d0a 2020  ependents),\..  
+00024e40: 276d 6f64 656c 4c65 6e67 7468 273a 6565  'modelLength':ee
+00024e50: 2e4e 756d 6265 7228 6e6f 496e 6465 7065  .Number(noIndepe
+00024e60: 6e64 656e 7473 295c 0d0a 2020 7d29 0d0a  ndents)\..  })..
+00024e70: 0d0a 2020 7265 7475 726e 2072 6564 7563  ..  return reduc
+00024e80: 6572 4f75 740d 0a23 2323 2323 2323 2323  erOut..#########
+00024e90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024eb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024ed0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00024ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024f10: 2323 2323 2323 2323 2323 230d 0a23 436f  ###########..#Co
+00024f20: 6465 2066 6f72 2066 696e 6469 6e67 2074  de for finding t
+00024f30: 6865 2064 6174 6520 6f66 2070 6561 6b20  he date of peak 
+00024f40: 6f66 2067 7265 656e 0d0a 2320 416c 736f  of green..# Also
+00024f50: 2063 6f6e 7665 7274 7320 6974 2074 6f20   converts it to 
+00024f60: 4a75 6c69 616e 2064 6179 2c20 6d6f 6e74  Julian day, mont
+00024f70: 682c 2061 6e64 2064 6179 206f 6620 6d6f  h, and day of mo
+00024f80: 6e74 680d 0a6d 6f6e 7468 5265 6d61 7020  nth..monthRemap 
+00024f90: 3d5b 312c 2031 2c20 312c 2031 2c20 312c  =[1, 1, 1, 1, 1,
+00024fa0: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
+00024fb0: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
+00024fc0: 2c20 312c 2031 2c20 312c 2031 2c20 312c  , 1, 1, 1, 1, 1,
+00024fd0: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
+00024fe0: 312c 2031 2c20 312c 2031 2c20 312c 2032  1, 1, 1, 1, 1, 2
+00024ff0: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
+00025000: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
+00025010: 322c 2032 2c20 322c 2032 2c20 322c 2032  2, 2, 2, 2, 2, 2
+00025020: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
+00025030: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
+00025040: 322c 2033 2c20 332c 2033 2c20 332c 2033  2, 3, 3, 3, 3, 3
+00025050: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
+00025060: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
+00025070: 332c 2033 2c20 332c 2033 2c20 332c 2033  3, 3, 3, 3, 3, 3
+00025080: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
+00025090: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
+000250a0: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
+000250b0: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
+000250c0: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
+000250d0: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
+000250e0: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
+000250f0: 2034 2c20 342c 2034 2c20 352c 2035 2c20   4, 4, 4, 5, 5, 
+00025100: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
+00025110: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
+00025120: 2035 2c20 352c 2035 2c20 352c 2035 2c20   5, 5, 5, 5, 5, 
+00025130: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
+00025140: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
+00025150: 2035 2c20 352c 2036 2c20 362c 2036 2c20   5, 5, 6, 6, 6, 
+00025160: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
+00025170: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
+00025180: 2036 2c20 362c 2036 2c20 362c 2036 2c20   6, 6, 6, 6, 6, 
+00025190: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
+000251a0: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
+000251b0: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
+000251c0: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
+000251d0: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
+000251e0: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
+000251f0: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
+00025200: 2c20 372c 2037 2c20 372c 2037 2c20 382c  , 7, 7, 7, 7, 8,
+00025210: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
+00025220: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
+00025230: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
+00025240: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
+00025250: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
+00025260: 2c20 382c 2038 2c20 382c 2039 2c20 392c  , 8, 8, 8, 9, 9,
+00025270: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
+00025280: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
+00025290: 2c20 392c 2039 2c20 392c 2039 2c20 392c  , 9, 9, 9, 9, 9,
+000252a0: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
+000252b0: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
+000252c0: 2c20 392c 2031 302c 2031 302c 2031 302c  , 9, 10, 10, 10,
+000252d0: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+000252e0: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+000252f0: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+00025300: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+00025310: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+00025320: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+00025330: 2031 302c 2031 302c 2031 302c 2031 302c   10, 10, 10, 10,
+00025340: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+00025350: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+00025360: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+00025370: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+00025380: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+00025390: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+000253a0: 2031 312c 2031 312c 2031 312c 2031 312c   11, 11, 11, 11,
+000253b0: 2031 312c 2031 312c 2031 322c 2031 322c   11, 11, 12, 12,
+000253c0: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+000253d0: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+000253e0: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+000253f0: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+00025400: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+00025410: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+00025420: 2031 322c 2031 322c 2031 322c 2031 322c   12, 12, 12, 12,
+00025430: 2031 3220 5d0d 0a6d 6f6e 7468 4461 7952   12 ]..monthDayR
+00025440: 656d 6170 203d 205b 312c 2032 2c20 332c  emap = [1, 2, 3,
+00025450: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
+00025460: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
+00025470: 332c 2031 342c 2031 352c 2031 362c 2031  3, 14, 15, 16, 1
+00025480: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
+00025490: 312c 2032 322c 2032 332c 2032 342c 2032  1, 22, 23, 24, 2
+000254a0: 352c 2032 362c 2032 372c 2032 382c 2032  5, 26, 27, 28, 2
+000254b0: 392c 2033 302c 2033 312c 2031 2c20 322c  9, 30, 31, 1, 2,
+000254c0: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+000254d0: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
+000254e0: 2c20 3133 2c20 3134 2c20 3135 2c20 3136  , 13, 14, 15, 16
+000254f0: 2c20 3137 2c20 3138 2c20 3139 2c20 3230  , 17, 18, 19, 20
+00025500: 2c20 3231 2c20 3232 2c20 3233 2c20 3234  , 21, 22, 23, 24
+00025510: 2c20 3235 2c20 3236 2c20 3237 2c20 3238  , 25, 26, 27, 28
+00025520: 2c20 312c 2032 2c20 332c 2034 2c20 352c  , 1, 2, 3, 4, 5,
+00025530: 2036 2c20 372c 2038 2c20 392c 2031 302c   6, 7, 8, 9, 10,
+00025540: 2031 312c 2031 322c 2031 332c 2031 342c   11, 12, 13, 14,
+00025550: 2031 352c 2031 362c 2031 372c 2031 382c   15, 16, 17, 18,
+00025560: 2031 392c 2032 302c 2032 312c 2032 322c   19, 20, 21, 22,
+00025570: 2032 332c 2032 342c 2032 352c 2032 362c   23, 24, 25, 26,
+00025580: 2032 372c 2032 382c 2032 392c 2033 302c   27, 28, 29, 30,
+00025590: 2033 312c 2031 2c20 322c 2033 2c20 342c   31, 1, 2, 3, 4,
+000255a0: 2035 2c20 362c 2037 2c20 382c 2039 2c20   5, 6, 7, 8, 9, 
+000255b0: 3130 2c20 3131 2c20 3132 2c20 3133 2c20  10, 11, 12, 13, 
+000255c0: 3134 2c20 3135 2c20 3136 2c20 3137 2c20  14, 15, 16, 17, 
+000255d0: 3138 2c20 3139 2c20 3230 2c20 3231 2c20  18, 19, 20, 21, 
+000255e0: 3232 2c20 3233 2c20 3234 2c20 3235 2c20  22, 23, 24, 25, 
+000255f0: 3236 2c20 3237 2c20 3238 2c20 3239 2c20  26, 27, 28, 29, 
+00025600: 3330 2c20 312c 2032 2c20 332c 2034 2c20  30, 1, 2, 3, 4, 
+00025610: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
+00025620: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
+00025630: 342c 2031 352c 2031 362c 2031 372c 2031  4, 15, 16, 17, 1
+00025640: 382c 2031 392c 2032 302c 2032 312c 2032  8, 19, 20, 21, 2
+00025650: 322c 2032 332c 2032 342c 2032 352c 2032  2, 23, 24, 25, 2
+00025660: 362c 2032 372c 2032 382c 2032 392c 2033  6, 27, 28, 29, 3
+00025670: 302c 2033 312c 2031 2c20 322c 2033 2c20  0, 31, 1, 2, 3, 
+00025680: 342c 2035 2c20 362c 2037 2c20 382c 2039  4, 5, 6, 7, 8, 9
+00025690: 2c20 3130 2c20 3131 2c20 3132 2c20 3133  , 10, 11, 12, 13
+000256a0: 2c20 3134 2c20 3135 2c20 3136 2c20 3137  , 14, 15, 16, 17
+000256b0: 2c20 3138 2c20 3139 2c20 3230 2c20 3231  , 18, 19, 20, 21
+000256c0: 2c20 3232 2c20 3233 2c20 3234 2c20 3235  , 22, 23, 24, 25
+000256d0: 2c20 3236 2c20 3237 2c20 3238 2c20 3239  , 26, 27, 28, 29
+000256e0: 2c20 3330 2c20 312c 2032 2c20 332c 2034  , 30, 1, 2, 3, 4
+000256f0: 2c20 352c 2036 2c20 372c 2038 2c20 392c  , 5, 6, 7, 8, 9,
+00025700: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
+00025710: 2031 342c 2031 352c 2031 362c 2031 372c   14, 15, 16, 17,
+00025720: 2031 382c 2031 392c 2032 302c 2032 312c   18, 19, 20, 21,
+00025730: 2032 322c 2032 332c 2032 342c 2032 352c   22, 23, 24, 25,
+00025740: 2032 362c 2032 372c 2032 382c 2032 392c   26, 27, 28, 29,
+00025750: 2033 302c 2033 312c 2031 2c20 322c 2033   30, 31, 1, 2, 3
+00025760: 2c20 342c 2035 2c20 362c 2037 2c20 382c  , 4, 5, 6, 7, 8,
+00025770: 2039 2c20 3130 2c20 3131 2c20 3132 2c20   9, 10, 11, 12, 
+00025780: 3133 2c20 3134 2c20 3135 2c20 3136 2c20  13, 14, 15, 16, 
+00025790: 3137 2c20 3138 2c20 3139 2c20 3230 2c20  17, 18, 19, 20, 
+000257a0: 3231 2c20 3232 2c20 3233 2c20 3234 2c20  21, 22, 23, 24, 
+000257b0: 3235 2c20 3236 2c20 3237 2c20 3238 2c20  25, 26, 27, 28, 
+000257c0: 3239 2c20 3330 2c20 3331 2c20 312c 2032  29, 30, 31, 1, 2
+000257d0: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
+000257e0: 2038 2c20 392c 2031 302c 2031 312c 2031   8, 9, 10, 11, 1
+000257f0: 322c 2031 332c 2031 342c 2031 352c 2031  2, 13, 14, 15, 1
+00025800: 362c 2031 372c 2031 382c 2031 392c 2032  6, 17, 18, 19, 2
+00025810: 302c 2032 312c 2032 322c 2032 332c 2032  0, 21, 22, 23, 2
+00025820: 342c 2032 352c 2032 362c 2032 372c 2032  4, 25, 26, 27, 2
+00025830: 382c 2032 392c 2033 302c 2031 2c20 322c  8, 29, 30, 1, 2,
+00025840: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+00025850: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
+00025860: 2c20 3133 2c20 3134 2c20 3135 2c20 3136  , 13, 14, 15, 16
+00025870: 2c20 3137 2c20 3138 2c20 3139 2c20 3230  , 17, 18, 19, 20
+00025880: 2c20 3231 2c20 3232 2c20 3233 2c20 3234  , 21, 22, 23, 24
+00025890: 2c20 3235 2c20 3236 2c20 3237 2c20 3238  , 25, 26, 27, 28
+000258a0: 2c20 3239 2c20 3330 2c20 3331 2c20 312c  , 29, 30, 31, 1,
+000258b0: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
+000258c0: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
+000258d0: 2031 322c 2031 332c 2031 342c 2031 352c   12, 13, 14, 15,
+000258e0: 2031 362c 2031 372c 2031 382c 2031 392c   16, 17, 18, 19,
+000258f0: 2032 302c 2032 312c 2032 322c 2032 332c   20, 21, 22, 23,
+00025900: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
+00025910: 2032 382c 2032 392c 2033 302c 2031 2c20   28, 29, 30, 1, 
+00025920: 322c 2033 2c20 342c 2035 2c20 362c 2037  2, 3, 4, 5, 6, 7
+00025930: 2c20 382c 2039 2c20 3130 2c20 3131 2c20  , 8, 9, 10, 11, 
+00025940: 3132 2c20 3133 2c20 3134 2c20 3135 2c20  12, 13, 14, 15, 
+00025950: 3136 2c20 3137 2c20 3138 2c20 3139 2c20  16, 17, 18, 19, 
+00025960: 3230 2c20 3231 2c20 3232 2c20 3233 2c20  20, 21, 22, 23, 
+00025970: 3234 2c20 3235 2c20 3236 2c20 3237 2c20  24, 25, 26, 27, 
+00025980: 3238 2c20 3239 2c20 3330 2c20 3331 205d  28, 29, 30, 31 ]
+00025990: 0d0a 6a75 6c69 616e 4461 7920 3d20 5b31  ..julianDay = [1
+000259a0: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
+000259b0: 2037 2c20 382c 2039 2c20 3130 2c20 3131   7, 8, 9, 10, 11
+000259c0: 2c20 3132 2c20 3133 2c20 3134 2c20 3135  , 12, 13, 14, 15
+000259d0: 2c20 3136 2c20 3137 2c20 3138 2c20 3139  , 16, 17, 18, 19
+000259e0: 2c20 3230 2c20 3231 2c20 3232 2c20 3233  , 20, 21, 22, 23
+000259f0: 2c20 3234 2c20 3235 2c20 3236 2c20 3237  , 24, 25, 26, 27
+00025a00: 2c20 3238 2c20 3239 2c20 3330 2c20 3331  , 28, 29, 30, 31
+00025a10: 2c20 3332 2c20 3333 2c20 3334 2c20 3335  , 32, 33, 34, 35
+00025a20: 2c20 3336 2c20 3337 2c20 3338 2c20 3339  , 36, 37, 38, 39
+00025a30: 2c20 3430 2c20 3431 2c20 3432 2c20 3433  , 40, 41, 42, 43
+00025a40: 2c20 3434 2c20 3435 2c20 3436 2c20 3437  , 44, 45, 46, 47
+00025a50: 2c20 3438 2c20 3439 2c20 3530 2c20 3531  , 48, 49, 50, 51
+00025a60: 2c20 3532 2c20 3533 2c20 3534 2c20 3535  , 52, 53, 54, 55
+00025a70: 2c20 3536 2c20 3537 2c20 3538 2c20 3539  , 56, 57, 58, 59
+00025a80: 2c20 3630 2c20 3631 2c20 3632 2c20 3633  , 60, 61, 62, 63
+00025a90: 2c20 3634 2c20 3635 2c20 3636 2c20 3637  , 64, 65, 66, 67
+00025aa0: 2c20 3638 2c20 3639 2c20 3730 2c20 3731  , 68, 69, 70, 71
+00025ab0: 2c20 3732 2c20 3733 2c20 3734 2c20 3735  , 72, 73, 74, 75
+00025ac0: 2c20 3736 2c20 3737 2c20 3738 2c20 3739  , 76, 77, 78, 79
+00025ad0: 2c20 3830 2c20 3831 2c20 3832 2c20 3833  , 80, 81, 82, 83
+00025ae0: 2c20 3834 2c20 3835 2c20 3836 2c20 3837  , 84, 85, 86, 87
+00025af0: 2c20 3838 2c20 3839 2c20 3930 2c20 3931  , 88, 89, 90, 91
+00025b00: 2c20 3932 2c20 3933 2c20 3934 2c20 3935  , 92, 93, 94, 95
+00025b10: 2c20 3936 2c20 3937 2c20 3938 2c20 3939  , 96, 97, 98, 99
+00025b20: 2c20 3130 302c 2031 3031 2c20 3130 322c  , 100, 101, 102,
+00025b30: 2031 3033 2c20 3130 342c 2031 3035 2c20   103, 104, 105, 
+00025b40: 3130 362c 2031 3037 2c20 3130 382c 2031  106, 107, 108, 1
+00025b50: 3039 2c20 3131 302c 2031 3131 2c20 3131  09, 110, 111, 11
+00025b60: 322c 2031 3133 2c20 3131 342c 2031 3135  2, 113, 114, 115
+00025b70: 2c20 3131 362c 2031 3137 2c20 3131 382c  , 116, 117, 118,
+00025b80: 2031 3139 2c20 3132 302c 2031 3231 2c20   119, 120, 121, 
+00025b90: 3132 322c 2031 3233 2c20 3132 342c 2031  122, 123, 124, 1
+00025ba0: 3235 2c20 3132 362c 2031 3237 2c20 3132  25, 126, 127, 12
+00025bb0: 382c 2031 3239 2c20 3133 302c 2031 3331  8, 129, 130, 131
+00025bc0: 2c20 3133 322c 2031 3333 2c20 3133 342c  , 132, 133, 134,
+00025bd0: 2031 3335 2c20 3133 362c 2031 3337 2c20   135, 136, 137, 
+00025be0: 3133 382c 2031 3339 2c20 3134 302c 2031  138, 139, 140, 1
+00025bf0: 3431 2c20 3134 322c 2031 3433 2c20 3134  41, 142, 143, 14
+00025c00: 342c 2031 3435 2c20 3134 362c 2031 3437  4, 145, 146, 147
+00025c10: 2c20 3134 382c 2031 3439 2c20 3135 302c  , 148, 149, 150,
+00025c20: 2031 3531 2c20 3135 322c 2031 3533 2c20   151, 152, 153, 
+00025c30: 3135 342c 2031 3535 2c20 3135 362c 2031  154, 155, 156, 1
+00025c40: 3537 2c20 3135 382c 2031 3539 2c20 3136  57, 158, 159, 16
+00025c50: 302c 2031 3631 2c20 3136 322c 2031 3633  0, 161, 162, 163
+00025c60: 2c20 3136 342c 2031 3635 2c20 3136 362c  , 164, 165, 166,
+00025c70: 2031 3637 2c20 3136 382c 2031 3639 2c20   167, 168, 169, 
+00025c80: 3137 302c 2031 3731 2c20 3137 322c 2031  170, 171, 172, 1
+00025c90: 3733 2c20 3137 342c 2031 3735 2c20 3137  73, 174, 175, 17
+00025ca0: 362c 2031 3737 2c20 3137 382c 2031 3739  6, 177, 178, 179
+00025cb0: 2c20 3138 302c 2031 3831 2c20 3138 322c  , 180, 181, 182,
+00025cc0: 2031 3833 2c20 3138 342c 2031 3835 2c20   183, 184, 185, 
+00025cd0: 3138 362c 2031 3837 2c20 3138 382c 2031  186, 187, 188, 1
+00025ce0: 3839 2c20 3139 302c 2031 3931 2c20 3139  89, 190, 191, 19
+00025cf0: 322c 2031 3933 2c20 3139 342c 2031 3935  2, 193, 194, 195
+00025d00: 2c20 3139 362c 2031 3937 2c20 3139 382c  , 196, 197, 198,
+00025d10: 2031 3939 2c20 3230 302c 2032 3031 2c20   199, 200, 201, 
+00025d20: 3230 322c 2032 3033 2c20 3230 342c 2032  202, 203, 204, 2
+00025d30: 3035 2c20 3230 362c 2032 3037 2c20 3230  05, 206, 207, 20
+00025d40: 382c 2032 3039 2c20 3231 302c 2032 3131  8, 209, 210, 211
+00025d50: 2c20 3231 322c 2032 3133 2c20 3231 342c  , 212, 213, 214,
+00025d60: 2032 3135 2c20 3231 362c 2032 3137 2c20   215, 216, 217, 
+00025d70: 3231 382c 2032 3139 2c20 3232 302c 2032  218, 219, 220, 2
+00025d80: 3231 2c20 3232 322c 2032 3233 2c20 3232  21, 222, 223, 22
+00025d90: 342c 2032 3235 2c20 3232 362c 2032 3237  4, 225, 226, 227
+00025da0: 2c20 3232 382c 2032 3239 2c20 3233 302c  , 228, 229, 230,
+00025db0: 2032 3331 2c20 3233 322c 2032 3333 2c20   231, 232, 233, 
+00025dc0: 3233 342c 2032 3335 2c20 3233 362c 2032  234, 235, 236, 2
+00025dd0: 3337 2c20 3233 382c 2032 3339 2c20 3234  37, 238, 239, 24
+00025de0: 302c 2032 3431 2c20 3234 322c 2032 3433  0, 241, 242, 243
+00025df0: 2c20 3234 342c 2032 3435 2c20 3234 362c  , 244, 245, 246,
+00025e00: 2032 3437 2c20 3234 382c 2032 3439 2c20   247, 248, 249, 
+00025e10: 3235 302c 2032 3531 2c20 3235 322c 2032  250, 251, 252, 2
+00025e20: 3533 2c20 3235 342c 2032 3535 2c20 3235  53, 254, 255, 25
+00025e30: 362c 2032 3537 2c20 3235 382c 2032 3539  6, 257, 258, 259
+00025e40: 2c20 3236 302c 2032 3631 2c20 3236 322c  , 260, 261, 262,
+00025e50: 2032 3633 2c20 3236 342c 2032 3635 2c20   263, 264, 265, 
+00025e60: 3236 362c 2032 3637 2c20 3236 382c 2032  266, 267, 268, 2
+00025e70: 3639 2c20 3237 302c 2032 3731 2c20 3237  69, 270, 271, 27
+00025e80: 322c 2032 3733 2c20 3237 342c 2032 3735  2, 273, 274, 275
+00025e90: 2c20 3237 362c 2032 3737 2c20 3237 382c  , 276, 277, 278,
+00025ea0: 2032 3739 2c20 3238 302c 2032 3831 2c20   279, 280, 281, 
+00025eb0: 3238 322c 2032 3833 2c20 3238 342c 2032  282, 283, 284, 2
+00025ec0: 3835 2c20 3238 362c 2032 3837 2c20 3238  85, 286, 287, 28
+00025ed0: 382c 2032 3839 2c20 3239 302c 2032 3931  8, 289, 290, 291
+00025ee0: 2c20 3239 322c 2032 3933 2c20 3239 342c  , 292, 293, 294,
+00025ef0: 2032 3935 2c20 3239 362c 2032 3937 2c20   295, 296, 297, 
+00025f00: 3239 382c 2032 3939 2c20 3330 302c 2033  298, 299, 300, 3
+00025f10: 3031 2c20 3330 322c 2033 3033 2c20 3330  01, 302, 303, 30
+00025f20: 342c 2033 3035 2c20 3330 362c 2033 3037  4, 305, 306, 307
+00025f30: 2c20 3330 382c 2033 3039 2c20 3331 302c  , 308, 309, 310,
+00025f40: 2033 3131 2c20 3331 322c 2033 3133 2c20   311, 312, 313, 
+00025f50: 3331 342c 2033 3135 2c20 3331 362c 2033  314, 315, 316, 3
+00025f60: 3137 2c20 3331 382c 2033 3139 2c20 3332  17, 318, 319, 32
+00025f70: 302c 2033 3231 2c20 3332 322c 2033 3233  0, 321, 322, 323
+00025f80: 2c20 3332 342c 2033 3235 2c20 3332 362c  , 324, 325, 326,
+00025f90: 2033 3237 2c20 3332 382c 2033 3239 2c20   327, 328, 329, 
+00025fa0: 3333 302c 2033 3331 2c20 3333 322c 2033  330, 331, 332, 3
+00025fb0: 3333 2c20 3333 342c 2033 3335 2c20 3333  33, 334, 335, 33
+00025fc0: 362c 2033 3337 2c20 3333 382c 2033 3339  6, 337, 338, 339
+00025fd0: 2c20 3334 302c 2033 3431 2c20 3334 322c  , 340, 341, 342,
+00025fe0: 2033 3433 2c20 3334 342c 2033 3435 2c20   343, 344, 345, 
+00025ff0: 3334 362c 2033 3437 2c20 3334 382c 2033  346, 347, 348, 3
+00026000: 3439 2c20 3335 302c 2033 3531 2c20 3335  49, 350, 351, 35
+00026010: 322c 2033 3533 2c20 3335 342c 2033 3535  2, 353, 354, 355
+00026020: 2c20 3335 362c 2033 3537 2c20 3335 382c  , 356, 357, 358,
+00026030: 2033 3539 2c20 3336 302c 2033 3631 2c20   359, 360, 361, 
+00026040: 3336 322c 2033 3633 2c20 3336 342c 2033  362, 363, 364, 3
+00026050: 3635 205d 0d0a 0d0a 2323 2323 2323 2323  65 ]....########
+00026060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000260a0: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
+000260b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000260c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000260d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000260e0: 2323 2323 2323 2323 2323 2323 0d0a 2346  ############..#F
+000260f0: 756e 6374 696f 6e20 666f 7220 6765 7474  unction for gett
+00026100: 696e 6720 7468 6520 6461 7465 206f 6620  ing the date of 
+00026110: 7468 6520 7065 616b 206f 6620 7665 6720  the peak of veg 
+00026120: 7669 676f 722d 2063 616e 2068 616e 646c  vigor- can handl
+00026130: 6520 6261 6e64 7320 6e65 6761 7469 7665  e bands negative
+00026140: 6c79 2063 6f72 7265 6c61 7465 6420 746f  ly correlated to
+00026150: 2076 6567 2069 6e0d 0a23 6368 616e 6765   veg in..#change
+00026160: 4469 7244 6963 7420 6469 6374 696f 6e61  DirDict dictiona
+00026170: 7279 2061 626f 7665 0d0a 6465 6620 6765  ry above..def ge
+00026180: 7450 6561 6b44 6174 6528 636f 6566 6673  tPeakDate(coeffs
+00026190: 2c70 6561 6b44 6972 6563 7469 6f6e 203d  ,peakDirection =
+000261a0: 2031 293a 0d0a 0d0a 2020 7369 6e20 3d20   1):....  sin = 
+000261b0: 636f 6566 6673 2e73 656c 6563 7428 5b30  coeffs.select([0
+000261c0: 5d29 0d0a 2020 636f 7320 3d20 636f 6566  ])..  cos = coef
+000261d0: 6673 2e73 656c 6563 7428 5b31 5d29 0d0a  fs.select([1])..
+000261e0: 0d0a 2020 2346 696e 6420 7768 6572 6520  ..  #Find where 
+000261f0: 696e 2063 7963 6c65 2073 6c6f 7065 2069  in cycle slope i
+00026200: 7320 7a65 726f 0d0a 2020 6772 6565 6e44  s zero..  greenD
+00026210: 6174 6520 3d20 2828 7369 6e2e 6469 7669  ate = ((sin.divi
+00026220: 6465 2863 6f73 2929 2e61 7461 6e28 2929  de(cos)).atan())
+00026230: 2e64 6976 6964 6528 322a 6d61 7468 2e70  .divide(2*math.p
+00026240: 6929 2e72 656e 616d 6528 5b27 7065 616b  i).rename(['peak
+00026250: 4461 7465 275d 290d 0a20 2067 7265 656e  Date'])..  green
+00026260: 4461 7465 4c61 7465 7220 3d20 6772 6565  DateLater = gree
+00026270: 6e44 6174 652e 6164 6428 302e 3529 0d0a  nDate.add(0.5)..
+00026280: 2020 2343 6865 636b 2077 6869 6368 2064    #Check which d
+00026290: 3120 736c 6f70 6520 3d20 3020 6973 2074  1 slope = 0 is t
+000262a0: 6865 206d 6178 2062 7920 7072 6564 6963  he max by predic
+000262b0: 7469 6e67 206f 7574 2074 6865 2076 616c  ting out the val
+000262c0: 7565 0d0a 2020 7072 6564 6963 7465 6431  ue..  predicted1
+000262d0: 203d 2063 6f65 6666 732e 7365 6c65 6374   = coeffs.select
+000262e0: 285b 305d 295c 0d0a 2020 2020 2020 2020  ([0])\..        
+000262f0: 2020 2020 2020 2e61 6464 2873 696e 2e6d        .add(sin.m
+00026300: 756c 7469 706c 7928 6772 6565 6e44 6174  ultiply(greenDat
+00026310: 652e 6d75 6c74 6970 6c79 2832 2a6d 6174  e.multiply(2*mat
+00026320: 682e 7069 292e 7369 6e28 2929 295c 0d0a  h.pi).sin()))\..
+00026330: 2020 2020 2020 2020 2020 2020 2020 2e61                .a
+00026340: 6464 2863 6f73 2e6d 756c 7469 706c 7928  dd(cos.multiply(
+00026350: 6772 6565 6e44 6174 652e 6d75 6c74 6970  greenDate.multip
+00026360: 6c79 2832 2a6d 6174 682e 7069 292e 636f  ly(2*math.pi).co
+00026370: 7328 2929 295c 0d0a 2020 2020 2020 2020  s()))\..        
+00026380: 2020 2020 2020 2e72 656e 616d 6528 5b27        .rename(['
+00026390: 7072 6564 6963 7465 6427 5d29 5c0d 0a20  predicted'])\.. 
+000263a0: 2020 2020 2020 2020 2020 2020 202e 6d75               .mu
+000263b0: 6c74 6970 6c79 2865 652e 496d 6167 652e  ltiply(ee.Image.
+000263c0: 636f 6e73 7461 6e74 2870 6561 6b44 6972  constant(peakDir
+000263d0: 6563 7469 6f6e 2929 5c0d 0a20 2020 2020  ection))\..     
+000263e0: 2020 2020 2020 2020 202e 6164 6442 616e           .addBan
+000263f0: 6473 2867 7265 656e 4461 7465 290d 0a20  ds(greenDate).. 
+00026400: 2070 7265 6469 6374 6564 3220 3d20 636f   predicted2 = co
+00026410: 6566 6673 2e73 656c 6563 7428 5b30 5d29  effs.select([0])
+00026420: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+00026430: 202e 6164 6428 7369 6e2e 6d75 6c74 6970   .add(sin.multip
+00026440: 6c79 2867 7265 656e 4461 7465 4c61 7465  ly(greenDateLate
+00026450: 722e 6d75 6c74 6970 6c79 2832 2a6d 6174  r.multiply(2*mat
+00026460: 682e 7069 292e 7369 6e28 2929 295c 0d0a  h.pi).sin()))\..
+00026470: 2020 2020 2020 2020 2020 2020 2020 2e61                .a
+00026480: 6464 2863 6f73 2e6d 756c 7469 706c 7928  dd(cos.multiply(
+00026490: 6772 6565 6e44 6174 654c 6174 6572 2e6d  greenDateLater.m
+000264a0: 756c 7469 706c 7928 322a 6d61 7468 2e70  ultiply(2*math.p
+000264b0: 6929 2e63 6f73 2829 2929 5c0d 0a20 2020  i).cos()))\..   
+000264c0: 2020 2020 2020 2020 2020 202e 7265 6e61             .rena
+000264d0: 6d65 285b 2770 7265 6469 6374 6564 275d  me(['predicted']
+000264e0: 295c 0d0a 2020 2020 2020 2020 2020 2020  )\..            
+000264f0: 2020 2e6d 756c 7469 706c 7928 6565 2e49    .multiply(ee.I
+00026500: 6d61 6765 2e63 6f6e 7374 616e 7428 7065  mage.constant(pe
+00026510: 616b 4469 7265 6374 696f 6e29 295c 0d0a  akDirection))\..
+00026520: 2020 2020 2020 2020 2020 2020 2020 2e61                .a
+00026530: 6464 4261 6e64 7328 6772 6565 6e44 6174  ddBands(greenDat
+00026540: 654c 6174 6572 290d 0a20 2066 696e 616c  eLater)..  final
+00026550: 4772 6565 6e44 6174 6520 3d20 6565 2e49  GreenDate = ee.I
+00026560: 6d61 6765 436f 6c6c 6563 7469 6f6e 285b  mageCollection([
+00026570: 7072 6564 6963 7465 6431 2c70 7265 6469  predicted1,predi
+00026580: 6374 6564 325d 292e 7175 616c 6974 794d  cted2]).qualityM
+00026590: 6f73 6169 6328 2770 7265 6469 6374 6564  osaic('predicted
+000265a0: 2729 2e73 656c 6563 7428 5b27 7065 616b  ').select(['peak
+000265b0: 4461 7465 275d 292e 7265 6e61 6d65 285b  Date']).rename([
+000265c0: 2770 6561 6b4a 756c 6961 6e44 6179 275d  'peakJulianDay']
+000265d0: 290d 0a0d 0a20 2066 696e 616c 4772 6565  )....  finalGree
+000265e0: 6e44 6174 6520 3d20 6669 6e61 6c47 7265  nDate = finalGre
+000265f0: 656e 4461 7465 2e77 6865 7265 2866 696e  enDate.where(fin
+00026600: 616c 4772 6565 6e44 6174 652e 6c74 2830  alGreenDate.lt(0
+00026610: 292c 2067 7265 656e 4461 7465 2e61 6464  ), greenDate.add
+00026620: 2831 2929 2e6d 756c 7469 706c 7928 3336  (1)).multiply(36
+00026630: 3529 2e69 6e74 3136 2829 3b0d 0a0d 0a20  5).int16();.... 
+00026640: 2023 436f 6e76 6572 7420 746f 206d 6f6e   #Convert to mon
+00026650: 7468 2061 6e64 2064 6179 206f 6620 6d6f  th and day of mo
+00026660: 6e74 680d 0a20 2067 7265 656e 4d6f 6e74  nth..  greenMont
+00026670: 6820 3d20 6669 6e61 6c47 7265 656e 4461  h = finalGreenDa
+00026680: 7465 2e72 656d 6170 286a 756c 6961 6e44  te.remap(julianD
+00026690: 6179 2c6d 6f6e 7468 5265 6d61 7029 2e72  ay,monthRemap).r
+000266a0: 656e 616d 6528 5b27 7065 616b 4d6f 6e74  ename(['peakMont
+000266b0: 6827 5d29 0d0a 2020 6772 6565 6e4d 6f6e  h'])..  greenMon
+000266c0: 7468 4461 7920 3d20 6669 6e61 6c47 7265  thDay = finalGre
+000266d0: 656e 4461 7465 2e72 656d 6170 286a 756c  enDate.remap(jul
+000266e0: 6961 6e44 6179 2c6d 6f6e 7468 4461 7952  ianDay,monthDayR
+000266f0: 656d 6170 292e 7265 6e61 6d65 285b 2770  emap).rename(['p
+00026700: 6561 6b44 6179 4f66 4d6f 6e74 6827 5d29  eakDayOfMonth'])
+00026710: 0d0a 2020 6772 6565 6e53 7461 636b 203d  ..  greenStack =
+00026720: 2066 696e 616c 4772 6565 6e44 6174 652e   finalGreenDate.
+00026730: 6164 6442 616e 6473 2867 7265 656e 4d6f  addBands(greenMo
+00026740: 6e74 6829 2e61 6464 4261 6e64 7328 6772  nth).addBands(gr
+00026750: 6565 6e4d 6f6e 7468 4461 7929 0d0a 2020  eenMonthDay)..  
+00026760: 7265 7475 726e 2067 7265 656e 5374 6163  return greenStac
+00026770: 6b0d 0a20 2023 4d61 702e 6164 644c 6179  k..  #Map.addLay
+00026780: 6572 2867 7265 656e 5374 6163 6b2c 7b27  er(greenStack,{'
+00026790: 6d69 6e27 3a31 2c27 6d61 7827 3a31 327d  min':1,'max':12}
+000267a0: 2c27 6772 6565 6e4d 6f6e 7468 272c 4661  ,'greenMonth',Fa
+000267b0: 6c73 6529 0d0a 0d0a 2323 2323 2323 2323  lse)....########
+000267c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000267d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000267e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000267f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026800: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
+00026810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026840: 2323 2323 2323 2323 2323 2323 0d0a 2346  ############..#F
+00026850: 756e 6374 696f 6e20 666f 7220 6765 7474  unction for gett
+00026860: 696e 6720 6c65 6674 2073 756d 2075 6e64  ing left sum und
+00026870: 6572 2074 6865 2063 7572 7665 2066 6f72  er the curve for
+00026880: 2061 2073 696e 676c 6520 6772 6f77 696e   a single growin
+00026890: 6720 7365 6173 6f6e 0d0a 2354 616b 6573  g season..#Takes
+000268a0: 2063 6172 6520 6f66 206e 6f72 6d61 6c69   care of normali
+000268b0: 7a61 7469 6f6e 2062 7920 666f 7263 696e  zation by forcin
+000268c0: 6720 7468 6520 6d69 6e20 7661 6c75 6520  g the min value 
+000268d0: 616c 6f6e 6720 7468 6520 6375 7276 6520  along the curve 
+000268e0: 300d 0a23 6279 2074 616b 696e 6720 7468  0..#by taking th
+000268f0: 6520 616d 706c 6974 7564 6520 6173 2074  e amplitude as t
+00026900: 6865 2069 6e74 6572 6365 7074 0d0a 2341  he intercept..#A
+00026910: 7373 756d 6573 2074 6865 2073 696e 2061  ssumes the sin a
+00026920: 6e64 2063 6f73 2063 6f65 6666 7320 6172  nd cos coeffs ar
+00026930: 6520 7468 6520 6861 726d 436f 6566 6673  e the harmCoeffs
+00026940: 0d0a 2374 3020 6973 2074 6865 2073 7461  ..#t0 is the sta
+00026950: 7274 2074 696d 6520 2864 6566 6175 6c74  rt time (default
+00026960: 7320 746f 2030 2928 6d69 6e20 7661 6c75  s to 0)(min valu
+00026970: 6520 7368 6f75 6c64 2062 6520 6275 7420  e should be but 
+00026980: 646f 6573 6e27 7420 6861 7665 2074 6f20  doesn't have to 
+00026990: 6265 2030 290d 0a23 7431 2069 7320 7468  be 0)..#t1 is th
+000269a0: 6520 656e 6420 7469 6d65 2028 6465 6661  e end time (defa
+000269b0: 756c 7473 2074 6f20 3129 286d 6178 2076  ults to 1)(max v
+000269c0: 616c 7565 2073 686f 756c 6420 6265 2062  alue should be b
+000269d0: 7574 2064 6f65 736e 2774 2068 6176 6520  ut doesn't have 
+000269e0: 746f 2062 6520 3129 0d0a 0d0a 2345 7861  to be 1)....#Exa
+000269f0: 6d70 6c65 206f 6620 7768 6174 2074 6869  mple of what thi
+00026a00: 7320 636f 6465 2069 7320 646f 696e 6720  s code is doing 
+00026a10: 6361 6e20 6265 2066 6f75 6e64 2068 6572  can be found her
+00026a20: 653a 0d0a 2320 2068 7474 703a 2f2f 7777  e:..#  http://ww
+00026a30: 772e 776f 6c66 7261 6d61 6c70 6861 2e63  w.wolframalpha.c
+00026a40: 6f6d 2f69 6e70 7574 2f3f 693d 696e 7465  om/input/?i=inte
+00026a50: 6772 6174 652b 302e 3135 3934 3930 3734  grate+0.15949074
+00026a60: 3932 3339 3932 3135 372b 2532 422b 2d30  923992157+%2B+-0
+00026a70: 2e30 3832 3837 3539 392a 7369 6e28 322b  .08287599*sin(2+
+00026a80: 5049 2b54 292b 2532 422b 2d30 2e31 3132  PI+T)+%2B+-0.112
+00026a90: 3532 3031 3036 3133 2a63 6f73 2832 2b50  52010613*cos(2+P
+00026aa0: 492b 5429 2b2b 6672 6f6d 2b30 2b74 6f2b  I+T)++from+0+to+
+00026ab0: 310d 0a64 6566 2067 6574 4172 6561 556e  1..def getAreaUn
+00026ac0: 6465 7243 7572 7665 2868 6172 6d43 6f65  derCurve(harmCoe
+00026ad0: 6666 732c 7430 3d20 302c 7431 203d 2031  ffs,t0= 0,t1 = 1
+00026ae0: 293a 0d0a 0d0a 2020 2350 756c 6c20 6170  ):....  #Pull ap
+00026af0: 6172 7420 7468 6520 6d6f 6465 6c0d 0a20  art the model.. 
+00026b00: 2061 6d70 6c69 7475 6465 203d 2068 6172   amplitude = har
+00026b10: 6d43 6f65 6666 732e 7365 6c65 6374 285b  mCoeffs.select([
+00026b20: 315d 292e 6879 706f 7428 6861 726d 436f  1]).hypot(harmCo
+00026b30: 6566 6673 2e73 656c 6563 7428 5b30 5d29  effs.select([0])
+00026b40: 290d 0a20 2069 6e74 6572 6563 6570 744e  )..  intereceptN
+00026b50: 6f72 6d61 6c69 7a65 6420 3d20 616d 706c  ormalized = ampl
+00026b60: 6974 7564 6523 5768 656e 206d 616b 696e  itude#When makin
+00026b70: 6720 7468 6520 6d69 6e20 302c 2074 6865  g the min 0, the
+00026b80: 2069 6e74 6572 6365 7074 2062 6563 6f6d   intercept becom
+00026b90: 6573 2074 6865 2061 6d70 6c69 7475 6465  es the amplitude
+00026ba0: 2028 7468 6520 6879 706f 7465 6e75 7365   (the hypotenuse
+00026bb0: 290d 0a20 2073 696e 203d 2068 6172 6d43  )..  sin = harmC
+00026bc0: 6f65 6666 732e 7365 6c65 6374 285b 305d  oeffs.select([0]
+00026bd0: 290d 0a20 2063 6f73 203d 2068 6172 6d43  )..  cos = harmC
+00026be0: 6f65 6666 732e 7365 6c65 6374 285b 315d  oeffs.select([1]
+00026bf0: 290d 0a0d 0a20 2023 4669 6e64 2074 6865  )....  #Find the
+00026c00: 2073 756d 2066 726f 6d20 2d20 696e 6669   sum from - infi
+00026c10: 6e69 7479 2074 6f20 300d 0a20 2073 756d  nity to 0..  sum
+00026c20: 3020 3d20 696e 7465 7265 6365 7074 4e6f  0 = intereceptNo
+00026c30: 726d 616c 697a 6564 2e6d 756c 7469 706c  rmalized.multipl
+00026c40: 7928 7430 295c 0d0a 2020 2020 2020 2020  y(t0)\..        
+00026c50: 2020 2020 2e73 7562 7472 6163 7428 7369      .subtract(si
+00026c60: 6e2e 6469 7669 6465 2832 2a6d 6174 682e  n.divide(2*math.
+00026c70: 7069 292e 6d75 6c74 6970 6c79 286d 6174  pi).multiply(mat
+00026c80: 682e 7369 6e28 322a 6d61 7468 2e70 692a  h.sin(2*math.pi*
+00026c90: 7430 2929 295c 0d0a 2020 2020 2020 2020  t0)))\..        
+00026ca0: 2020 2020 2e61 6464 2863 6f73 2e64 6976      .add(cos.div
+00026cb0: 6964 6528 322a 6d61 7468 2e70 6929 2e6d  ide(2*math.pi).m
+00026cc0: 756c 7469 706c 7928 6d61 7468 2e63 6f73  ultiply(math.cos
+00026cd0: 2832 2a6d 6174 682e 7069 2a74 3029 2929  (2*math.pi*t0)))
+00026ce0: 0d0a 2020 2346 696e 6420 7468 6520 7375  ..  #Find the su
+00026cf0: 6d20 6672 6f6d 202d 2069 6e66 696e 6974  m from - infinit
+00026d00: 7920 746f 2031 0d0a 2020 7375 6d31 203d  y to 1..  sum1 =
+00026d10: 2069 6e74 6572 6563 6570 744e 6f72 6d61   intereceptNorma
+00026d20: 6c69 7a65 642e 6d75 6c74 6970 6c79 2874  lized.multiply(t
+00026d30: 3129 5c0d 0a20 2020 2020 2020 202e 7375  1)\..        .su
+00026d40: 6274 7261 6374 2873 696e 2e64 6976 6964  btract(sin.divid
+00026d50: 6528 322a 6d61 7468 2e70 6929 2e6d 756c  e(2*math.pi).mul
+00026d60: 7469 706c 7928 6d61 7468 2e73 696e 2832  tiply(math.sin(2
+00026d70: 2a6d 6174 682e 7069 2a74 3129 2929 5c0d  *math.pi*t1)))\.
+00026d80: 0a20 2020 2020 2020 202e 6164 6428 636f  .        .add(co
+00026d90: 732e 6469 7669 6465 2832 2a6d 6174 682e  s.divide(2*math.
+00026da0: 7069 292e 6d75 6c74 6970 6c79 286d 6174  pi).multiply(mat
+00026db0: 682e 636f 7328 322a 6d61 7468 2e70 692a  h.cos(2*math.pi*
+00026dc0: 7431 2929 290d 0a20 2023 4669 6e64 2074  t1)))..  #Find t
+00026dd0: 6865 2064 6966 6665 7265 6e63 650d 0a20  he difference.. 
+00026de0: 206c 6566 7453 756d 203d 2073 756d 312e   leftSum = sum1.
+00026df0: 7375 6274 7261 6374 2873 756d 3029 2e72  subtract(sum0).r
+00026e00: 656e 616d 6528 5b27 4155 4327 5d29 0d0a  ename(['AUC'])..
+00026e10: 2020 7265 7475 726e 206c 6566 7453 756d    return leftSum
+00026e20: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
+00026e30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026e40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026e60: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+00026e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026e90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026eb0: 2323 2323 2323 2323 0d0a 6465 6620 6765  ########..def ge
+00026ec0: 7450 6861 7365 416d 706c 6974 7564 6550  tPhaseAmplitudeP
+00026ed0: 6561 6b28 636f 6566 6673 2c74 3020 3d20  eak(coeffs,t0 = 
+00026ee0: 302c 7431 203d 2031 293a 0d0a 2020 2350  0,t1 = 1):..  #P
+00026ef0: 6172 7365 2074 6865 206d 6f64 656c 0d0a  arse the model..
+00026f00: 2020 6261 6e64 4e61 6d65 7320 3d20 636f    bandNames = co
+00026f10: 6566 6673 2e62 616e 644e 616d 6573 2829  effs.bandNames()
+00026f20: 0d0a 2020 6261 6e64 4e75 6d62 6572 203d  ..  bandNumber =
+00026f30: 2062 616e 644e 616d 6573 2e6c 656e 6774   bandNames.lengt
+00026f40: 6828 290d 0a20 206e 6f44 6570 656e 6465  h()..  noDepende
+00026f50: 6e74 7320 3d20 6565 2e4e 756d 6265 7228  nts = ee.Number(
+00026f60: 636f 6566 6673 2e67 6574 2827 6e6f 4465  coeffs.get('noDe
+00026f70: 7065 6e64 656e 7473 2729 290d 0a20 206d  pendents'))..  m
+00026f80: 6f64 656c 4c65 6e67 7468 203d 2065 652e  odelLength = ee.
+00026f90: 4e75 6d62 6572 2863 6f65 6666 732e 6765  Number(coeffs.ge
+00026fa0: 7428 276d 6f64 656c 4c65 6e67 7468 2729  t('modelLength')
+00026fb0: 290d 0a20 2069 6e74 6572 6365 7074 4261  )..  interceptBa
+00026fc0: 6e64 7320 3d20 6565 2e4c 6973 742e 7365  nds = ee.List.se
+00026fd0: 7175 656e 6365 2830 2c62 616e 644e 756d  quence(0,bandNum
+00026fe0: 6265 722e 7375 6274 7261 6374 2831 292c  ber.subtract(1),
+00026ff0: 6d6f 6465 6c4c 656e 6774 6829 0d0a 0d0a  modelLength)....
+00027000: 2020 6d6f 6465 6c73 203d 2065 652e 4c69    models = ee.Li
+00027010: 7374 2e73 6571 7565 6e63 6528 302c 6e6f  st.sequence(0,no
+00027020: 4465 7065 6e64 656e 7473 2e73 7562 7472  Dependents.subtr
+00027030: 6163 7428 3129 290d 0a0d 0a20 2064 6566  act(1))....  def
+00027040: 206d 6f64 656c 4765 7474 6572 286d 6e29   modelGetter(mn)
+00027050: 3a0d 0a20 2020 206d 6e20 3d20 6565 2e4e  :..    mn = ee.N
+00027060: 756d 6265 7228 6d6e 290d 0a20 2020 2072  umber(mn)..    r
+00027070: 6574 7572 6e20 6261 6e64 4e61 6d65 732e  eturn bandNames.
+00027080: 736c 6963 6528 6d6e 2e6d 756c 7469 706c  slice(mn.multipl
+00027090: 7928 6d6f 6465 6c4c 656e 6774 6829 2c6d  y(modelLength),m
+000270a0: 6e2e 6d75 6c74 6970 6c79 286d 6f64 656c  n.multiply(model
+000270b0: 4c65 6e67 7468 292e 6164 6428 6d6f 6465  Length).add(mode
+000270c0: 6c4c 656e 6774 6829 290d 0a0d 0a20 2070  lLength))....  p
+000270d0: 6172 7365 644d 6f64 656c 203d 6d6f 6465  arsedModel =mode
+000270e0: 6c73 2e6d 6170 286d 6f64 656c 4765 7474  ls.map(modelGett
+000270f0: 6572 290d 0a0d 0a0d 0a20 2023 7072 696e  er)......  #prin
+00027100: 7428 2750 6172 7365 6420 6861 726d 6f6e  t('Parsed harmon
+00027110: 6963 2072 6567 7265 7373 696f 6e20 6d6f  ic regression mo
+00027120: 6465 6c27 2c70 6172 7365 644d 6f64 656c  del',parsedModel
+00027130: 290d 0a0d 0a20 2023 4974 6572 6174 6520  )....  #Iterate 
+00027140: 6163 726f 7373 206d 6f64 656c 7320 746f  across models to
+00027150: 2063 6f6e 7665 7274 2074 6f20 7068 6173   convert to phas
+00027160: 652c 2061 6d70 6c69 7475 6465 2c20 616e  e, amplitude, an
+00027170: 6420 7065 616b 0d0a 2020 6465 6620 7061  d peak..  def pa
+00027180: 7047 6574 7465 7228 706d 293a 0d0a 2020  pGetter(pm):..  
+00027190: 2020 706d 203d 2065 652e 4c69 7374 2870    pm = ee.List(p
+000271a0: 6d29 3b0d 0a20 2020 206d 6f64 656c 436f  m);..    modelCo
+000271b0: 6566 6673 203d 2063 6f65 6666 732e 7365  effs = coeffs.se
+000271c0: 6c65 6374 2870 6d29 0d0a 0d0a 2020 2020  lect(pm)....    
+000271d0: 696e 7465 7263 6570 7420 3d20 6d6f 6465  intercept = mode
+000271e0: 6c43 6f65 6666 732e 7365 6c65 6374 2827  lCoeffs.select('
+000271f0: 2e2a 5f69 6e74 6572 6365 7074 2729 0d0a  .*_intercept')..
+00027200: 2020 2020 6861 726d 436f 6566 6673 203d      harmCoeffs =
+00027210: 206d 6f64 656c 436f 6566 6673 2e73 656c   modelCoeffs.sel
+00027220: 6563 7428 272e 2a5f 3230 305f 7965 6172  ect('.*_200_year
+00027230: 2729 0d0a 2020 2020 6f75 744e 616d 6520  ')..    outName 
+00027240: 3d20 6565 2e53 7472 696e 6728 6565 2e53  = ee.String(ee.S
+00027250: 7472 696e 6728 706d 2e67 6574 2831 2929  tring(pm.get(1))
+00027260: 2e73 706c 6974 2827 5f27 292e 6765 7428  .split('_').get(
+00027270: 3029 290d 0a20 2020 2073 6967 6e20 3d20  0))..    sign = 
+00027280: 6565 2e4e 756d 6265 7228 6565 2e44 6963  ee.Number(ee.Dic
+00027290: 7469 6f6e 6172 7928 6368 616e 6765 4469  tionary(changeDi
+000272a0: 7244 6963 7429 2e67 6574 286f 7574 4e61  rDict).get(outNa
+000272b0: 6d65 2929 2e6d 756c 7469 706c 7928 2d31  me)).multiply(-1
+000272c0: 290d 0a0d 0a20 2020 2061 6d70 6c69 7475  )....    amplitu
+000272d0: 6465 203d 2068 6172 6d43 6f65 6666 732e  de = harmCoeffs.
+000272e0: 7365 6c65 6374 285b 315d 292e 6879 706f  select([1]).hypo
+000272f0: 7428 6861 726d 436f 6566 6673 2e73 656c  t(harmCoeffs.sel
+00027300: 6563 7428 5b30 5d29 295c 0d0a 2020 2020  ect([0]))\..    
+00027310: 2020 2020 2020 2020 2020 2e6d 756c 7469            .multi
+00027320: 706c 7928 3229 5c0d 0a20 2020 2020 2020  ply(2)\..       
+00027330: 2020 2020 2020 202e 7265 6e61 6d65 285b         .rename([
+00027340: 6f75 744e 616d 652e 6361 7428 275f 616d  outName.cat('_am
+00027350: 706c 6974 7564 6527 295d 290d 0a20 2020  plitude')])..   
+00027360: 2070 6861 7365 203d 2068 6172 6d43 6f65   phase = harmCoe
+00027370: 6666 732e 7365 6c65 6374 285b 305d 292e  ffs.select([0]).
+00027380: 6174 616e 3228 6861 726d 436f 6566 6673  atan2(harmCoeffs
+00027390: 2e73 656c 6563 7428 5b31 5d29 295c 0d0a  .select([1]))\..
+000273a0: 2020 2020 2020 2020 2020 2020 2020 2e75                .u
+000273b0: 6e69 7453 6361 6c65 282d 6d61 7468 2e70  nitScale(-math.p
+000273c0: 692c 206d 6174 682e 7069 295c 0d0a 2020  i, math.pi)\..  
+000273d0: 2020 2020 2020 2020 2020 2020 2e72 656e              .ren
+000273e0: 616d 6528 5b6f 7574 4e61 6d65 2e63 6174  ame([outName.cat
+000273f0: 2827 5f70 6861 7365 2729 5d29 0d0a 0d0a  ('_phase')])....
+00027400: 2020 2020 2347 6574 2070 6561 6b20 6461      #Get peak da
+00027410: 7465 2069 6e66 6f0d 0a20 2020 2070 6561  te info..    pea
+00027420: 6b44 6174 6520 3d20 6765 7450 6561 6b44  kDate = getPeakD
+00027430: 6174 6528 6861 726d 436f 6566 6673 2c73  ate(harmCoeffs,s
+00027440: 6967 6e29 0d0a 2020 2020 7065 616b 4461  ign)..    peakDa
+00027450: 7465 4261 6e64 4e61 6d65 7320 3d20 7065  teBandNames = pe
+00027460: 616b 4461 7465 2e62 616e 644e 616d 6573  akDate.bandNames
+00027470: 2829 0d0a 2020 2020 7065 616b 4461 7465  ()..    peakDate
+00027480: 4261 6e64 4e61 6d65 7320 3d20 7065 616b  BandNames = peak
+00027490: 4461 7465 4261 6e64 4e61 6d65 732e 6d61  DateBandNames.ma
+000274a0: 7028 6c61 6d62 6461 2062 6e3a 206f 7574  p(lambda bn: out
+000274b0: 4e61 6d65 2e63 6174 2865 652e 5374 7269  Name.cat(ee.Stri
+000274c0: 6e67 2827 5f27 292e 6361 7428 6565 2e53  ng('_').cat(ee.S
+000274d0: 7472 696e 6728 626e 2929 2929 0d0a 0d0a  tring(bn))))....
+000274e0: 2020 2020 2347 6574 2074 6865 206c 6566      #Get the lef
+000274f0: 7420 7375 6d0d 0a20 2020 206c 6566 7453  t sum..    leftS
+00027500: 756d 203d 2067 6574 4172 6561 556e 6465  um = getAreaUnde
+00027510: 7243 7572 7665 2868 6172 6d43 6f65 6666  rCurve(harmCoeff
+00027520: 732c 7430 2c74 3129 0d0a 2020 2020 6c65  s,t0,t1)..    le
+00027530: 6674 5375 6d42 616e 644e 616d 6573 203d  ftSumBandNames =
+00027540: 206c 6566 7453 756d 2e62 616e 644e 616d   leftSum.bandNam
+00027550: 6573 2829 0d0a 2020 2020 6c65 6674 5375  es()..    leftSu
+00027560: 6d42 616e 644e 616d 6573 203d 206c 6566  mBandNames = lef
+00027570: 7453 756d 4261 6e64 4e61 6d65 732e 6d61  tSumBandNames.ma
+00027580: 7028 6c61 6d62 6461 2062 6e3a 206f 7574  p(lambda bn: out
+00027590: 4e61 6d65 2e63 6174 2865 652e 5374 7269  Name.cat(ee.Stri
+000275a0: 6e67 2827 5f27 292e 6361 7428 6565 2e53  ng('_').cat(ee.S
+000275b0: 7472 696e 6728 626e 2929 2929 0d0a 0d0a  tring(bn))))....
+000275c0: 2020 2020 7265 7475 726e 2061 6d70 6c69      return ampli
+000275d0: 7475 6465 5c0d 0a20 2020 2020 2020 2020  tude\..         
+000275e0: 2020 202e 6164 6442 616e 6473 2870 6861     .addBands(pha
+000275f0: 7365 295c 0d0a 2020 2020 2020 2020 2020  se)\..          
+00027600: 2020 2e61 6464 4261 6e64 7328 7065 616b    .addBands(peak
+00027610: 4461 7465 2e72 656e 616d 6528 7065 616b  Date.rename(peak
+00027620: 4461 7465 4261 6e64 4e61 6d65 7329 295c  DateBandNames))\
+00027630: 0d0a 2020 2020 2020 2020 2020 2020 2e61  ..            .a
+00027640: 6464 4261 6e64 7328 6c65 6674 5375 6d2e  ddBands(leftSum.
+00027650: 7265 6e61 6d65 286c 6566 7453 756d 4261  rename(leftSumBa
+00027660: 6e64 4e61 6d65 7329 290d 0a0d 0a0d 0a0d  ndNames)).......
+00027670: 0a20 2023 436f 6e76 6572 7420 746f 2061  .  #Convert to a
+00027680: 6e20 696d 6167 650d 0a20 2070 6861 7365  n image..  phase
+00027690: 416d 706c 6974 7564 6520 3d70 6172 7365  Amplitude =parse
+000276a0: 644d 6f64 656c 2e6d 6170 2870 6170 4765  dModel.map(papGe
+000276b0: 7474 6572 290d 0a0d 0a20 2070 6861 7365  tter)....  phase
+000276c0: 416d 706c 6974 7564 6520 3d20 6565 2e49  Amplitude = ee.I
+000276d0: 6d61 6765 436f 6c6c 6563 7469 6f6e 2e66  mageCollection.f
+000276e0: 726f 6d49 6d61 6765 7328 7068 6173 6541  romImages(phaseA
+000276f0: 6d70 6c69 7475 6465 290d 0a0d 0a20 2070  mplitude)....  p
+00027700: 6861 7365 416d 706c 6974 7564 6520 3d20  haseAmplitude = 
+00027710: 6565 2e49 6d61 6765 2863 6f6c 6c65 6374  ee.Image(collect
+00027720: 696f 6e54 6f49 6d61 6765 2870 6861 7365  ionToImage(phase
+00027730: 416d 706c 6974 7564 6529 292e 666c 6f61  Amplitude)).floa
+00027740: 7428 295c 0d0a 2020 2020 2020 2020 2e63  t()\..        .c
+00027750: 6f70 7950 726f 7065 7274 6965 7328 636f  opyProperties(co
+00027760: 6566 6673 2c5b 2773 7973 7465 6d3a 7469  effs,['system:ti
+00027770: 6d65 5f73 7461 7274 275d 290d 0a20 2023  me_start'])..  #
+00027780: 7072 696e 7428 2770 6127 2c70 6861 7365  print('pa',phase
+00027790: 416d 706c 6974 7564 6529 3b0d 0a20 2072  Amplitude);..  r
+000277a0: 6574 7572 6e20 7068 6173 6541 6d70 6c69  eturn phaseAmpli
+000277b0: 7475 6465 3b0d 0a0d 0a23 2323 2323 2323  tude;....#######
+000277c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000277d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000277e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000277f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027800: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+00027810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027840: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+00027850: 4675 6e63 7469 6f6e 2066 6f72 2061 7070  Function for app
+00027860: 6c79 696e 6720 6861 726d 6f6e 6963 2072  lying harmonic r
+00027870: 6567 7265 7373 696f 6e20 6d6f 6465 6c20  egression model 
+00027880: 746f 2073 6574 206f 6620 7072 6564 6963  to set of predic
+00027890: 746f 7220 7365 7473 0d0a 6465 6620 6e65  tor sets..def ne
+000278a0: 7750 7265 6469 6374 2863 6f65 6666 732c  wPredict(coeffs,
+000278b0: 6861 726d 6f6e 6963 7329 3a0d 0a20 2023  harmonics):..  #
+000278c0: 5061 7273 6520 7468 6520 6d6f 6465 6c0d  Parse the model.
+000278d0: 0a20 2062 616e 644e 616d 6573 203d 2063  .  bandNames = c
+000278e0: 6f65 6666 732e 6261 6e64 4e61 6d65 7328  oeffs.bandNames(
+000278f0: 290d 0a20 2062 616e 644e 756d 6265 7220  )..  bandNumber 
+00027900: 3d20 6261 6e64 4e61 6d65 732e 6c65 6e67  = bandNames.leng
+00027910: 7468 2829 0d0a 2020 6e6f 4465 7065 6e64  th()..  noDepend
+00027920: 656e 7473 203d 2065 652e 4e75 6d62 6572  ents = ee.Number
+00027930: 2863 6f65 6666 732e 6765 7428 276e 6f44  (coeffs.get('noD
+00027940: 6570 656e 6465 6e74 7327 2929 0d0a 2020  ependents'))..  
+00027950: 6d6f 6465 6c4c 656e 6774 6820 3d20 6565  modelLength = ee
+00027960: 2e4e 756d 6265 7228 636f 6566 6673 2e67  .Number(coeffs.g
+00027970: 6574 2827 6d6f 6465 6c4c 656e 6774 6827  et('modelLength'
+00027980: 2929 0d0a 2020 696e 7465 7263 6570 7442  ))..  interceptB
+00027990: 616e 6473 203d 2065 652e 4c69 7374 2e73  ands = ee.List.s
+000279a0: 6571 7565 6e63 6528 302c 6261 6e64 4e75  equence(0,bandNu
+000279b0: 6d62 6572 2e73 7562 7472 6163 7428 3129  mber.subtract(1)
+000279c0: 2c6d 6f64 656c 4c65 6e67 7468 290d 0a20  ,modelLength).. 
+000279d0: 2074 696d 6542 616e 6420 3d20 6565 2e4c   timeBand = ee.L
+000279e0: 6973 7428 6861 726d 6f6e 6963 732e 6765  ist(harmonics.ge
+000279f0: 7428 2769 6e64 4261 6e64 4e61 6d65 7327  t('indBandNames'
+00027a00: 2929 2e67 6574 2830 290d 0a20 2061 6374  )).get(0)..  act
+00027a10: 7561 6c42 616e 6473 203d 2068 6172 6d6f  ualBands = harmo
+00027a20: 6e69 6373 2e67 6574 2827 6465 7042 616e  nics.get('depBan
+00027a30: 644e 756d 6265 7273 2729 0d0a 2020 696e  dNumbers')..  in
+00027a40: 6442 616e 6473 203d 2068 6172 6d6f 6e69  dBands = harmoni
+00027a50: 6373 2e67 6574 2827 696e 6442 616e 644e  cs.get('indBandN
+00027a60: 756d 6265 7273 2729 0d0a 2020 696e 6442  umbers')..  indB
+00027a70: 616e 644e 616d 6573 203d 2065 652e 4c69  andNames = ee.Li
+00027a80: 7374 2868 6172 6d6f 6e69 6373 2e67 6574  st(harmonics.get
+00027a90: 2827 696e 6442 616e 644e 616d 6573 2729  ('indBandNames')
+00027aa0: 290d 0a20 2064 6570 4261 6e64 4e61 6d65  )..  depBandName
+00027ab0: 7320 3d20 6565 2e4c 6973 7428 6861 726d  s = ee.List(harm
+00027ac0: 6f6e 6963 732e 6765 7428 2764 6570 4261  onics.get('depBa
+00027ad0: 6e64 4e61 6d65 7327 2929 0d0a 2020 7072  ndNames'))..  pr
+00027ae0: 6564 6963 7465 6442 616e 644e 616d 6573  edictedBandNames
+00027af0: 203d 2064 6570 4261 6e64 4e61 6d65 732e   = depBandNames.
+00027b00: 6d61 7028 6c61 6d62 6461 2064 6570 626e  map(lambda depbn
+00027b10: 6d73 3a65 652e 5374 7269 6e67 2864 6570  ms:ee.String(dep
+00027b20: 626e 6d73 292e 6361 7428 275f 7072 6564  bnms).cat('_pred
+00027b30: 6963 7465 6427 2929 0d0a 2020 7072 6564  icted'))..  pred
+00027b40: 6963 7465 6442 616e 644e 756d 6265 7273  ictedBandNumbers
+00027b50: 203d 2065 652e 4c69 7374 2e73 6571 7565   = ee.List.seque
+00027b60: 6e63 6528 302c 7072 6564 6963 7465 6442  nce(0,predictedB
+00027b70: 616e 644e 616d 6573 2e6c 656e 6774 6828  andNames.length(
+00027b80: 292e 7375 6274 7261 6374 2831 2929 0d0a  ).subtract(1))..
+00027b90: 0d0a 2020 6d6f 6465 6c73 203d 2065 652e  ..  models = ee.
+00027ba0: 4c69 7374 2e73 6571 7565 6e63 6528 302c  List.sequence(0,
+00027bb0: 6e6f 4465 7065 6e64 656e 7473 2e73 7562  noDependents.sub
+00027bc0: 7472 6163 7428 3129 290d 0a20 2064 6566  tract(1))..  def
+00027bd0: 206d 6e47 6574 7465 7228 6d6e 293a 0d0a   mnGetter(mn):..
+00027be0: 2020 2020 6d6e 203d 2065 652e 4e75 6d62      mn = ee.Numb
+00027bf0: 6572 286d 6e29 0d0a 2020 2020 7265 7475  er(mn)..    retu
+00027c00: 726e 2062 616e 644e 616d 6573 2e73 6c69  rn bandNames.sli
+00027c10: 6365 286d 6e2e 6d75 6c74 6970 6c79 286d  ce(mn.multiply(m
+00027c20: 6f64 656c 4c65 6e67 7468 292c 6d6e 2e6d  odelLength),mn.m
+00027c30: 756c 7469 706c 7928 6d6f 6465 6c4c 656e  ultiply(modelLen
+00027c40: 6774 6829 2e61 6464 286d 6f64 656c 4c65  gth).add(modelLe
+00027c50: 6e67 7468 2929 0d0a 0d0a 2020 7061 7273  ngth))....  pars
+00027c60: 6564 4d6f 6465 6c20 3d6d 6f64 656c 732e  edModel =models.
+00027c70: 6d61 7028 6d6e 4765 7474 6572 290d 0a0d  map(mnGetter)...
+00027c80: 0a20 2023 7072 696e 7428 2750 6172 7365  .  #print('Parse
+00027c90: 6420 6861 726d 6f6e 6963 2072 6567 7265  d harmonic regre
+00027ca0: 7373 696f 6e20 6d6f 6465 6c27 2c70 6172  ssion model',par
+00027cb0: 7365 644d 6f64 656c 2c70 7265 6469 6374  sedModel,predict
+00027cc0: 6564 4261 6e64 4e61 6d65 7329 0d0a 0d0a  edBandNames)....
+00027cd0: 2020 2341 7070 6c79 2070 6172 7365 6420    #Apply parsed 
+00027ce0: 6d6f 6465 6c0d 0a20 2064 6566 2070 7265  model..  def pre
+00027cf0: 6447 6574 7465 7228 696d 6729 3a0d 0a20  dGetter(img):.. 
+00027d00: 2020 2074 696d 6520 3d20 696d 672e 7365     time = img.se
+00027d10: 6c65 6374 2874 696d 6542 616e 6429 0d0a  lect(timeBand)..
+00027d20: 2020 2020 6163 7475 616c 203d 2069 6d67      actual = img
+00027d30: 2e73 656c 6563 7428 6163 7475 616c 4261  .select(actualBa
+00027d40: 6e64 7329 2e66 6c6f 6174 2829 0d0a 2020  nds).float()..  
+00027d50: 2020 7072 6564 6963 746f 7242 616e 6473    predictorBands
+00027d60: 203d 2069 6d67 2e73 656c 6563 7428 696e   = img.select(in
+00027d70: 6442 616e 644e 616d 6573 290d 0a0d 0a20  dBandNames).... 
+00027d80: 2020 2023 4974 6572 6174 6520 6163 726f     #Iterate acro
+00027d90: 7373 2065 6163 6820 6d6f 6465 6c20 666f  ss each model fo
+00027da0: 7220 6561 6368 2064 6570 656e 6465 6e74  r each dependent
+00027db0: 2076 6172 6961 626c 650d 0a20 2020 2064   variable..    d
+00027dc0: 6566 2070 6d47 6574 7465 7228 706d 293a  ef pmGetter(pm):
+00027dd0: 0d0a 2020 2020 2020 706d 203d 2065 652e  ..      pm = ee.
+00027de0: 4c69 7374 2870 6d29 0d0a 2020 2020 2020  List(pm)..      
+00027df0: 6d6f 6465 6c43 6f65 6666 7320 3d20 636f  modelCoeffs = co
+00027e00: 6566 6673 2e73 656c 6563 7428 706d 290d  effs.select(pm).
+00027e10: 0a20 2020 2020 206f 7574 4e61 6d65 203d  .      outName =
+00027e20: 2065 652e 5374 7269 6e67 2870 6d2e 6765   ee.String(pm.ge
+00027e30: 7428 3129 292e 6361 7428 275f 7072 6564  t(1)).cat('_pred
+00027e40: 6963 7465 6427 290d 0a20 2020 2020 2069  icted')..      i
+00027e50: 6e74 6572 6365 7074 203d 206d 6f64 656c  ntercept = model
+00027e60: 436f 6566 6673 2e73 656c 6563 7428 6d6f  Coeffs.select(mo
+00027e70: 6465 6c43 6f65 6666 732e 6261 6e64 4e61  delCoeffs.bandNa
+00027e80: 6d65 7328 292e 736c 6963 6528 302c 3129  mes().slice(0,1)
+00027e90: 290d 0a20 2020 2020 206f 7468 6572 7320  )..      others 
+00027ea0: 3d20 6d6f 6465 6c43 6f65 6666 732e 7365  = modelCoeffs.se
+00027eb0: 6c65 6374 286d 6f64 656c 436f 6566 6673  lect(modelCoeffs
+00027ec0: 2e62 616e 644e 616d 6573 2829 2e73 6c69  .bandNames().sli
+00027ed0: 6365 2831 2c4e 6f6e 6529 290d 0a0d 0a20  ce(1,None)).... 
+00027ee0: 2020 2020 2070 7265 6469 6374 6564 203d       predicted =
+00027ef0: 2070 7265 6469 6374 6f72 4261 6e64 732e   predictorBands.
+00027f00: 6d75 6c74 6970 6c79 286f 7468 6572 7329  multiply(others)
+00027f10: 2e72 6564 7563 6528 6565 2e52 6564 7563  .reduce(ee.Reduc
+00027f20: 6572 2e73 756d 2829 292e 6164 6428 696e  er.sum()).add(in
+00027f30: 7465 7263 6570 7429 2e66 6c6f 6174 2829  tercept).float()
+00027f40: 0d0a 2020 2020 2020 7265 7475 726e 2070  ..      return p
+00027f50: 7265 6469 6374 6564 2e66 6c6f 6174 2829  redicted.float()
+00027f60: 0d0a 0d0a 0d0a 2020 2020 7072 6564 6963  ......    predic
+00027f70: 7465 644c 6973 7420 3d70 6172 7365 644d  tedList =parsedM
+00027f80: 6f64 656c 2e6d 6170 2870 6d47 6574 7465  odel.map(pmGette
+00027f90: 7229 0d0a 0d0a 2020 2020 2343 6f6e 7665  r)....    #Conve
+00027fa0: 7274 2074 6f20 616e 2069 6d61 6765 0d0a  rt to an image..
+00027fb0: 2020 2020 7072 6564 6963 7465 644c 6973      predictedLis
+00027fc0: 7420 3d20 6565 2e49 6d61 6765 436f 6c6c  t = ee.ImageColl
+00027fd0: 6563 7469 6f6e 2e66 726f 6d49 6d61 6765  ection.fromImage
+00027fe0: 7328 7072 6564 6963 7465 644c 6973 7429  s(predictedList)
+00027ff0: 0d0a 2020 2020 7072 6564 6963 7465 6449  ..    predictedI
+00028000: 6d61 6765 203d 2063 6f6c 6c65 6374 696f  mage = collectio
+00028010: 6e54 6f49 6d61 6765 2870 7265 6469 6374  nToImage(predict
+00028020: 6564 4c69 7374 292e 7365 6c65 6374 2870  edList).select(p
+00028030: 7265 6469 6374 6564 4261 6e64 4e75 6d62  redictedBandNumb
+00028040: 6572 732c 7072 6564 6963 7465 6442 616e  ers,predictedBan
+00028050: 644e 616d 6573 290d 0a0d 0a20 2020 2023  dNames)....    #
+00028060: 5365 7420 736f 6d65 206d 6574 6164 6174  Set some metadat
+00028070: 610d 0a20 2020 206f 7574 203d 2061 6374  a..    out = act
+00028080: 7561 6c2e 6164 6442 616e 6473 2870 7265  ual.addBands(pre
+00028090: 6469 6374 6564 496d 6167 652e 666c 6f61  dictedImage.floa
+000280a0: 7428 2929 5c0d 0a20 2020 202e 636f 7079  t())\..    .copy
+000280b0: 5072 6f70 6572 7469 6573 2869 6d67 2c5b  Properties(img,[
+000280c0: 2773 7973 7465 6d3a 7469 6d65 5f73 7461  'system:time_sta
+000280d0: 7274 272c 2773 7973 7465 6d3a 7469 6d65  rt','system:time
+000280e0: 5f65 6e64 275d 290d 0a20 2020 2072 6574  _end'])..    ret
+000280f0: 7572 6e20 6f75 740d 0a0d 0a20 2070 7265  urn out....  pre
+00028100: 6469 6374 6564 203d 6861 726d 6f6e 6963  dicted =harmonic
+00028110: 732e 6d61 7028 7072 6564 4765 7474 6572  s.map(predGetter
+00028120: 290d 0a0d 0a20 2070 7265 6469 6374 6564  )....  predicted
+00028130: 203d 2065 652e 496d 6167 6543 6f6c 6c65   = ee.ImageColle
+00028140: 6374 696f 6e28 7072 6564 6963 7465 6429  ction(predicted)
+00028150: 0d0a 0d0a 2020 234d 6170 2e61 6464 4c61  ....  #Map.addLa
+00028160: 7965 7228 7072 6564 6963 7465 642c 7b7d  yer(predicted,{}
+00028170: 2c27 7072 6564 6963 7465 6427 2c46 616c  ,'predicted',Fal
+00028180: 7365 290d 0a0d 0a20 2072 6574 7572 6e20  se)....  return 
+00028190: 7072 6564 6963 7465 640d 0a0d 0a23 2323  predicted....###
+000281a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000281b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000281c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000281d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000281e0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
+000281f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028230: 230d 0a23 4675 6e63 7469 6f6e 2074 6f20  #..#Function to 
+00028240: 6765 7420 6120 6475 6d6d 7920 696d 6167  get a dummy imag
+00028250: 6520 7374 6163 6b20 666f 7220 7379 6e74  e stack for synt
+00028260: 6865 7469 6320 7469 6d65 2073 6572 6965  hetic time serie
+00028270: 730d 0a64 6566 2067 6574 4461 7465 5374  s..def getDateSt
+00028280: 6163 6b28 7374 6172 7459 6561 722c 656e  ack(startYear,en
+00028290: 6459 6561 722c 7374 6172 744a 756c 6961  dYear,startJulia
+000282a0: 6e2c 656e 644a 756c 6961 6e2c 6672 6571  n,endJulian,freq
+000282b0: 7565 6e63 7929 3a0d 0a20 2079 6561 7273  uency):..  years
+000282c0: 203d 2065 652e 4c69 7374 2e73 6571 7565   = ee.List.seque
+000282d0: 6e63 6528 7374 6172 7459 6561 722c 656e  nce(startYear,en
+000282e0: 6459 6561 7229 0d0a 2020 6461 7465 7320  dYear)..  dates 
+000282f0: 3d20 6565 2e4c 6973 742e 7365 7175 656e  = ee.List.sequen
+00028300: 6365 2873 7461 7274 4a75 6c69 616e 2c65  ce(startJulian,e
+00028310: 6e64 4a75 6c69 616e 2c66 7265 7175 656e  ndJulian,frequen
+00028320: 6379 290d 0a0d 0a20 2064 6566 2079 7247  cy)....  def yrG
+00028330: 6574 7465 7228 7972 293a 0d0a 2020 2020  etter(yr):..    
+00028340: 6465 6620 6447 6574 7465 7228 6429 3a0d  def dGetter(d):.
+00028350: 0a20 2020 2020 2072 6574 7572 6e20 6565  .      return ee
+00028360: 2e44 6174 652e 6672 6f6d 594d 4428 7972  .Date.fromYMD(yr
+00028370: 2c31 2c31 292e 6164 7661 6e63 6528 642c  ,1,1).advance(d,
+00028380: 2764 6179 2729 0d0a 2020 2020 6473 203d  'day')..    ds =
+00028390: 2064 6174 6573 2e6d 6170 2864 4765 7474   dates.map(dGett
+000283a0: 6572 290d 0a20 2020 2072 6574 7572 6e20  er)..    return 
+000283b0: 6473 0d0a 0d0a 2020 6461 7465 5365 7473  ds....  dateSets
+000283c0: 203d 2079 6561 7273 2e6d 6170 2879 7247   = years.map(yrG
+000283d0: 6574 7465 7229 0d0a 0d0a 2020 6c20 3d20  etter)....  l = 
+000283e0: 7261 6e67 6528 312c 6c65 6e28 696e 6465  range(1,len(inde
+000283f0: 784e 616d 6573 292b 3129 0d0a 2020 6c20  xNames)+1)..  l 
+00028400: 3d20 5b69 2569 2066 6f72 2069 2069 6e20  = [i%i for i in 
+00028410: 6c5d 0d0a 2020 6320 3d20 6565 2e49 6d61  l]..  c = ee.Ima
+00028420: 6765 286c 292e 7265 6e61 6d65 2869 6e64  ge(l).rename(ind
+00028430: 6578 4e61 6d65 7329 0d0a 2020 6320 3d20  exNames)..  c = 
+00028440: 632e 6469 7669 6465 2863 290d 0a0d 0a20  c.divide(c).... 
+00028450: 2064 6174 6553 6574 7320 3d20 6461 7465   dateSets = date
+00028460: 5365 7473 2e66 6c61 7474 656e 2829 0d0a  Sets.flatten()..
+00028470: 0d0a 2020 6465 6620 6474 4765 7474 6572  ..  def dtGetter
+00028480: 2864 7429 3a0d 0a20 2020 2064 7420 3d20  (dt):..    dt = 
+00028490: 6565 2e44 6174 6528 6474 290d 0a20 2020  ee.Date(dt)..   
+000284a0: 2079 203d 2064 742e 6765 7428 2779 6561   y = dt.get('yea
+000284b0: 7227 290d 0a20 2020 2064 203d 2064 742e  r')..    d = dt.
+000284c0: 6765 7446 7261 6374 696f 6e28 2779 6561  getFraction('yea
+000284d0: 7227 290d 0a20 2020 2069 203d 2065 652e  r')..    i = ee.
+000284e0: 496d 6167 6528 792e 6164 6428 6429 292e  Image(y.add(d)).
+000284f0: 666c 6f61 7428 292e 7365 6c65 6374 285b  float().select([
+00028500: 305d 2c5b 2779 6561 7227 5d29 0d0a 0d0a  0],['year'])....
+00028510: 2020 2020 6920 3d20 632e 6164 6442 616e      i = c.addBan
+00028520: 6473 2869 292e 666c 6f61 7428 295c 0d0a  ds(i).float()\..
+00028530: 2020 2020 2020 2e73 6574 2827 7379 7374        .set('syst
+00028540: 656d 3a74 696d 655f 7374 6172 7427 2c64  em:time_start',d
+00028550: 742e 6d69 6c6c 6973 2829 295c 0d0a 2020  t.millis())\..  
+00028560: 2020 2020 2e73 6574 2827 7379 7374 656d      .set('system
+00028570: 3a74 696d 655f 656e 6427 2c64 742e 6164  :time_end',dt.ad
+00028580: 7661 6e63 6528 6672 6571 7565 6e63 792c  vance(frequency,
+00028590: 2764 6179 2729 2e6d 696c 6c69 7328 2929  'day').millis())
+000285a0: 0d0a 2020 2020 7265 7475 726e 2069 0d0a  ..    return i..
+000285b0: 2020 7374 6163 6b20 3d20 6461 7465 5365    stack = dateSe
+000285c0: 7473 2e6d 6170 2864 7447 6574 7465 7229  ts.map(dtGetter)
+000285d0: 0d0a 2020 7374 6163 6b20 3d20 6565 2e49  ..  stack = ee.I
+000285e0: 6d61 6765 436f 6c6c 6563 7469 6f6e 2e66  mageCollection.f
+000285f0: 726f 6d49 6d61 6765 7328 7374 6163 6b29  romImages(stack)
+00028600: 0d0a 2020 7265 7475 726e 2073 7461 636b  ..  return stack
+00028610: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
+00028620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028650: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+00028660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000286a0: 2323 2323 2323 2323 0d0a 6465 6620 6765  ########..def ge
+000286b0: 7448 6172 6d6f 6e69 6343 6f65 6666 6963  tHarmonicCoeffic
+000286c0: 6965 6e74 7341 6e64 4669 7428 616c 6c49  ientsAndFit(allI
+000286d0: 6d61 6765 732c 696e 6465 784e 616d 6573  mages,indexNames
+000286e0: 2c77 6869 6368 4861 726d 6f6e 6963 7320  ,whichHarmonics 
+000286f0: 3d20 5b32 5d2c 6465 7472 656e 6420 3d20  = [2],detrend = 
+00028700: 4661 6c73 6529 3a0d 0a0d 0a20 2023 5365  False):....  #Se
+00028710: 6c65 6374 2064 6573 6972 6564 2062 616e  lect desired ban
+00028720: 6473 0d0a 2020 616c 6c49 6e64 6963 6573  ds..  allIndices
+00028730: 203d 2061 6c6c 496d 6167 6573 2e73 656c   = allImages.sel
+00028740: 6563 7428 696e 6465 784e 616d 6573 290d  ect(indexNames).
+00028750: 0a0d 0a20 2023 4164 6420 6461 7465 2062  ...  #Add date b
+00028760: 616e 640d 0a20 2069 6620 6465 7472 656e  and..  if detren
+00028770: 643a 0d0a 2020 2020 616c 6c49 6e64 6963  d:..    allIndic
+00028780: 6573 203d 2061 6c6c 496e 6469 6365 732e  es = allIndices.
+00028790: 6d61 7028 6164 6444 6174 6542 616e 6429  map(addDateBand)
+000287a0: 0d0a 2020 656c 7365 3a0d 0a20 2020 2061  ..  else:..    a
+000287b0: 6c6c 496e 6469 6365 7320 3d20 616c 6c49  llIndices = allI
+000287c0: 6e64 6963 6573 2e6d 6170 2861 6464 5965  ndices.map(addYe
+000287d0: 6172 4672 6163 7469 6f6e 4261 6e64 290d  arFractionBand).
+000287e0: 0a0d 0a0d 0a20 2023 4164 6420 696e 6465  .....  #Add inde
+000287f0: 7065 6e64 656e 7420 7072 6564 6963 746f  pendent predicto
+00028800: 7273 2028 6861 726d 6f6e 6963 7329 0d0a  rs (harmonics)..
+00028810: 2020 7769 7468 4861 726d 6f6e 6963 7320    withHarmonics 
+00028820: 3d20 6765 7448 6172 6d6f 6e69 6373 3228  = getHarmonics2(
+00028830: 616c 6c49 6e64 6963 6573 2c27 7965 6172  allIndices,'year
+00028840: 272c 7768 6963 6848 6172 6d6f 6e69 6373  ',whichHarmonics
+00028850: 2c64 6574 7265 6e64 290d 0a20 2077 6974  ,detrend)..  wit
+00028860: 6848 6172 6d6f 6e69 6373 426e 7320 3d20  hHarmonicsBns = 
+00028870: 6565 2e49 6d61 6765 2877 6974 6848 6172  ee.Image(withHar
+00028880: 6d6f 6e69 6373 2e66 6972 7374 2829 292e  monics.first()).
+00028890: 6261 6e64 4e61 6d65 7328 292e 736c 6963  bandNames().slic
+000288a0: 6528 6c65 6e28 696e 6465 784e 616d 6573  e(len(indexNames
+000288b0: 292b 312c 4e6f 6e65 290d 0a0d 0a20 2023  )+1,None)....  #
+000288c0: 4f70 7469 6f6e 616c 6c79 2063 6861 7274  Optionally chart
+000288d0: 2074 6865 2063 6f6c 6c65 6374 696f 6e20   the collection 
+000288e0: 7769 7468 2068 6172 6d6f 6e69 6373 0d0a  with harmonics..
+000288f0: 0d0a 2020 2346 6974 2061 206c 696e 6561  ..  #Fit a linea
+00028900: 7220 7265 6772 6573 7369 6f6e 206d 6f64  r regression mod
+00028910: 656c 0d0a 2020 636f 6566 6673 203d 206e  el..  coeffs = n
+00028920: 6577 526f 6275 7374 4d75 6c74 6970 6c65  ewRobustMultiple
+00028930: 4c69 6e65 6172 3228 7769 7468 4861 726d  Linear2(withHarm
+00028940: 6f6e 6963 7329 0d0a 0d0a 2020 2343 616e  onics)....  #Can
+00028950: 2076 6973 7561 6c69 7a65 2074 6865 2070   visualize the p
+00028960: 6861 7365 2061 6e64 2061 6d70 6c69 7475  hase and amplitu
+00028970: 6465 2069 6620 6f6e 6c79 2074 6865 2066  de if only the f
+00028980: 6972 7374 2028 5b32 5d29 2068 6172 6d6f  irst ([2]) harmo
+00028990: 6e69 6320 6973 2063 686f 7365 6e0d 0a20  nic is chosen.. 
+000289a0: 2023 2069 6620 7768 6963 6848 6172 6d6f   # if whichHarmo
+000289b0: 6e69 6373 203d 3d20 327b 0d0a 2020 2320  nics == 2{..  # 
+000289c0: 2020 2070 6120 3d20 6765 7450 6861 7365     pa = getPhase
+000289d0: 416d 706c 6974 7564 6528 636f 6566 6673  Amplitude(coeffs
+000289e0: 293b 0d0a 2020 2320 202f 2f20 5475 726e  );..  #  // Turn
+000289f0: 2074 6865 2048 5356 2064 6174 6120 696e   the HSV data in
+00028a00: 746f 2061 6e20 5247 4220 696d 6167 6520  to an RGB image 
+00028a10: 616e 6420 6164 6420 6974 2074 6f20 7468  and add it to th
+00028a20: 6520 6d61 702e 0d0a 2020 2320 2073 6561  e map...  #  sea
+00028a30: 736f 6e61 6c69 7479 203d 2070 612e 7365  sonality = pa.se
+00028a40: 6c65 6374 285b 312c 305d 292e 6164 6442  lect([1,0]).addB
+00028a50: 616e 6473 2861 6c6c 496e 6469 6365 732e  ands(allIndices.
+00028a60: 7365 6c65 6374 285b 696e 6465 784e 616d  select([indexNam
+00028a70: 6573 5b30 5d5d 292e 6d65 616e 2829 292e  es[0]]).mean()).
+00028a80: 6873 7654 6f52 6762 2829 3b0d 0a20 2023  hsvToRgb();..  #
+00028a90: 2020 2f2f 204d 6170 2e61 6464 4c61 7965    // Map.addLaye
+00028aa0: 7228 7365 6173 6f6e 616c 6974 792c 207b  r(seasonality, {
+00028ab0: 7d2c 2027 5365 6173 6f6e 616c 6974 7927  }, 'Seasonality'
+00028ac0: 293b 0d0a 2020 2320 207d 0d0a 0d0a 0d0a  );..  #  }......
+00028ad0: 0d0a 2020 234d 6170 2e61 6464 4c61 7965  ..  #Map.addLaye
+00028ae0: 7228 636f 6566 6673 2c7b 7d2c 2748 6172  r(coeffs,{},'Har
+00028af0: 6d6f 6e69 6320 5265 6772 6573 7369 6f6e  monic Regression
+00028b00: 2043 6f65 6666 6963 6965 6e74 7327 2c46   Coefficients',F
+00028b10: 616c 7365 290d 0a20 2070 7265 6469 6374  alse)..  predict
+00028b20: 6564 203d 206e 6577 5072 6564 6963 7428  ed = newPredict(
+00028b30: 636f 6566 6673 2c77 6974 6848 6172 6d6f  coeffs,withHarmo
+00028b40: 6e69 6373 290d 0a20 2072 6574 7572 6e20  nics)..  return 
+00028b50: 5b63 6f65 6666 732c 7072 6564 6963 7465  [coeffs,predicte
+00028b60: 645d 0d0a 2323 2323 2323 2323 2323 2323  d]..############
+00028b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028ba0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+00028bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028bf0: 2323 2323 2323 2323 0d0a 2353 696d 706c  ########..#Simpl
+00028c00: 6520 7072 6564 6963 7420 6675 6e63 7469  e predict functi
+00028c10: 6f6e 2066 6f72 2068 6172 6d6f 6e69 6320  on for harmonic 
+00028c20: 636f 6566 6669 6369 656e 7473 0d0a 2345  coefficients..#E
+00028c30: 7870 6563 7473 2063 6f65 6666 7320 6672  xpects coeffs fr
+00028c40: 6f6d 2067 6574 4861 726d 6f6e 6963 436f  om getHarmonicCo
+00028c50: 6566 6669 6369 656e 7473 416e 6446 6974  efficientsAndFit
+00028c60: 2066 756e 6374 696f 6e0d 0a23 4461 7465   function..#Date
+00028c70: 2069 6d61 6765 2069 7320 6578 7065 6374   image is expect
+00028c80: 6564 2074 6f20 6265 2079 7979 792e 6464  ed to be yyyy.dd
+00028c90: 2077 6865 7265 2064 6420 6973 2074 6865   where dd is the
+00028ca0: 2064 6179 206f 6620 7965 6172 202f 2033   day of year / 3
+00028cb0: 3635 2028 7072 6f70 6f72 7469 6f6e 206f  65 (proportion o
+00028cc0: 6620 7965 6172 290d 0a23 6578 2e20 7379  f year)..#ex. sy
+00028cd0: 6e74 6849 6d61 6765 2863 6f65 6666 732c  nthImage(coeffs,
+00028ce0: 6565 2e49 6d61 6765 285b 3230 3139 2e36  ee.Image([2019.6
+00028cf0: 5d29 2c5b 2762 6c75 6527 2c27 6772 6565  ]),['blue','gree
+00028d00: 6e27 2c27 7265 6427 2c27 6e69 7227 2c27  n','red','nir','
+00028d10: 7377 6972 3127 2c27 7377 6972 3227 2c27  swir1','swir2','
+00028d20: 4e42 5227 2c27 4e44 5649 275d 2c5b 322c  NBR','NDVI'],[2,
+00028d30: 345d 2c74 7275 6529 0d0a 6465 6620 7379  4],true)..def sy
+00028d40: 6e74 6849 6d61 6765 2863 6f65 6666 732c  nthImage(coeffs,
+00028d50: 6461 7465 496d 6167 652c 696e 6465 784e  dateImage,indexN
+00028d60: 616d 6573 2c68 6172 6d6f 6e69 6373 2c64  ames,harmonics,d
+00028d70: 6574 7265 6e64 293a 0d0a 2020 2353 6574  etrend):..  #Set
+00028d80: 2075 7020 636f 6e73 7461 6e74 2069 6d61   up constant ima
+00028d90: 6765 2074 6f20 6d75 6c74 6970 6c79 2063  ge to multiply c
+00028da0: 6f65 6666 7320 6279 0d0a 2020 636f 6e73  oeffs by..  cons
+00028db0: 7449 6d61 6765 203d 2065 652e 496d 6167  tImage = ee.Imag
+00028dc0: 6528 3129 0d0a 2020 6966 2064 6574 7265  e(1)..  if detre
+00028dd0: 6e64 3a63 6f6e 7374 496d 6167 6520 3d20  nd:constImage = 
+00028de0: 636f 6e73 7449 6d61 6765 2e61 6464 4261  constImage.addBa
+00028df0: 6e64 7328 6461 7465 496d 6167 6529 0d0a  nds(dateImage)..
+00028e00: 2020 666f 7220 6861 726d 2069 6e20 6861    for harm in ha
+00028e10: 726d 6f6e 6963 733a 0d0a 2020 2020 636f  rmonics:..    co
+00028e20: 6e73 7449 6d61 6765 203d 2063 6f6e 7374  nstImage = const
+00028e30: 496d 6167 652e 6164 6442 616e 6473 2865  Image.addBands(e
+00028e40: 652e 496d 6167 6528 5b64 6174 6549 6d61  e.Image([dateIma
+00028e50: 6765 2e6d 756c 7469 706c 7928 6861 726d  ge.multiply(harm
+00028e60: 2a6d 6174 682e 7069 292e 7369 6e28 295d  *math.pi).sin()]
+00028e70: 292e 7265 6e61 6d65 285b 277b 7d5f 7369  ).rename(['{}_si
+00028e80: 6e27 2e66 6f72 6d61 7428 6861 726d 2a31  n'.format(harm*1
+00028e90: 3030 295d 2929 2020 2020 2020 2020 2020  00)]))          
+00028ea0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00028eb0: 2066 6f72 2068 6172 6d20 696e 2068 6172   for harm in har
+00028ec0: 6d6f 6e69 6373 3a0d 0a20 2020 2063 6f6e  monics:..    con
+00028ed0: 7374 496d 6167 6520 3d20 636f 6e73 7449  stImage = constI
+00028ee0: 6d61 6765 2e61 6464 4261 6e64 7328 6565  mage.addBands(ee
+00028ef0: 2e49 6d61 6765 285b 6461 7465 496d 6167  .Image([dateImag
+00028f00: 652e 6d75 6c74 6970 6c79 2868 6172 6d2a  e.multiply(harm*
+00028f10: 6d61 7468 2e70 6929 2e63 6f73 2829 5d29  math.pi).cos()])
+00028f20: 2e72 656e 616d 6528 5b27 7b7d 5f63 6f73  .rename(['{}_cos
+00028f30: 272e 666f 726d 6174 2868 6172 6d2a 3130  '.format(harm*10
+00028f40: 3029 5d29 290d 0a20 200d 0a20 2023 2063  0)]))..  ..  # c
+00028f50: 6f65 6666 7373 426e 203d 2063 6f65 6666  oeffssBn = coeff
+00028f60: 732e 7365 6c65 6374 2865 652e 5374 7269  s.select(ee.Stri
+00028f70: 6e67 2869 6e64 6578 4e61 6d65 735b 305d  ng(indexNames[0]
+00028f80: 292e 6361 7428 275f 2e2a 2729 290d 0a20  ).cat('_.*')).. 
+00028f90: 2023 2070 7269 6e74 2863 6f6e 7374 496d   # print(constIm
+00028fa0: 6167 652e 6261 6e64 4e61 6d65 7328 292e  age.bandNames().
+00028fb0: 6765 7449 6e66 6f28 292c 636f 6566 6673  getInfo(),coeffs
+00028fc0: 7342 6e2e 6261 6e64 4e61 6d65 7328 292e  sBn.bandNames().
+00028fd0: 6765 7449 6e66 6f28 2929 0d0a 2020 2350  getInfo())..  #P
+00028fe0: 7265 6469 6374 2076 616c 7565 7320 666f  redict values fo
+00028ff0: 7220 6561 6368 2062 616e 640d 0a20 206f  r each band..  o
+00029000: 7574 203d 2065 652e 496d 6167 6528 3129  ut = ee.Image(1)
+00029010: 3b0d 0a20 2064 6566 2070 7265 6469 6374  ;..  def predict
+00029020: 5772 6170 7065 7228 626e 2c6f 7574 293a  Wrapper(bn,out):
+00029030: 0d0a 2020 2020 626e 203d 2065 652e 5374  ..    bn = ee.St
+00029040: 7269 6e67 2862 6e29 0d0a 2020 2020 2353  ring(bn)..    #S
+00029050: 656c 6563 7420 636f 6566 6673 2066 6f72  elect coeffs for
+00029060: 2074 6861 7420 6261 6e64 0d0a 2020 2020   that band..    
+00029070: 636f 6566 6673 7342 6e20 3d20 636f 6566  coeffssBn = coef
+00029080: 6673 2e73 656c 6563 7428 6565 2e53 7472  fs.select(ee.Str
+00029090: 696e 6728 626e 292e 6361 7428 275f 2e2a  ing(bn).cat('_.*
+000290a0: 2729 290d 0a20 2020 2070 7265 6469 6374  '))..    predict
+000290b0: 6564 203d 2063 6f6e 7374 496d 6167 652e  ed = constImage.
+000290c0: 6d75 6c74 6970 6c79 2863 6f65 6666 7373  multiply(coeffss
+000290d0: 426e 292e 7265 6475 6365 2827 7375 6d27  Bn).reduce('sum'
+000290e0: 292e 7265 6e61 6d65 2862 6e29 0d0a 2020  ).rename(bn)..  
+000290f0: 2020 7265 7475 726e 2065 652e 496d 6167    return ee.Imag
+00029100: 6528 6f75 7429 2e61 6464 4261 6e64 7328  e(out).addBands(
+00029110: 7072 6564 6963 7465 6429 0d0a 0d0a 2020  predicted)....  
+00029120: 6f75 7420 3d20 6565 2e49 6d61 6765 2865  out = ee.Image(e
+00029130: 652e 4c69 7374 2869 6e64 6578 4e61 6d65  e.List(indexName
+00029140: 7329 2e69 7465 7261 7465 2870 7265 6469  s).iterate(predi
+00029150: 6374 5772 6170 7065 722c 6f75 7429 293b  ctWrapper,out));
+00029160: 0d0a 0d0a 2020 6f75 7420 3d20 6f75 742e  ....  out = out.
+00029170: 7365 6c65 6374 2865 652e 4c69 7374 2e73  select(ee.List.s
+00029180: 6571 7565 6e63 6528 312c 206f 7574 2e62  equence(1, out.b
+00029190: 616e 644e 616d 6573 2829 2e73 697a 6528  andNames().size(
+000291a0: 292e 7375 6274 7261 6374 2831 2929 290d  ).subtract(1))).
+000291b0: 0a0d 0a20 2072 6574 7572 6e20 6f75 740d  ...  return out.
+000291c0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+000291d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000291e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000291f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029200: 2323 2323 2323 0d0a 2357 7261 7070 6572  ######..#Wrapper
+00029210: 2066 756e 6374 696f 6e20 746f 2067 6574   function to get
+00029220: 2063 6c69 6d61 7465 2064 6174 610d 0a23   climate data..#
+00029230: 2053 7570 706f 7274 733a 0d0a 2320 4e41   Supports:..# NA
+00029240: 5341 2f4f 524e 4c2f 4441 594d 4554 5f56  SA/ORNL/DAYMET_V
+00029250: 330d 0a23 204e 4153 412f 4f52 4e4c 2f44  3..# NASA/ORNL/D
+00029260: 4159 4d45 545f 5634 0d0a 2320 5543 5342  AYMET_V4..# UCSB
+00029270: 2d43 4847 2f43 4849 5250 532f 4441 494c  -CHG/CHIRPS/DAIL
+00029280: 5920 2870 7265 6369 7069 7461 7469 6f6e  Y (precipitation
+00029290: 206f 6e6c 7929 0d0a 2361 6e64 2070 6f73   only)..#and pos
+000292a0: 7369 626c 7920 6f74 6865 7273 0d0a 6465  sibly others..de
+000292b0: 6620 6765 7443 6c69 6d61 7465 5772 6170  f getClimateWrap
+000292c0: 7065 7228 636f 6c6c 6563 7469 6f6e 4e61  per(collectionNa
+000292d0: 6d65 2c73 7475 6479 4172 6561 2c73 7461  me,studyArea,sta
+000292e0: 7274 5965 6172 2c65 6e64 5965 6172 2c73  rtYear,endYear,s
+000292f0: 7461 7274 4a75 6c69 616e 2c65 6e64 4a75  tartJulian,endJu
+00029300: 6c69 616e 2c74 696d 6562 7566 6665 722c  lian,timebuffer,
+00029310: 7765 6967 6874 732c 636f 6d70 6f73 6974  weights,composit
+00029320: 696e 6752 6564 7563 6572 2c65 7870 6f72  ingReducer,expor
+00029330: 7443 6f6d 706f 7369 7465 7320 3d20 4661  tComposites = Fa
+00029340: 6c73 652c 6578 706f 7274 5061 7468 526f  lse,exportPathRo
+00029350: 6f74 203d 204e 6f6e 652c 6372 7320 3d20  ot = None,crs = 
+00029360: 4e6f 6e65 2c74 7261 6e73 666f 726d 203d  None,transform =
+00029370: 204e 6f6e 652c 7363 616c 6520 3d20 4e6f   None,scale = No
+00029380: 6e65 2c65 7870 6f72 7442 616e 6473 203d  ne,exportBands =
+00029390: 204e 6f6e 6529 3a0d 0a20 2061 7267 7320   None):..  args 
+000293a0: 3d20 666f 726d 6174 4172 6773 286c 6f63  = formatArgs(loc
+000293b0: 616c 7328 2929 0d0a 2020 6966 2027 6172  als())..  if 'ar
+000293c0: 6773 2720 696e 2061 7267 732e 6b65 7973  gs' in args.keys
+000293d0: 2829 3a0d 0a20 2020 2064 656c 2061 7267  ():..    del arg
+000293e0: 735b 2761 7267 7327 5d0d 0a20 2070 7269  s['args']..  pri
+000293f0: 6e74 2861 7267 7329 0d0a 0d0a 2020 2350  nt(args)....  #P
+00029400: 7265 7061 7265 2064 6174 6573 0d0a 2020  repare dates..  
+00029410: 2357 7261 7020 7468 6520 6461 7465 7320  #Wrap the dates 
+00029420: 6966 206e 6565 6465 640d 0a20 2077 7261  if needed..  wra
+00029430: 704f 6666 7365 7420 3d20 300d 0a20 2069  pOffset = 0..  i
+00029440: 6620 7374 6172 744a 756c 6961 6e20 3e20  f startJulian > 
+00029450: 656e 644a 756c 6961 6e3a 0d0a 2020 2020  endJulian:..    
+00029460: 7772 6170 4f66 6673 6574 203d 2033 3635  wrapOffset = 365
+00029470: 0d0a 0d0a 2020 7374 6172 7444 6174 6520  ....  startDate 
+00029480: 3d20 6565 2e44 6174 652e 6672 6f6d 594d  = ee.Date.fromYM
+00029490: 4428 7374 6172 7459 6561 722c 312c 3129  D(startYear,1,1)
+000294a0: 2e61 6476 616e 6365 2873 7461 7274 4a75  .advance(startJu
+000294b0: 6c69 616e 2d31 2c27 6461 7927 290d 0a20  lian-1,'day').. 
+000294c0: 2065 6e64 4461 7465 203d 2065 652e 4461   endDate = ee.Da
+000294d0: 7465 2e66 726f 6d59 4d44 2865 6e64 5965  te.fromYMD(endYe
+000294e0: 6172 2c31 2c31 292e 6164 7661 6e63 6528  ar,1,1).advance(
+000294f0: 656e 644a 756c 6961 6e2d 312b 7772 6170  endJulian-1+wrap
+00029500: 4f66 6673 6574 2c27 6461 7927 290d 0a20  Offset,'day').. 
+00029510: 2070 7269 6e74 2827 5374 6172 7420 616e   print('Start an
+00029520: 6420 656e 6420 6461 7465 733a 272c 2073  d end dates:', s
+00029530: 7461 7274 4461 7465 2e66 6f72 6d61 7428  tartDate.format(
+00029540: 2759 5959 592d 4d4d 2d64 6427 292e 6765  'YYYY-MM-dd').ge
+00029550: 7449 6e66 6f28 292c 2065 6e64 4461 7465  tInfo(), endDate
+00029560: 2e66 6f72 6d61 7428 2759 5959 592d 4d4d  .format('YYYY-MM
+00029570: 2d64 6427 292e 6765 7449 6e66 6f28 2929  -dd').getInfo())
+00029580: 0d0a 2020 7072 696e 7428 274a 756c 6961  ..  print('Julia
+00029590: 6e20 6461 7973 2061 7265 3a27 2c73 7461  n days are:',sta
+000295a0: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
+000295b0: 616e 290d 0a0d 0a20 2023 4765 7420 636c  an)....  #Get cl
+000295c0: 696d 6174 6520 6461 7461 0d0a 2020 6320  imate data..  c 
+000295d0: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
+000295e0: 7469 6f6e 2863 6f6c 6c65 6374 696f 6e4e  tion(collectionN
+000295f0: 616d 6529 5c0d 0a20 2020 2020 2020 2020  ame)\..         
+00029600: 2020 2e66 696c 7465 7242 6f75 6e64 7328    .filterBounds(
+00029610: 7374 7564 7941 7265 6129 5c0d 0a20 2020  studyArea)\..   
+00029620: 2020 2020 2020 2020 2e66 696c 7465 7244          .filterD
+00029630: 6174 6528 7374 6172 7444 6174 652c 656e  ate(startDate,en
+00029640: 6444 6174 652e 6164 7661 6e63 6528 312c  dDate.advance(1,
+00029650: 2764 6179 2729 295c 0d0a 2020 2020 2020  'day'))\..      
+00029660: 2020 2020 202e 6669 6c74 6572 2865 652e       .filter(ee.
+00029670: 4669 6c74 6572 2e63 616c 656e 6461 7252  Filter.calendarR
+00029680: 616e 6765 2873 7461 7274 4a75 6c69 616e  ange(startJulian
+00029690: 2c65 6e64 4a75 6c69 616e 2929 0d0a 0d0a  ,endJulian))....
+000296a0: 2020 2353 6574 2074 6f20 6170 7072 6f70    #Set to approp
+000296b0: 7269 6174 6520 7265 7361 6d70 6c69 6e67  riate resampling
+000296c0: 206d 6574 686f 640d 0a20 2063 203d 2063   method..  c = c
+000296d0: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
+000296e0: 2069 6d67 2e72 6573 616d 706c 6528 2762   img.resample('b
+000296f0: 6963 7562 6963 2729 290d 0a20 204d 6170  icubic'))..  Map
+00029700: 2e61 6464 4c61 7965 7228 632c 7b7d 2c27  .addLayer(c,{},'
+00029710: 5261 7720 436c 696d 6174 6527 2c46 616c  Raw Climate',Fal
+00029720: 7365 290d 0a0d 0a20 2023 4372 6561 7465  se)....  #Create
+00029730: 2063 6f6d 706f 7369 7465 2074 696d 6520   composite time 
+00029740: 7365 7269 6573 0d0a 2020 7473 203d 2063  series..  ts = c
+00029750: 6f6d 706f 7369 7465 5469 6d65 5365 7269  ompositeTimeSeri
+00029760: 6573 2863 2c73 7461 7274 5965 6172 2c65  es(c,startYear,e
+00029770: 6e64 5965 6172 2c73 7461 7274 4a75 6c69  ndYear,startJuli
+00029780: 616e 2c65 6e64 4a75 6c69 616e 2c74 696d  an,endJulian,tim
+00029790: 6562 7566 6665 722c 7765 6967 6874 732c  ebuffer,weights,
+000297a0: 4e6f 6e65 2c63 6f6d 706f 7369 7469 6e67  None,compositing
+000297b0: 5265 6475 6365 7229 0d0a 2020 7473 203d  Reducer)..  ts =
+000297c0: 2065 652e 496d 6167 6543 6f6c 6c65 6374   ee.ImageCollect
+000297d0: 696f 6e28 7473 2e6d 6170 286c 616d 6264  ion(ts.map(lambd
+000297e0: 6120 6920 3a20 692e 666c 6f61 7428 2929  a i : i.float())
+000297f0: 290d 0a0d 0a20 2023 4578 706f 7274 2063  )....  #Export c
+00029800: 6f6d 706f 7369 7465 2063 6f6c 6c65 6374  omposite collect
+00029810: 696f 6e0d 0a20 2069 6620 6578 706f 7274  ion..  if export
+00029820: 436f 6d70 6f73 6974 6573 3a0d 0a20 2020  Composites:..   
+00029830: 2023 5365 7420 7570 2065 7870 6f72 7420   #Set up export 
+00029840: 6261 6e64 7320 6966 206e 6f74 2073 7065  bands if not spe
+00029850: 6369 6669 6564 0d0a 2020 2020 6966 2065  cified..    if e
+00029860: 7870 6f72 7442 616e 6473 203d 3d20 4e6f  xportBands == No
+00029870: 6e65 3a0d 0a20 2020 2020 2065 7870 6f72  ne:..      expor
+00029880: 7442 616e 6473 203d 2065 652e 4c69 7374  tBands = ee.List
+00029890: 2865 652e 496d 6167 6528 7473 2e66 6972  (ee.Image(ts.fir
+000298a0: 7374 2829 292e 6261 6e64 4e61 6d65 7328  st()).bandNames(
+000298b0: 2929 0d0a 0d0a 2020 2020 6578 706f 7274  ))....    export
+000298c0: 436f 6c6c 6563 7469 6f6e 2865 7870 6f72  Collection(expor
+000298d0: 7450 6174 6852 6f6f 742c 636f 6c6c 6563  tPathRoot,collec
+000298e0: 7469 6f6e 4e61 6d65 2e73 706c 6974 2827  tionName.split('
+000298f0: 2f27 295b 2d31 5d2c 7374 7564 7941 7265  /')[-1],studyAre
+00029900: 612c 2063 7273 2c74 7261 6e73 666f 726d  a, crs,transform
+00029910: 2c73 6361 6c65 2c74 732c 7374 6172 7459  ,scale,ts,startY
+00029920: 6561 722c 656e 6459 6561 722c 7374 6172  ear,endYear,star
+00029930: 744a 756c 6961 6e2c 656e 644a 756c 6961  tJulian,endJulia
+00029940: 6e2c 636f 6d70 6f73 6974 696e 6752 6564  n,compositingRed
+00029950: 7563 6572 2c74 696d 6562 7566 6665 722c  ucer,timebuffer,
+00029960: 6578 706f 7274 4261 6e64 7329 0d0a 0d0a  exportBands)....
+00029970: 2020 7265 7475 726e 2074 7323 2323 230d    return ts####.
+00029980: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00029990: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000299a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000299b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000299c0: 2323 2323 2323 0d0a 2341 6464 7320 6162  ######..#Adds ab
+000299d0: 736f 6c75 7465 2064 6966 6665 7265 6e63  solute differenc
+000299e0: 6520 6672 6f6d 2061 2073 7065 6369 6669  e from a specifi
+000299f0: 6564 2062 616e 6420 7375 6d6d 6172 697a  ed band summariz
+00029a00: 6564 2062 7920 6120 7072 6f76 6964 6564  ed by a provided
+00029a10: 2070 6572 6365 6e74 696c 650d 0a23 496e   percentile..#In
+00029a20: 7465 6e64 6564 2066 6f72 2063 7573 746f  tended for custo
+00029a30: 6d20 736f 7274 696e 6720 6163 726f 7373  m sorting across
+00029a40: 2063 6f6c 6c65 6374 696f 6e73 0d0a 6465   collections..de
+00029a50: 6620 6164 6441 6273 4469 6666 2869 6e43  f addAbsDiff(inC
+00029a60: 6f6c 6c65 6374 696f 6e2c 2071 7561 6c69  ollection, quali
+00029a70: 7479 4261 6e64 2c20 7065 7263 656e 7469  tyBand, percenti
+00029a80: 6c65 2c73 6967 6e29 3a0d 0a20 2062 6573  le,sign):..  bes
+00029a90: 7451 7561 6c69 7479 203d 2069 6e43 6f6c  tQuality = inCol
+00029aa0: 6c65 6374 696f 6e2e 7365 6c65 6374 285b  lection.select([
+00029ab0: 7175 616c 6974 7942 616e 645d 292e 7265  qualityBand]).re
+00029ac0: 6475 6365 2865 652e 5265 6475 6365 722e  duce(ee.Reducer.
+00029ad0: 7065 7263 656e 7469 6c65 285b 7065 7263  percentile([perc
+00029ae0: 656e 7469 6c65 5d29 290d 0a20 2064 6566  entile]))..  def
+00029af0: 2077 2869 6d61 6765 293a 0d0a 2020 2020   w(image):..    
+00029b00: 6465 6c74 6120 3d20 696d 6167 652e 7365  delta = image.se
+00029b10: 6c65 6374 285b 7175 616c 6974 7942 616e  lect([qualityBan
+00029b20: 645d 292e 7375 6274 7261 6374 2862 6573  d]).subtract(bes
+00029b30: 7451 7561 6c69 7479 292e 6162 7328 292e  tQuality).abs().
+00029b40: 6d75 6c74 6970 6c79 2873 6967 6e29 0d0a  multiply(sign)..
+00029b50: 2020 2020 7265 7475 726e 2069 6d61 6765      return image
+00029b60: 2e61 6464 4261 6e64 7328 6465 6c74 612e  .addBands(delta.
+00029b70: 7365 6c65 6374 285b 305d 2c20 5b27 6465  select([0], ['de
+00029b80: 6c74 6127 5d29 290d 0a20 206f 7574 203d  lta']))..  out =
+00029b90: 2069 6e43 6f6c 6c65 6374 696f 6e2e 6d61   inCollection.ma
+00029ba0: 7028 7729 0d0a 2020 7265 7475 726e 206f  p(w)..  return o
+00029bb0: 7574 0d0a 0d0a 2323 2323 2323 2323 2323  ut....##########
+00029bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029bf0: 2323 2323 2323 2323 2323 230d 0a23 4d65  ###########..#Me
+00029c00: 7468 6f64 2066 6f72 2061 7070 6c79 696e  thod for applyin
+00029c10: 6720 7468 6520 7175 616c 6974 794d 6f73  g the qualityMos
+00029c20: 6169 6320 6675 6e63 7469 6f6e 2075 7369  aic function usi
+00029c30: 6e67 2061 2073 7065 6369 6669 6564 2070  ng a specified p
+00029c40: 6572 6365 6e74 696c 650d 0a23 5573 6566  ercentile..#Usef
+00029c50: 756c 2077 6865 6e20 7468 6520 6d61 7820  ul when the max 
+00029c60: 6f66 2074 6865 2071 7561 6c69 7479 2062  of the quality b
+00029c70: 616e 6420 6973 206e 6f74 2077 6861 7420  and is not what 
+00029c80: 6973 2077 616e 7465 640d 0a64 6566 2063  is wanted..def c
+00029c90: 7573 746f 6d51 7561 6c69 7479 4d6f 7361  ustomQualityMosa
+00029ca0: 6963 2869 6e43 6f6c 6c65 6374 696f 6e2c  ic(inCollection,
+00029cb0: 7175 616c 6974 7942 616e 642c 7065 7263  qualityBand,perc
+00029cc0: 656e 7469 6c65 293a 0d0a 2020 2341 6464  entile):..  #Add
+00029cd0: 2061 6e20 6162 736f 6c75 7465 2064 6966   an absolute dif
+00029ce0: 6665 7265 6e63 6520 6672 6f6d 2074 6865  ference from the
+00029cf0: 2073 7065 6369 6669 6564 2070 6572 6365   specified perce
+00029d00: 6e74 696c 650d 0a20 2023 5468 6973 2069  ntile..  #This i
+00029d10: 7320 696e 7665 7274 6564 2066 6f72 2074  s inverted for t
+00029d20: 6865 2071 7561 6c69 7479 4d6f 7361 6963  he qualityMosaic
+00029d30: 2066 756e 6374 696f 6e20 746f 2070 726f   function to pro
+00029d40: 7065 726c 7920 7072 696f 7269 7469 7a65  perly prioritize
+00029d50: 0d0a 2020 696e 436f 6c6c 6563 7469 6f6e  ..  inCollection
+00029d60: 4465 6c74 6120 3d20 6164 6441 6273 4469  Delta = addAbsDi
+00029d70: 6666 2869 6e43 6f6c 6c65 6374 696f 6e2c  ff(inCollection,
+00029d80: 2071 7561 6c69 7479 4261 6e64 2c20 7065   qualityBand, pe
+00029d90: 7263 656e 7469 6c65 2c2d 3129 0d0a 0d0a  rcentile,-1)....
+00029da0: 2020 2341 7070 6c79 2074 6865 2071 7561    #Apply the qua
+00029db0: 6c69 7479 4d6f 7361 6963 2066 756e 6374  lityMosaic funct
+00029dc0: 696f 6e0d 0a20 2072 6574 7572 6e20 696e  ion..  return in
+00029dd0: 436f 6c6c 6563 7469 6f6e 4465 6c74 612e  CollectionDelta.
+00029de0: 7175 616c 6974 794d 6f73 6169 6328 2764  qualityMosaic('d
+00029df0: 656c 7461 2729 0d0a 0d0a 2323 2323 2323  elta')....######
+00029e00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029e30: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+00029e40: 0a23 4f6e 2d74 6865 2d66 6c79 2062 6173  .#On-the-fly bas
+00029e50: 6963 2077 6174 6572 206d 6173 6b69 6e67  ic water masking
+00029e60: 206d 6574 686f 640d 0a23 5468 6973 206d   method..#This m
+00029e70: 6574 686f 6420 6973 2075 7365 6420 746f  ethod is used to
+00029e80: 2070 726f 7669 6465 2061 2074 696d 652d   provide a time-
+00029e90: 7365 6e73 6974 6976 6520 7761 7465 7220  sensitive water 
+00029ea0: 6d61 736b 0d0a 2354 6869 7320 6d65 7468  mask..#This meth
+00029eb0: 6f64 2074 656e 6473 2074 6f20 776f 726b  od tends to work
+00029ec0: 2077 656c 6c20 6966 2074 6865 7265 2069   well if there i
+00029ed0: 7320 6e6f 2077 6574 2073 6e6f 7720 7072  s no wet snow pr
+00029ee0: 6573 656e 740d 0a23 5765 7420 736e 6f77  esent..#Wet snow
+00029ef0: 206f 7665 7220 666c 6174 2061 7265 6173   over flat areas
+00029f00: 2063 616e 2072 6573 756c 7420 696e 2066   can result in f
+00029f10: 616c 7365 2070 6f73 6974 6976 6573 0d0a  alse positives..
+00029f20: 2344 6573 6967 6e65 6420 746f 2077 6f72  #Designed to wor
+00029f30: 6b20 7769 7468 2054 4f41 2064 6174 612e  k with TOA data.
+00029f40: 2053 5220 6461 7461 2077 696c 6c20 7265   SR data will re
+00029f50: 7375 6c74 2069 6e20 6661 6c73 6520 6e65  sult in false ne
+00029f60: 6761 7469 7665 7320 286f 6d69 7373 696f  gatives (omissio
+00029f70: 6e29 0d0a 6465 6620 7369 6d70 6c65 5761  n)..def simpleWa
+00029f80: 7465 724d 6173 6b28 696d 672c 636f 6e74  terMask(img,cont
+00029f90: 7261 6374 5069 7865 6c73 203d 2030 2c73  ractPixels = 0,s
+00029fa0: 6c6f 7065 5f74 6872 6573 6820 3d20 3130  lope_thresh = 10
+00029fb0: 2c65 6c65 7661 7469 6f6e 496d 6167 6550  ,elevationImageP
+00029fc0: 6174 6820 3d20 2255 5347 532f 3344 4550  ath = "USGS/3DEP
+00029fd0: 2f31 306d 222c 656c 6576 6174 696f 6e46  /10m",elevationF
+00029fe0: 6f63 616c 4d65 616e 5261 6469 7573 203d  ocalMeanRadius =
+00029ff0: 2035 2e35 293a 0d0a 2020 696d 6720 3d20   5.5):..  img = 
+0002a000: 6164 6454 4341 6e67 6c65 7328 696d 6729  addTCAngles(img)
+0002a010: 0d0a 2020 6e65 6420 3d20 6565 2e49 6d61  ..  ned = ee.Ima
+0002a020: 6765 2865 6c65 7661 7469 6f6e 496d 6167  ge(elevationImag
+0002a030: 6550 6174 6829 2e72 6573 616d 706c 6528  ePath).resample(
+0002a040: 2762 6963 7562 6963 2729 0d0a 2020 736c  'bicubic')..  sl
+0002a050: 6f70 6520 3d20 6565 2e54 6572 7261 696e  ope = ee.Terrain
+0002a060: 2e73 6c6f 7065 286e 6564 2e66 6f63 616c  .slope(ned.focal
+0002a070: 5f6d 6561 6e28 656c 6576 6174 696f 6e46  _mean(elevationF
+0002a080: 6f63 616c 4d65 616e 5261 6469 7573 2929  ocalMeanRadius))
+0002a090: 0d0a 2020 666c 6174 203d 2073 6c6f 7065  ..  flat = slope
+0002a0a0: 2e6c 7465 2873 6c6f 7065 5f74 6872 6573  .lte(slope_thres
+0002a0b0: 6829 0d0a 0d0a 2020 7761 7465 724d 6173  h)....  waterMas
+0002a0c0: 6b20 3d20 696d 672e 7365 6c65 6374 285b  k = img.select([
+0002a0d0: 2774 6341 6e67 6c65 4257 275d 292e 6774  'tcAngleBW']).gt
+0002a0e0: 6528 2d30 2e30 3529 5c0d 0a20 2020 202e  e(-0.05)\..    .
+0002a0f0: 416e 6428 696d 672e 7365 6c65 6374 285b  And(img.select([
+0002a100: 2774 6341 6e67 6c65 4247 275d 292e 6c74  'tcAngleBG']).lt
+0002a110: 6528 302e 3035 2929 5c0d 0a20 2020 202e  e(0.05))\..    .
+0002a120: 416e 6428 696d 672e 7365 6c65 6374 285b  And(img.select([
+0002a130: 2762 7269 6768 746e 6573 7327 5d29 2e6c  'brightness']).l
+0002a140: 7428 302e 3329 295c 0d0a 2020 2020 2e41  t(0.3))\..    .A
+0002a150: 6e64 2866 6c61 7429 2e66 6f63 616c 5f6d  nd(flat).focal_m
+0002a160: 696e 2863 6f6e 7472 6163 7450 6978 656c  in(contractPixel
+0002a170: 7329 0d0a 0d0a 2020 7265 7475 726e 2077  s)....  return w
+0002a180: 6174 6572 4d61 736b 2e72 656e 616d 6528  aterMask.rename(
+0002a190: 5b27 7761 7465 724d 6173 6b27 5d29 0d0a  ['waterMask'])..
+0002a1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a1e0: 2323 2323 230d 0a23 4a65 6666 2048 6f20  #####..#Jeff Ho 
+0002a1f0: 4d65 7468 6f64 2066 6f72 2061 6c67 616c  Method for algal
+0002a200: 2062 6c6f 6f6d 2064 6574 6563 7469 6f6e   bloom detection
+0002a210: 0d0a 2368 7474 7073 3a2f 2f77 7777 2e6e  ..#https://www.n
+0002a220: 6174 7572 652e 636f 6d2f 6172 7469 636c  ature.com/articl
+0002a230: 6573 2f73 3431 3538 362d 3031 392d 3136  es/s41586-019-16
+0002a240: 3438 2d37 0d0a 0d0a 2320 5369 6d70 6c69  48-7....# Simpli
+0002a250: 6669 6564 2053 6372 6970 7420 666f 7220  fied Script for 
+0002a260: 4c61 6e64 7361 7420 5761 7465 7220 5175  Landsat Water Qu
+0002a270: 616c 6974 790d 0a23 2050 726f 6475 6365  ality..# Produce
+0002a280: 7320 6120 6d61 7020 6f66 2061 6e20 616c  s a map of an al
+0002a290: 6761 6c20 626c 6f6f 6d20 696e 204c 616b  gal bloom in Lak
+0002a2a0: 6520 4572 6965 206f 6e20 3230 3131 2f39  e Erie on 2011/9
+0002a2b0: 2f33 0d0a 2320 4372 6561 7465 6420 6f6e  /3..# Created on
+0002a2c0: 2031 322f 372f 3230 3135 2062 7920 4a65   12/7/2015 by Je
+0002a2d0: 6666 2048 6f0d 0a0d 0a23 2053 7065 6369  ff Ho....# Speci
+0002a2e0: 6669 6573 2061 2074 6872 6573 686f 6c64  fies a threshold
+0002a2f0: 2066 6f72 2068 7565 2074 6f20 6573 7469   for hue to esti
+0002a300: 6d61 7465 2022 6772 6565 6e22 2070 6978  mate "green" pix
+0002a310: 656c 730d 0a23 2074 6869 7320 6973 2075  els..# this is u
+0002a320: 7365 6420 6173 2061 6e20 6164 6469 7469  sed as an additi
+0002a330: 6f6e 616c 2066 696c 7465 7220 746f 2072  onal filter to r
+0002a340: 6566 696e 6520 7468 6520 616c 676f 7269  efine the algori
+0002a350: 7468 6d20 6162 6f76 650d 0a64 6566 2048  thm above..def H
+0002a360: 6f43 616c 6347 7265 656e 6e65 7373 2869  oCalcGreenness(i
+0002a370: 6d67 293a 0d0a 2020 236d 6170 2072 2c20  mg):..  #map r, 
+0002a380: 672c 2061 6e64 2062 2066 6f72 206d 6f72  g, and b for mor
+0002a390: 6520 7265 6164 6162 6c65 2061 6c67 6562  e readable algeb
+0002a3a0: 7261 2062 656c 6f77 0d0a 2020 7220 3d20  ra below..  r = 
+0002a3b0: 696d 672e 7365 6c65 6374 285b 2772 6564  img.select(['red
+0002a3c0: 275d 290d 0a20 2067 203d 2069 6d67 2e73  '])..  g = img.s
+0002a3d0: 656c 6563 7428 5b27 6772 6565 6e27 5d29  elect(['green'])
+0002a3e0: 0d0a 2020 6220 3d20 696d 672e 7365 6c65  ..  b = img.sele
+0002a3f0: 6374 285b 2762 6c75 6527 5d29 0d0a 0d0a  ct(['blue'])....
+0002a400: 2020 2363 616c 6375 6c61 7465 2069 6e74    #calculate int
+0002a410: 656e 7369 7479 2c20 6875 650d 0a20 2049  ensity, hue..  I
+0002a420: 203d 2072 2e61 6464 2867 292e 6164 6428   = r.add(g).add(
+0002a430: 6229 2e72 656e 616d 6528 5b27 4927 5d29  b).rename(['I'])
+0002a440: 0d0a 2020 6d69 6e73 203d 2072 2e6d 696e  ..  mins = r.min
+0002a450: 2867 292e 6d69 6e28 6229 2e72 656e 616d  (g).min(b).renam
+0002a460: 6528 5b27 6d69 6e73 275d 290d 0a20 2048  e(['mins'])..  H
+0002a470: 203d 206d 696e 732e 7768 6572 6528 6d69   = mins.where(mi
+0002a480: 6e73 2e65 7128 7229 2c28 622e 7375 6274  ns.eq(r),(b.subt
+0002a490: 7261 6374 2872 2929 2e64 6976 6964 6528  ract(r)).divide(
+0002a4a0: 492e 7375 6274 7261 6374 2872 2e6d 756c  I.subtract(r.mul
+0002a4b0: 7469 706c 7928 3329 2929 2e61 6464 2831  tiply(3))).add(1
+0002a4c0: 2920 290d 0a20 2048 203d 2048 2e77 6865  ) )..  H = H.whe
+0002a4d0: 7265 286d 696e 732e 6571 2867 292c 2872  re(mins.eq(g),(r
+0002a4e0: 2e73 7562 7472 6163 7428 6729 292e 6469  .subtract(g)).di
+0002a4f0: 7669 6465 2849 2e73 7562 7472 6163 7428  vide(I.subtract(
+0002a500: 672e 6d75 6c74 6970 6c79 2833 2929 292e  g.multiply(3))).
+0002a510: 6164 6428 3229 2029 0d0a 2020 4820 3d20  add(2) )..  H = 
+0002a520: 482e 7768 6572 6528 6d69 6e73 2e65 7128  H.where(mins.eq(
+0002a530: 6229 2c28 672e 7375 6274 7261 6374 2862  b),(g.subtract(b
+0002a540: 2929 2e64 6976 6964 6528 492e 7375 6274  )).divide(I.subt
+0002a550: 7261 6374 2862 2e6d 756c 7469 706c 7928  ract(b.multiply(
+0002a560: 3329 2929 2029 0d0a 0d0a 2020 2370 6978  3))) )....  #pix
+0002a570: 656c 7320 7769 7468 2068 7565 2062 656c  els with hue bel
+0002a580: 6f77 2031 2e36 206d 6f72 6520 6c69 6b65  ow 1.6 more like
+0002a590: 6c79 2074 6f20 6265 2062 6c6f 6f6d 2061  ly to be bloom a
+0002a5a0: 6e64 206e 6f74 2073 7573 7065 6e64 6564  nd not suspended
+0002a5b0: 2073 6564 696d 656e 740d 0a20 2048 7468   sediment..  Hth
+0002a5c0: 7265 7368 203d 2048 2e6c 7465 2831 2e36  resh = H.lte(1.6
+0002a5d0: 290d 0a0d 0a20 2072 6574 7572 6e20 482e  )....  return H.
+0002a5e0: 7265 6e61 6d65 2827 4827 290d 0a0d 0a0d  rename('H').....
+0002a5f0: 0a23 4170 706c 7920 626c 6f6f 6d20 6465  .#Apply bloom de
+0002a600: 7465 6374 696f 6e20 616c 676f 7269 7468  tection algorith
+0002a610: 6d0d 0a64 6566 2048 6f43 616c 6341 6c67  m..def HoCalcAlg
+0002a620: 6f72 6974 686d 3128 696d 6167 6529 3a0d  orithm1(image):.
+0002a630: 0a20 2074 7275 6563 6f6c 6f72 203d 2031  .  truecolor = 1
+0002a640: 2023 7368 6f77 2074 7275 6520 636f 6c6f   #show true colo
+0002a650: 7220 696d 6167 6520 6173 2077 656c 6c0d  r image as well.
+0002a660: 0a20 2074 6573 7454 6872 6573 6820 3d20  .  testThresh = 
+0002a670: 4661 6c73 6520 2320 6164 6420 6120 6269  False # add a bi
+0002a680: 6e61 7279 2069 6d61 6765 2063 6c61 7373  nary image class
+0002a690: 6966 7969 6e67 2069 6e74 6f20 2262 6c6f  ifying into "blo
+0002a6a0: 6f6d 2261 6e64 2022 6e6f 6e2d 626c 6f6f  om"and "non-bloo
+0002a6b0: 6d0d 0a20 2062 6c6f 6f6d 5468 7265 7368  m..  bloomThresh
+0002a6c0: 6f6c 6420 3d20 302e 3032 3334 3620 2374  old = 0.02346 #t
+0002a6d0: 6872 6573 686f 6c64 2066 6f72 2063 6c61  hreshold for cla
+0002a6e0: 7373 6966 6963 6174 696f 6e20 6669 7420  ssification fit 
+0002a6f0: 6261 7365 6420 6f6e 206f 7468 6572 2064  based on other d
+0002a700: 6174 610d 0a20 2067 7265 656e 6573 7354  ata..  greenessT
+0002a710: 6872 6573 686f 6c64 203d 2031 2e36 0d0a  hreshold = 1.6..
+0002a720: 0d0a 2020 2320 416c 676f 7269 7468 6d20  ..  # Algorithm 
+0002a730: 3120 6261 7365 6420 6f6e 3a0d 0a20 2023  1 based on:..  #
+0002a740: 2057 616e 672c 204d 2e2c 2026 2053 6869   Wang, M., & Shi
+0002a750: 2c20 572e 2028 3230 3037 292e 2054 6865  , W. (2007). The
+0002a760: 204e 4952 2d53 5749 5220 636f 6d62 696e   NIR-SWIR combin
+0002a770: 6564 2061 746d 6f73 7068 6572 6963 0d0a  ed atmospheric..
+0002a780: 2020 2320 2063 6f72 7265 6374 696f 6e20    #  correction 
+0002a790: 6170 7072 6f61 6368 2066 6f72 204d 4f44  approach for MOD
+0002a7a0: 4953 206f 6365 616e 2063 6f6c 6f72 2064  IS ocean color d
+0002a7b0: 6174 6120 7072 6f63 6573 7369 6e67 2e0d  ata processing..
+0002a7c0: 0a20 2023 2020 4f70 7469 6373 2045 7870  .  #  Optics Exp
+0002a7d0: 7265 7373 2c20 3135 2832 3429 2c20 3135  ress, 15(24), 15
+0002a7e0: 3732 32e2 8093 3135 3733 332e 0d0a 0d0a  722...15733.....
+0002a7f0: 2020 2320 4164 6420 7365 636f 6e64 6172    # Add secondar
+0002a800: 7920 6669 6c74 6572 2075 7369 6e67 2067  y filter using g
+0002a810: 7265 656e 6e65 7373 2066 756e 6374 696f  reenness functio
+0002a820: 6e20 6265 6c6f 770d 0a20 2069 6d61 6765  n below..  image
+0002a830: 203d 2069 6d61 6765 2e61 6464 4261 6e64   = image.addBand
+0002a840: 7328 486f 4361 6c63 4772 6565 6e6e 6573  s(HoCalcGreennes
+0002a850: 7328 696d 6167 6529 290d 0a0d 0a20 2023  s(image))....  #
+0002a860: 2041 7070 6c79 2061 6c67 6f72 6974 686d   Apply algorithm
+0002a870: 2031 3a20 4234 202d 2031 2e30 332a 4235   1: B4 - 1.03*B5
+0002a880: 0d0a 2020 2362 6c6f 6f6d 3120 3d20 696d  ..  #bloom1 = im
+0002a890: 6167 652e 7365 6c65 6374 2827 6e69 7227  age.select('nir'
+0002a8a0: 292e 7375 6274 7261 6374 2869 6d61 6765  ).subtract(image
+0002a8b0: 2e73 656c 6563 7428 2773 7769 7231 2729  .select('swir1')
+0002a8c0: 2e6d 756c 7469 706c 7928 312e 3033 2929  .multiply(1.03))
+0002a8d0: 2e72 656e 616d 6528 2762 6c6f 6f6d 3127  .rename('bloom1'
+0002a8e0: 290d 0a0d 0a20 2023 2047 6574 2062 696e  )....  # Get bin
+0002a8f0: 6172 7920 696d 6167 6520 6279 2061 7070  ary image by app
+0002a900: 6c79 696e 6720 7468 6520 7468 7265 7368  lying the thresh
+0002a910: 6f6c 640d 0a20 2062 6c6f 6f6d 315f 6d61  old..  bloom1_ma
+0002a920: 736b 203d 2069 6d61 6765 2e73 656c 6563  sk = image.selec
+0002a930: 7428 2248 2229 2e6c 7465 2867 7265 656e  t("H").lte(green
+0002a940: 6573 7354 6872 6573 686f 6c64 292e 7265  essThreshold).re
+0002a950: 6e61 6d65 285b 2262 6c6f 6f6d 315f 6d61  name(["bloom1_ma
+0002a960: 736b 225d 290d 0a0d 0a0d 0a20 2072 6574  sk"])......  ret
+0002a970: 7572 6e20 696d 6167 655c 0d0a 2020 2020  urn image\..    
+0002a980: 2020 2020 2020 2e61 6464 4261 6e64 7328        .addBands(
+0002a990: 626c 6f6f 6d31 295c 0d0a 2020 2020 2020  bloom1)\..      
+0002a9a0: 2020 2020 2e61 6464 4261 6e64 7328 626c      .addBands(bl
+0002a9b0: 6f6f 6d31 5f6d 6173 6b29 0d0a 0d0a 0d0a  oom1_mask)......
+0002a9c0: 0d0a 0d0a 2320 2f2f 2f2f 2f2f 2f2f 2f2f  ....# //////////
+0002a9d0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a9e0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a9f0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa00: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa10: 0d0a 2320 2f2f 2045 4e44 2046 554e 4354  ..# // END FUNCT
+0002aa20: 494f 4e53 0d0a 2320 2f2f 2f2f 2f2f 2f2f  IONS..# ////////
+0002aa30: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa40: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa50: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa60: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002aa70: 2f2f 2f2f 2f2f 2f2f 0d0a 0d0a 0d0a 7465  ////////......te
+0002aa80: 7374 4172 6561 7320 3d20 7b7d 3b0d 0a74  stAreas = {};..t
+0002aa90: 6573 7441 7265 6173 5b27 434f 275d 203d  estAreas['CO'] =
+0002aaa0: 2065 652e 4765 6f6d 6574 7279 2e50 6f6c   ee.Geometry.Pol
+0002aab0: 7967 6f6e 280d 0a20 2020 2020 2020 205b  ygon(..        [
+0002aac0: 5b5b 2d31 3038 2e32 3836 3330 3530 3930  [[-108.286305090
+0002aad0: 3634 3735 392c 2033 382e 3038 3533 3433  64759, 38.085343
+0002aae0: 3633 3831 3230 3932 355d 2c0d 0a20 2020  638120925],..   
+0002aaf0: 2020 2020 2020 205b 2d31 3038 2e32 3836         [-108.286
+0002ab00: 3330 3530 3930 3634 3735 392c 2033 372e  30509064759, 37.
+0002ab10: 3138 3035 3132 3230 3039 3239 3435 5d2c  18051220092945],
+0002ab20: 0d0a 2020 2020 2020 2020 2020 5b2d 3130  ..          [-10
+0002ab30: 362e 3734 3832 3139 3135 3331 3437 3539  6.74821915314759
+0002ab40: 2c20 3337 2e31 3830 3531 3232 3030 3932  , 37.18051220092
+0002ab50: 3934 355d 2c0d 0a20 2020 2020 2020 2020  945],..         
+0002ab60: 205b 2d31 3036 2e37 3438 3231 3931 3533   [-106.748219153
+0002ab70: 3134 3735 392c 2033 382e 3038 3533 3433  14759, 38.085343
+0002ab80: 3633 3831 3230 3932 355d 5d5d 2c20 4e6f  638120925]]], No
+0002ab90: 6e65 2c20 4661 6c73 6529 0d0a 7465 7374  ne, False)..test
+0002aba0: 4172 6561 735b 2743 4f5f 4e6f 7274 6827  Areas['CO_North'
+0002abb0: 5d20 3d20 6565 2e47 656f 6d65 7472 792e  ] = ee.Geometry.
+0002abc0: 506f 6c79 676f 6e28 0d0a 2020 2020 2020  Polygon(..      
+0002abd0: 2020 5b5b 5b2d 3130 362e 3431 3937 3738    [[[-106.419778
+0002abe0: 3639 3333 3935 3234 2c20 3430 2e39 3739  69339524, 40.979
+0002abf0: 3437 3730 3233 3933 3233 345d 2c0d 0a20  47702393234],.. 
+0002ac00: 2020 2020 2020 2020 205b 2d31 3036 2e34           [-106.4
+0002ac10: 3139 3737 3836 3933 3339 3532 342c 2033  1977869339524, 3
+0002ac20: 392e 3936 3430 3633 3231 3831 3430 3031  9.96406321814001
+0002ac30: 5d2c 0d0a 2020 2020 2020 2020 2020 5b2d  ],..          [-
+0002ac40: 3130 352e 3230 3537 3839 3433 3535 3832  105.205789435582
+0002ac50: 3734 2c20 3339 2e39 3634 3036 3332 3138  74, 39.964063218
+0002ac60: 3134 3030 315d 2c0d 0a20 2020 2020 2020  14001],..       
+0002ac70: 2020 205b 2d31 3035 2e32 3035 3738 3934     [-105.2057894
+0002ac80: 3335 3538 3237 342c 2034 302e 3937 3934  3558274, 40.9794
+0002ac90: 3737 3032 3339 3332 3334 5d5d 5d2c 204e  7702393234]]], N
+0002aca0: 6f6e 652c 2046 616c 7365 290d 0a74 6573  one, False)..tes
+0002acb0: 7441 7265 6173 5b27 4341 275d 203d 6565  tAreas['CA'] =ee
+0002acc0: 2e47 656f 6d65 7472 792e 506f 6c79 676f  .Geometry.Polygo
+0002acd0: 6e28 0d0a 2020 2020 2020 2020 5b5b 5b2d  n(..        [[[-
+0002ace0: 3131 392e 3936 3338 3337 3630 3238 3735  119.963837602875
+0002acf0: 3036 2c20 3337 2e31 3338 3135 3035 3734  06, 37.138150574
+0002ad00: 3130 3837 3134 5d2c 0d0a 2020 2020 2020  108714],..      
+0002ad10: 2020 2020 5b2d 3131 392e 3936 3338 3337      [-119.963837
+0002ad20: 3630 3238 3735 3036 2c20 3336 2e34 3037  60287506, 36.407
+0002ad30: 3734 3431 3231 3036 3432 345d 2c0d 0a20  74412106424],.. 
+0002ad40: 2020 2020 2020 2020 205b 2d31 3137 2e39           [-117.9
+0002ad50: 3533 3333 3935 3536 3030 3030 362c 2033  5333955600006, 3
+0002ad60: 362e 3430 3737 3434 3132 3130 3634 3234  6.40774412106424
+0002ad70: 5d2c 0d0a 2020 2020 2020 2020 2020 5b2d  ],..          [-
+0002ad80: 3131 372e 3935 3333 3339 3535 3630 3030  117.953339556000
+0002ad90: 3036 2c20 3337 2e31 3338 3135 3035 3734  06, 37.138150574
+0002ada0: 3130 3837 3134 5d5d 5d2c 204e 6f6e 652c  108714]]], None,
+0002adb0: 2046 616c 7365 290d 0a0d 0a74 6573 7441   False)....testA
+0002adc0: 7265 6173 5b27 4341 5f53 6d61 6c6c 275d  reas['CA_Small']
+0002add0: 203d 2065 652e 4765 6f6d 6574 7279 2e50   = ee.Geometry.P
+0002ade0: 6f6c 7967 6f6e 280d 0a20 2020 2020 2020  olygon(..       
+0002adf0: 205b 5b5b 2d31 3233 2e32 3235 3636 3936   [[[-123.2256696
+0002ae00: 3833 3734 3632 352c 2033 392e 3637 3732  8374625, 39.6772
+0002ae10: 3039 3539 3932 3639 3135 355d 2c0d 0a20  09599269155],.. 
+0002ae20: 2020 2020 2020 2020 205b 2d31 3233 2e32           [-123.2
+0002ae30: 3235 3636 3936 3833 3734 3632 352c 2033  2566968374625, 3
+0002ae40: 382e 3939 3331 3739 3530 3436 3937 3538  8.99317950469758
+0002ae50: 365d 2c0d 0a20 2020 2020 2020 2020 205b  6],..          [
+0002ae60: 2d31 3232 2e36 3034 3934 3231 3434 3638  -122.60494214468
+0002ae70: 3337 352c 2033 382e 3939 3331 3739 3530  375, 38.99317950
+0002ae80: 3436 3937 3538 365d 2c0d 0a20 2020 2020  4697586],..     
+0002ae90: 2020 2020 205b 2d31 3232 2e36 3034 3934       [-122.60494
+0002aea0: 3231 3434 3638 3337 352c 2033 392e 3637  214468375, 39.67
+0002aeb0: 3732 3039 3539 3932 3639 3135 355d 5d5d  7209599269155]]]
+0002aec0: 2c20 4e6f 6e65 2c20 4661 6c73 6529 0d0a  , None, False)..
+0002aed0: 0d0a 7465 7374 4172 6561 735b 2748 4927  ..testAreas['HI'
+0002aee0: 5d20 3d20 6565 2e47 656f 6d65 7472 792e  ] = ee.Geometry.
+0002aef0: 506f 6c79 676f 6e28 0d0a 2020 2020 2020  Polygon(..      
+0002af00: 2020 5b5b 5b2d 3136 302e 3530 3832 3438    [[[-160.508248
+0002af10: 3734 3435 3035 3434 2c20 3232 2e36 3539  74450544, 22.659
+0002af20: 3831 3435 3133 3930 3934 3734 5d2c 0d0a  814513909474],..
+0002af30: 2020 2020 2020 2020 2020 5b2d 3136 302e            [-160.
+0002af40: 3530 3832 3438 3734 3435 3035 3434 2c20  50824874450544, 
+0002af50: 3138 2e35 3437 3530 3330 3939 3539 3832  18.5475030995982
+0002af60: 375d 2c0d 0a20 2020 2020 2020 2020 205b  7],..          [
+0002af70: 2d31 3534 2e33 3535 3930 3439 3934 3530  -154.35590499450
+0002af80: 3534 342c 2031 382e 3534 3735 3033 3039  544, 18.54750309
+0002af90: 3935 3938 3237 5d2c 0d0a 2020 2020 2020  959827],..      
+0002afa0: 2020 2020 5b2d 3135 342e 3335 3539 3034      [-154.355904
+0002afb0: 3939 3435 3035 3434 2c20 3232 2e36 3539  99450544, 22.659
+0002afc0: 3831 3435 3133 3930 3934 3734 5d5d 5d2c  814513909474]]],
+0002afd0: 204e 6f6e 652c 2046 616c 7365 290d 0a     None, False)..
```

### Comparing `geeViz-2023.7.5/geeViz/migrateGEEAssets.py` & `geeViz-2023.8.1/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/phEEnoViz.py` & `geeViz-2023.8.1/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz/taskManagerLib.py` & `geeViz-2023.8.1/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/geeViz.egg-info/PKG-INFO` & `geeViz-2023.8.1/geeViz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.5
+Version: 2023.8.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.5/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.8.1/geeViz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.5/setup.py` & `geeViz-2023.8.1/setup.py`

 * *Files identical despite different names*

