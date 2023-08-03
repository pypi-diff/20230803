# Comparing `tmp/mly_pipeline-0.5.9.tar.gz` & `tmp/mly_pipeline-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.9.tar", last modified: Fri Jul 21 10:16:23 2023, max compression
+gzip compressed data, was "mly_pipeline-0.6.tar", last modified: Thu Aug  3 12:30:36 2023, max compression
```

## Comparing `mly_pipeline-0.5.9.tar` & `mly_pipeline-0.6.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.616546 mly_pipeline-0.5.9/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.9/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.9/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.9/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-21 10:16:23.615546 mly_pipeline-0.5.9/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.9/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.447545 mly_pipeline-0.5.9/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.405544 mly_pipeline-0.5.9/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.503545 mly_pipeline-0.5.9/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2500354 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6427 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9090 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9551 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    69042 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.521546 mly_pipeline-0.5.9/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.536546 mly_pipeline-0.5.9/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.9/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.540546 mly_pipeline-0.5.9/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.9/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.590546 mly_pipeline-0.5.9/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14813 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1142 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4472 2023-05-12 22:36:26.000000 mly_pipeline-0.5.9/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      420 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18215 2023-05-12 22:36:26.000000 mly_pipeline-0.5.9/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3014 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9144 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8510 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1716 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7979 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3317 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26439 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27117 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.598546 mly_pipeline-0.5.9/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5974 2023-07-17 10:26:32.000000 mly_pipeline-0.5.9/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.9/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.9/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1763 2023-07-13 11:09:19.000000 mly_pipeline-0.5.9/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2017 2023-07-13 10:41:45.000000 mly_pipeline-0.5.9/docs/source/runningasearchoffline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13127 2023-07-13 10:22:53.000000 mly_pipeline-0.5.9/docs/source/runningasearchonline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14239 2023-07-11 11:08:34.000000 mly_pipeline-0.5.9/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.608546 mly_pipeline-0.5.9/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.9/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    27971 2023-07-11 10:01:40.000000 mly_pipeline-0.5.9/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.9/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30927 2023-07-12 09:32:36.000000 mly_pipeline-0.5.9/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13202 2023-07-20 15:14:03.000000 mly_pipeline-0.5.9/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33609 2023-07-19 15:01:03.000000 mly_pipeline-0.5.9/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.9/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    19085 2023-07-20 13:01:50.000000 mly_pipeline-0.5.9/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17405 2023-07-18 15:42:00.000000 mly_pipeline-0.5.9/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-17 13:33:09.000000 mly_pipeline-0.5.9/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.614546 mly_pipeline-0.5.9/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.9/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.9/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.613546 mly_pipeline-0.5.9/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2705 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-21 09:26:47.000000 mly_pipeline-0.5.9/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-21 10:16:23.616546 mly_pipeline-0.5.9/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:36.001137 mly_pipeline-0.6/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      140 2023-08-03 10:26:43.000000 mly_pipeline-0.6/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-07-24 14:34:35.000000 mly_pipeline-0.6/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-07-24 14:34:35.000000 mly_pipeline-0.6/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6679 2023-08-03 12:30:36.000137 mly_pipeline-0.6/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.6/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.850136 mly_pipeline-0.6/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.6/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.843136 mly_pipeline-0.6/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.886136 mly_pipeline-0.6/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.6/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.6/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2500354 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6427 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9090 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9551 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    69042 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.904136 mly_pipeline-0.6/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.920136 mly_pipeline-0.6/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.6/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.925136 mly_pipeline-0.6/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.963137 mly_pipeline-0.6/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14813 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1142 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4472 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      420 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.6/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-07-17 10:27:02.000000 mly_pipeline-0.6/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18215 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.6/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.6/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3014 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.6/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9144 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8510 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1716 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.6/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7979 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3317 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26439 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27117 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.970137 mly_pipeline-0.6/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5974 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1763 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2017 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/runningasearchoffline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13127 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/runningasearchonline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14239 2023-07-24 14:34:35.000000 mly_pipeline-0.6/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.980137 mly_pipeline-0.6/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.6/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    27971 2023-07-24 14:34:35.000000 mly_pipeline-0.6/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.6/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8056 2023-08-02 09:51:41.000000 mly_pipeline-0.6/mly_pipeline/create_status_page.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31178 2023-08-03 09:20:18.000000 mly_pipeline-0.6/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13630 2023-08-03 12:28:22.000000 mly_pipeline-0.6/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    24793 2023-08-01 13:34:48.000000 mly_pipeline-0.6/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-24 14:34:35.000000 mly_pipeline-0.6/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    19064 2023-08-03 09:35:09.000000 mly_pipeline-0.6/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17405 2023-07-24 14:34:35.000000 mly_pipeline-0.6/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-24 14:34:35.000000 mly_pipeline-0.6/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.999137 mly_pipeline-0.6/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.6/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-24 14:34:35.000000 mly_pipeline-0.6/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-08-03 12:30:35.984137 mly_pipeline-0.6/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6679 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2740 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      261 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-08-03 12:30:35.000000 mly_pipeline-0.6/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      828 2023-08-03 12:29:16.000000 mly_pipeline-0.6/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-08-03 12:30:36.001137 mly_pipeline-0.6/setup.cfg
```

### Comparing `mly_pipeline-0.5.9/.gitlab-ci.yml` & `mly_pipeline-0.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/LICENSE` & `mly_pipeline-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/PKG-INFO` & `mly_pipeline-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.9
+Version: 0.6
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.9/README.md` & `mly_pipeline-0.6/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/Makefile` & `mly_pipeline-0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.6/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.6/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.6/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.6/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.6/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/index.doctree` & `mly_pipeline-0.6/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.6/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.6/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.6/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/Getting Started.html` & `mly_pipeline-0.6/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/GettingStarted.html` & `mly_pipeline-0.6/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/How to use.html` & `mly_pipeline-0.6/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/HowToUse.html` & `mly_pipeline-0.6/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/Installation.html` & `mly_pipeline-0.6/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_modules/index.html` & `mly_pipeline-0.6/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_modules/io.html` & `mly_pipeline-0.6/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.6/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.6/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.6/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.6/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.6/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.6/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/basic.css` & `mly_pipeline-0.6/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.6/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.6/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.6/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.6/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/doctools.js` & `mly_pipeline-0.6/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.6/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/jquery.js` & `mly_pipeline-0.6/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/language_data.js` & `mly_pipeline-0.6/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/pygments.css` & `mly_pipeline-0.6/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.6/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.6/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/underscore.js` & `mly_pipeline-0.6/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/_static/websupport.js` & `mly_pipeline-0.6/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/genindex.html` & `mly_pipeline-0.6/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/gettingstarted.html` & `mly_pipeline-0.6/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/howtouse.html` & `mly_pipeline-0.6/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/index.html` & `mly_pipeline-0.6/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/installation.html` & `mly_pipeline-0.6/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/objects.inv` & `mly_pipeline-0.6/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/py-modindex.html` & `mly_pipeline-0.6/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/runningasearch.html` & `mly_pipeline-0.6/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/search.html` & `mly_pipeline-0.6/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/searchindex.js` & `mly_pipeline-0.6/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/build/html/settingupasearch.html` & `mly_pipeline-0.6/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/conf.py` & `mly_pipeline-0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/index.rst` & `mly_pipeline-0.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/installation.rst` & `mly_pipeline-0.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/runningasearch.rst` & `mly_pipeline-0.6/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/runningasearchoffline.rst` & `mly_pipeline-0.6/docs/source/runningasearchoffline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/runningasearchonline.rst` & `mly_pipeline-0.6/docs/source/runningasearchonline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/docs/source/settingupasearch.rst` & `mly_pipeline-0.6/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/__init__.py` & `mly_pipeline-0.6/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.6/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.6/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/initialization.py` & `mly_pipeline-0.6/mly_pipeline/initialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,16 @@
 
                 f.write("kill $inferenceID $generationID" + "\n")
                 f.write("singularity instance stop --all" + "\n")
 
                 f.write("python -c \"from mly_pipeline.manager import manage_FAR_inefernce_files; manage_FAR_inefernce_files()\" "+ "\n")
                 f.write("# Need to add a manager of FAR files at the beggining of offline search"+ "\n")
             
