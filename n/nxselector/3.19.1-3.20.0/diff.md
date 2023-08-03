# Comparing `tmp/nxselector-3.19.1.tar.gz` & `tmp/nxselector-3.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxselector-3.19.1.tar", last modified: Fri May 26 04:55:07 2023, max compression
+gzip compressed data, was "nxselector-3.20.0.tar", last modified: Thu Aug  3 09:37:37 2023, max compression
```

## Comparing `nxselector-3.19.1.tar` & `nxselector-3.20.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-04-27 14:05:27.000000 nxselector-3.19.1/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      184 2023-05-22 08:52:51.000000 nxselector-3.19.1/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2023-05-26 04:55:07.704089 nxselector-3.19.1/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)    10354 2023-05-22 08:52:51.000000 nxselector-3.19.1/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.700089 nxselector-3.19.1/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      875 2023-05-22 08:52:51.000000 nxselector-3.19.1/man/nxselector.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     1068 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxselector
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.700089 nxselector-3.19.1/nxselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2023-05-26 04:55:07.000000 nxselector-3.19.1/nxselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     1214 2023-05-26 04:55:07.000000 nxselector-3.19.1/nxselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-05-26 04:55:07.000000 nxselector-3.19.1/nxselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-12-08 08:36:31.000000 nxselector-3.19.1/nxselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       43 2023-05-26 04:55:07.000000 nxselector-3.19.1/nxselector.egg-info/top_level.txt
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/nxsselector/
--rw-r--r--   0 jkotan   (15949) irc         (39)     5920 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/AddDataSourceDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2208 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/CommandThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3391 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/Data.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10030 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/Descriptions.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12784 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/Detectors.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4060 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/DynamicTools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4082 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/EdDataDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9561 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/EdListDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12723 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/Element.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20267 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ElementModel.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4895 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/Frames.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6093 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/GroupsDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1920 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/InfoDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10574 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/LDataDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3434 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/MessageBox.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6011 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/OrderDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20113 2023-05-25 14:20:10.000000 nxselector-3.19.1/nxsselector/Preferences.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11086 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/PropertiesDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    56155 2023-05-25 11:34:47.000000 nxselector-3.19.1/nxsselector/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    46631 2023-05-25 11:34:47.000000 nxselector-3.19.1/nxsselector/ServerState.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    34549 2023-05-25 11:34:47.000000 nxselector-3.19.1/nxsselector/Storage.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    37186 2023-05-26 04:54:13.000000 nxselector-3.19.1/nxsselector/Views.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      976 2023-05-26 04:54:13.000000 nxselector-3.19.1/nxsselector/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/nxsselector/images/
--rw-r--r--   0 jkotan   (15949) irc         (39)    23015 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/images/network_folder.png
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/nxsselector/qrc/
--rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/qrc/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      272 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/qrc/resources.qrc
--rw-r--r--   0 jkotan   (15949) irc         (39)     1216 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/qtapi.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/nxsselector/ui/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3274 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/AddDataSourceDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     2924 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/EdDataDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1142 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/EdListWg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1125 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/GroupsDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     4108 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/InfoDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     9738 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/LDataDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/OrderDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)    54547 2023-05-25 11:34:47.000000 nxselector-3.19.1/nxsselector/ui/Selector.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.19.1/nxsselector/ui/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      207 2023-05-26 04:55:07.704089 nxselector-3.19.1/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     7239 2023-05-25 11:34:47.000000 nxselector-3.19.1/setup.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 04:55:07.704089 nxselector-3.19.1/test/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2182 2019-10-16 16:59:28.000000 nxselector-3.19.1/test/testmy.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.705868 nxselector-3.20.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-04-27 14:05:27.000000 nxselector-3.20.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)      184 2023-05-22 08:52:51.000000 nxselector-3.20.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13863 2023-08-03 09:37:37.705868 nxselector-3.20.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10409 2023-06-23 08:08:12.000000 nxselector-3.20.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.701868 nxselector-3.20.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      875 2023-05-22 08:52:51.000000 nxselector-3.20.0/man/nxselector.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     1068 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxselector
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.701868 nxselector-3.20.0/nxselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13863 2023-08-03 09:37:37.000000 nxselector-3.20.0/nxselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1214 2023-08-03 09:37:37.000000 nxselector-3.20.0/nxselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-08-03 09:37:37.000000 nxselector-3.20.0/nxselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-12-08 08:36:31.000000 nxselector-3.20.0/nxselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       43 2023-08-03 09:37:37.000000 nxselector-3.20.0/nxselector.egg-info/top_level.txt
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.701868 nxselector-3.20.0/nxsselector/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5920 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/AddDataSourceDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2208 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/CommandThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3391 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/Data.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10030 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/Descriptions.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12784 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/Detectors.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4060 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/DynamicTools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4082 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/EdDataDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9561 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/EdListDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12723 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/Element.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20267 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ElementModel.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4895 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/Frames.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6093 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/GroupsDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1920 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/InfoDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10574 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/LDataDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3434 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/MessageBox.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6011 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/OrderDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20113 2023-05-25 14:20:10.000000 nxselector-3.20.0/nxsselector/Preferences.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11086 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/PropertiesDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    56920 2023-08-03 09:29:50.000000 nxselector-3.20.0/nxsselector/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46631 2023-05-25 11:34:47.000000 nxselector-3.20.0/nxsselector/ServerState.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    34549 2023-05-25 11:34:47.000000 nxselector-3.20.0/nxsselector/Storage.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    37186 2023-05-26 04:54:13.000000 nxselector-3.20.0/nxsselector/Views.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      976 2023-08-03 09:29:50.000000 nxselector-3.20.0/nxsselector/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.701868 nxselector-3.20.0/nxsselector/images/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23015 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/images/network_folder.png
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.705868 nxselector-3.20.0/nxsselector/qrc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/qrc/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      272 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/qrc/resources.qrc
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1216 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/qtapi.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.705868 nxselector-3.20.0/nxsselector/ui/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3274 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/AddDataSourceDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2924 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/EdDataDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1142 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/EdListWg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1125 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/GroupsDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4108 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/InfoDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9738 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/LDataDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/OrderDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)    54547 2023-05-25 11:34:47.000000 nxselector-3.20.0/nxsselector/ui/Selector.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.20.0/nxsselector/ui/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      207 2023-08-03 09:37:37.705868 nxselector-3.20.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7239 2023-05-25 11:34:47.000000 nxselector-3.20.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-03 09:37:37.705868 nxselector-3.20.0/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2182 2019-10-16 16:59:28.000000 nxselector-3.20.0/test/testmy.py
```

### Comparing `nxselector-3.19.1/COPYRIGHT` & `nxselector-3.20.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/PKG-INFO` & `nxselector-3.20.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxselector
-Version: 3.19.1
+Version: 3.20.0
 Summary: GUI for Setting Nexus Sardana Recorder
 Home-page: https://github.com/nexdatas/nxselector
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
@@ -67,48 +67,48 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian `buster` and `stretch` or Ubuntu  `focal`, `eoan`, `bionic` packages can be found in the HDRI repository.
+        Debian `bookworm`, `bullseye`, `buster` or Ubuntu  `lunar`, `jammy`, `focal` packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list, e.g.
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/buster-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally,
         
         .. code-block:: console
         
         	  $ apt-get update
