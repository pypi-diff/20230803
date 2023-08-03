# Comparing `tmp/hatch_ci-0.0.3b12.tar.gz` & `tmp/hatch_ci-0.0.3b13.tar.gz`

## Comparing `hatch_ci-0.0.3b12.tar` & `hatch_ci-0.0.3b13.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.gitattributes
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/Makefile
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.github/workflows/beta.yml
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.github/workflows/master.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.github/workflows/tags.yml
--rw-r--r--   0        0        0    24275 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    84025 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    48062 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0    84467 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/style.css
--rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/junit/junit.html
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/junit/junit.xml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    44948 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0    49030 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/script.py
--rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/tests/test_scm.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/LICENSE.txt
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/README.md
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/pyproject.toml
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b12/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.gitattributes
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/Makefile
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/master.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    23580 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    84025 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    48062 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0    84467 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    44948 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    48994 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/script.py
+-rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/test_scm.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/LICENSE.txt
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/README.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/pyproject.toml
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/PKG-INFO
```

### Comparing `hatch_ci-0.0.3b12/.pre-commit-config.yaml` & `hatch_ci-0.0.3b13/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/.github/workflows/beta.yml` & `hatch_ci-0.0.3b13/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/.github/workflows/master.yml` & `hatch_ci-0.0.3b13/.github/workflows/master.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.8", "3.9", "3.10", "3.11",]
     runs-on: ${{ matrix.os }}
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Dump env
         shell: bash
         env:
           GITHUB_DUMP: ${{ toJson(github) }}
         run: |
           echo "github env:"
           echo "$GITHUB_DUMP"
 
       - name: Set up Python interpreter [${{ matrix.python-version }}]
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         shell: bash
         run: |
             python -m pip install --upgrade pip
@@ -61,15 +61,15 @@
           py.test \
               --cov=hatch_ci \
               --cov-report=html:$OUTDIR/coverage --cov-report=xml:$OUTDIR/coverage.xml \
               --junitxml=$OUTDIR/junit/junit.xml --html=$OUTDIR/junit/junit.html --self-contained-html \
             tests
 
       - name: Upload pytest test results
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: pytest-results-${{ matrix.python-version }}-${{ matrix.os }}
           path: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         # Use always() to always run this step to publish test results when there are test failures
         if: always()
 
       - name: "Upload coverage to Codecov"
```

### Comparing `hatch_ci-0.0.3b12/.github/workflows/tags.yml` & `hatch_ci-0.0.3b13/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage.xml` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml`

 * *Files 4% similar despite different names*

#### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage.xml` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1690920296057" lines-valid="478" lines-covered="278" line-rate="0.5816" branches-valid="188" branches-covered="113" branch-rate="0.6011" complexity="0">
+<coverage version="7.2.7" timestamp="1690925691050" lines-valid="478" lines-covered="278" line-rate="0.5816" branches-valid="162" branches-covered="95" branch-rate="0.5864" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
-    <source>/Users/runner/work/hatch-ci/hatch-ci</source>
+    <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.5816" branch-rate="0.6011" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.5816" branch-rate="0.5864" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
@@ -26,15 +26,15 @@
             <line number="7" hits="0"/>
             <line number="9" hits="0"/>
             <line number="12" hits="0"/>
             <line number="13" hits="0"/>
             <line number="14" hits="0"/>
             <line number="17" hits="0"/>
             <line number="18" hits="0"/>
-            <line number="19" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="18,25"/>
+            <line number="19" hits="0"/>
             <line number="20" hits="0"/>
             <line number="21" hits="0"/>
             <line number="22" hits="0"/>
             <line number="23" hits="0"/>
             <line number="25" hits="0"/>
             <line number="32" hits="0"/>
             <line number="33" hits="0"/>
@@ -59,17 +59,17 @@
             <line number="65" hits="0"/>
             <line number="68" hits="0"/>
             <line number="75" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="78,79"/>
             <line number="78" hits="0"/>
             <line number="79" hits="0"/>
             <line number="82" hits="0"/>
             <line number="88" hits="0"/>
-            <line number="89" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="88,136"/>
+            <line number="89" hits="0"/>
             <line number="90" hits="0"/>
-            <line number="91" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="90,134"/>
+            <line number="91" hits="0"/>
             <line number="92" hits="0"/>
             <line number="94" hits="0"/>
             <line number="98" hits="0"/>
             <line number="100" hits="0"/>
             <line number="101" hits="0"/>
             <line number="106" hits="0"/>
             <line number="107" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="108,110"/>
