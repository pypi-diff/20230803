# Comparing `tmp/freestyle-hid-1.0.3.tar.gz` & `tmp/freestyle-hid-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freestyle-hid-1.0.3.tar", last modified: Sun May 16 20:32:33 2021, max compression
+gzip compressed data, was "freestyle-hid-1.1.0.tar", last modified: Thu Aug  3 09:05:35 2023, max compression
```

## Comparing `freestyle-hid-1.0.3.tar` & `freestyle-hid-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.620242 freestyle-hid-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.620242 freestyle-hid-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      518 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/LICENSES/0BSD.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10283 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/data/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/data/known-commands.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/data/known-commands.txt.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/freestyle_hid/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/_hidwrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     9103 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/_session.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/freestyle_hid/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tests/test_freestyle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/freestyle_hid/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tools/encrypted_setup_extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6626 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tools/extract_chatter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2088 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tools/hid_console.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/freestyle_hid/tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/freestyle_hid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      931 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-05-16 20:32:33.000000 freestyle-hid-1.0.3/freestyle_hid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-05-16 20:32:33.624242 freestyle-hid-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-05-16 20:32:26.000000 freestyle-hid-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.220912 freestyle-hid-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.228912 freestyle-hid-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.228912 freestyle-hid-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/LICENSES/0BSD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.228912 freestyle-hid-1.1.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/data/known-commands.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/data/known-commands.txt.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.228912 freestyle-hid-1.1.0/freestyle_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/_freestyle_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/_hidwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/freestyle_hid/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tests/test_freestyle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/freestyle_hid/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tools/encrypted_setup_extractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6626 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tools/extract_chatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tools/hid_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/freestyle_hid/tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/freestyle_hid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 09:05:35.000000 freestyle-hid-1.1.0/freestyle_hid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-03 09:05:35.232912 freestyle-hid-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 09:05:22.000000 freestyle-hid-1.1.0/setup.py
```

### Comparing `freestyle-hid-1.0.3/.github/workflows/pypi.yml` & `freestyle-hid-1.1.0/.github/workflows/pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,23 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.9
+        python-version: 3.x
     - name: Install pypa/build
       run: |
         pip install build
     - name: Build a binary wheel and a source tarball
       run: |
         python -m build --sdist --wheel --outdir dist/ .
     - name: Publish package to TestPyPI
+      if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
     - name: Publish package to PyPI
       if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `freestyle-hid-1.0.3/.github/workflows/pytest.yml` & `freestyle-hid-1.1.0/.github/workflows/pytest.yml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 name: pytest
 
 on:
   push:
   pull_request:
 
 jobs:
-  test:
+  pytest:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: [3.7, 3.8, 3.9]
 
@@ -21,11 +21,11 @@
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
-        pip install .[dev,tools]
+        pip install .[dev,tools,encryption]
     - name: Test with pytest
       run: |
         pytest -vvv --mypy
```

### Comparing `freestyle-hid-1.0.3/.pre-commit-config.yaml` & `freestyle-hid-1.1.0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SPDX-FileCopyrightText: 2013 The freestyle-hid Authors
 #
 # SPDX-License-Identifier: 0BSD
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.0
+    rev: v4.4.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/PyCQA/isort
-    rev: 5.8.0
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies:
           - toml
 -   repo: https://github.com/psf/black
-    rev: 21.5b1
+    rev: 23.3.0
     hooks:
     - id: black
--   repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+-   repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
     - id: flake8
 -   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+    rev: v1.1.2
     hooks:
     - id: reuse
```

### Comparing `freestyle-hid-1.0.3/AUTHORS` & `freestyle-hid-1.1.0/AUTHORS`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Benjamin Schäfer
 Christos Arvanitis
 Diego Elio Pettenò
 Dorian Scholz
 Jim Sifferle
 L. Guruprasad
 Leonard Lausen
+MPM1107
 Mathieu Grivois
 Muhammad Kaisar Arkhan
 Naokazu Terada
 Noel Cragg
 Red Daly
 Ryan Jarvis
 Samuel Martin
```