-        	  $ apt-get install python-nxsrecselector nxselector
+        	  $ apt-get install python3-nxsrecselector nxselector nxsrecselector
         
         To instal other NexDaTaS packages
         
         .. code-block:: console
         
-        	  $ apt-get install python-nxswriter nxsconfigtool nxstools python-nxsconfigserver nxsconfigserver-db
+        	  $ apt-get install python3-nxswriter nxsconfigtool nxstools python3-nxsconfigserver nxsconfigserver-db
         
         and
         
         .. code-block:: console
         
-        	  $ apt-get install python-sardana-nxsrecorder nxstaurusgui
+        	  $ apt-get install python3-sardana-nxsrecorder nxstaurusgui
         
         for NeXus recorder and MacroGUI packages.
         
         From pip
         ^^^^^^^^
         
         To install it from pip you need also to install pyqt5, e.g.
@@ -165,21 +165,21 @@
         Next, run Astor and change start-up levels: for Pool to 2,
         for MacroServer to 3 and restart servers.
         
         Alternatively, terminate Pool and MacroServer in the terminals and run
         
         .. code-block:: console
         
-                  $ nxsetup -s Pool -l2
+                  $ nxsetup start Pool -l2
         
         wait until Pool is started and run
         
         .. code-block:: console
         
-                  $ nxsetup -s MacroServer -l3
+                  $ nxsetup start MacroServer -l3
         
         
         Additionally, one can create dummy devices by running `sar_demo` in
         
         .. code-block:: console
         
         	  $ spock