@@ -94,25 +94,25 @@
         </class>
         <class name="common.py" filename="src/hatch_ci/common.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
           </lines>
         </class>
-        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="0">
+        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
             <line number="6" hits="0"/>
-            <line number="7" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,6"/>
+            <line number="7" hits="0"/>
             <line number="8" hits="0"/>
           </lines>
         </class>
-        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8063" branch-rate="0.7581">
+        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8063" branch-rate="0.7115">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -148,15 +148,15 @@
             <line number="61" hits="1"/>
             <line number="62" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="63" hits="1"/>
             <line number="64" hits="1"/>
             <line number="66" hits="1"/>
             <line number="67" hits="1"/>
             <line number="69" hits="1"/>
-            <line number="70" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="70" hits="1"/>
             <line number="71" hits="0"/>
             <line number="74" hits="1"/>
             <line number="75" hits="1"/>
             <line number="76" hits="1"/>
             <line number="77" hits="1"/>
             <line number="78" hits="1"/>
             <line number="80" hits="1"/>
@@ -178,30 +178,30 @@
             <line number="106" hits="1"/>
             <line number="107" hits="1"/>
             <line number="109" hits="1"/>
             <line number="110" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="111" hits="1"/>
             <line number="114" hits="1"/>
             <line number="115" hits="1"/>
-            <line number="116" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="116" hits="1"/>
             <line number="117" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,119"/>
             <line number="118" hits="0"/>
             <line number="119" hits="0"/>
             <line number="121" hits="0"/>
             <line number="122" hits="0"/>
             <line number="124" hits="0"/>
             <line number="125" hits="0"/>
             <line number="127" hits="0"/>
             <line number="128" hits="0"/>
             <line number="136" hits="0"/>
             <line number="138" hits="1"/>
             <line number="139" hits="1"/>
             <line number="140" hits="1"/>
             <line number="142" hits="1"/>
-            <line number="143" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="143" hits="1"/>
             <line number="144" hits="1"/>
             <line number="145" hits="1"/>
             <line number="146" hits="1"/>
             <line number="147" hits="0"/>
             <line number="148" hits="0"/>
             <line number="149" hits="1"/>
             <line number="151" hits="1"/>
@@ -231,27 +231,27 @@
             <line number="195" hits="1"/>
             <line number="196" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="197"/>
             <line number="197" hits="0"/>
             <line number="198" hits="1"/>
             <line number="199" hits="1"/>
             <line number="200" hits="1"/>
             <line number="202" hits="1"/>
-            <line number="203" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="203" hits="1"/>
             <line number="204" hits="1"/>
             <line number="205" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="206" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="207" hits="1"/>
             <line number="208" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="209" hits="1"/>
             <line number="210" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="213"/>
             <line number="211" hits="1"/>
             <line number="213" hits="0"/>
             <line number="214" hits="1"/>
             <line number="216" hits="1"/>
-            <line number="217" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="217" hits="1"/>
             <line number="218" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
             <line number="224" hits="1"/>
             <line number="230" hits="1"/>
             <line number="232" hits="1"/>
             <line number="233" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="234"/>
             <line number="234" hits="0"/>
             <line number="235" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="236"/>
@@ -339,15 +339,15 @@
             <line number="138" hits="0"/>
             <line number="141" hits="0"/>
             <line number="145" hits="0"/>
             <line number="162" hits="0"/>
             <line number="163" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9423" branch-rate="0.8462">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9423" branch-rate="0.8286">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="3" hits="1"/>
             <line number="4" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
@@ -359,28 +359,28 @@
             <line number="17" hits="1"/>
             <line number="20" hits="1"/>
             <line number="21" hits="1"/>
             <line number="24" hits="1"/>
             <line number="25" hits="1"/>
             <line number="28" hits="1"/>
             <line number="29" hits="1"/>
-            <line number="30" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="30" hits="1"/>
             <line number="31" hits="1"/>
             <line number="32" hits="1"/>
             <line number="33" hits="1"/>
             <line number="34" hits="1"/>
             <line number="36" hits="1"/>
             <line number="39" hits="1"/>
             <line number="40" hits="1"/>
             <line number="41" hits="1"/>
             <line number="43" hits="1"/>
