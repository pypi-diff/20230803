# Comparing `tmp/invideoquiz-xblock-1.2.1.tar.gz` & `tmp/invideoquiz-xblock-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invideoquiz-xblock-1.2.1.tar", last modified: Thu Nov 24 11:19:51 2022, max compression
+gzip compressed data, was "invideoquiz-xblock-1.3.1.tar", last modified: Thu Aug  3 12:10:46 2023, max compression
```

## Comparing `invideoquiz-xblock-1.2.1.tar` & `invideoquiz-xblock-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3235 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5905 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/invideoquiz.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/public/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/public/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/public/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/public/css/invideoquiz.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/public/html/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/public/html/invideoquiz.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz/public/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)      546 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/public/js/src/config.js
--rw-r--r--   0 runner    (1001) docker     (122)     6046 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/public/js/src/invideoquiz.js
--rw-r--r--   0 runner    (1001) docker     (122)      263 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/invideoquiz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      636 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-24 11:19:51.000000 invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      607 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-24 11:19:51.267026 invideoquiz-xblock-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6002 2022-11-24 11:19:40.000000 invideoquiz-xblock-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/LICENSE-BSD-3c
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.968996 invideoquiz-xblock-1.3.1/invideoquiz/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5905 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/invideoquiz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.968996 invideoquiz-xblock-1.3.1/invideoquiz/public/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/public/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/invideoquiz/public/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/public/css/invideoquiz.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/invideoquiz/public/html/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/public/html/invideoquiz.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.968996 invideoquiz-xblock-1.3.1/invideoquiz/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/invideoquiz/public/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/public/js/src/config.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6046 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/public/js/src/invideoquiz.js
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/invideoquiz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-03 12:10:46.000000 invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-03 12:10:46.972996 invideoquiz-xblock-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-08-03 12:10:40.000000 invideoquiz-xblock-1.3.1/setup.py
```

### Comparing `invideoquiz-xblock-1.2.1/LICENSE` & `invideoquiz-xblock-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/PKG-INFO` & `invideoquiz-xblock-1.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: invideoquiz-xblock
-Version: 1.2.1
+Version: 1.3.1
 Summary: Helper XBlock to locate CAPA problems within videos.
-Home-page: UNKNOWN
 License: AGPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
+License-File: LICENSE-BSD-3c
 
-UNKNOWN
-
+Helper XBlock to locate CAPA problems within videos.
```

### Comparing `invideoquiz-xblock-1.2.1/README.rst` & `invideoquiz-xblock-1.3.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 In Video Quiz XBlock
 ====================
 
 This XBlock allows for edX components to be displayed to users inside of videos at specific time points.
 
+License
+-------
+
+This software was forked from https://github.com/Stanford-Online/xblock-in-video-quiz
+
+All contribution made to those repositories, the last of which is tagged
+`final-bsd-3c-contribution`_, are licensed by the original contributors under
+the terms of the `BSD 3-Clause License`_.
+
+This software is now maintained for the purpose of the Open edX Project, which
+licenses any further contributions to this repository under `the AGPLv3 license`_.
+
+.. _final-bsd-3c-contribution: https://github.com/openedx/xblock-in-video-quiz/releases/tag/final-bsd-3c-contribution
+.. _BSD 3-Clause License: ./LICENSE-BSD-3c
+.. _the APGLv3 license: ./LICENSE
+
+
 Overview
 --------
 
 This XBlock expects to have a Video component and a Problem component
 added to the same Unit as itself.
 
 The XBlock is then configured (see below) to map timestamps (in seconds)
```

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz/invideoquiz.py` & `invideoquiz-xblock-1.3.1/invideoquiz/invideoquiz.py`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz/public/README.txt` & `invideoquiz-xblock-1.3.1/invideoquiz/public/README.txt`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz/public/css/invideoquiz.css` & `invideoquiz-xblock-1.3.1/invideoquiz/public/css/invideoquiz.css`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz/public/js/src/config.js` & `invideoquiz-xblock-1.3.1/invideoquiz/public/js/src/config.js`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz/public/js/src/invideoquiz.js` & `invideoquiz-xblock-1.3.1/invideoquiz/public/js/src/invideoquiz.js`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/invideoquiz_xblock.egg-info/PKG-INFO` & `invideoquiz-xblock-1.3.1/invideoquiz_xblock.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: invideoquiz-xblock
-Version: 1.2.1
+Version: 1.3.1
 Summary: Helper XBlock to locate CAPA problems within videos.
-Home-page: UNKNOWN
 License: AGPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
+License-File: LICENSE-BSD-3c
 
-UNKNOWN
-
+Helper XBlock to locate CAPA problems within videos.
```

### Comparing `invideoquiz-xblock-1.2.1/requirements/constraints.txt` & `invideoquiz-xblock-1.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.2.1/setup.py` & `invideoquiz-xblock-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 VERSION = get_version("invideoquiz/__init__.py")
 
 
 setup(
     name='invideoquiz-xblock',
     version=VERSION,
     description='Helper XBlock to locate CAPA problems within videos.',
+    long_description='Helper XBlock to locate CAPA problems within videos.',
     license='AGPL v3',
     packages=[
         'invideoquiz',
     ],
     install_requires=load_requirements('requirements/base.in'),
     dependency_links=[
         'https://github.com/openedx/xblock-utils/tarball/c39bf653e4f27fb3798662ef64cde99f57603f79#egg=xblock-utils',
@@ -145,18 +146,16 @@
             'invideoquiz = invideoquiz:InVideoQuizXBlock',
         ],
     },
     package_data=package_data('invideoquiz', ['static', 'public']),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
 )
```