@@ -189,31 +189,31 @@
         Setting NeXus Servers
         ^^^^^^^^^^^^^^^^^^^^^
         
         To set up  NeXus Servers run
         
         .. code-block:: console
         
-        	  $ nxsetup -x
+        	  $ nxsetup set
         
         or
         
         .. code-block:: console
         
-                  $ nxsetup -x NXSDataWriter
-                  $ nxsetup -x NXSConfigServer
-        	  $ nxsetup -x NXSRecSelector
+                  $ nxsetup set NXSDataWriter
+                  $ nxsetup set NXSConfigServer
+        	  $ nxsetup set NXSRecSelector
         
         for specific servers.
         
         If the `RecoderPath` property of MacroServer is not set one can do it by
         
         .. code-block:: console
         
-        	  $ nxsetup -a /usr/lib/python2.7/dist-packages/sardananxsrecorder
+        	  $ nxsetup add-recoder-path /usr/lib/python2.7/dist-packages/sardananxsrecorder
         
         where the path should point the `sardananxsrecorder` package.
         
         General overview
         ================
         
         ----------------
```

### Comparing `nxselector-3.19.1/README.rst` & `nxselector-3.20.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,48 +57,48 @@
 .. code-block:: console
 
 	  $ python setup.py install
 
 Debian packages
 ^^^^^^^^^^^^^^^
 
-Debian `buster` and `stretch` or Ubuntu  `focal`, `eoan`, `bionic` packages can be found in the HDRI repository.
+Debian `bookworm`, `bullseye`, `buster` or Ubuntu  `lunar`, `jammy`, `focal` packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
 	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
 
 and then download the corresponding source list, e.g.
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/buster-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
 
 Finally,
 
 .. code-block:: console
 
 	  $ apt-get update
-	  $ apt-get install python-nxsrecselector nxselector
+	  $ apt-get install python3-nxsrecselector nxselector nxsrecselector
 
 To instal other NexDaTaS packages
 
 .. code-block:: console
 
-	  $ apt-get install python-nxswriter nxsconfigtool nxstools python-nxsconfigserver nxsconfigserver-db
+	  $ apt-get install python3-nxswriter nxsconfigtool nxstools python3-nxsconfigserver nxsconfigserver-db
 
 and
 
 .. code-block:: console
 
-	  $ apt-get install python-sardana-nxsrecorder nxstaurusgui
+	  $ apt-get install python3-sardana-nxsrecorder nxstaurusgui
 
 for NeXus recorder and MacroGUI packages.
 
 From pip
 ^^^^^^^^
 
 To install it from pip you need also to install pyqt5, e.g.
@@ -155,21 +155,21 @@
 Next, run Astor and change start-up levels: for Pool to 2,
 for MacroServer to 3 and restart servers.
 
 Alternatively, terminate Pool and MacroServer in the terminals and run
 
 .. code-block:: console
 
-          $ nxsetup -s Pool -l2
+          $ nxsetup start Pool -l2
 
 wait until Pool is started and run
 
 .. code-block:: console
 