+            # Making the FAR plot for the status page
+            f.write("python -c \"from mly_pipeline.manager import far_plot; far_plot();\" "+ "\n")
             # If FAR is already calculated we only need this to run
             f.write("nohup python -m mly_pipeline.offline_search &> search.out & echo $!>>.jobids.txt" + "\n\n")
 
 
 
 def main():
     
@@ -701,12 +703,20 @@
 
         print("Search stopped")
     else:
 
         raise FileNotFoundError(f"The path provided {search_path} does not have a .jobids.txt file to start the search.")
 
 
+def _status_page():
+
+    from .manager import manage_status_page
+    manage_status_page()
+
+
+    
+
 
 if __name__ == "__main__":
     
      main()
```

### Comparing `mly_pipeline-0.5.9/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.6/mly_pipeline/make_eff_estimation.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .search_functions import far, stackVirgo
 
 with open('config.json') as json_file:
     config = json.load(json_file)
 
 config = stackVirgo(config)
 
-os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
+#os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
 which_python = str(subprocess.check_output(['which','python']))[2:-3]
 print(which_python)
 
 # # # Managing arguments
 # 
 # List of arguments to pass:
@@ -105,15 +105,15 @@
             efficiencies = Validator.accuracy(models=models, 
                                         duration=1, 
                                         size=size,
                                         fs=1024,
                                         detectors=config['detectors'], 
                                         labels={"type": "signal"},
                                         backgroundType="real",
-                                        injectionFolder=injection_path,
+                                        injection_source=injection_path,
                                         injectionSNR = injectionSNR,
                                         noiseSourceFile = noiseSource,
                                         windowSize = 16, 
                                         plugins=["correlation_30"], 
                                         mapping=2 * [{"noise":[ 1, 0], "signal":[0, 1]}],
                                         name=f"{injection_path.split('/')[-1]}_{gps_time_start}-{gps_time_end}",
                                         savePath = efficiencyDirectory,
@@ -126,15 +126,15 @@
             efficiencies = Validator.accuracy(models=models, 
                                 duration=1, 
                                 size=size,
                                 fs=1024,
                                 detectors=config['detectors'], 
                                 labels={"type": "signal"},
                                 backgroundType="real",
-                                injectionFolder=injection_path,
+                                injection_source=injection_path,
                                 injectionSNR = injectionSNR,
                                 noiseSourceFile = noiseSource,
                                 windowSize = 16, 
                                 plugins=["correlation_30"], 
                                 mapping=2 * [{"noise":[ 1, 0], "signal":[0, 1]}],
                                 name=f"{injection_path.split('/')[-1]}_{gps_time_start}-{gps_time_end}",
                                 savePath = efficiencyDirectory,
@@ -146,31 +146,31 @@
     
     elif mode=='plot':
         
         farfile_inverse_interpolation = config["farfile"]+"/FARfile_interpolation_inverse.pkl"
         efficiencyDirectory = config["efficiencies"]+"/"
 
         thresholds = {#'10year': far(farfile_inverse_interpolation, 1/(10*365*24*3600) , inverse = True)
-                      '1year': far(farfile_inverse_interpolation, 1/(365*24*3600) , inverse = True)
-                      ,'1month': far(farfile_inverse_interpolation, 1/(365*24*3600/12) , inverse = True)
-                      ,'2hours': far(farfile_inverse_interpolation, 1/(2*3600) , inverse = True)
+                      '4years': far(farfile_inverse_interpolation, 1/(4*365*24*3600) , inverse = True)
+                      ,'1year': far(farfile_inverse_interpolation, 1/(1*365*24*3600) , inverse = True)
+                      ,'12hours': far(farfile_inverse_interpolation, 1/(12*3600) , inverse = True)
 
                      }
 
         print(thresholds)
         
         tkeys=list(thresholds.keys())    
         
         tests= dirlist(efficiencyDirectory)
 
         tests.remove('condor')
         tests.remove('history')
         
         timeInterval = tests[0].split("_")[-1][:-4]
-        
+
         colours=['#377eb8', '#ff7f00', '#4daf4a',
                   '#f781bf', '#a65628', '#984ea3',
                   '#999999', '#e41a1c', '#dede00']
 
         fig,ax=plt.subplots(2,3,figsize=(15,10))
 
         ACC50={}
@@ -200,19 +200,27 @@
 
                     mvave=moving_average(acc,10)
                     for snr in range(1,len(looper)):
 
                         if mvave[snr]>50 and mvave[hrss-1]<=50:
                             ACC50[tkeys[t]][label]=looper[snr]
 
-                    ax[0,t].set_title('Efficiency of FAR '+tkeys[t])
+                    if t==len(tkeys)-1:
+                        ax[0,t].set_title(f"FAR {tkeys[t]} [ {timeInterval} ]")
+                    elif t==0:
+                        ax[0,t].set_title(f"Efficiency at FAR {tkeys[t]}")
+                    else:
+                        ax[0,t].set_title(f"FAR {tkeys[t]}")
+
                     ax[0,t].set_xlabel(xlabel)
                     ax[0,t].set_ylim(0,100)
                     ax[0,t].grid(True,which='both')
 
+
+
                 elif 'snrs' in data.keys():
                     looper = data['snrs']
                     xlabel = 'SNR'
                     
                     
                     for snr in range(len(looper)):
                         count=0
@@ -238,22 +246,22 @@
         ax[1,0].set_ylabel("% of signals detected")
 
         ax[0,2].legend()
         ax[1,2].legend()
 
         fig.savefig('./Efficiencies.png')
 
+        os.mkdir(efficiencyDirectory + 'history/'+timeInterval)
         for test in tests:
 
             os.system('mv '+ efficiencyDirectory + test 
-                      +' '+ efficiencyDirectory + 'history/'+ test)
+                      +' '+ efficiencyDirectory + 'history/'+timeInterval + '/' + test)
 
-            os.system('cp ./Efficiencies.png '
-                      +efficiencyDirectory+'history/Efficiencies_'
-                    +timeInterval+'.png')
+        os.system('cp ./Efficiencies.png '
+                    +efficiencyDirectory+'history/' +timeInterval +'/Efficiencies.png')
 
             
     elif mode=='condor':
         
 
         accounting_group_user=config['accounting_group_user']
         accounting_group=config['accounting_group']
@@ -296,14 +304,15 @@
                        ,error=error
                        ,output=output
                        ,log=log
                        ,getenv=True
                        ,dag=dagman
                        ,extra_lines=["accounting_group_user="+accounting_group_user
                                     ,"accounting_group="+accounting_group
+                                    ,"request_memory = 6144M"
                                     ,"request_disk            = 64M"])
 
             job_list.append(job)
             
             
             
             
