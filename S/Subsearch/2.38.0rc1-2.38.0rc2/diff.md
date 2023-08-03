# Comparing `tmp/Subsearch-2.38.0rc1.tar.gz` & `tmp/Subsearch-2.38.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.38.0rc1.tar", last modified: Sat Jul 29 16:20:14 2023, max compression
+gzip compressed data, was "Subsearch-2.38.0rc2.tar", last modified: Thu Aug  3 14:02:36 2023, max compression
```

## Comparing `Subsearch-2.38.0rc1.tar` & `Subsearch-2.38.0rc2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.880535 Subsearch-2.38.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/language_data.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screen_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/screens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/language_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/subsearch_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/system_tray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/core_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.485712 Subsearch-2.38.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-03 14:02:36.485712 Subsearch-2.38.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:02:36.485712 Subsearch-2.38.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.473712 Subsearch-2.38.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 14:02:36.000000 Subsearch-2.38.0rc2/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/language_data.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/subsearch/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.477712 Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.481712 Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screen_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.481712 Subsearch-2.38.0rc2/src/subsearch/gui/screens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screens/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screens/language_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screens/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/screens/subsearch_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/system_tray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.481712 Subsearch-2.38.0rc2/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/providers/core_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:36.485712 Subsearch-2.38.0rc2/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/io_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/io_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/io_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/io_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-03 14:02:18.000000 Subsearch-2.38.0rc2/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.38.0rc1/LICENSE` & `Subsearch-2.38.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/PKG-INFO` & `Subsearch-2.38.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.38.0rc1
+Version: 2.38.0rc2
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.38.0rc1/README.md` & `Subsearch-2.38.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/pyproject.toml` & `Subsearch-2.38.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
 ]
 dependencies = [
-    "selectolax==0.3.15",
+    "selectolax==0.3.16",
     "cloudscraper==1.2.71",
     "num2words==0.5.12",
     "packaging==23.1",
     "requests==2.31.0",
     "pillow==10.0.0",
     "pystray==0.19.4",
     "toml==0.10.2",
@@ -65,15 +65,15 @@
 
 [project.optional-dependencies]
 optional = [
     "black==23.7.0",
     "isort==5.12.0",
     "twine==4.0.2",
     "build==0.10.0",
-    "cx_Freeze==6.15.4",
+    "cx_Freeze==6.15.5",
     "mypy==1.4.1",
     "pipreqs==0.4.13",
 ]
 dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "tox==4.6.4"]
 
 [tool.pytest.ini_options]
 filterwarnings = ['ignore::DeprecationWarning']
```

### Comparing `Subsearch-2.38.0rc1/setup.py` & `Subsearch-2.38.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.38.0rc2/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.38.0rc1
+Version: 2.38.0rc2
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.38.0rc1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.38.0rc2/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/__init__.py` & `Subsearch-2.38.0rc2/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/core.py` & `Subsearch-2.38.0rc2/src/subsearch/core.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/data/data_classes.py` & `Subsearch-2.38.0rc2/src/subsearch/data/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 @dataclass(order=True, slots=True)
 class AppConfig:
     """
     This class is a data structure used to store various configuration options for an application.
     These options include preferences related to subtitle filters, file extensions, providers,
-    automatic actions, context menu options, logging, and other features.
+    automatic actions, context menu options,  and other features.
 
     Attributes:
         language (str): The language setting for the application.
         accept_threshold (int): The threshold value for accepting subtitles.
         hearing_impaired (bool): A flag indicating whether to include hearing-impaired subtitles.
         non_hearing_impaired (bool): A flag indicating whether to include non-hearing-impaired subtitles.
         only_foreign_parts (bool): A flag indicating whether to include only foreign parts subtitles.
@@ -103,15 +103,15 @@
         show_terminal (bool): A flag indicating whether to show the terminal in the application.
         autoload (dict[str, Union[bool, str]]): A dictionary containing autoload options.
         file_extensions (dict[str, bool]): A dictionary containing file extensions.
         providers (dict[str, bool]): A dictionary containing provider options.
         manual_download_on_fail (bool): A flag indicating whether to enable manual downloads on failure.
         multithreading (bool): A flag indicating whether to enable multithreading.
         single_instance (bool): A flag indicating whether to enable single-instance mode.
-        logging (bool): A flag indicating whether to enable logging for the application.
+
 
     Examples:
         >>> config = AppConfig(
         ...     language="english",
         ...     accept_threshold=False,
         ...     hearing_impaired=90,
         ...     non_hearing_impaired=True,
@@ -123,15 +123,14 @@
         ...     show_terminal=False,
         ...     autoload={"rename": True, "move": True, "target_path": "."},
         ...     file_extensions=False,
         ...     providers=True,
         ...     manual_download_on_fail={"mkv": True, "avi": False ...},
         ...     multithreading={"subscene_site": True, "opensubtitles_site": True, "opensubtitles_hash": True ...},
         ...     single_instance=False,
-        ...     logging=True,
         ... )
     """
 
     language: str
     accept_threshold: int
     hearing_impaired: bool
     non_hearing_impaired: bool