-            <line number="44" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="44" hits="1"/>
             <line number="45" hits="1"/>
             <line number="47" hits="1"/>
-            <line number="48" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="48" hits="1"/>
             <line number="49" hits="1"/>
             <line number="51" hits="1"/>
             <line number="52" hits="1"/>
             <line number="53" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="54" hits="1"/>
             <line number="55" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="56" hits="1"/>
@@ -456,15 +456,15 @@
             <line number="185" hits="1"/>
             <line number="186" hits="1"/>
             <line number="187" hits="1"/>
             <line number="188" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="189" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="190" hits="1"/>
             <line number="191" hits="1"/>
-            <line number="193" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="193" hits="1"/>
             <line number="194" hits="1"/>
             <line number="195" hits="1"/>
             <line number="198" hits="1"/>
             <line number="213" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="214" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="215" hits="1"/>
             <line number="216" hits="1"/>
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/coverage_html.js` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 2 statements   2 run 0 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1__version__ = "0.0.3" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -223,13 +223,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 72 statements   0 run 72 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1from __future__ import annotations 
 2 
 3import argparse 
 4import functools 
 5import logging 
@@ -151,8 +151,8 @@
 132 raise 
 133 
 134 return _fn1 
 135 
 136 return _fn 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   0 run 1 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   0 run 5 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/scm.py: 79%</title>
+    <title>Coverage for src/hatch_ci/scm.py: 78%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/scm.py</b>:
-            <span class="pc_cov">79%</span>
+            <span class="pc_cov">78%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -350,13 +350,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/scm.py: 79% ******
+****** Coverage for src/hatch_ci/scm.py: 78% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 160 statements   129 run 31 missing 0 excluded 7 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -284,8 +284,8 @@
 260 if str(cur) == cur.root: 260&#x202F;&#x219B;&#x202F;261line 260 didn't jump
 to line 261, because the condition on line 260 was never true
 261 break 
 262 cur = cur.parent 
 263 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -254,13 +254,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 65 statements   0 run 65 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -184,8 +184,8 @@
 163 raise RuntimeError(f"unsupported mode {options.mode=}") 
 164 
 165 
 166if __name__ == "__main__": 
 167 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -368,13 +368,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 156 statements   147 run 9 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1from __future__ import annotations 
 2 
 3import ast 
 4import json 
 5import re 
@@ -305,8 +305,8 @@
 277 short = gdata["sha"] + ("*" if dirty else "") 
 278 
 279 set_module_var(path, "__version__", version) 
 280 set_module_var(path, "__hash__", short) 
 281 return version 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -166,13 +166,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 17 statements   0 run 17 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
 
 
 1from hatchling.version.source.plugin.interface import VersionSourceInterface 
 2 
 3from .common import PLUGIN_NAME 
 4 
 5 
@@ -92,8 +92,8 @@
 76 f"no 'version-file' key for plugin {self.PLUGIN_NAME}" 
 77 ) 
 78 version = tools.update_version(initfile, getenv("GITHUB_DUMP"),
 abort=False) 
 79 return {"version": version} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 20:04 +0000
+at 2023-08-01 21:34 +0000
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/favicon_32.png` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/index.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">59%</span>
+            <span class="pc_cov">58%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -75,17 +75,17 @@
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_cli_py.html">src/hatch_ci/cli.py</a></td>
                 <td>72</td>
                 <td>72</td>
                 <td>0</td>
-                <td>24</td>
+                <td>18</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 96">0%</td>
+                <td class="right" data-ratio="0 90">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_common_py.html">src/hatch_ci/common.py</a></td>
                 <td>1</td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
@@ -93,26 +93,26 @@
                 <td class="right" data-ratio="0 1">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_hooks_py.html">src/hatch_ci/hooks.py</a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
-                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 7">0%</td>
+                <td>0</td>
+                <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_scm_py.html">src/hatch_ci/scm.py</a></td>
                 <td>160</td>
                 <td>31</td>
                 <td>0</td>
-                <td>62</td>
+                <td>52</td>
                 <td>7</td>
-                <td class="right" data-ratio="176 222">79%</td>
+                <td class="right" data-ratio="166 212">78%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_script_py.html">src/hatch_ci/script.py</a></td>
                 <td>65</td>
                 <td>65</td>
                 <td>2</td>
                 <td>20</td>
@@ -120,17 +120,17 @@
                 <td class="right" data-ratio="0 85">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
                 <td>156</td>
                 <td>9</td>
                 <td>0</td>