@@ -328,14 +337,15 @@
                        ,error=error
                        ,output=output
                        ,log=log
                        ,getenv=True
                        ,dag=dagman
                        ,extra_lines=["accounting_group_user="+accounting_group_user
                                     ,"accounting_group="+accounting_group
+                                    ,"request_memory = 6144M"
                                     ,"request_disk            = 64M"])
 
             job_list.append(job)
 
 
         plot_job = Job(name = 'plotJob'
                    ,executable = which_python
```

### Comparing `mly_pipeline-0.5.9/mly_pipeline/manager.py` & `mly_pipeline-0.6/mly_pipeline/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pickle
 import argparse
 import sys ,time
 import pandas as pd
 import os
 import logging
 import subprocess
-
+import random
 
 from mly.tools import dirlist
 from mly.datatools import *
 from .search_functions import *
 
 
 
@@ -207,54 +207,14 @@
 
             
             # We remove all json files already included in a dataFrame
             for file in jsonList:
                 os.system("rm "+output_directory+file )
 
 
-            # # Plotting all available events in a zero-lagged score rate
-            # # (Might remove in the future, used to see consistency)
-            # testNumber=0
-            # dFramesList  = []
-            # scores=[]
-            # # Listing the files in the directory
-            # # Separating the json from pkl
-            # fileList = dirlist(output_directory)
-            # for file in fileList:
-            #     if ".pkl" in file : dFramesList.append(file)
-
-            # for file in dFramesList:
-
-            #     with open(output_directory+file,'rb') as obj:
-            #         frame_ = pickle.load(obj)
-
-            #     testNumber+=len(frame_)
-
-            #     scores+=list(frame_[frame_['combined']>=restriction]['combined'])
-
-
-            # s=np.sort(scores)[::-1]
-
-
-            # fig,ax1=plt.subplots(figsize=(6,6))
-
-            # ax1.loglog(s,np.arange(len(s))+1,label='O3a '+config['detectors']+' backround')
-            # ax1.set_title(config['detectors']+"-FAR up to : "+str(from_gps(gpstime.gps_time_now()))+", total time: "+"{:.2f}".format(testNumber/config['timeUnit'])+timeUnitDict[config['timeUnit']])
-
-
-            # #ax1.set_yticks(np.array([1e0,1e1,119,1e3,1e4,1e5,1e6]))
-            # #ax1.set_yticklabels(np.array(['10 years','1 year','1 month','3.6 days','8.64 hours', '51.84 min' ,'5.18 min']))
-
-            # ax1.set_ylim(1,)
-            # if restriction>0: ax1.set_xlim(restriction,1)
-            # ax1.set_xlabel("Scores")
-            # ax1.set_ylabel("FAR")
-            # plt.savefig('./'+config['detectors']+"_far.png")
-            # plt.close('all')
-
             
         logger.debug(f"PROCESSES before FAR management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         # # # FileSystem for FAR management
         #
         # Listing all files saved in the temp file (files to be managed)
         detectors= list( det for det in config['detectors'])
@@ -343,261 +303,85 @@
                     except Exception as e:
                         pass
 
         logger.debug(f"PROCESSES before efficiency and buffers management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         # # # Efficiency test buffer management
         #
-        
-        if os.path.isdir(config['efficiencies']):
-            
-            # How many inferences to wait to run the test, roughly how often in seconds
-
-            efficiencyTestBuffer = config["eff_config"]["howOften"]
-
-            # We load all the buffer pods that live in temp
-            buffer_set = []
-            pod_list = sorted(dirlist(config['bufferDirectory']+"/temp"))
-            
-            num_pods = len(pod_list)
-            
-            # If number of the buffer pods are more than maxDataFrameSize, we 
-            # putting them in a dataSet to be used.
-            logger.info(f"Buffer size accumulated: {num_pods}/{efficiencyTestBuffer} .Start efficiency test: {num_pods >= efficiencyTestBuffer}")
-            # I there are enough buffer pods we can save them to be used in an efficiency test.
-            if num_pods >= efficiencyTestBuffer:
-                
-                for each_pod in pod_list[:efficiencyTestBuffer]:
-                    pod = DataPod.load(config['bufferDirectory']+"/temp/"+each_pod) 
-                    buffer_set.append(pod)
-
-                buffer_dataset = DataSet(buffer_set)
-                buffer_dataset.save(config['bufferDirectory']+"/BUFFER_SET")
-
-                logger.info(f"Saving {config['bufferDirectory']}/BUFFER_SET")
-                # Removing all the ones we used after we made sure the set is saved.   
-                for each_pod in pod_list[:efficiencyTestBuffer]:
 
-                    os.system("rm "+config['bufferDirectory']+"/temp/"+each_pod)
-                    
-                # Running the efficiencies script only if the previous has finished.
-                if len(dirlist(config['efficiencies'])) <= 2:
-                    print("RUN EFFICIENCY? YES")
-                    os.system("nohup python -m mly_pipeline.make_eff_estimation --mode condor > efficiencyTest.out &")
-                    logger.info(f"Efficiency test initiated")
-
-
-        logger.debug(f"PROCESSES before fartest management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+        if os.path.isdir(config['efficiencies']):
+            manage_efficiency_test(config)
 
         # # # FAR test management 
         #
 
         manage_FAR_inefernce_files(config)
+        
+        # Update FAR plot
+        far_plot()
+        # # # Update status page
+        manage_status_page()  
 
-        # # The list of all temporary inference files
-        # if os.path.isdir(config['falseAlarmRates']):
-            
-        #     inference_temp_files = dirlist(config['falseAlarmRates'])
-
-        #     for directory in ['hourly', 'condor', 'FARfile','temp']:
-        #         if directory in inference_temp_files: inference_temp_files.remove(directory)
-
-
-        #     # The list of all the files in hourly (grouped by hour/DAG of generation)
-        #     hourly_files = dirlist(config['falseAlarmRates']+"/hourly")
-
-        #     # The list of all condor dagman directories
-        #     condor_files =  dirlist(config['falseAlarmRates']+"/condor")
-
-        #     # The group names (start-end gps) in inference_temp_files
-        #     inference_temp_files_groups = list(file.split("_")[0] for file in inference_temp_files)
-        #     inference_temp_files_groups = list(dict.fromkeys(inference_temp_files_groups))
-
-        #     # The group names inside hourly
-        #     hourly_files_groups = list(file.split("_")[0] for file in hourly_files)
-
-        #     # The group names of condor directories
-        #     condor_groups= list(file.split("_")[0] for file in condor_files)
-
-        #     logger.debug(f"HOURLY GROUPS: {len(hourly_files_groups)}")
-        #     logger.debug(f"TEMP GROUPS: {len(inference_temp_files_groups)}")
-
-        #     # First we will go through the files that already have a group inside hourly
-        #     # We will add them in their corresponding hourly group file and remove them 
-        #     # from inference_temp_files
-
-        #     for hgroup, hfile_name in zip(hourly_files_groups, hourly_files):
-
-        #         if hgroup in inference_temp_files_groups:
-
-        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
-        #                 hfile = pickle.load(obj)
-                    
-        #             hfile_size = int(hfile_name.split("_")[-1][:-4])
-
-        #             to_remove_from_inference_temp_files = []
-
-        #             for file_name in inference_temp_files:
-                        
-        #                 if hgroup in file_name:
-
-        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
-        #                         file = pickle.load(obj)
-
-        #                     file = file[file['score'] >= restriction]
-
-        #                     hfile = pd.concat([hfile, file], ignore_index=True)
-                            
-        #                     # Adding the size of the file to the hourly file
-        #                     hfile_size += int(file_name.split("_")[-1][:-4])
-
-        #                     #TEMPORARY
-        #                     os.system("rm "+config['falseAlarmRates']+"/"+file_name)
-        #                     to_remove_from_inference_temp_files.append(file_name)
-
-        #             new_hfile_name = "_".join(hfile_name.split("_")[:-1])+"_"+str(hfile_size)
-        #             with open(config['falseAlarmRates']+"/hourly/"+new_hfile_name+'.pkl', 'wb') as output:
-        #                 pickle.dump(hfile, output, 4)
-
-        #             os.system("rm "+config['falseAlarmRates']+"/hourly/"+hfile_name)
-
-        #             for file_name in to_remove_from_inference_temp_files:
-        #                 inference_temp_files.remove(file_name)
-
-        #     # Now we can create new hourly files for the new groups that appeared
-        #     # First we reset the inference_temp_files. There will be no already existing froup
-        #     # for those files
-
-        #     # Reseting temp_file_groups 
-        #     inference_temp_files_groups = list(file.split("_")[0] for file in inference_temp_files)
-        #     inference_temp_files_groups = list(dict.fromkeys(inference_temp_files_groups))
-
-        #     # A check to make sure all files left do not belong in an existing group.
-        #     check = all( [ all([hgroup not in file for file in inference_temp_files]) for hgroup in hourly_files_groups] )
-        #     logger.debug(f"All groups left are new: {check}")
-
-
-        #     for tgroup in inference_temp_files_groups:
-
-        #         to_remove_from_inference_temp_files = []
-
-        #         for file_name in inference_temp_files:
-
-        #             if tgroup in file_name:
-
-        #                 if len(to_remove_from_inference_temp_files)==0:
-
-        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
-        #                         new_hfile = pickle.load(obj)
-
-        #                     new_hfile_size = int(file_name.split("_")[-1][:-4])
-
-        #                     to_remove_from_inference_temp_files.append(file_name)
-                        
-        #                 else:
-
-        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
-        #                         file = pickle.load(obj)
-
-        #                     new_hfile = pd.concat([new_hfile, file], ignore_index=True)
-
-        #                     new_hfile_size += int(file_name.split("_")[-1][:-4])
-
-        #                     to_remove_from_inference_temp_files.append(file_name)
-
-        #         new_hfile_name = tgroup+"_"+str(new_hfile_size)
-        #         with open(config['falseAlarmRates']+"/hourly/"+new_hfile_name+'.pkl', 'wb') as output:
-        #             pickle.dump(new_hfile, output, 4)
-
-        #         logger.info(f"Informing / Saving FAR file : {config['falseAlarmRates']}/hourly/{new_hfile_name}.pkl")
-
-        #         for file_name in to_remove_from_inference_temp_files:
-        #             inference_temp_files.remove(file_name)
-
-        #             #TEMPORARY
-        #             os.system("rm "+config['falseAlarmRates']+"/"+file_name)
-
-        #     logger.debug(f"This should be zero, inference_temp_files: {len(inference_temp_files)}")
-
-
-        #     hourly_files = dirlist(config['falseAlarmRates']+"/hourly") 
-
-        #     for i, hfile_name in enumerate(hourly_files):
+        # Timing
+        logger.info(f"Manager loop time:{time.time()-loopT0}, waiting 5 minutes ... ")
+        sys.stdout.flush()
 
-        #         if i==0: 
-        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
-        #                 farfile = pickle.load(obj)
+        time.sleep(5*60)
+        
 
-        #             farfile_size = int(hfile_name.split("_")[-1][:-4])
-        #         else:
-                    
-        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
-        #                 farfile_part = pickle.load(obj)
 
-        #             farfile = pd.concat([farfile, farfile_part], ignore_index=True)
 
-        #             farfile_size += int(hfile_name.split("_")[-1][:-4])
 
-        #     # Deleting the old FARfile before creating the new one (they have the size of tests on their name).
-        #     farfile_to_delete = None
-        #     old_far_files = dirlist(config['falseAlarmRates']+"/FARfile")
-        #     for file in old_far_files:
-        #         if 'FARfile_interpolation' not in file:
-        #             farfile_to_delete = file
-        #             logger.info(f"FARfile to be replaced: {farfile_to_delete}")
-        #             break 
-
-        #     if len(hourly_files)!=0:
-        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_"+str(farfile_size)+".pkl", 'wb') as output:
-        #             pickle.dump(farfile, output, 4)
-
-        #             logger.info(f"New FARfile saved: {config['falseAlarmRates']}/FARfile/FARfile_{farfile_size}.pkl")
-
-        #         far_interpolation_output = far_interpolation(farfile, farfile_size, inverse = False)
-        #         far_interpolation_output_inverse = far_interpolation(farfile, farfile_size, inverse = True)
-
-        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation.pkl", 'wb') as output:
-        #             pickle.dump( far_interpolation_output , output, 4)
-        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_reserve.pkl", 'wb') as output:
-        #             pickle.dump( far_interpolation_output , output, 4)
-                    
-        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_inverse.pkl", 'wb') as output:
-        #             pickle.dump(far_interpolation_output_inverse , output, 4)
-        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_inverse_reserve.pkl", 'wb') as output:
-        #             pickle.dump(far_interpolation_output_inverse , output, 4)
-                
-        #         logger.info(f"New FARfile interpolations saced")
-
-        #         if (farfile_to_delete is not None 
-        #                 and farfile_to_delete!="FARfile_"+str(farfile_size)+".pkl"):
-        #             os.system("rm "+config['falseAlarmRates']+"/FARfile/"+farfile_to_delete)
-                
-        #     # Overwriting config farfile when enough files
-        #     if len(hourly_files)!=0 and (farfile_size) >= 1*365*24*3600 and (config['path']+"/"+config['falseAlarmRates'] not in config['farfile']):
 
-        #         with open('config.json') as json_file:
-        #             _config = json.load(json_file)
-        #             _config['farfile'] = config['falseAlarmRates']+"/FARfile"
-        #         with open("config.json", "w") as config_json:
-        #             json.dump(_config, config_json,indent=4)
-        #             config_json.close()
+def manage_efficiency_test(config = None):
 
-        #         logger.info(f"FARFILE UPDATED FROM THE TEMPORARY TO THE SEARCH LOCAL!")
-        #         raise SystemError("This is just an interuption to load the new FAR sourse.")
+    if config is None:
+        with open('config.json') as json_file:
+            config = json.load(json_file)
 
+    # # # Efficiency test buffer management
+    
+    
+    # How many inferences to wait to run the test, roughly how often in seconds
 
-        # Timing
-        logger.info(f"Manager loop time:{time.time()-loopT0}, waiting 5 minutes ... ")
-        sys.stdout.flush()
+    efficiencyTestBuffer = config["eff_config"]["howOften"]
 
-        time.sleep(5*60)
+    # We load all the buffer pods that live in temp
+    buffer_set = []
+    pod_list = dirlist(config['bufferDirectory']+"/temp")
+    # Shuffling the pods so that the ones used are randomly distributed along the time.
+    random.shuffle(pod_list)
+    
+    num_pods = len(pod_list)
+    
+    # If number of the buffer pods are more than maxDataFrameSize, we 
+    # putting them in a dataSet to be used.
+    logger.info(f"Buffer size accumulated: {num_pods}/{efficiencyTestBuffer} .Start efficiency test: {num_pods >= efficiencyTestBuffer}")
+    # I there are enough buffer pods we can save them to be used in an efficiency test.
+    if num_pods >= efficiencyTestBuffer:
         
+        for each_pod in pod_list[:efficiencyTestBuffer]:
+            pod = DataPod.load(config['bufferDirectory']+"/temp/"+each_pod) 
+            buffer_set.append(pod)
+
+        buffer_dataset = DataSet(buffer_set)
+        buffer_dataset.save(config['bufferDirectory']+"/BUFFER_SET")
+
+        # Deleting the files in temp
+        for each_pod in pod_list:    
+            os.remove(config['bufferDirectory']+"/temp/"+each_pod)
+        
+        # Running the efficiencies script only if the previous has finished.
+        if len(dirlist(config['efficiencies'])) <= 2:
 
+            issue_efficiency_test()
+            logger.info(f"Efficiency test initiated")
 
-
+def issue_efficiency_test():
+            os.system("nohup python -m mly_pipeline.make_eff_estimation --mode condor > efficiencyTest.out &")
 
 def manage_FAR_inefernce_files(config = None):
 
     if config is None:
         with open('config.json') as json_file:
             config = json.load(json_file)
     # # # FAR test management 
@@ -795,14 +579,76 @@
                 json.dump(_config, config_json,indent=4)
                 config_json.close()
 
             logger.info(f"FARFILE UPDATED FROM THE TEMPORARY TO THE SEARCH LOCAL!")
             raise SystemError("This is just an interuption to load the new FAR sourse.")
 
 
+# add here the page function
+def manage_status_page():
+    os.system("nohup python -m mly_pipeline.create_status_page --mode condor > status_page.out &")
+
+def far_plot():
+
+    farfile_path = config['farfile']
+
+
+    for file in os.listdir(farfile_path):
+        if 'interpolation' not in file:
+            main_file = file
+            break
+
+
+    interpolation= farfile_path + '/FARfile_interpolation.pkl'
+    inverse_interpolation= farfile_path + '/FARfile_interpolation_inverse.pkl'
+
+    testnums=int(main_file.split('_')[-1][:-4])
+    years_of_background = "{:0.2f}".format(testnums/365/24/3600)
+
+    with open(interpolation,'rb') as handle:
+        interp= pickle.load(handle)
+
+    with open(inverse_interpolation,'rb') as handle:
+        inverse= pickle.load(handle)
+
+    s = np.arange(1e-2,1,1e-4)
+
+    halfday_score = inverse(1/(12*3600))
+    month_score = inverse(1/(30*24*3600))
+    year_score = inverse(1/(365*24*3600))
+    fouryear_score = inverse(1/(4*365*24*3600))
+
+    print(month_score,year_score,fouryear_score)
+
+    data = interp(s)*24*3600*365
+    print(data[-1])
+    fig, ax  = plt.subplots()
+
+    ax.axis([s[0], 1, data[-1], data[0]])
+
+    ax.loglog(s,data) # IFAR months
+    ax.axvline(x=halfday_score,ls='--',color='black',label ='2/day')#,color=colours[i])
+    ax.axvline(x=month_score,ls='--',color='green',label ='1/month')#,color=colours[i])
+    ax.axvline(x=year_score,ls='--',color='orange',label = '1/year')#,color=colours[i])
+    ax.axvline(x=fouryear_score,ls='--',color='red', label = '1/4years')#,color=colours[i])
+    ax.set_title(f"Background score distribution of {years_of_background} years")
+    ax.set_ylabel("IFAR (years)")
+    ax.set_xlabel("Scores")
+
+    ax.text(halfday_score, 1e3, "{:6.3f}".format(halfday_score), color ='black',fontweight ='bold',horizontalalignment = 'right',verticalalignment ='top')
+    ax.text(month_score, 1e2, "{:6.3f}".format(month_score), color ='green',fontweight ='bold',horizontalalignment = 'right',verticalalignment ='top')
+    ax.text(year_score, 1e1, "{:6.3f}".format(year_score), color ='orange',fontweight ='bold',horizontalalignment = 'right',verticalalignment ='top')
+    ax.text(fouryear_score, 1e0, "{:6.3f}".format(fouryear_score), color ='red',fontweight ='bold',horizontalalignment = 'right',verticalalignment ='top')
+
+
+    ax.legend()
+
+    plt.savefig('far.png')
+
+
 
 if __name__ == "__main__":
         
     main(config)
```

### Comparing `mly_pipeline-0.5.9/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.6/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/offline_search.py` & `mly_pipeline-0.6/mly_pipeline/offline_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                                                 size = 1,
                                                 detectors = config["detectors"],
                                                 backgroundType = "real",
                                                 noiseSourceFile = buffer_pod,
                                                 windowSize = config["required_buffer"],          
                                                 mapping = mapping,
                                                 strides = None,
-                                                plugins = ["correlation_30",'snr'],
+                                                plugins = ["correlation_30"],
                                                 restriction = None,
                                                 podreturn = True,
                                                 **subconfig
                                             )
             except Exception as e:
                 raise(e)
                 continue
@@ -297,15 +297,14 @@
             ifos = [f"{detector}1" for detector in config["detectors"]] 
             
             # Create mly_output dictionary, GraceDB event file basis
             mly_output = {
                 "gpstime": result["GPSH"][0],
                 "far": far(config['farfile']+"/"+"FARfile_interpolation.pkl"
                                             ,result["total"][0], inverse = False),
-                "snr": thepod.snr[-1],
                 "ifos": ifos,
                 "scores": {
                     "coincidence": result["scores1"][0],
                     "coherency": result["scores2"][0],
                     "combined": result["total"][0]
                 }
 
@@ -356,25 +355,25 @@
                     
                 # Saving trigger background DataPod into the trigger_directory
                 with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
                     pickle.dump(buffer_pod, mly_pkl, 4)
 
                 # Creating the strain plot
                 thepod.plot(type_="strain")
-                plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_strain.png")
+                plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_strain.png")
                 plt.clf()
                 # Creating the correlation plot
                 thepod.plot(type_="correlation")
                 plt.savefig(
-                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_correlation.png")
+                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_correlation.png")
                 plt.clf()
                 # Creating the tf_map plot
                 thepod.plot('tf_map')
                 plt.savefig(
-                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_tfmap.png")
+                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_tfmap.png")
 
                 if config['skymap']:
 
                     # Create skymap plugin:
                     sky_map_plugin = createSkymapPlugin(
                         config["nside"], config["fs"], config["duration"])
 
@@ -397,15 +396,15 @@
 
                 mly_output['trigger']=False
 
             mly_output_list.append(mly_output)
             sys.stdout.flush()
 
 
-        tempFrame = pd.DataFrame(columns = ['gpstime','far','snr','ifos'
+        tempFrame = pd.DataFrame(columns = ['gpstime','far','ifos'
                                                     ,'coincidence','coherency'
                                                     ,'combined','central_time','duration','central_freq','bandwidth'
                                                     ,'trigger'])
 
 
         # A check value to make sure we add all the json files.
         frameSizeCheck = len(mly_output_list) 
@@ -427,15 +426,15 @@
 
 
             tempFrame=pd.concat([tempFrame, pd.DataFrame.from_dict(p)]
                                     ,ignore_index=True)
 
                 # Reseting index and sorting by GPS time
             tempFrame = tempFrame.sort_values(by="gpstime").reset_index(drop=True)
-            tempFrame = tempFrame[['gpstime','far','snr','ifos'
+            tempFrame = tempFrame[['gpstime','far','ifos'
                                                     ,'coincidence','coherency'
                                                     ,'combined','central_time','duration','central_freq','bandwidth'
                                                     ,'trigger']]
 
 
         with open(config['output_directory']+file_name_prefix+".pkl", 'wb') as output:
             pickle.dump(tempFrame, output, 4)
```

### Comparing `mly_pipeline-0.5.9/mly_pipeline/search.py` & `mly_pipeline-0.6/mly_pipeline/search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/search_functions.py` & `mly_pipeline-0.6/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.6/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.6/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.9/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.6/mly_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.9
+Version: 0.6
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.9/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.6/mly_pipeline.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 docs/source/runningasearch.rst
 docs/source/runningasearchoffline.rst
 docs/source/runningasearchonline.rst
 docs/source/settingupasearch.rst
 mly_pipeline/__init__.py
 mly_pipeline/continuous_FAR.py
 mly_pipeline/continuous_FAR_test.py
+mly_pipeline/create_status_page.py
 mly_pipeline/initialization.py
 mly_pipeline/make_eff_estimation.py
 mly_pipeline/manager.py
 mly_pipeline/mly_to_grace.py
 mly_pipeline/offline_search.py
 mly_pipeline/search.py
 mly_pipeline/search_functions.py
```

### Comparing `mly_pipeline-0.5.9/pyproject.toml` & `mly_pipeline-0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.9"
+version = "0.6"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
@@ -21,11 +21,11 @@
 
 ]
 
 [project.scripts]
 mly-pipeline-init = "mly_pipeline.initialization:main"
 mly-pipeline-start = "mly_pipeline.initialization:_start_search"
 mly-pipeline-stop = "mly_pipeline.initialization:_end_search"
-
+mly-pipeline-statuspage = "mly_pipeline.initialization:_status_page"
```