@@ -143,15 +142,14 @@
     show_terminal: bool
     subtitle_post_processing: dict[str, Union[bool, str]]
     file_extensions: dict[str, bool]
     providers: dict[str, bool]
     manual_download_on_fail: bool
     multithreading: bool
     single_instance: bool
-    logging: bool
 
 
 @dataclass(order=True, slots=True)
 class SubsceneCookie:
     """
     Represents Subscene website preferences stored in a cookie.
```

### Comparing `Subsearch-2.38.0rc1/src/subsearch/data/language_data.toml` & `Subsearch-2.38.0rc2/src/subsearch/data/language_data.toml`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/__init__.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resource_loader.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/resource_loader.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/spritesheet.png` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/subsearch.ico` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/config.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/config.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/sprites.tcl` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `Subsearch-2.38.0rc2/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/screen_manager.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/screen_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/screens/download_manager.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/screens/download_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/screens/language_options.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/screens/language_options.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/screens/search_options.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/screens/search_options.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/screens/subsearch_options.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/screens/subsearch_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,16 @@
         self.subsearch_options: dict[str, Any] = {
             "gui.context_menu": "Context menu",
             "gui.context_menu_icon": "Context menu icon",
             "gui.system_tray": "System tray icon",
             "gui.summary_notification": "Notification when done",
             "gui.show_terminal": "Terminal while searching",
             "misc.manual_download_on_fail": "Manual download on fail",
-            "misc.logging": "Create log file",
             "misc.multithreading": "Multithreading",
-            "misc.single_instance": "Multiple instances",
+            "misc.single_instance": "Single instance",
         }
         for name, description in self.subsearch_options.items():
             self.subsearch_options[name] = [
                 io_toml.load_toml_value(FILE_PATHS.config, name),
                 description,
             ]
```

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/system_tray.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/system_tray.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/gui/utils.py` & `Subsearch-2.38.0rc2/src/subsearch/gui/utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/providers/core_provider.py` & `Subsearch-2.38.0rc2/src/subsearch/providers/core_provider.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.38.0rc2/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/providers/subscene.py` & `Subsearch-2.38.0rc2/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.38.0rc2/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/decorators.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/exceptions.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/io_app.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/io_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         },
         "file_extensions": file_extensions,
         "providers": providers,
         "misc": {
             "manual_download_on_fail": True,
             "multithreading": True,
             "single_instance": True,
-            "logging": True,
         },
     }
     return config
 
 
 @no_type_check
 def get_video_file_data() -> VideoFile:
```

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/io_file_system.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/io_file_system.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/io_log.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/io_log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/io_toml.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/io_toml.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/state_manager.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/state_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/string_parser.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.38.0rc1/src/subsearch/utils/update.py` & `Subsearch-2.38.0rc2/src/subsearch/utils/update.py`

 * *Files identical despite different names*