-          $ nxsetup -s MacroServer -l3
+          $ nxsetup start MacroServer -l3
 
 
 Additionally, one can create dummy devices by running `sar_demo` in
 
 .. code-block:: console
 
 	  $ spock
@@ -179,31 +179,31 @@
 Setting NeXus Servers
 ^^^^^^^^^^^^^^^^^^^^^
 
 To set up  NeXus Servers run
 
 .. code-block:: console
 
-	  $ nxsetup -x
+	  $ nxsetup set
 
 or
 
 .. code-block:: console
 
-          $ nxsetup -x NXSDataWriter
-          $ nxsetup -x NXSConfigServer
-	  $ nxsetup -x NXSRecSelector
+          $ nxsetup set NXSDataWriter
+          $ nxsetup set NXSConfigServer
+	  $ nxsetup set NXSRecSelector
 
 for specific servers.
 
 If the `RecoderPath` property of MacroServer is not set one can do it by
 
 .. code-block:: console
 
-	  $ nxsetup -a /usr/lib/python2.7/dist-packages/sardananxsrecorder
+	  $ nxsetup add-recoder-path /usr/lib/python2.7/dist-packages/sardananxsrecorder
 
 where the path should point the `sardananxsrecorder` package.
 
 General overview
 ================
 
 ----------------
```

### Comparing `nxselector-3.19.1/man/nxselector.1` & `nxselector-3.20.0/man/nxselector.1`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxselector` & `nxselector-3.20.0/nxselector`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxselector.egg-info/PKG-INFO` & `nxselector-3.20.0/nxselector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxselector
-Version: 3.19.1
+Version: 3.20.0
 Summary: GUI for Setting Nexus Sardana Recorder
 Home-page: https://github.com/nexdatas/nxselector
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
@@ -67,48 +67,48 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian `buster` and `stretch` or Ubuntu  `focal`, `eoan`, `bionic` packages can be found in the HDRI repository.
+        Debian `bookworm`, `bullseye`, `buster` or Ubuntu  `lunar`, `jammy`, `focal` packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list, e.g.
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/buster-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally,
         
         .. code-block:: console
         
         	  $ apt-get update
-        	  $ apt-get install python-nxsrecselector nxselector
+        	  $ apt-get install python3-nxsrecselector nxselector nxsrecselector
         
         To instal other NexDaTaS packages
         
         .. code-block:: console
         
-        	  $ apt-get install python-nxswriter nxsconfigtool nxstools python-nxsconfigserver nxsconfigserver-db
+        	  $ apt-get install python3-nxswriter nxsconfigtool nxstools python3-nxsconfigserver nxsconfigserver-db
         
         and
         
         .. code-block:: console
         
-        	  $ apt-get install python-sardana-nxsrecorder nxstaurusgui
+        	  $ apt-get install python3-sardana-nxsrecorder nxstaurusgui
         
         for NeXus recorder and MacroGUI packages.
         
         From pip
         ^^^^^^^^
         
         To install it from pip you need also to install pyqt5, e.g.
@@ -165,21 +165,21 @@
         Next, run Astor and change start-up levels: for Pool to 2,
         for MacroServer to 3 and restart servers.
         
         Alternatively, terminate Pool and MacroServer in the terminals and run
         
         .. code-block:: console
         
-                  $ nxsetup -s Pool -l2
+                  $ nxsetup start Pool -l2
         
         wait until Pool is started and run
         
         .. code-block:: console
         
-                  $ nxsetup -s MacroServer -l3
+                  $ nxsetup start MacroServer -l3
         
         
         Additionally, one can create dummy devices by running `sar_demo` in
         
         .. code-block:: console
         
         	  $ spock
@@ -189,31 +189,31 @@
         Setting NeXus Servers
         ^^^^^^^^^^^^^^^^^^^^^
         
         To set up  NeXus Servers run
         
         .. code-block:: console
         
-        	  $ nxsetup -x
+        	  $ nxsetup set
         
         or
         
         .. code-block:: console
         
