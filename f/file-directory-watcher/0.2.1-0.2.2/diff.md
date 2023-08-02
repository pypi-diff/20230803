# Comparing `tmp/file-directory-watcher-0.2.1.tar.gz` & `tmp/file-directory-watcher-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-directory-watcher-0.2.1.tar", last modified: Wed Aug  2 22:02:08 2023, max compression
+gzip compressed data, was "file-directory-watcher-0.2.2.tar", last modified: Wed Aug  2 22:32:34 2023, max compression
```

## Comparing `file-directory-watcher-0.2.1.tar` & `file-directory-watcher-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.757838 file-directory-watcher-0.2.1/.github/
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/.github/workflows/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      936 2023-08-02 21:56:39.000000 file-directory-watcher-0.2.1/.github/workflows/build.yaml
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       47 2023-08-02 18:50:10.000000 file-directory-watcher-0.2.1/.gitignore
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/.vscode/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      785 2023-08-02 21:34:08.000000 file-directory-watcher-0.2.1/.vscode/launch.json
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)     1071 2023-08-02 21:59:42.000000 file-directory-watcher-0.2.1/LICENSE
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       88 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/PKG-INFO
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-07-23 19:32:17.000000 file-directory-watcher-0.2.1/README.md
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      205 2023-08-02 21:28:01.000000 file-directory-watcher-0.2.1/pyproject.toml
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       20 2023-08-02 21:57:10.000000 file-directory-watcher-0.2.1/requirements.txt
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       38 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/setup.cfg
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.757838 file-directory-watcher-0.2.1/src/
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/src/fdw/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      347 2023-08-02 21:36:02.000000 file-directory-watcher-0.2.1/src/fdw/__main__.py
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/src/file_directory_watcher/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)     4551 2023-08-02 20:03:21.000000 file-directory-watcher-0.2.1/src/file_directory_watcher/app.py
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)     6495 2023-08-02 21:29:04.000000 file-directory-watcher-0.2.1/src/file_directory_watcher/argument_parser.py
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)     1644 2023-08-02 21:29:15.000000 file-directory-watcher-0.2.1/src/file_directory_watcher/cli.py
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)     3755 2023-08-02 21:29:19.000000 file-directory-watcher-0.2.1/src/file_directory_watcher/utils.py
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       88 2023-08-02 22:02:08.000000 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/PKG-INFO
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      549 2023-08-02 22:02:08.000000 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/SOURCES.txt
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)        1 2023-08-02 22:02:08.000000 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/dependency_links.txt
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       42 2023-08-02 22:02:08.000000 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/entry_points.txt
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)       27 2023-08-02 22:02:08.000000 file-directory-watcher-0.2.1/src/file_directory_watcher.egg-info/top_level.txt
-drwxrwxr-x   0 michalpokusa  (1000) michalpokusa  (1000)        0 2023-08-02 22:02:08.761838 file-directory-watcher-0.2.1/tools/
--rw-rw-r--   0 michalpokusa  (1000) michalpokusa  (1000)      332 2023-08-02 21:56:51.000000 file-directory-watcher-0.2.1/tools/build.bash
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.127840 file-directory-watcher-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.119840 file-directory-watcher-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:32:34.127840 file-directory-watcher-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/src/fdw/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/src/fdw/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/src/file_directory_watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/src/file_directory_watcher/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/src/file_directory_watcher/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/src/file_directory_watcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/src/file_directory_watcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 22:32:34.000000 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 22:32:34.000000 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:32:34.000000 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 22:32:34.000000 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 22:32:34.000000 file-directory-watcher-0.2.2/src/file_directory_watcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:32:34.123840 file-directory-watcher-0.2.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-08-02 22:32:19.000000 file-directory-watcher-0.2.2/tools/reinstall.bash
```

### Comparing `file-directory-watcher-0.2.1/.github/workflows/build.yaml` & `file-directory-watcher-0.2.2/.github/workflows/publish-to-pypi.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,31 @@
-name: Build
+name: Build and Publish to PyPI
 
 on:
-  workflow_dispatch:
-    inputs:
-      version:
-        type: string
-        description: 'Version of the app'
-        default: 'dev'
-        required: true
+  push:
+    tags:
+      - "*"
 
 jobs:
-  build:
+  build-and-publish-to-pypi:
+    name: Build and Publish to PyPI
     runs-on: ubuntu-latest
-
-    env:
-      VERSION: "${{ inputs.version }}"
-
     steps:
-    - name: Checkout repository
-      uses: actions/checkout@v3
+      - name: Checkout code
+        uses: actions/checkout@v2
 
-    - name: Set up Python
-      uses: actions/setup-python@v3
-      with:
-        python-version: '3.10'
-
-    - name: Install dependencies
-      run: |
-        python3 -m pip install --upgrade pip
-        pip3 install -r requirements.txt
-
-    - name: Build app
-      run: |
-        echo $(pwd)
-        echo "__version__ = \"${{ env.VERSION }}\"" > src/file_directory_watcher/version.py
-        cat src/file_directory_watcher/version.py
-        bash tools/build.bash
-
-    - name: Upload artifact
-      uses: actions/upload-artifact@v3
-      with:
-        name: fdw
-        path: build/dist/fdw
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.x
+
+      - name: Install dependencies
+        run: python3 -m pip install --upgrade pip build twine
+
+      - name: Build package
+        run: python3 -m build
+
+      - name: Publish to PyPI
+        env:
+          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
+        run: twine upload dist/*
```

### Comparing `file-directory-watcher-0.2.1/LICENSE` & `file-directory-watcher-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.2.1/src/file_directory_watcher/app.py` & `file-directory-watcher-0.2.2/src/file_directory_watcher/app.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.2.1/src/file_directory_watcher/argument_parser.py` & `file-directory-watcher-0.2.2/src/file_directory_watcher/argument_parser.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.2.1/src/file_directory_watcher/cli.py` & `file-directory-watcher-0.2.2/src/file_directory_watcher/cli.py`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.2.1/src/file_directory_watcher/utils.py` & `file-directory-watcher-0.2.2/src/file_directory_watcher/utils.py`

 * *Files identical despite different names*