-                <td>78</td>
+                <td>70</td>
                 <td>8</td>
-                <td class="right" data-ratio="213 234">91%</td>
+                <td class="right" data-ratio="205 226">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>17</td>
                 <td>17</td>
                 <td>0</td>
                 <td>2</td>
@@ -140,29 +140,29 @@
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>478</td>
                 <td>200</td>
                 <td>2</td>
-                <td>188</td>
+                <td>162</td>
                 <td>15</td>
-                <td class="right" data-ratio="391 666">59%</td>
+                <td class="right" data-ratio="373 640">58%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 20:04 +0000
+            created at 2023-08-01 21:34 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html"/>
         <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 
-****** Coverage report: 59% ******
+****** Coverage report: 58% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-01 20:04 +0000
+coverage.py_v7.2.7, created at 2023-08-01 21:34 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
-src/hatch_ci/cli.py      72         72      0        24       0       0%
+src/hatch_ci/cli.py      72         72      0        18       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
-src/hatch_ci/hooks.py    5          5       0        2        0       0%
-src/hatch_ci/scm.py      160        31      0        62       7       79%
+src/hatch_ci/hooks.py    5          5       0        0        0       0%
+src/hatch_ci/scm.py      160        31      0        52       7       78%
 src/hatch_ci/script.py   65         65      2        20       0       0%
-src/hatch_ci/tools.py    156        9       0        78       8       91%
+src/hatch_ci/tools.py    156        9       0        70       8       91%
 src/hatch_ci/            17         17      0        2        0       0%
 version_hook.py
-Total                    478        200     2        188      15      59%
+Total                    478        200     2        162      15      58%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-01 20:04 +0000
+coverage.py_v7.2.7, created at 2023-08-01 21:34 +0000
  ____
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/keybd_open.png` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/status.json` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/status.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8706886574074074%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_cli_py': {'index': {'nums': {insert: [(5, 18), (7, 18)], delete: "*

 * *            "[7, 5]}}}, 'd_7005a4ce5d73f943_hooks_py': {'index': {'nums': {insert: [(6, 0), (7, "*

 * *            "0)], delete: [7, 5]}}}, 'd_7005a4ce5d73f943_scm_py': {'hash': "*

 * *            "'41bce2f71040e14bf267c82fc061941f', 'index': {'nums': {insert: [(5, 52)], delete: "*

 * *            "[5]}}}, 'd_7005a4ce5d73f943_tools_py': {'hash': 'a8d6f2dd9ac0362526ec26b96e255458', "*

 * *            "'index': {'nums': {insert:  […]*

```diff
@@ -23,17 +23,17 @@
                 "html_filename": "d_7005a4ce5d73f943_cli_py.html",
                 "nums": [
                     0,
                     1,
                     72,
                     0,
                     72,
-                    24,
+                    18,
                     0,
-                    24
+                    18
                 ],
                 "relative_filename": "src/hatch_ci/cli.py"
             }
         },
         "d_7005a4ce5d73f943_common_py": {
             "hash": "3f1c2e747e86fae3744447395f472601",
             "index": {
@@ -57,32 +57,32 @@
                 "html_filename": "d_7005a4ce5d73f943_hooks_py.html",
                 "nums": [
                     0,
                     1,
                     5,
                     0,
                     5,
-                    2,
                     0,
-                    2
+                    0,
+                    0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "009a288b8e6acd516f800540a2c57e1b",
+            "hash": "41bce2f71040e14bf267c82fc061941f",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     160,
                     0,
                     31,
-                    62,
+                    52,
                     7,
                     15
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_script_py": {
@@ -99,24 +99,24 @@
                     0,
                     20
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "d26b99f9fdb0ce4b436056b8755ef082",
+            "hash": "a8d6f2dd9ac0362526ec26b96e255458",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
                     156,
                     0,
                     9,
-                    78,
+                    70,
                     8,
                     12
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
@@ -134,10 +134,10 @@
                     2
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "1eecc3ffb76f2d9076e9ef4762de9385",
+    "globals": "78efd540b1740235466229ddcdf3f22d",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/coverage/style.css` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/junit/junit.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.html`

 * *Files 2% similar despite different names*

```diff
@@ -435,17 +435,17 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 01-Aug-2023 at 20:04:56 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 01-Aug-2023 at 21:34:51 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>13 tests ran in 2.47 seconds. </p>
+    <p>13 tests ran in 0.95 seconds. </p>
     <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">13 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
