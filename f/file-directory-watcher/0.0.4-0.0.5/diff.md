# Comparing `tmp/file-directory-watcher-0.0.4.tar.gz` & `tmp/file-directory-watcher-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-directory-watcher-0.0.4.tar", last modified: Thu Aug  3 19:36:43 2023, max compression
+gzip compressed data, was "file-directory-watcher-0.0.5.tar", last modified: Thu Aug  3 19:40:27 2023, max compression
```

## Comparing `file-directory-watcher-0.0.4.tar` & `file-directory-watcher-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.037657 file-directory-watcher-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:36:43.037657 file-directory-watcher-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/src/fdw/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/src/fdw/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/src/file_directory_watcher/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/src/file_directory_watcher/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/src/file_directory_watcher/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/src/file_directory_watcher/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/src/file_directory_watcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 19:36:43.000000 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-03 19:36:43.000000 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:36:43.000000 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 19:36:43.000000 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 19:36:43.000000 file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:36:43.033656 file-directory-watcher-0.0.4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-08-03 19:36:25.000000 file-directory-watcher-0.0.4/tools/reinstall.bash
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.578551 file-directory-watcher-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-03 19:40:27.578551 file-directory-watcher-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:40:27.578551 file-directory-watcher-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/src/fdw/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/src/fdw/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.574551 file-directory-watcher-0.0.5/src/file_directory_watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/src/file_directory_watcher/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/src/file_directory_watcher/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/src/file_directory_watcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/src/file_directory_watcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.578551 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-03 19:40:27.000000 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-03 19:40:27.000000 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:40:27.000000 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 19:40:27.000000 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 19:40:27.000000 file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:40:27.578551 file-directory-watcher-0.0.5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-08-03 19:40:10.000000 file-directory-watcher-0.0.5/tools/reinstall.bash
```

### Comparing `file-directory-watcher-0.0.4/.github/workflows/publish-to-pypi.yaml` & `file-directory-watcher-0.0.5/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/LICENSE` & `file-directory-watcher-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/src/file_directory_watcher/app.py` & `file-directory-watcher-0.0.5/src/file_directory_watcher/app.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/src/file_directory_watcher/argument_parser.py` & `file-directory-watcher-0.0.5/src/file_directory_watcher/argument_parser.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/src/file_directory_watcher/cli.py` & `file-directory-watcher-0.0.5/src/file_directory_watcher/cli.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/src/file_directory_watcher/utils.py` & `file-directory-watcher-0.0.5/src/file_directory_watcher/utils.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.4/src/file_directory_watcher.egg-info/SOURCES.txt` & `file-directory-watcher-0.0.5/src/file_directory_watcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