-                  $ nxsetup -x NXSDataWriter
-                  $ nxsetup -x NXSConfigServer
-        	  $ nxsetup -x NXSRecSelector
+                  $ nxsetup set NXSDataWriter
+                  $ nxsetup set NXSConfigServer
+        	  $ nxsetup set NXSRecSelector
         
         for specific servers.
         
         If the `RecoderPath` property of MacroServer is not set one can do it by
         
         .. code-block:: console
         
-        	  $ nxsetup -a /usr/lib/python2.7/dist-packages/sardananxsrecorder
+        	  $ nxsetup add-recoder-path /usr/lib/python2.7/dist-packages/sardananxsrecorder
         
         where the path should point the `sardananxsrecorder` package.
         
         General overview
         ================
         
         ----------------
```

### Comparing `nxselector-3.19.1/nxselector.egg-info/SOURCES.txt` & `nxselector-3.20.0/nxselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/AddDataSourceDlg.py` & `nxselector-3.20.0/nxsselector/AddDataSourceDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/CommandThread.py` & `nxselector-3.20.0/nxsselector/CommandThread.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Data.py` & `nxselector-3.20.0/nxsselector/Data.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Descriptions.py` & `nxselector-3.20.0/nxsselector/Descriptions.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Detectors.py` & `nxselector-3.20.0/nxsselector/Detectors.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/DynamicTools.py` & `nxselector-3.20.0/nxsselector/DynamicTools.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/EdDataDlg.py` & `nxselector-3.20.0/nxsselector/EdDataDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/EdListDlg.py` & `nxselector-3.20.0/nxsselector/EdListDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Element.py` & `nxselector-3.20.0/nxsselector/Element.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ElementModel.py` & `nxselector-3.20.0/nxsselector/ElementModel.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Frames.py` & `nxselector-3.20.0/nxsselector/Frames.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/GroupsDlg.py` & `nxselector-3.20.0/nxsselector/GroupsDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/InfoDlg.py` & `nxselector-3.20.0/nxsselector/InfoDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/LDataDlg.py` & `nxselector-3.20.0/nxsselector/LDataDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/MessageBox.py` & `nxselector-3.20.0/nxsselector/MessageBox.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/OrderDlg.py` & `nxselector-3.20.0/nxsselector/OrderDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Preferences.py` & `nxselector-3.20.0/nxsselector/Preferences.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/PropertiesDlg.py` & `nxselector-3.20.0/nxsselector/PropertiesDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Selector.py` & `nxselector-3.20.0/nxsselector/Selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,32 @@
 
 import logging
 import gc
 #: (:obj:`logging.Logger`) logger object
 logger = logging.getLogger(__name__)
 
 
+def setLoggerLevel(logger, level):
+    global _logginglevel
+    """ sets logging level from string
+    :param logger: logger
+    :type logger: :obj:`logging.logger`
+    :param level: logging level
+    :type level: :obj:`str`
+    """
+    levels = {'debug': logging.DEBUG,
+              'info': logging.INFO,
+              'warning': logging.WARNING,
+              'error': logging.ERROR,
+              'critical': logging.CRITICAL}
+    _logginglevel = level if level in levels else "warning"
+    dlevel = levels.get(level, logging.WARNING)
+    logger.setLevel(dlevel)
+
+
 @UILoadable(with_ui='ui')
 class Selector(Qt.QDialog, TaurusBaseWidget):
     """ main window application dialog """
 
     #: (:class:`taurus.qt.Qt.pyqtSignal`) doorName  signal
     doorName = Qt.pyqtSignal(str)
 
@@ -1431,60 +1449,66 @@
     umode = None
     setdefault = False
     door = None
     switch = True
 
     logger.debug("Using %s" % qt_api)
     if standalone:
-        import taurus.core.util.argparse
-        parser = taurus.core.util.argparse.get_taurus_parser()
+        import argparse
+        parser = argparse.ArgumentParser(
+            description="NeXus Component Selector GUI")
 