@@ -453,38 +453,38 @@
           <th class="sortable links" col="links">Links</th></tr>
         <tr hidden="true" id="not-found-message">
           <th colspan="4">No results found. Try to check the filters</th></tr></thead>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_lookup</td>
-          <td class="col-duration">0.11</td>
+          <td class="col-duration">0.03</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.97</td>
+          <td class="col-duration">0.25</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
-Cloning into &#x27;/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/EHS071&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/KS15M4&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
-From /private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
+From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_abort_exception</td>
@@ -529,15 +529,15 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_set_module_var</td>
-          <td class="col-duration">0.01</td>
+          <td class="col-duration">0.00</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
@@ -556,36 +556,36 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_master</td>
-          <td class="col-duration">0.18</td>
+          <td class="col-duration">0.05</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_beta</td>
-          <td class="col-duration">0.40</td>
+          <td class="col-duration">0.10</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.4&#x27;
 Updated 1 path from the index
 Updated 1 path from the index
 Switched to a new branch &#x27;beta/0.0.2&#x27;
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_release</td>
-          <td class="col-duration">0.29</td>
+          <td class="col-duration">0.06</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,56 +1,54 @@
 ****** junit.html ******
-Report generated on 01-Aug-2023 at 20:04:56 by pytest-html v3.2.0
+Report generated on 01-Aug-2023 at 21:34:51 by pytest-html v3.2.0
 ***** Summary *****
-13 tests ran in 2.47 seconds.
+13 tests ran in 0.95 seconds.
 (Un)check the boxes to filter the results.
 *13 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
-Passed tests/test_scm.py::test_lookup                        0.11
+Passed tests/test_scm.py::test_lookup                        0.03
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.97
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.25
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
-&#x27;/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-of-
-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-
-repo1&#x27;... done. Switched to a new branch &#x27;beta/0.0.2&#x27; Cloning
-into &#x27;/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-
-of-runner/pytest-0/test_handle_remote_and_local_r0/EHS071&#x27;... done.
-Switched to a new branch &#x27;beta/0.0.1&#x27; fatal: a branch named
-&#x27;master&#x27; already exists From /private/var/folders/24/
-8k48jl6d249_n_qfxwsl6xvm0000gn/T/pytest-of-runner/pytest-0/
+&#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
+test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
+0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
+test_handle_remote_and_local_r0/KS15M4&#x27;... done. Switched to a new
+branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
+already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
 No log output captured.
 Passed tests/test_tools.py::test_indent                      0.00
 No log output captured.
 Passed tests/test_tools.py::test_list_of_paths               0.00
 No log output captured.
 Passed tests/test_tools.py::test_get_module_var              0.00
 No log output captured.
-Passed tests/test_tools.py::test_set_module_var              0.01
+Passed tests/test_tools.py::test_set_module_var              0.00
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
-Passed tests/test_tools.py::test_update_version_master       0.18
+Passed tests/test_tools.py::test_update_version_master       0.05
 No log output captured.
-Passed tests/test_tools.py::test_update_version_beta         0.40
+Passed tests/test_tools.py::test_update_version_beta         0.10
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.29
+Passed tests/test_tools.py::test_update_version_release      0.06
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/junit/junit.xml` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml`

 * *Files 10% similar despite different names*

#### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/junit/junit.xml` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="13" time="2.463" timestamp="2023-08-01T20:04:53.667825" hostname="Mac-1690920197002.local">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.117"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.980"/>
-    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_urmtree" time="0.003"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="13" time="0.939" timestamp="2023-08-01T21:34:50.187960" hostname="fv-az306-295">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.032"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.259"/>
+    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.002"/>
+    <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.004"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.011"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.005"/>
+    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.186"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.402"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.299"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.051"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.108"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.066"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/index.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <thead><tr class="summary">
 <th class="summary">File</th>
 <th class="summary">Imprecision</th>
 <th class="summary">Lines</th>
 </tr></thead>
 <tfoot><tr class="summary summary-quality-1">
 <th class="summary summary-filename">Total</th>
-<th class="summary summary-precision">18.14% imprecise</th>
+<th class="summary summary-precision">18.04% imprecise</th>
 <th class="summary summary-lines">937 LOC</th>
 </tr></tfoot>
 <tbody>
 <tr class="summary summary-quality-0">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/__init__.py.html">hatch_ci</a></td>
 <td class="summary summary-precision">0.00% imprecise</td>
 <td class="summary summary-lines">2 LOC</td>