### Comparing `freestyle-hid-1.0.3/LICENSE` & `freestyle-hid-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/LICENSES/0BSD.txt` & `freestyle-hid-1.1.0/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/LICENSES/Apache-2.0.txt` & `freestyle-hid-1.1.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/LICENSES/MIT.txt` & `freestyle-hid-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/PKG-INFO` & `freestyle-hid-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 Metadata-Version: 2.1
 Name: freestyle-hid
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python implementation of the HID protocol used by Abbott FreeStyle devices
 Home-page: https://github.com/glucometers-tech/freestyle-hid
 Author: Diego Elio Pettenò
 Author-email: flameeyes@flameeyes.com
 License: Apache-2.0
-Description: <!--
-        SPDX-FileCopyrightText: 2013 The freestyle-hid Authors
-        
-        SPDX-License-Identifier: Apache-2.0
-        -->
-        
-        # Python library to interact with Abbott FreeStyle devices
-        
-        This repository includes a library and some tools to interact with Abbott
-        FreeStyle devices that use their
-        [shared HID protocol](https://protocols.glucometers.tech/abbott/shared-hid-protocol.html).
-        
-        ## Tools
-        
-        There are a number of tools that interact with either the devices or with
-        USB session captures that are installed together when selecting the `tools`
-        extra:
-        
-         * `freestyle-hid-console` allows sending direct text messages to a compatible
-           device on the console;
-         * `freestyle-extract-chatter` can produce a "chatter" file based on a capture
-           of an USB session, either from Linux or Windows.
-         * `freestyle-encrypted-setup-extract` is an experimental tool to extract the
-           encryption parameters of devices using the encrypted protocol (e.g. Libre2).
-        
-        ## Development
-        
-        If you want to contribute code, please note that the target language
-        is Python 3.7, and that the style to follow is for the most part PEP8
-        compatible.
-        
-        To set up your development environment follow these guidelines:
-        
-        ```shell
-        $ git clone https://github.com/glucometers-tech/freestyle-hid.git
-        $ cd freestyle-hid
-        $ python3 -m venv --python=python3.7
-        $ . venv/bin/activate
-        $ pip install -e .[dev,tools]
-        $ pre-commit install
-        ```
-        
 Keywords: glucometer,diabetes,freestyle,abbott
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hidapi
+Provides-Extra: encryption
 Provides-Extra: tools
 Provides-Extra: dev
+License-File: AUTHORS
+License-File: LICENSE
+License-File: LICENSES/0BSD.txt
+License-File: LICENSES/Apache-2.0.txt
+License-File: LICENSES/MIT.txt
+
+<!--
+SPDX-FileCopyrightText: 2013 The freestyle-hid Authors
+
+SPDX-License-Identifier: Apache-2.0
+-->
+
+# Python library to interact with Abbott FreeStyle devices
+
+This repository includes a library and some tools to interact with Abbott
+FreeStyle devices that use their
+[shared HID protocol](https://protocols.glucometers.tech/abbott/shared-hid-protocol.html).
+
+## Tools
+
+There are a number of tools that interact with either the devices or with
+USB session captures that are installed together when selecting the `tools`
+extra:
+
+ * `freestyle-hid-console` allows sending direct text messages to a compatible
+   device on the console;
+ * `freestyle-extract-chatter` can produce a "chatter" file based on a capture
+   of an USB session, either from Linux or Windows.
+ * `freestyle-encrypted-setup-extract` is an experimental tool to extract the
+   encryption parameters of devices using the encrypted protocol (e.g. Libre2).
+
+## Development
+
+If you want to contribute code, please note that the target language
+is Python 3.7, and that the style to follow is for the most part PEP8
+compatible.
+
+To set up your development environment follow these guidelines:
+
+```shell
+$ git clone https://github.com/glucometers-tech/freestyle-hid.git
+$ cd freestyle-hid
+$ python3 -m venv --python=python3.7
+$ . venv/bin/activate
+$ pip install -e .[dev,tools]
+$ pre-commit install
+```
```

### Comparing `freestyle-hid-1.0.3/README.md` & `freestyle-hid-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/freestyle_hid/_hidwrapper.py` & `freestyle-hid-1.1.0/freestyle_hid/_hidwrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 except ImportError:
     hid = None
 
 from ._exceptions import HIDError
 
 
 class HidWrapper(abc.ABC):
-
     _handle: Union[BinaryIO, "hid.device"]
 
     def write(self, report: bytes) -> None:
         if len(report) > 65:
             raise HIDError(f"Invalid report length {len(report)}.")
 
         written = self._handle.write(report)
```

### Comparing `freestyle-hid-1.0.3/freestyle_hid/_session.py` & `freestyle-hid-1.1.0/freestyle_hid/_session.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 # SPDX-FileCopyrightText: © 2013 The freestyle-hid Authors
 # SPDX-License-Identifier: Apache-2.0
 
 import csv
 import logging
 import pathlib
+import random
 import re
 from typing import AnyStr, Callable, Iterator, Optional, Sequence, Tuple
 
 import construct
 
-from ._exceptions import ChecksumError, CommandError
+from ._exceptions import (
+    ChecksumError,
+    CommandError,
+    EncryptionHandshakeError,
+    EncryptionNotInitialized,
+    MissingFreeStyleKeys,
+)
+from ._freestyle_encryption import SpeckCMAC, SpeckEncrypt
 from ._hidwrapper import HidWrapper
 
+try:
+    from freestyle_keys import libre2 as libre2_keys
+
+    _HAS_LIBRE2_KEYS = True
+except ImportError:
+    _HAS_LIBRE2_KEYS = False
+
 ABBOTT_VENDOR_ID = 0x1A61
 
 _INIT_COMMAND = 0x01
 _INIT_RESPONSE = 0x71
 
 _KEEPALIVE_RESPONSE = 0x22
 _UNKNOWN_MESSAGE_RESPONSE = 0x30
@@ -51,30 +66,52 @@
 
 _is_init_reply = _create_matcher(_INIT_RESPONSE, b"\x01")
 _is_keepalive_response = _create_matcher(_KEEPALIVE_RESPONSE, None)
 _is_unknown_message_error = _create_matcher(_UNKNOWN_MESSAGE_RESPONSE, b"\x85")
 _is_encryption_missing_error = _create_matcher(_ENCRYPTION_SETUP_RESPONSE, b"\x15")
 _is_encryption_setup_error = _create_matcher(_ENCRYPTION_SETUP_RESPONSE, b"\x14")
 
+_HID_REPORT = construct.Struct(
+    number=construct.Byte, content=construct.Padded(64, construct.GreedyBytes)
+)
+
 _FREESTYLE_MESSAGE = construct.Struct(
-    hid_report=construct.Const(0, construct.Byte),
     message_type=construct.Byte,
     command=construct.Padded(
-        63,  # command can only be up to 62 bytes, but one is used for length.
+        55,  # command can only be up to 54 bytes, but one is used for length.
         construct.Prefixed(construct.Byte, construct.GreedyBytes),
     ),
+    iv_counter=construct.Padding(4),
+    mac=construct.Int32ul,
 )
 
-_FREESTYLE_ENCRYPTED_MESSAGE = construct.Struct(
-    hid_report=construct.Const(0, construct.Byte),
-    message_type=construct.Byte,
-    command=construct.Padded(
-        63,  # command can only be up to 62 bytes, but one is used for length.
-        construct.GreedyBytes,
-    ),
+_CHALLENGE_MESSAGE = construct.Struct(
+    subcmd=construct.Const(0x16, construct.Byte),
+    reader_nonce=construct.Bytes(8),
+    iv=construct.BytesInteger(7, signed=False, swapped=False),
+)
+
+_CHALLENGE_RESPONSE_NOMAC_RAW = construct.Struct(
+    message_type=construct.Const(_ENCRYPTION_SETUP_COMMAND, construct.Byte),
+    length=construct.Const(0x1A, construct.Byte),
+    response_subcmd=construct.Const(0x17, construct.Byte),
+    response=construct.Bytes(16),
+    const1=construct.Const(0x01, construct.Byte),
+)
+
+_CHALLENGE_RESPONSE_RAW = construct.Struct(
+    response=_CHALLENGE_RESPONSE_NOMAC_RAW,
+    mac=construct.Int64ul,
+)
+
+_CHALLENGE_ACCEPTED_MESSAGE = construct.Struct(
+    subcmd=construct.Const(0x18, construct.Byte),
+    encrypted_nonces=construct.Bytes(16),
+    iv=construct.BytesInteger(7, signed=False, swapped=False),
+    mac=construct.Int64ul,
 )
 
 _TEXT_COMPLETION_RE = re.compile(b"CMD (?:OK|Fail!)")
 _TEXT_REPLY_FORMAT = re.compile(
     b"^(?P<message>.*)CKSM:(?P<checksum>[0-9A-F]{8})\r\n"
     b"CMD (?P<status>OK|Fail!)\r\n$",
     re.DOTALL,
@@ -115,65 +152,174 @@
     def __init__(
         self,
         product_id: Optional[int],
         device_path: Optional[pathlib.Path],
         text_message_type: int,
         text_reply_message_type: int,
         encoding: str = "ascii",
+        encrypted: bool = False,
     ) -> None:
-        self._handle = HidWrapper.open(device_path, ABBOTT_VENDOR_ID, product_id)
+        if encrypted and not _HAS_LIBRE2_KEYS:
+            raise MissingFreeStyleKeys()
 
+        self._handle = HidWrapper.open(device_path, ABBOTT_VENDOR_ID, product_id)
         self._text_message_type = text_message_type
         self._text_reply_message_type = text_reply_message_type
         self._encoding = encoding
+        self._encrypted_protocol = encrypted
+
+    def encryption_handshake(self):
+        self.send_command(0x05, b"")
+        response = self.read_response()
+        assert response[0] == 0x06
+        serial = response[1][:13]
+
+        crypt = SpeckCMAC(libre2_keys.AUTHORIZATION_ENCRYPTION_KEY)
+        auth_enc_key = crypt.derive("AuthrEnc".encode(), serial)
+        auth_enc = SpeckEncrypt(auth_enc_key)
+        crypt = SpeckCMAC(libre2_keys.AUTHORIZATION_MAC_KEY)
+        auth_mac_key = crypt.derive("AuthrMAC".encode(), serial)
+        auth_mac = SpeckCMAC(auth_mac_key)
+
+        self.send_command(_ENCRYPTION_SETUP_COMMAND, b"\x11")
+        (response_type, response_bytes) = self.read_response()
+
+        if response_type != _ENCRYPTION_SETUP_RESPONSE:
+            raise EncryptionHandshakeError(
+                f"Unexpected response type: {response_type:02x}"
+            )
+
+        challenge_response = _CHALLENGE_MESSAGE.parse(response_bytes)
+        host_nonce = random.randbytes(8)
+
+        encrypted_challenge_response = auth_enc.encrypt(
+            challenge_response.iv, challenge_response.reader_nonce + host_nonce
+        )
+
+        raw_response_nomac = _CHALLENGE_RESPONSE_NOMAC_RAW.build(
+            {"response": encrypted_challenge_response}
+        )
+        response_mac = auth_mac.sign(raw_response_nomac)
+        raw_response = _CHALLENGE_RESPONSE_RAW.build(
+            {
+                "response": {"response": encrypted_challenge_response},
+                "mac": response_mac,
+            }
+        )
+
+        self._write_hid(raw_response)
+        (response_type, response_bytes) = self.read_response()
+
+        if response_type != _ENCRYPTION_SETUP_RESPONSE:
+            raise EncryptionHandshakeError(
+                f"Unexpected response type: {response_type:02x}"
+            )
+
+        acceptance_response = _CHALLENGE_ACCEPTED_MESSAGE.parse(response_bytes)
+
+        # We need to reconstruct the raw message, so we include the expected type and size.
+        mac = auth_mac.sign(b"\x33\x22" + response_bytes[:24])
+
+        if mac != acceptance_response.mac:
+            raise EncryptionHandshakeError(
+                f"Challenge acceptance has incorrect MAC! Expected {mac:016x} received {acceptance_response.mac:016x}."
+            )
+
+        decoded_nonces = auth_enc.decrypt(
+            acceptance_response.iv, acceptance_response.encrypted_nonces
+        )
+
+        if decoded_nonces != host_nonce + challenge_response.reader_nonce:
+            raise EncryptionHandshakeError("Decrypted nonces do not match expectation.")
+
+        context_key = serial + challenge_response.reader_nonce + host_nonce
+
+        logging.debug(f"Context key established: {context_key.hex()}")
+
+        crypt = SpeckCMAC(libre2_keys.SESSION_ENCRYPTION_KEY)
+        ses_enc_key = crypt.derive("SessnEnc".encode(), context_key)
+        crypt = SpeckCMAC(libre2_keys.SESSION_MAC_KEY)
+        ses_mac_key = crypt.derive("SessnMAC".encode(), context_key)
+        self.crypt_enc = SpeckEncrypt(ses_enc_key)
+        self.crypt_mac = SpeckCMAC(ses_mac_key)
 
     def connect(self):
         """Open connection to the device, starting the knocking sequence."""
+        if self._encrypted_protocol:
+            self.encryption_handshake()
         self.send_command(_INIT_COMMAND, b"")
         response = self.read_response()
         if not _is_init_reply(response):
             raise ConnectionError(
                 f"Connection error: unexpected message %{response[0]:02x}:{response[1].hex()}"
             )
 
+    def encrypt_message(self, packet: bytes):
+        output = bytearray(packet)
+        # 0xFF IV is actually 0, because of some weird padding
+        encrypted = self.crypt_enc.encrypt(0xFF, packet[1:56])
+        output[1:56] = encrypted
+        # Not giving a f**k about the IV counter for now
+        output[56:60] = bytes(4)
+        mac = self.crypt_mac.sign(output[0:60])
+        output[60:64] = int.to_bytes(mac, 8, byteorder="little", signed=False)[4:]
+        return bytes(output)
+
+    def decrypt_message(self, packet: bytes):
+        output = bytearray(packet)
+        mac = self.crypt_mac.sign(packet[:60])
+        mac = int.to_bytes(mac, 8, byteorder="little", signed=False)[4:]
+        assert mac == packet[60:64]
+        iv = int.from_bytes(packet[56:60], "big", signed=False) << 8
+        output[1:56] = self.crypt_enc.decrypt(iv, packet[1:56])
+        return bytes(output)
+
+    def _write_hid(self, packet: bytes, hid_report: int = 0) -> None:
+        usb_packet = _HID_REPORT.build({"number": hid_report, "content": packet})
+        logging.debug(f"Sending packet: {usb_packet!r}")
+        self._handle.write(usb_packet)
+
     def send_command(self, message_type: int, command: bytes, encrypted: bool = False):
         """Send a raw command to the device.
 
         Args:
           message_type: The first byte sent with the report to the device.
           command: The command to send out the device.
         """
-        if encrypted:
-            assert message_type not in _ALWAYS_UNENCRYPTED_MESSAGES
-            meta_construct = _FREESTYLE_ENCRYPTED_MESSAGE
-        else:
-            meta_construct = _FREESTYLE_MESSAGE
 
-        usb_packet = meta_construct.build(
-            {"message_type": message_type, "command": command}
+        message = _FREESTYLE_MESSAGE.build(
+            {"message_type": message_type, "command": command, "mac": 0}
         )
 
-        logging.debug(f"Sending packet: {usb_packet!r}")
-        self._handle.write(usb_packet)
+        if (
+            self._encrypted_protocol
+            and message_type not in _ALWAYS_UNENCRYPTED_MESSAGES
+        ):
+            message = self.encrypt_message(message)
+
+        self._write_hid(message)
 
     def read_response(self, encrypted: bool = False) -> Tuple[int, bytes]:
         """Read the response from the device and extracts it."""
         usb_packet = self._handle.read()
 
         logging.debug(f"Read packet: {usb_packet!r}")
 
         assert usb_packet
         message_type = usb_packet[0]
 
-        if not encrypted or message_type in _ALWAYS_UNENCRYPTED_MESSAGES:
-            message_length = usb_packet[1]
-            message_end_idx = 2 + message_length
-            message_content = usb_packet[2:message_end_idx]
-        else:
-            message_content = usb_packet[1:]
+        if (
+            self._encrypted_protocol
+            and message_type not in _ALWAYS_UNENCRYPTED_MESSAGES
+        ):
+            usb_packet = self.decrypt_message(usb_packet)
+
+        message_length = usb_packet[1]
+        message_end_idx = 2 + message_length
+        message_content = usb_packet[2:message_end_idx]
 
         # hidapi module returns a list of bytes rather than a bytes object.
         message = (message_type, bytes(message_content))
 
         # There appears to be a stray number of 22 01 xx messages being returned
         # by some devices after commands are sent. These do not appear to have
         # meaning, so ignore them and proceed to the next. These are always sent
@@ -182,15 +328,15 @@
         if _is_keepalive_response(message):
             return self.read_response(encrypted=encrypted)
 
         if _is_unknown_message_error(message):
             raise CommandError("Invalid command")
 
         if _is_encryption_missing_error(message):
-            raise CommandError("Device encryption not initialized.")
+            raise EncryptionNotInitialized("Device encryption not initialized.")
 
         if _is_encryption_setup_error(message):
             raise CommandError("Device encryption initialization failed.")
 
         return message
 
     def _send_text_command_raw(self, command: bytes) -> bytes:
```

### Comparing `freestyle-hid-1.0.3/freestyle_hid/tests/test_freestyle.py` & `freestyle-hid-1.1.0/freestyle_hid/tests/test_freestyle.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 
 class TestFreeStyle(unittest.TestCase):
     def test_outgoing_command(self):
         """Test the generation of a new outgoing message."""
 
         self.assertEqual(
-            b"\0\x17\7command\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0"
+            b"\x17\7command\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0"
             b"\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0",
             _session._FREESTYLE_MESSAGE.build(
-                {"message_type": 23, "command": b"command"}
+                {"message_type": 23, "command": b"command", "mac": 0}
             ),
         )
```

### Comparing `freestyle-hid-1.0.3/freestyle_hid/tools/encrypted_setup_extractor.py` & `freestyle-hid-1.1.0/freestyle_hid/tools/encrypted_setup_extractor.py`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/freestyle_hid/tools/extract_chatter.py` & `freestyle-hid-1.1.0/freestyle_hid/tools/extract_chatter.py`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/freestyle_hid/tools/hid_console.py` & `freestyle-hid-1.1.0/freestyle_hid/tools/hid_console.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,35 +42,49 @@
 @click.option(
     "--encoding",
     "-e",
     type=str,
     help="Encoding to use to decode commands returned by the meter",
     default="ascii",
 )
+@click.option(
+    "--encrypted-protocol / --no-encrypted-protocol",
+    default=False,
+    help=(
+        "Whether to use the encrypted protocol to communicate to the device."
+        " This is necessary to talk to Libre2 glucometers."
+    ),
+)
 @click.argument(
     "device-path",
     type=click.Path(exists=True, dir_okay=False, writable=True, allow_dash=False),
     callback=lambda ctx, param, value: pathlib.Path(value) if value else None,
     required=False,
 )
 def main(
     *,
     text_command_type: int,
     text_reply_type: int,
     product_id: Optional[int],
     device_path: Optional[pathlib.Path],
     encoding: str,
+    encrypted_protocol: bool,
 ):
     if not product_id and not device_path:
         raise click.UsageError(
             "One of --product-id or DEVICE_PATH need to be provided."
         )
 
     session = freestyle_hid.Session(
-        product_id, device_path, text_command_type, text_reply_type, encoding=encoding
+        product_id,
+        device_path,
+        text_command_type,
+        text_reply_type,
+        encoding=encoding,
+        encrypted=encrypted_protocol,
     )
 
     session.connect()
 
     while True:
         if sys.stdin.isatty():
             command = input(">>> ")
```

### Comparing `freestyle-hid-1.0.3/freestyle_hid.egg-info/PKG-INFO` & `freestyle-hid-1.1.0/freestyle_hid.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 Metadata-Version: 2.1
 Name: freestyle-hid
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python implementation of the HID protocol used by Abbott FreeStyle devices
 Home-page: https://github.com/glucometers-tech/freestyle-hid
 Author: Diego Elio Pettenò
 Author-email: flameeyes@flameeyes.com
 License: Apache-2.0
-Description: <!--
-        SPDX-FileCopyrightText: 2013 The freestyle-hid Authors
-        
-        SPDX-License-Identifier: Apache-2.0
-        -->
-        
-        # Python library to interact with Abbott FreeStyle devices
-        
-        This repository includes a library and some tools to interact with Abbott
-        FreeStyle devices that use their
-        [shared HID protocol](https://protocols.glucometers.tech/abbott/shared-hid-protocol.html).
-        
-        ## Tools
-        
-        There are a number of tools that interact with either the devices or with
-        USB session captures that are installed together when selecting the `tools`
-        extra:
-        
-         * `freestyle-hid-console` allows sending direct text messages to a compatible
-           device on the console;
-         * `freestyle-extract-chatter` can produce a "chatter" file based on a capture
-           of an USB session, either from Linux or Windows.
-         * `freestyle-encrypted-setup-extract` is an experimental tool to extract the
-           encryption parameters of devices using the encrypted protocol (e.g. Libre2).
-        
-        ## Development
-        
-        If you want to contribute code, please note that the target language
-        is Python 3.7, and that the style to follow is for the most part PEP8
-        compatible.
-        
-        To set up your development environment follow these guidelines:
-        
-        ```shell
-        $ git clone https://github.com/glucometers-tech/freestyle-hid.git
-        $ cd freestyle-hid
-        $ python3 -m venv --python=python3.7
-        $ . venv/bin/activate
-        $ pip install -e .[dev,tools]
-        $ pre-commit install
-        ```
-        
 Keywords: glucometer,diabetes,freestyle,abbott
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hidapi
+Provides-Extra: encryption
 Provides-Extra: tools
 Provides-Extra: dev
+License-File: AUTHORS
+License-File: LICENSE
+License-File: LICENSES/0BSD.txt
+License-File: LICENSES/Apache-2.0.txt
+License-File: LICENSES/MIT.txt
+
+<!--
+SPDX-FileCopyrightText: 2013 The freestyle-hid Authors
+
+SPDX-License-Identifier: Apache-2.0
+-->
+
+# Python library to interact with Abbott FreeStyle devices
+
+This repository includes a library and some tools to interact with Abbott
+FreeStyle devices that use their
+[shared HID protocol](https://protocols.glucometers.tech/abbott/shared-hid-protocol.html).
+
+## Tools
+
+There are a number of tools that interact with either the devices or with
+USB session captures that are installed together when selecting the `tools`
+extra:
+
+ * `freestyle-hid-console` allows sending direct text messages to a compatible
+   device on the console;
+ * `freestyle-extract-chatter` can produce a "chatter" file based on a capture
+   of an USB session, either from Linux or Windows.
+ * `freestyle-encrypted-setup-extract` is an experimental tool to extract the
+   encryption parameters of devices using the encrypted protocol (e.g. Libre2).
+
+## Development
+
+If you want to contribute code, please note that the target language
+is Python 3.7, and that the style to follow is for the most part PEP8
+compatible.
+
+To set up your development environment follow these guidelines:
+
+```shell
+$ git clone https://github.com/glucometers-tech/freestyle-hid.git
+$ cd freestyle-hid
+$ python3 -m venv --python=python3.7
+$ . venv/bin/activate
+$ pip install -e .[dev,tools]
+$ pre-commit install
+```
```

### Comparing `freestyle-hid-1.0.3/freestyle_hid.egg-info/SOURCES.txt` & `freestyle-hid-1.1.0/freestyle_hid.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 LICENSES/0BSD.txt
 LICENSES/Apache-2.0.txt
 LICENSES/MIT.txt
 data/known-commands.txt
 data/known-commands.txt.license
 freestyle_hid/__init__.py
 freestyle_hid/_exceptions.py
+freestyle_hid/_freestyle_encryption.py
 freestyle_hid/_hidwrapper.py
 freestyle_hid/_session.py
 freestyle_hid/py.typed
 freestyle_hid.egg-info/PKG-INFO
 freestyle_hid.egg-info/SOURCES.txt
 freestyle_hid.egg-info/dependency_links.txt
 freestyle_hid.egg-info/entry_points.txt
```

### Comparing `freestyle-hid-1.0.3/pyproject.toml` & `freestyle-hid-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freestyle-hid-1.0.3/setup.cfg` & `freestyle-hid-1.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 install_requires = 
 	construct
 python_requires = ~= 3.7
 
 [options.extras_require]
 hidapi = 
 	hidapi
+encryption = 
+	freestyle-keys
 tools = 
 	click
 	click_log
 	usbmon-tools ~= 3.0
 dev = 
 	mypy
 	pre-commit
```

