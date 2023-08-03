# Comparing `tmp/xblock_qualtrics_survey-1.2.2.tar.gz` & `tmp/xblock_qualtrics_survey-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock_qualtrics_survey-1.2.2.tar", last modified: Thu Dec 15 11:30:57 2022, max compression
+gzip compressed data, was "xblock_qualtrics_survey-1.3.0.tar", last modified: Thu Aug  3 12:21:41 2023, max compression
```

## Comparing `xblock_qualtrics_survey-1.2.2.tar` & `xblock_qualtrics_survey-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4093 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/public/
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/public/view.css
--rw-r--r--   0 runner    (1001) docker     (122)      565 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/public/view.js
--rw-r--r--   0 runner    (1001) docker     (122)      166 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/public/view.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/scenarios/
--rw-r--r--   0 runner    (1001) docker     (122)      567 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/scenarios/qualtrics-survey-single-simple.xml
--rw-r--r--   0 runner    (1001) docker     (122)      285 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/test_workbench.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      431 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/qualtricssurvey/xblocks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5150 2022-12-15 11:30:49.000000 xblock_qualtrics_survey-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 11:30:57.863356 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4093 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      980 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-12-15 11:30:57.000000 xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.036769 xblock_qualtrics_survey-1.3.0/qualtricssurvey/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.036769 xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.036769 xblock_qualtrics_survey-1.3.0/qualtricssurvey/public/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/public/view.css
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/public/view.js
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/public/view.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/qualtricssurvey/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/scenarios/qualtrics-survey-single-simple.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/qualtricssurvey/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/test_workbench.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/qualtricssurvey/xblocks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5074 2023-08-03 12:21:32.000000 xblock_qualtrics_survey-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:21:41.040770 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-08-03 12:21:41.000000 xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/top_level.txt
```

### Comparing `xblock_qualtrics_survey-1.2.2/LICENSE` & `xblock_qualtrics_survey-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/PKG-INFO` & `xblock_qualtrics_survey-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: xblock_qualtrics_survey
-Version: 1.2.2
+Version: 1.3.0
 Summary: XBlock for linking to a Qualtrics survey
 Home-page: https://github.com/Stanford-Online/xblock-qualtrics-survey
 Author: David Adams
 Author-email: dcadams@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Qualtrics Survey
 ==================
 
@@ -129,9 +126,7 @@
    :width: 100%
 .. |image-cms-settings-menu| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/cms-settings-menu.png
    :width: 100%
 .. |image-cms-view| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/cms-view.png
    :width: 100%
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/lms-view-normal.png
    :width: 100%
-
-
```

### Comparing `xblock_qualtrics_survey-1.2.2/README.rst` & `xblock_qualtrics_survey-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/fragment.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/fragment.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/mixins/scenario.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/mixins/scenario.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/models.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Handle data access logic for the XBlock
 """
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from xblock.fields import Scope
 from xblock.fields import String
 
 
 class QualtricsSurveyModelMixin:
     """
     Handle data access for XBlock instances
```

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/public/view.js` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/public/view.js`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/test_display.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/tests/test_workbench.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/tests/test_workbench.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/qualtricssurvey/views.py` & `xblock_qualtrics_survey-1.3.0/qualtricssurvey/views.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/requirements/constraints.txt` & `xblock_qualtrics_survey-1.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.2.2/setup.py` & `xblock_qualtrics_survey-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 from os import path
 
 from setuptools import find_packages, setup
 
 
-version = '1.2.2'
+version = '1.3.0'
 description = __doc__.strip().split('\n')[0]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst')) as file_in:
     long_description = file_in.read()
 
 
 def load_requirements(*requirements_paths):
@@ -116,16 +116,14 @@
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: JavaScript',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Topic :: Education',
         'Topic :: Internet :: WWW/HTTP',
     ],
     test_suite='qualtricssurvey.tests',
 )
```

### Comparing `xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/PKG-INFO` & `xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: xblock-qualtrics-survey
-Version: 1.2.2
+Version: 1.3.0
 Summary: XBlock for linking to a Qualtrics survey
 Home-page: https://github.com/Stanford-Online/xblock-qualtrics-survey
 Author: David Adams
 Author-email: dcadams@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Qualtrics Survey
 ==================
 
@@ -129,9 +126,7 @@
    :width: 100%
 .. |image-cms-settings-menu| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/cms-settings-menu.png
    :width: 100%
 .. |image-cms-view| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/cms-view.png
    :width: 100%
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/qualtrics-survey/static/images/lms-view-normal.png
    :width: 100%
-
-
```

### Comparing `xblock_qualtrics_survey-1.2.2/xblock_qualtrics_survey.egg-info/SOURCES.txt` & `xblock_qualtrics_survey-1.3.0/xblock_qualtrics_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