@@ -46,15 +46,15 @@
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/script.py.html">hatch_ci.script</a></td>
 <td class="summary summary-precision">26.35% imprecise</td>
 <td class="summary summary-lines">167 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/tools.py.html">hatch_ci.tools</a></td>
-<td class="summary summary-precision">22.06% imprecise</td>
+<td class="summary summary-precision">21.71% imprecise</td>
 <td class="summary summary-lines">281 LOC</td>
 </tr>
 <tr class="summary summary-quality-1">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/version_hook.py.html">hatch_ci.version_hook</a></td>
 <td class="summary summary-precision">12.66% imprecise</td>
 <td class="summary summary-lines">79 LOC</td>
 </tr>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
 ****** Mypy Type Check Coverage Summary ******
               Summary from index
 File                  Imprecision      Lines
-Total                 18.14% imprecise 937 LOC
+Total                 18.04% imprecise 937 LOC
 hatch_ci              0.00% imprecise  2 LOC
 hatch_ci.cli          19.85% imprecise 136 LOC
 hatch_ci.common       0.00% imprecise  1 LOC
 hatch_ci.hooks        37.50% imprecise 8 LOC
 hatch_ci.scm          9.13% imprecise  263 LOC
 hatch_ci.script       26.35% imprecise 167 LOC
-hatch_ci.tools        22.06% imprecise 281 LOC
+hatch_ci.tools        21.71% imprecise 281 LOC
 hatch_ci.version_hook 12.66% imprecise 79 LOC
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/mypy-html.css` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/cli.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/script.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -440,18 +440,17 @@
 <span class="line-any" title="No Anys on this line!">                        continue</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x6)">                    if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">                        raise ValidationError(</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x8)">                            f"cannot extract non Constant variable "</span>
-<span class="line-any" title="Any Types on this line: 
-Unannotated (x2)
-Explicit (x2)">                            f"{target.id} ({type(subnode.value)})"</span>
+Unannotated (x10)
+Explicit (x2)">                            f"cannot extract non Constant variable "</span>
+<span class="line-empty" title="No Anys on this line!">                            f"{target.id} ({type(subnode.value)})"</span>
 <span class="line-empty" title="No Anys on this line!">                        )</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x2)">                    if isinstance(subnode.value, ast.Str):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">                        value = subnode.value.s</span>
 <span class="line-any" title="Any Types on this line: 
@@ -625,18 +624,17 @@
 <span class="line-precise" title="No Anys on this line!">        if not match1:</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(f"cannot parse current version '{current}'")</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x7)">        if match1.group("version") != match.group("version"):</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
-Explicit (x2)">                f"building package for {current} from '{gdata['ref']}' "</span>
-<span class="line-precise" title="Any Types on this line: 
-Explicit (x2)
-Omitted Generics (x4)">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
+Explicit (x4)
+Omitted Generics (x4)">                f"building package for {current} from '{gdata['ref']}' "</span>
+<span class="line-empty" title="No Anys on this line!">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
 <span class="line-empty" title="No Anys on this line!">            )</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x4)">        if match.group("what") == "beta":</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)
 Unannotated (x2)">            version = f"{match1.group('version')}b{gdata['run_number']}"</span>
 <span class="line-empty" title="No Anys on this line!"></span>
```

### Comparing `hatch_ci-0.0.3b12/build/qa-3.11-macos-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/src/hatch_ci/cli.py` & `hatch_ci-0.0.3b13/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/src/hatch_ci/scm.py` & `hatch_ci-0.0.3b13/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/src/hatch_ci/script.py` & `hatch_ci-0.0.3b13/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/src/hatch_ci/tools.py` & `hatch_ci-0.0.3b13/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.3b13/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/tests/conftest.py` & `hatch_ci-0.0.3b13/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/tests/test_scm.py` & `hatch_ci-0.0.3b13/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/tests/test_tools.py` & `hatch_ci-0.0.3b13/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/LICENSE.txt` & `hatch_ci-0.0.3b13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/README.md` & `hatch_ci-0.0.3b13/README.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/pyproject.toml` & `hatch_ci-0.0.3b13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b12/PKG-INFO` & `hatch_ci-0.0.3b13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.3b12
+Version: 0.0.3b13
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
```