-        parser.add_option(
+        parser.add_argument(
             "-s", "--server", dest="server",
             help="selector server")
-        parser.add_option(
+        parser.add_argument(
             "-d", "--door", dest="door",
             help="door device name")
-        parser.add_option(
+        parser.add_argument(
             "-t", "--style", dest="style",
             help="Qt style")
-        parser.add_option(
+        parser.add_argument(
             "-y", "--stylesheet", dest="stylesheet",
             help="Qt stylesheet")
-        parser.add_option(
+        parser.add_argument(
             "-m", "--mode", dest="mode",
             help="interface mode, i.e. simple, user, advanced, "
             "special, expert")
-        parser.add_option(
-            "", "--set-as-default-mode",
+        parser.add_argument(
+            "--set-as-default-mode",
             action="store_true",
             default=False,
             dest="setdefault",
             help="set the current mode as default")
-        parser.add_option(
-            "", "--dont-switch-mntgrp",
+        parser.add_argument(
+            "--dont-switch-mntgrp",
             action="store_false",
             default=True,
             dest="switch",
             help="do not switch MntGrp to the ActiveMntGrp")
+        parser.add_argument(
+            "--log", dest="log",
+            help="logging level, i.e. debug, info, warning, error, critical")
 
         app = Application(
             sys.argv,
-            cmd_line_parser=parser,
             app_name="NXS Component Selector",
             app_version=__version__,
             org_domain="desy.de",
             org_name="DESY")
 
         app.setWindowIcon(Qt.QIcon(":/configtools.png"))
 
-        (options, _) = parser.parse_args()
+        options = parser.parse_args()
         if options.style:
             app.setStyle(options.style)
 
+        if options.log:
+            setLoggerLevel(logger, options.log)
+
         server = options.server
         if options.stylesheet:
             app.setStyleSheet(options.stylesheet)
         elif options.style == "cleanlooks":
             pyqtver = __qt.PYQT_VERSION.split(".")
             if pyqtver and pyqtver[0] == "4":
                 # fix for cleanlooks tooltip colors
```

### Comparing `nxselector-3.19.1/nxsselector/ServerState.py` & `nxselector-3.20.0/nxsselector/ServerState.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Storage.py` & `nxselector-3.20.0/nxsselector/Storage.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/Views.py` & `nxselector-3.20.0/nxsselector/Views.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/__init__.py` & `nxselector-3.20.0/nxsselector/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # package constructor
 
 """ --- NXS Selector --
 GUI for setting Sardana NeXus Recorder
 """
 
 #: (:obj:`str`) version of the application
-__version__ = "3.19.1"
+__version__ = "3.20.0"
```

### Comparing `nxselector-3.19.1/nxsselector/images/network_folder.png` & `nxselector-3.20.0/nxsselector/images/network_folder.png`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/qrc/__init__.py` & `nxselector-3.20.0/nxsselector/qrc/__init__.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/qtapi.py` & `nxselector-3.20.0/nxsselector/qtapi.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/AddDataSourceDlg.ui` & `nxselector-3.20.0/nxsselector/ui/AddDataSourceDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/EdDataDlg.ui` & `nxselector-3.20.0/nxsselector/ui/EdDataDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/EdListWg.ui` & `nxselector-3.20.0/nxsselector/ui/EdListWg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/GroupsDlg.ui` & `nxselector-3.20.0/nxsselector/ui/GroupsDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/InfoDlg.ui` & `nxselector-3.20.0/nxsselector/ui/InfoDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/LDataDlg.ui` & `nxselector-3.20.0/nxsselector/ui/LDataDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/OrderDlg.ui` & `nxselector-3.20.0/nxsselector/ui/OrderDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/Selector.ui` & `nxselector-3.20.0/nxsselector/ui/Selector.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/nxsselector/ui/__init__.py` & `nxselector-3.20.0/nxsselector/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/setup.py` & `nxselector-3.20.0/setup.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.19.1/test/testmy.py` & `nxselector-3.20.0/test/testmy.py`

 * *Files identical despite different names*

