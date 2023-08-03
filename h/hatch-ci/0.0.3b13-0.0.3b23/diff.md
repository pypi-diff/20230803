# Comparing `tmp/hatch_ci-0.0.3b13.tar.gz` & `tmp/hatch_ci-0.0.3b23.tar.gz`

## Comparing `hatch_ci-0.0.3b13.tar` & `hatch_ci-0.0.3b23.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.gitattributes
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/Makefile
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/beta.yml
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/master.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.github/workflows/tags.yml
--rw-r--r--   0        0        0    23580 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    84025 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    48062 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0    84467 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    44948 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0    48994 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/script.py
--rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/test_scm.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/LICENSE.txt
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/README.md
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/pyproject.toml
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b13/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.gitattributes
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/Makefile
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.github/workflows/tags.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/.keepme
+-rw-r--r--   0        0        0    25505 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   113919 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    20531 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    67137 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/tests/test_scm.py
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/LICENSE.txt
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/README.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/pyproject.toml
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 hatch_ci-0.0.3b23/PKG-INFO
```

### Comparing `hatch_ci-0.0.3b13/.pre-commit-config.yaml` & `hatch_ci-0.0.3b23/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/.github/workflows/beta.yml` & `hatch_ci-0.0.3b23/.github/workflows/master.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,111 @@
-name: Beta build
+name: Master build
 
 on:
   push:
     branches:
-      - 'beta/**'
+      - master
+env:
+  PACKAGE: hatch_ci
+  XTARGET: '3.11'
 
 jobs:
   build:
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.8", "3.9", "3.10", "3.11",]
     runs-on: ${{ matrix.os }}
 
     steps:
-      - uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v3
 
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
 
-      - name: Install dependencies
+      - name: Install dependencies from tests/requirements.txt
         shell: bash
         run: |
             python -m pip install --upgrade pip
             pip install setuptools build wheel twine
             pip install -r tests/requirements.txt
 
-      - name: Lint tests (ruff)
+      - name: Lint checks (ruff)
         shell: bash
         env:
           PYTHONPATH: src
         run: |
-          ruff check src
+           ruff check .
 
-      - name: Static tests (mypy)
+      - name: Static checks (mypy)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
           mypy src \
             --no-incremental --xslt-html-report $OUTDIR/mypy
 
-      - name: Runtime tests (unitest, coverage etc.)
+      - name: Runtime checks (pytest, coverage etc.)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
           py.test \
-              --cov=hatch_ci \
+              --cov=${{ env.PACKAGE }} \
               --cov-report=html:$OUTDIR/coverage --cov-report=xml:$OUTDIR/coverage.xml \
               --junitxml=$OUTDIR/junit/junit.xml --html=$OUTDIR/junit/junit.html --self-contained-html \
             tests
+          touch build/.keepme
 
-      - name: Upload pytest test results
-        uses: actions/upload-artifact@v2
+      - name: Build wheel packages
+        if: ${{ ! contains(matrix.os, 'windows') }}
+        env:
+          GITHUB_DUMP: ${{ toJson(github) }}
+        run: |
+          python -m build
+          mv dist build
+
+      - name: Artifacts uploads
+        uses: actions/upload-artifact@v3
         with:
-          name: pytest-results-${{ matrix.python-version }}-${{ matrix.os }}
-          path: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
+          name: qa-results-${{ matrix.python-version }}-${{ matrix.os }}
+          path: |
+            build/qa-${{ matrix.python-version }}-${{ matrix.os}}
+            build/dist
+            build/.keepme
         # Use always() to always run this step to publish test results when there are test failures
         if: always()
 
+  publish:
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        python-version: ["3.8", "3.9", "3.10", "3.11",]
+    runs-on: ${{ matrix.os }}
+    needs: build
+    steps:
+      - name: Artifacts download
+        uses: actions/download-artifact@v3
+        with:
+          name: qa-results-${{ matrix.python-version }}-${{ matrix.os }}
+
       - name: "Upload coverage to Codecov"
         uses: codecov/codecov-action@v3
+        if: ${{ matrix.python-version == env.XTARGET }}
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           fail_ci_if_error: true
-          files: build/qa-${{ matrix.python-version }}-${{ matrix.os}}/coverage.xml
+          files: qa-${{ matrix.python-version }}-${{ matrix.os }}/coverage.xml
           verbose: true
-
-      - name: Build wheel package
-        env:
-          PYTHONPATH: src
-          GITHUB_DUMP: ${{ toJson(github) }}
-        run: |
-          # this is special for hatch-ci plugin
-          python -m pip install --edit .
-          python -m build -n
-
-      - name: Publish packages to pypi (beta)
-        shell: bash
-        env:
-          TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-          TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
-        run: |
-          twine upload --skip-existing --non-interactive --repository pypi dist/*
-
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage.xml`

 * *Files 4% similar despite different names*

#### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1690925691050" lines-valid="478" lines-covered="278" line-rate="0.5816" branches-valid="162" branches-covered="95" branch-rate="0.5864" complexity="0">
+<coverage version="7.2.7" timestamp="1691092148037" lines-valid="524" lines-covered="324" line-rate="0.6183" branches-valid="174" branches-covered="109" branch-rate="0.6264" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.5816" branch-rate="0.5864" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.6183" branch-rate="0.6264" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
@@ -104,15 +104,15 @@
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
             <line number="6" hits="0"/>
             <line number="7" hits="0"/>
             <line number="8" hits="0"/>
           </lines>
         </class>
-        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8063" branch-rate="0.7115">
+        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8333" branch-rate="0.7692">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -208,73 +208,75 @@
             <line number="158" hits="1"/>
             <line number="165" hits="1"/>
             <line number="166" hits="1"/>
             <line number="167" hits="1"/>
             <line number="168" hits="0"/>
             <line number="169" hits="0"/>
             <line number="170" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="171" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="173"/>
+            <line number="171" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="172" hits="1"/>
-            <line number="173" hits="0"/>
-            <line number="174" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="175,176"/>
+            <line number="173" hits="1"/>
+            <line number="174" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="175"/>
             <line number="175" hits="0"/>
-            <line number="176" hits="0"/>
-            <line number="177" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="170,178"/>
+            <line number="176" hits="1"/>
+            <line number="177" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="178"/>
             <line number="178" hits="0"/>
             <line number="181" hits="1"/>
             <line number="183" hits="1"/>
-            <line number="188" hits="1"/>
-            <line number="189" hits="1"/>
-            <line number="190" hits="1"/>
+            <line number="184" hits="1"/>
+            <line number="186" hits="1"/>
+            <line number="191" hits="1"/>
             <line number="192" hits="1"/>
-            <line number="193" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="194" hits="1"/>
+            <line number="193" hits="1"/>
             <line number="195" hits="1"/>
-            <line number="196" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="197"/>
-            <line number="197" hits="0"/>
+            <line number="196" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="197" hits="1"/>
             <line number="198" hits="1"/>
-            <line number="199" hits="1"/>
-            <line number="200" hits="1"/>
+            <line number="199" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="200"/>
+            <line number="200" hits="0"/>
+            <line number="201" hits="1"/>
             <line number="202" hits="1"/>
             <line number="203" hits="1"/>
-            <line number="204" hits="1"/>
-            <line number="205" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="206" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="205" hits="1"/>
+            <line number="206" hits="1"/>
             <line number="207" hits="1"/>
             <line number="208" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="209" hits="1"/>
-            <line number="210" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="213"/>
-            <line number="211" hits="1"/>
-            <line number="213" hits="0"/>
+            <line number="209" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="210" hits="1"/>
+            <line number="211" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="212" hits="1"/>
+            <line number="213" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="216"/>
             <line number="214" hits="1"/>
-            <line number="216" hits="1"/>
+            <line number="216" hits="0"/>
             <line number="217" hits="1"/>
-            <line number="218" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
-            <line number="224" hits="1"/>
-            <line number="230" hits="1"/>
-            <line number="232" hits="1"/>
-            <line number="233" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="234"/>
-            <line number="234" hits="0"/>
-            <line number="235" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="236"/>
-            <line number="236" hits="0"/>
-            <line number="238" hits="1"/>
-            <line number="247" hits="1"/>
-            <line number="248" hits="1"/>
-            <line number="249" hits="1"/>
+            <line number="219" hits="1"/>
+            <line number="220" hits="1"/>
+            <line number="221" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
+            <line number="227" hits="1"/>
+            <line number="233" hits="1"/>
+            <line number="235" hits="1"/>
+            <line number="236" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="237"/>
+            <line number="237" hits="0"/>
+            <line number="238" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="239"/>
+            <line number="239" hits="0"/>
+            <line number="241" hits="1"/>
+            <line number="250" hits="1"/>
             <line number="251" hits="1"/>
+            <line number="252" hits="1"/>
             <line number="254" hits="1"/>
-            <line number="255" hits="1"/>
-            <line number="256" hits="1"/>
-            <line number="257" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="263"/>
-            <line number="258" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="257" hits="1"/>
+            <line number="258" hits="1"/>
             <line number="259" hits="1"/>
-            <line number="260" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="261"/>
-            <line number="261" hits="0"/>
+            <line number="260" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="266"/>
+            <line number="261" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="262" hits="1"/>
-            <line number="263" hits="0"/>
+            <line number="263" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="264"/>
+            <line number="264" hits="0"/>
+            <line number="265" hits="1"/>
+            <line number="266" hits="0"/>
           </lines>
         </class>
         <class name="script.py" filename="src/hatch_ci/script.py" complexity="0" line-rate="0" branch-rate="0">
           <methods/>
           <lines>
             <line number="12" hits="0"/>
             <line number="14" hits="0"/>
@@ -321,191 +323,235 @@
             <line number="96" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="97,98"/>
             <line number="97" hits="0"/>
             <line number="98" hits="0"/>
             <line number="99" hits="0"/>
             <line number="100" hits="0"/>
             <line number="101" hits="0"/>
             <line number="102" hits="0"/>
-            <line number="116" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,162"/>
+            <line number="116" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,166"/>
             <line number="118" hits="0"/>
             <line number="119" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="120,126"/>
             <line number="120" hits="0"/>
             <line number="125" hits="0"/>
             <line number="126" hits="0"/>
             <line number="127" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="128,131"/>
             <line number="128" hits="0"/>
             <line number="131" hits="0"/>
             <line number="134" hits="0"/>
             <line number="137" hits="0"/>
             <line number="138" hits="0"/>
             <line number="141" hits="0"/>
+            <line number="142" hits="0"/>
             <line number="145" hits="0"/>
-            <line number="162" hits="0"/>
-            <line number="163" hits="0"/>
+            <line number="149" hits="0"/>
+            <line number="166" hits="0"/>
+            <line number="167" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9423" branch-rate="0.8286">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9444" branch-rate="0.8415">
           <methods/>
           <lines>
-            <line number="1" hits="1"/>
             <line number="3" hits="1"/>
-            <line number="4" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
+            <line number="8" hits="1"/>
             <line number="9" hits="1"/>
-            <line number="12" hits="1"/>
-            <line number="13" hits="1"/>
-            <line number="16" hits="1"/>
-            <line number="17" hits="1"/>
-            <line number="20" hits="1"/>
-            <line number="21" hits="1"/>
-            <line number="24" hits="1"/>
-            <line number="25" hits="1"/>
-            <line number="28" hits="1"/>
-            <line number="29" hits="1"/>
+            <line number="11" hits="1"/>
+            <line number="14" hits="1"/>
+            <line number="15" hits="1"/>
+            <line number="18" hits="1"/>
+            <line number="19" hits="1"/>
+            <line number="22" hits="1"/>
+            <line number="23" hits="1"/>
+            <line number="26" hits="1"/>
+            <line number="27" hits="1"/>
             <line number="30" hits="1"/>
             <line number="31" hits="1"/>
             <line number="32" hits="1"/>
             <line number="33" hits="1"/>
             <line number="34" hits="1"/>
+            <line number="35" hits="1"/>
             <line number="36" hits="1"/>
-            <line number="39" hits="1"/>
-            <line number="40" hits="1"/>
+            <line number="38" hits="1"/>
             <line number="41" hits="1"/>
+            <line number="42" hits="1"/>
             <line number="43" hits="1"/>
-            <line number="44" hits="1"/>
             <line number="45" hits="1"/>
+            <line number="46" hits="1"/>
             <line number="47" hits="1"/>
-            <line number="48" hits="1"/>
             <line number="49" hits="1"/>
+            <line number="50" hits="1"/>
             <line number="51" hits="1"/>
-            <line number="52" hits="1"/>
-            <line number="53" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="53" hits="1"/>
             <line number="54" hits="1"/>
             <line number="55" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="56" hits="1"/>
-            <line number="57" hits="1"/>
-            <line number="60" hits="1"/>
+            <line number="57" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="58" hits="1"/>
+            <line number="59" hits="1"/>
             <line number="62" hits="1"/>
-            <line number="63" hits="1"/>
             <line number="64" hits="1"/>
-            <line number="66" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="67"/>
-            <line number="67" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="68,69"/>
-            <line number="68" hits="0"/>
-            <line number="69" hits="1"/>
-            <line number="70" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="71"/>
-            <line number="71" hits="0"/>
-            <line number="74" hits="1"/>
-            <line number="77" hits="1"/>
+            <line number="65" hits="1"/>
+            <line number="66" hits="1"/>
+            <line number="68" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="69"/>
+            <line number="69" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="70,71"/>
+            <line number="70" hits="0"/>
+            <line number="71" hits="1"/>
+            <line number="72" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="73"/>
+            <line number="73" hits="0"/>
+            <line number="76" hits="1"/>
             <line number="79" hits="1"/>
-            <line number="80" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="81" hits="1"/>
-            <line number="82" hits="1"/>
+            <line number="82" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="83" hits="1"/>
             <line number="84" hits="1"/>
             <line number="86" hits="1"/>
-            <line number="87" hits="1"/>
-            <line number="90" hits="1"/>
-            <line number="91" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="88" hits="1"/>
+            <line number="89" hits="1"/>
+            <line number="92" hits="1"/>
+            <line number="93" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="94" hits="1"/>
-            <line number="114" hits="1"/>
-            <line number="115" hits="1"/>
-            <line number="116" hits="1"/>
-            <line number="117" hits="1"/>
-            <line number="119" hits="1"/>
-            <line number="121" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="122" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="123"/>
-            <line number="123" hits="0"/>
-            <line number="124" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="125" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="126" hits="1"/>
-            <line number="127" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="128" hits="1"/>
+            <line number="95" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="98" hits="1"/>
+            <line number="99" hits="1"/>
+            <line number="102" hits="1"/>
+            <line number="122" hits="1"/>
+            <line number="123" hits="1"/>
+            <line number="124" hits="1"/>
+            <line number="125" hits="1"/>
+            <line number="127" hits="1"/>
+            <line number="129" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="130" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="131"/>
+            <line number="131" hits="0"/>
             <line number="132" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="133" hits="1"/>
-            <line number="134" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="137"/>
-            <line number="135" hits="1"/>
-            <line number="137" hits="0"/>
-            <line number="138" hits="1"/>
-            <line number="139" hits="1"/>
+            <line number="133" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="134" hits="1"/>
+            <line number="135" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="136" hits="1"/>
+            <line number="140" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="141" hits="1"/>
-            <line number="142" hits="1"/>
-            <line number="143" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="146"/>
-            <line number="144" hits="1"/>
-            <line number="145" hits="1"/>
+            <line number="142" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="145"/>
+            <line number="143" hits="1"/>
+            <line number="145" hits="0"/>
             <line number="146" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="147" hits="1"/>
             <line number="148" hits="1"/>
-            <line number="151" hits="1"/>
-            <line number="166" hits="1"/>
-            <line number="167" hits="1"/>
-            <line number="168" hits="1"/>
-            <line number="170" hits="1"/>
-            <line number="171" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="172" hits="1"/>
-            <line number="173" hits="1"/>
-            <line number="175" hits="1"/>
-            <line number="176" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="177" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="178" hits="1"/>
-            <line number="179" hits="1"/>
-            <line number="180" hits="1"/>
-            <line number="181" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="182" hits="1"/>
-            <line number="183" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="186"/>
+            <line number="149" hits="1"/>
+            <line number="152" hits="1"/>
+            <line number="153" hits="1"/>
+            <line number="155" hits="1"/>
+            <line number="156" hits="1"/>
+            <line number="157" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="158" hits="1"/>
+            <line number="159" hits="1"/>
+            <line number="160" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="161" hits="1"/>
+            <line number="162" hits="1"/>
+            <line number="165" hits="1"/>
+            <line number="181" hits="1"/>
             <line number="184" hits="1"/>
             <line number="185" hits="1"/>
             <line number="186" hits="1"/>
-            <line number="187" hits="1"/>
-            <line number="188" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="188" hits="1"/>
             <line number="189" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="190" hits="1"/>
             <line number="191" hits="1"/>
             <line number="193" hits="1"/>
-            <line number="194" hits="1"/>
-            <line number="195" hits="1"/>
+            <line number="194" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="195" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="196" hits="1"/>
+            <line number="197" hits="1"/>
             <line number="198" hits="1"/>
-            <line number="213" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="214" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="215" hits="1"/>
+            <line number="199" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="200" hits="1"/>
+            <line number="201" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="204"/>
+            <line number="202" hits="1"/>
+            <line number="203" hits="1"/>
+            <line number="204" hits="1"/>
+            <line number="205" hits="1"/>
+            <line number="206" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="207" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="208" hits="1"/>
+            <line number="209" hits="1"/>
+            <line number="211" hits="1"/>
+            <line number="212" hits="1"/>
+            <line number="213" hits="1"/>
             <line number="216" hits="1"/>
-            <line number="217" hits="1"/>
-            <line number="218" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="219" hits="1"/>
-            <line number="220" hits="1"/>
-            <line number="221" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="222" hits="1"/>
-            <line number="223" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="226" hits="1"/>
-            <line number="239" hits="1"/>
+            <line number="231" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="232" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="233" hits="1"/>
+            <line number="234" hits="1"/>
+            <line number="235" hits="1"/>
+            <line number="236" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="237" hits="1"/>
+            <line number="238" hits="1"/>
+            <line number="239" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="240" hits="1"/>
-            <line number="242" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="243"/>
-            <line number="243" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="244,245"/>
-            <line number="244" hits="0"/>
-            <line number="245" hits="0"/>
-            <line number="247" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="248" hits="1"/>
-            <line number="253" hits="1"/>
-            <line number="255" hits="1"/>
+            <line number="241" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="244" hits="1"/>
             <line number="256" hits="1"/>
-            <line number="258" hits="1"/>
-            <line number="260" hits="1"/>
-            <line number="261" hits="1"/>
-            <line number="263" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="266" hits="1"/>
-            <line number="267" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="268"/>
-            <line number="268" hits="0"/>
-            <line number="269" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="270" hits="1"/>
+            <line number="267" hits="1"/>
+            <line number="269" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="270"/>
+            <line number="270" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="271,272"/>
+            <line number="271" hits="0"/>
+            <line number="272" hits="0"/>
             <line number="274" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="275" hits="1"/>
-            <line number="277" hits="1"/>
-            <line number="279" hits="1"/>
-            <line number="280" hits="1"/>
             <line number="281" hits="1"/>
+            <line number="283" hits="1"/>
+            <line number="284" hits="1"/>
+            <line number="286" hits="1"/>
+            <line number="287" hits="1"/>
+            <line number="289" hits="1"/>
+            <line number="290" hits="1"/>
+            <line number="291" hits="1"/>
+            <line number="292" hits="1"/>
+            <line number="293" hits="1"/>
+            <line number="295" hits="1"/>
+            <line number="296" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="299" hits="1"/>
+            <line number="300" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="301"/>
+            <line number="301" hits="0"/>
+            <line number="302" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="303" hits="1"/>
+            <line number="307" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="308" hits="1"/>
+            <line number="309" hits="1"/>
+            <line number="311" hits="1"/>
+            <line number="312" hits="1"/>
+            <line number="315" hits="1"/>
+            <line number="328" hits="1"/>
+            <line number="329" hits="1"/>
+            <line number="330" hits="1"/>
+            <line number="331" hits="1"/>
+            <line number="334" hits="1"/>
+            <line number="360" hits="1"/>
+            <line number="361" hits="1"/>
+            <line number="362" hits="1"/>
+            <line number="364" hits="1"/>
+            <line number="366" hits="1"/>
+            <line number="367" hits="1"/>
+            <line number="368" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="369" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="370"/>
+            <line number="370" hits="0"/>
+            <line number="371" hits="1"/>
+            <line number="373" hits="1"/>
+            <line number="374" hits="1"/>
+            <line number="375" hits="1"/>
+            <line number="377" hits="1"/>
+            <line number="378" hits="1"/>
+            <line number="379" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="380" hits="1"/>
+            <line number="381" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="382"/>
+            <line number="382" hits="0"/>
+            <line number="383" hits="1"/>
+            <line number="384" hits="1"/>
+            <line number="385" hits="1"/>
           </lines>
         </class>
         <class name="version_hook.py" filename="src/hatch_ci/version_hook.py" complexity="0" line-rate="0" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
 1__version__ = "0.0.3" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/scm.py: 78%</title>
+    <title>Coverage for src/hatch_ci/scm.py: 82%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/scm.py</b>:
-            <span class="pc_cov">78%</span>
+            <span class="pc_cov">82%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,27 +51,27 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">160 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">129<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">31<span class="text"> missing</span></button>
+            <span class="text">162 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">135<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">27<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
-            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">7<span class="text"> partial</span></button>
+            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">8<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -248,115 +248,118 @@
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">result</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="nam">txt</span> <span class="op">=</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"status"</span><span class="op">,</span> <span class="str">"--porcelain"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">except</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">CalledProcessError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">"invalid repo"</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">171&#x202F;&#x219B;&#x202F;173</span><span class="annotate long">line 171 didn't jump to line 173, because the condition on line 171 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">tag</span><span class="op">,</span> <span class="nam">filename</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="num">2</span><span class="op">]</span><span class="op">,</span> <span class="nam">line</span><span class="op">[</span><span class="num">3</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="key">if</span> <span class="nam">tag</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">mapper</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">tag</span><span class="op">,</span> <span class="nam">filename</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="num">2</span><span class="op">]</span><span class="op">,</span> <span class="nam">line</span><span class="op">[</span><span class="num">3</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="key">if</span> <span class="nam">tag</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">mapper</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">174&#x202F;&#x219B;&#x202F;175</span><span class="annotate long">line 174 didn't jump to line 175, because the condition on line 174 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">f"cannot map git status for '{tag}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">mapper</span><span class="op">[</span><span class="nam">tag</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">mapper</span><span class="op">[</span><span class="nam">tag</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">177&#x202F;&#x219B;&#x202F;178</span><span class="annotate long">line 177 didn't jump to line 178</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">                <span class="nam">result</span><span class="op">[</span><span class="nam">filename</span><span class="op">]</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">                    <span class="op">(</span><span class="nam">result</span><span class="op">[</span><span class="nam">filename</span><span class="op">]</span> <span class="op">|</span> <span class="nam">value</span><span class="op">)</span> <span class="key">if</span> <span class="nam">filename</span> <span class="key">in</span> <span class="nam">result</span> <span class="key">else</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="key">def</span> <span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="nam">paths</span><span class="op">:</span> <span class="nam">ListOfArgs</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="nam">all_paths</span> <span class="op">=</span> <span class="nam">to_list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"add"</span><span class="op">,</span> <span class="op">*</span><span class="nam">all_paths</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="nam">message</span><span class="op">,</span> <span class="op">*</span><span class="nam">all_paths</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="key">def</span> <span class="nam">branch</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">origin</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"master"</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">name</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">            <span class="nam">name</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span> <span class="key">or</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="key">return</span> <span class="nam">name</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">origin</span> <span class="key">or</span> <span class="nam">origin</span> <span class="key">is</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">196&#x202F;&#x219B;&#x202F;197</span><span class="annotate long">line 196 didn't jump to line 197, because the condition on line 196 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"invalid {origin=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="nam">old</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">branch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="str">"-b"</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">"--track"</span><span class="op">,</span> <span class="nam">origin</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">        <span class="key">return</span> <span class="nam">old</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">old</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">old</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">    <span class="key">def</span> <span class="nam">branches</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepoBranches</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">GitRepoBranches</span><span class="op">(</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">        <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"branch"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">"--format"</span><span class="op">,</span> <span class="str">"%(refname)"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                <span class="nam">result</span><span class="op">.</span><span class="nam">local</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">            <span class="key">elif</span> <span class="nam">line</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/remotes/"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">210&#x202F;&#x219B;&#x202F;213</span><span class="annotate long">line 210 didn't jump to line 213, because the condition on line 210 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                <span class="nam">result</span><span class="op">.</span><span class="nam">remote</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">[</span><span class="num">13</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"invalid branch {line}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="key">def</span> <span class="nam">references</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">return</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">            <span class="str">f"refs/tags/{line.strip()}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-l"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">def</span> <span class="nam">clone</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="nam">dest</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="nam">force</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">branch</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepo</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">from</span> <span class="nam">shutil</span> <span class="key">import</span> <span class="nam">rmtree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">workdir</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">dest</span><span class="op">)</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">if</span> <span class="nam">force</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">233&#x202F;&#x219B;&#x202F;234</span><span class="annotate long">line 233 didn't jump to line 234, because the condition on line 233 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="nam">rmtree</span><span class="op">(</span><span class="nam">workdir</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="key">if</span> <span class="nam">workdir</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">235&#x202F;&#x219B;&#x202F;236</span><span class="annotate long">line 235 didn't jump to line 236, because the condition on line 235 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"target directory present {workdir}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">                <span class="str">"clone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">                <span class="op">*</span><span class="op">(</span><span class="op">[</span><span class="str">"--branch"</span><span class="op">,</span> <span class="nam">branch</span><span class="op">]</span> <span class="key">if</span> <span class="nam">branch</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">workdir</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">workdir</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="nam">repo</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">(</span><span class="nam">workdir</span><span class="op">=</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.name"</span><span class="op">,</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.name"</span><span class="op">]</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">        <span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.email"</span><span class="op">,</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.email"</span><span class="op">]</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">return</span> <span class="nam">repo</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="key">def</span> <span class="nam">dirty</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="key">return</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="nam">untracked_files</span><span class="op">=</span><span class="str">"no"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">def</span> <span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="nam">paths</span><span class="op">:</span> <span class="nam">ListOfArgs</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">all_paths</span> <span class="op">=</span> <span class="nam">to_list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"add"</span><span class="op">,</span> <span class="op">*</span><span class="nam">all_paths</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="nam">message</span><span class="op">,</span> <span class="op">*</span><span class="nam">all_paths</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">def</span> <span class="nam">branch</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">origin</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"master"</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">name</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="nam">name</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span> <span class="key">or</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">            <span class="key">return</span> <span class="nam">name</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">origin</span> <span class="key">or</span> <span class="nam">origin</span> <span class="key">is</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">199&#x202F;&#x219B;&#x202F;200</span><span class="annotate long">line 199 didn't jump to line 200, because the condition on line 199 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"invalid {origin=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="nam">old</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">branch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="str">"-b"</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">"--track"</span><span class="op">,</span> <span class="nam">origin</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="key">return</span> <span class="nam">old</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">old</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">old</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">def</span> <span class="nam">branches</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepoBranches</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">GitRepoBranches</span><span class="op">(</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">        <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"branch"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">"--format"</span><span class="op">,</span> <span class="str">"%(refname)"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">            <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/heads/"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                <span class="nam">result</span><span class="op">.</span><span class="nam">local</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">[</span><span class="num">11</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">            <span class="key">elif</span> <span class="nam">line</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"refs/remotes/"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">213&#x202F;&#x219B;&#x202F;216</span><span class="annotate long">line 213 didn't jump to line 216, because the condition on line 213 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                <span class="nam">result</span><span class="op">.</span><span class="nam">remote</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">[</span><span class="num">13</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"invalid branch {line}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="key">def</span> <span class="nam">references</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="key">return</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">            <span class="str">f"refs/tags/{line.strip()}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-l"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">            <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">def</span> <span class="nam">clone</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="nam">dest</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="nam">force</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="nam">branch</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepo</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">from</span> <span class="nam">shutil</span> <span class="key">import</span> <span class="nam">rmtree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="nam">workdir</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">dest</span><span class="op">)</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="key">if</span> <span class="nam">force</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">236&#x202F;&#x219B;&#x202F;237</span><span class="annotate long">line 236 didn't jump to line 237, because the condition on line 236 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="nam">rmtree</span><span class="op">(</span><span class="nam">workdir</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="key">if</span> <span class="nam">workdir</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">238&#x202F;&#x219B;&#x202F;239</span><span class="annotate long">line 238 didn't jump to line 239, because the condition on line 238 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"target directory present {workdir}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="str">"clone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">                <span class="op">*</span><span class="op">(</span><span class="op">[</span><span class="str">"--branch"</span><span class="op">,</span> <span class="nam">branch</span><span class="op">]</span> <span class="key">if</span> <span class="nam">branch</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">workdir</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                <span class="nam">workdir</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="nam">repo</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">(</span><span class="nam">workdir</span><span class="op">=</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.name"</span><span class="op">,</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.name"</span><span class="op">]</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.email"</span><span class="op">,</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="str">"user.email"</span><span class="op">]</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="key">def</span> <span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span><span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepo</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="nam">found</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">while</span> <span class="key">not</span> <span class="nam">found</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">257&#x202F;&#x219B;&#x202F;263</span><span class="annotate long">line 257 didn't jump to line 263, because the condition on line 257 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">cur</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="key">return</span> <span class="nam">GitRepo</span><span class="op">(</span><span class="nam">cur</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="key">if</span> <span class="nam">str</span><span class="op">(</span><span class="nam">cur</span><span class="op">)</span> <span class="op">==</span> <span class="nam">cur</span><span class="op">.</span><span class="nam">root</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">260&#x202F;&#x219B;&#x202F;261</span><span class="annotate long">line 260 didn't jump to line 261, because the condition on line 260 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">        <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">.</span><span class="nam">parent</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">        <span class="key">return</span> <span class="nam">repo</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="key">def</span> <span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span><span class="op">)</span> <span class="op">-></span> <span class="nam">GitRepo</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="nam">found</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">while</span> <span class="key">not</span> <span class="nam">found</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">260&#x202F;&#x219B;&#x202F;266</span><span class="annotate long">line 260 didn't jump to line 266, because the condition on line 260 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">cur</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">            <span class="key">return</span> <span class="nam">GitRepo</span><span class="op">(</span><span class="nam">cur</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="key">if</span> <span class="nam">str</span><span class="op">(</span><span class="nam">cur</span><span class="op">)</span> <span class="op">==</span> <span class="nam">cur</span><span class="op">.</span><span class="nam">root</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">263&#x202F;&#x219B;&#x202F;264</span><span class="annotate long">line 263 didn't jump to line 264, because the condition on line 263 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">            <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">.</span><span class="nam">parent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/scm.py: 78% ******
+****** Coverage for src/hatch_ci/scm.py: 82% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 160 statements   129 run 31 missing 0 excluded 7 partial *****
+***** 162 statements   135 run 27 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -182,110 +182,113 @@
 164 } 
 165 result: dict[str, int] = {} 
 166 try: 
 167 txt = self(["status", "--porcelain"]) 
 168 except subprocess.CalledProcessError as exc: 
 169 raise GitError("invalid repo") from exc 
 170 for line in txt.split("\n"): 
-171 if not line.strip(): 171&#x202F;&#x219B;&#x202F;173line 171 didn't jump to
-line 173, because the condition on line 171 was never false
+171 if not line.strip(): 
 172 continue 
 173 tag, filename = line[:2], line[3:] 
-174 if tag not in mapper: 
+174 if tag not in mapper: 174&#x202F;&#x219B;&#x202F;175line 174 didn't jump to
+line 175, because the condition on line 174 was never true
 175 raise GitError(f"cannot map git status for '{tag}'") 
 176 value = mapper[tag] 
-177 if value: 
+177 if value: 177&#x202F;&#x219B;&#x202F;178line 177 didn't jump to line 178
 178 result[filename] = ( 
 179 (result[filename] | value) if filename in result else value 
 180 ) 
 181 return result 
 182 
-183 def commit( 
-184 self, 
-185 paths: ListOfArgs, 
-186 message: str, 
-187 ) -> None: 
-188 all_paths = to_list_of_paths(paths) 
-189 self(["add", *all_paths]) 
-190 self(["commit", "-m", message, *all_paths]) 
-191 
-192 def branch(self, name: str | None = None, origin: str = "master") -> str: 
-193 if not name: 
-194 name = self.head.name or "" 
-195 return name[11:] if name.startswith("refs/heads/") else name 
-196 if not (origin or origin is None): 196&#x202F;&#x219B;&#x202F;197line 196
-didn't jump to line 197, because the condition on line 196 was never true
-197 raise RuntimeError(f"invalid {origin=}") 
-198 old = self.branch() 
-199 self(["checkout", "-b", name, "--track", origin]) 
-200 return old[11:] if old.startswith("refs/heads/") else old 
-201 
-202 @property 
-203 def branches(self) -> GitRepoBranches: 
-204 result = GitRepoBranches([], []) 
-205 for line in self(["branch", "-a", "--format", "%(refname)"]).split("\n"): 
-206 if not line.strip(): 
-207 continue 
-208 if line.startswith("refs/heads/"): 
-209 result.local.append(line[11:]) 
-210 elif line.startswith("refs/remotes/"): 210&#x202F;&#x219B;&#x202F;213line
-210 didn't jump to line 213, because the condition on line 210 was never false
-211 result.remote.append(line[13:]) 
-212 else: 
-213 raise RuntimeError(f"invalid branch {line}") 
-214 return result 
-215 
-216 @property 
-217 def references(self) -> list[str]: 
-218 return [ 
-219 f"refs/tags/{line.strip()}" 
-220 for line in self(["tag", "-l"]).split("\n") 
-221 if line.strip() 
-222 ] 
-223 
-224 def clone( 
-225 self, 
-226 dest: str | Path, 
-227 force: bool = False, 
-228 branch: str | None = None, 
-229 ) -> GitRepo: 
-230 from shutil import rmtree 
-231 
-232 workdir = Path(dest).absolute() 
-233 if force: 233&#x202F;&#x219B;&#x202F;234line 233 didn't jump to line 234,
-because the condition on line 233 was never true
-234 rmtree(workdir, ignore_errors=True) 
-235 if workdir.exists(): 235&#x202F;&#x219B;&#x202F;236line 235 didn't jump to
-line 236, because the condition on line 235 was never true
-236 raise ValueError(f"target directory present {workdir}") 
-237 
-238 self( 
-239 [ 
-240 "clone", 
-241 *(["--branch", branch] if branch else []), 
-242 self.workdir.absolute(), 
-243 workdir.absolute(), 
-244 ], 
-245 ) 
-246 
-247 repo = self.__class__(workdir=workdir) 
-248 repo(["config", "user.name", self(["config", "user.name"])]) 
-249 repo(["config", "user.email", self(["config", "user.email"])]) 
-250 
-251 return repo 
-252 
+183 def dirty(self) -> bool: 
+184 return bool(self.status(untracked_files="no")) 
+185 
+186 def commit( 
+187 self, 
+188 paths: ListOfArgs, 
+189 message: str, 
+190 ) -> None: 
+191 all_paths = to_list_of_paths(paths) 
+192 self(["add", *all_paths]) 
+193 self(["commit", "-m", message, *all_paths]) 
+194 
+195 def branch(self, name: str | None = None, origin: str = "master") -> str: 
+196 if not name: 
+197 name = self.head.name or "" 
+198 return name[11:] if name.startswith("refs/heads/") else name 
+199 if not (origin or origin is None): 199&#x202F;&#x219B;&#x202F;200line 199
+didn't jump to line 200, because the condition on line 199 was never true
+200 raise RuntimeError(f"invalid {origin=}") 
+201 old = self.branch() 
+202 self(["checkout", "-b", name, "--track", origin]) 
+203 return old[11:] if old.startswith("refs/heads/") else old 
+204 
+205 @property 
+206 def branches(self) -> GitRepoBranches: 
+207 result = GitRepoBranches([], []) 
+208 for line in self(["branch", "-a", "--format", "%(refname)"]).split("\n"): 
+209 if not line.strip(): 
+210 continue 
+211 if line.startswith("refs/heads/"): 
+212 result.local.append(line[11:]) 
+213 elif line.startswith("refs/remotes/"): 213&#x202F;&#x219B;&#x202F;216line
+213 didn't jump to line 216, because the condition on line 213 was never false
+214 result.remote.append(line[13:]) 
+215 else: 
+216 raise RuntimeError(f"invalid branch {line}") 
+217 return result 
+218 
+219 @property 
+220 def references(self) -> list[str]: 
+221 return [ 
+222 f"refs/tags/{line.strip()}" 
+223 for line in self(["tag", "-l"]).split("\n") 
+224 if line.strip() 
+225 ] 
+226 
+227 def clone( 
+228 self, 
+229 dest: str | Path, 
+230 force: bool = False, 
+231 branch: str | None = None, 
+232 ) -> GitRepo: 
+233 from shutil import rmtree 
+234 
+235 workdir = Path(dest).absolute() 
+236 if force: 236&#x202F;&#x219B;&#x202F;237line 236 didn't jump to line 237,
+because the condition on line 236 was never true
+237 rmtree(workdir, ignore_errors=True) 
+238 if workdir.exists(): 238&#x202F;&#x219B;&#x202F;239line 238 didn't jump to
+line 239, because the condition on line 238 was never true
+239 raise ValueError(f"target directory present {workdir}") 
+240 
+241 self( 
+242 [ 
+243 "clone", 
+244 *(["--branch", branch] if branch else []), 
+245 self.workdir.absolute(), 
+246 workdir.absolute(), 
+247 ], 
+248 ) 
+249 
+250 repo = self.__class__(workdir=workdir) 
+251 repo(["config", "user.name", self(["config", "user.name"])]) 
+252 repo(["config", "user.email", self(["config", "user.email"])]) 
 253 
-254def lookup(path: Path) -> GitRepo | None: 
-255 cur = path 
-256 found = False 
-257 while not found: 257&#x202F;&#x219B;&#x202F;263line 257 didn't jump to line
-263, because the condition on line 257 was never false
-258 if (cur / ".git").exists(): 
-259 return GitRepo(cur) 
-260 if str(cur) == cur.root: 260&#x202F;&#x219B;&#x202F;261line 260 didn't jump
-to line 261, because the condition on line 260 was never true
-261 break 
-262 cur = cur.parent 
-263 return None 
+254 return repo 
+255 
+256 
+257def lookup(path: Path) -> GitRepo | None: 
+258 cur = path 
+259 found = False 
+260 while not found: 260&#x202F;&#x219B;&#x202F;266line 260 didn't jump to line
+266, because the condition on line 260 was never false
+261 if (cur / ".git").exists(): 
+262 return GitRepo(cur) 
+263 if str(cur) == cur.root: 263&#x202F;&#x219B;&#x202F;264line 263 didn't jump
+to line 264, because the condition on line 263 was never true
+264 break 
+265 cur = cur.parent 
+266 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -51,27 +51,27 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">65 statements &nbsp;</span>
+            <span class="text">67 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">65<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">67<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">0<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -207,60 +207,64 @@
     <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="str">f"git checkout beta/{version}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">local</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="key">if</span> <span class="nam">local</span> <span class="op">!=</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"wrong version file {version=} != {local}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="com"># tag</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="com"># create an empty commit to mark the release</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"--allow-empty"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="com"># switch to master</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="com"># tag</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="com"># bump version</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="com"># switch to master (and incorporate the commit message)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"merge"</span><span class="op">,</span> <span class="str">f"beta/{version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com"># commit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">f"version bump {version} -> {new_version}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="str">        The release is almost complete.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">            git push origin release/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">            git push origin master</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com"># bump version</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="com"># commit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">f"version bump {version} -> {new_version}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">        The release is almost complete.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">        To revert this release:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">            git reset --hard HEAD~1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">            git tag -d release/{version}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">            git push origin release/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">            git push origin master</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">        To revert this release:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">            git reset --hard HEAD~1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">            git tag -d release/{version}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"unsupported mode {options.mode=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 65 statements   0 run 65 missing 2 excluded 0 partial *****
+***** 67 statements   0 run 67 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -143,49 +143,53 @@
 123 f"git checkout beta/{version}", 
 124 ) 
 125 return 
 126 local = match.group("beta") 
 127 if local != version: 
 128 options.error(f"wrong version file {version=} != {local}") 
 129 
-130 # tag 
-131 options.repo(["tag", "-a", f"release/{version}", "-m", f"released
-{version}"]) 
+130 # create an empty commit to mark the release 
+131 options.repo(["commit", "--allow-empty", "-m", f"released {version}"]) 
 132 
-133 # switch to master 
-134 options.repo(["checkout", master]) 
+133 # tag 
+134 options.repo(["tag", "-a", f"release/{version}", "-m", f"released
+{version}"]) 
 135 
-136 # bump version 
-137 new_version = tools.bump_version(version, options.mode) 
-138 tools.set_module_var(options.initfile, "__version__", new_version) 
+136 # switch to master (and incorporate the commit message) 
+137 options.repo(["checkout", master]) 
+138 options.repo(["merge", f"beta/{version}"]) 
 139 
-140 # commit 
-141 options.repo.commit( 
-142 options.initfile, f"version bump {version} -> {new_version}" 
-143 ) 
-144 
-145 print( # noqa: T201 
-146 tools.indent( 
-147 f""" 
-148 The release is almost complete. 
-149 
-150 To complete the release: 
-151 git push origin release/{version} 
-152 git push origin master 
+140 # bump version 
+141 new_version = tools.bump_version(version, options.mode) 
+142 tools.set_module_var(options.initfile, "__version__", new_version) 
+143 
+144 # commit 
+145 options.repo.commit( 
+146 options.initfile, f"version bump {version} -> {new_version}" 
+147 ) 
+148 
+149 print( # noqa: T201 
+150 tools.indent( 
+151 f""" 
+152 The release is almost complete. 
 153 
-154 To revert this release: 
-155 git reset --hard HEAD~1 
-156 git tag -d release/{version} 
-157 """ 
-158 ), 
-159 file=sys.stderr, 
-160 ) 
-161 else: 
-162 options.error(f"unsupported mode {options.mode=}") 
-163 raise RuntimeError(f"unsupported mode {options.mode=}") 
-164 
-165 
-166if __name__ == "__main__": 
-167 main() 
+154 To complete the release: 
+155 git push origin release/{version} 
+156 git push origin master 
+157 
+158 To revert this release: 
+159 git reset --hard HEAD~1 
+160 git tag -d release/{version} 
+161 """ 
+162 ), 
+163 file=sys.stderr, 
+164 ) 
+165 else: 
+166 options.error(f"unsupported mode {options.mode=}") 
+167 raise RuntimeError(f"unsupported mode {options.mode=}") 
+168 
+169 
+170if __name__ == "__main__": 
+171 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 10% similar despite different names*

```diff
@@ -51,330 +51,434 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">156 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">147<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">9<span class="text"> missing</span></button>
+            <span class="text">198 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">187<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">11<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
-            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">8<span class="text"> partial</span></button>
+            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">9<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">ast</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">re</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">scm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># see https://pypi.org/project/setuptools-github</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="com"># copy of setuptools_github.tools</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">ast</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">re</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">ToolsError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">class</span> <span class="nam">ValidationError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">class</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="key">class</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="key">class</span> <span class="nam">AbortExecutionError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="key">def</span> <span class="nam">_strip</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span> <span class="key">or</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">indent</span><span class="op">(</span><span class="nam">txt</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="op">:</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">explain</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">hint</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">message</span> <span class="op">=</span> <span class="nam">message</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_explain</span> <span class="op">=</span> <span class="nam">explain</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_hint</span> <span class="op">=</span> <span class="nam">hint</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">def</span> <span class="nam">explain</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_strip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_explain</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">def</span> <span class="nam">hint</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_strip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_hint</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">message</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">result</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">indent</span><span class="op">(</span><span class="str">"\n"</span> <span class="op">+</span> <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span><span class="op">[</span><span class="num">2</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">result</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"\nhint:"</span><span class="op">,</span> <span class="nam">indent</span><span class="op">(</span><span class="str">"\n"</span> <span class="op">+</span> <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span><span class="op">[</span><span class="num">2</span><span class="op">:</span><span class="op">]</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="key">def</span> <span class="nam">urmtree</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="str">"universal (win|*nix) rmtree"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">from</span> <span class="nam">os</span> <span class="key">import</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">from</span> <span class="nam">shutil</span> <span class="key">import</span> <span class="nam">rmtree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">from</span> <span class="nam">stat</span> <span class="key">import</span> <span class="nam">S_IWUSR</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">if</span> <span class="nam">name</span> <span class="op">==</span> <span class="str">"nt"</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">66&#x202F;&#x219B;&#x202F;67</span><span class="annotate long">line 66 didn't jump to line 67, because the condition on line 66 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">for</span> <span class="nam">p</span> <span class="key">in</span> <span class="nam">path</span><span class="op">.</span><span class="nam">rglob</span><span class="op">(</span><span class="str">"*"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">p</span><span class="op">.</span><span class="nam">chmod</span><span class="op">(</span><span class="nam">S_IWUSR</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="nam">rmtree</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">70&#x202F;&#x219B;&#x202F;71</span><span class="annotate long">line 70 didn't jump to line 71, because the condition on line 70 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"cannot remove {path=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="key">def</span> <span class="nam">indent</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">pre</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="str">"simple text indentation"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="key">from</span> <span class="nam">textwrap</span> <span class="key">import</span> <span class="nam">dedent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">scm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">class</span> <span class="nam">ToolsError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">class</span> <span class="nam">ValidationError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">class</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="nam">ToolsError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">class</span> <span class="nam">AbortExecutionError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">def</span> <span class="nam">_strip</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span> <span class="key">or</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">indent</span><span class="op">(</span><span class="nam">txt</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="op">:</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">explain</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">hint</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">message</span> <span class="op">=</span> <span class="nam">message</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_explain</span> <span class="op">=</span> <span class="nam">explain</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_hint</span> <span class="op">=</span> <span class="nam">hint</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">explain</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_strip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_explain</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">def</span> <span class="nam">hint</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_strip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_hint</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">message</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">result</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">indent</span><span class="op">(</span><span class="str">"\n"</span> <span class="op">+</span> <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span><span class="op">[</span><span class="num">2</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">result</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"\nhint:"</span><span class="op">,</span> <span class="nam">indent</span><span class="op">(</span><span class="str">"\n"</span> <span class="op">+</span> <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span><span class="op">[</span><span class="num">2</span><span class="op">:</span><span class="op">]</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="key">def</span> <span class="nam">urmtree</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="str">"universal (win|*nix) rmtree"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">from</span> <span class="nam">os</span> <span class="key">import</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">from</span> <span class="nam">shutil</span> <span class="key">import</span> <span class="nam">rmtree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">from</span> <span class="nam">stat</span> <span class="key">import</span> <span class="nam">S_IWUSR</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">if</span> <span class="nam">name</span> <span class="op">==</span> <span class="str">"nt"</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">68&#x202F;&#x219B;&#x202F;69</span><span class="annotate long">line 68 didn't jump to line 69, because the condition on line 68 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="key">for</span> <span class="nam">p</span> <span class="key">in</span> <span class="nam">path</span><span class="op">.</span><span class="nam">rglob</span><span class="op">(</span><span class="str">"*"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">            <span class="nam">p</span><span class="op">.</span><span class="nam">chmod</span><span class="op">(</span><span class="nam">S_IWUSR</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="nam">rmtree</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">72&#x202F;&#x219B;&#x202F;73</span><span class="annotate long">line 72 didn't jump to line 73, because the condition on line 72 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">raise</span> <span class="nam">RuntimeError</span><span class="op">(</span><span class="str">f"cannot remove {path=}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="key">def</span> <span class="nam">indent</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">pre</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">" "</span> <span class="op">*</span> <span class="num">2</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="str">"simple text indentation"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="nam">dedent</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="nam">last_eol</span> <span class="op">=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">[</span><span class="op">:</span><span class="op">-</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">last_eol</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">pre</span> <span class="op">+</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"\n"</span><span class="op">,</span> <span class="str">"\n"</span> <span class="op">+</span> <span class="nam">pre</span><span class="op">)</span> <span class="op">+</span> <span class="nam">last_eol</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span> <span class="key">if</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="key">def</span> <span class="nam">list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">Path</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="key">return</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="op">(</span><span class="op">[</span><span class="nam">paths</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">paths</span><span class="op">,</span> <span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">)</span> <span class="key">else</span> <span class="nam">paths</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="key">def</span> <span class="nam">get_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="str">"""extract from a python module in path the module level &lt;var> variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse using ast (no code-execution)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">        abort (bool): raise MissingVariable if var is not present</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">        None or str: the variable value if found or None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">from</span> <span class="nam">textwrap</span> <span class="key">import</span> <span class="nam">dedent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="nam">dedent</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">last_eol</span> <span class="op">=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">[</span><span class="op">:</span><span class="op">-</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="nam">last_eol</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">pre</span> <span class="op">+</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"\n"</span><span class="op">,</span> <span class="str">"\n"</span> <span class="op">+</span> <span class="nam">pre</span><span class="op">)</span> <span class="op">+</span> <span class="nam">last_eol</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span> <span class="key">if</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="key">def</span> <span class="nam">list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">Path</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">paths</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="key">return</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">return</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="op">(</span><span class="op">[</span><span class="nam">paths</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">paths</span><span class="op">,</span> <span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">)</span> <span class="key">else</span> <span class="nam">paths</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="key">def</span> <span class="nam">lstrip</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">left</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="nam">len</span><span class="op">(</span><span class="nam">left</span><span class="op">)</span> <span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">left</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="key">def</span> <span class="nam">get_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="str">"""extract from a python module in path the module level &lt;var> variable</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">    Raises:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">        MissingVariable: if the var is not found and abort is True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">    Notes:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="str">        this uses ast to parse path, so it doesn't load the module</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">class</span> <span class="nam">V</span><span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">NodeVisitor</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">keys</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span> <span class="op">=</span> <span class="nam">keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">result</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">def</span> <span class="nam">visit_Module</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: N802</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="com"># we extract the module level variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="key">for</span> <span class="nam">subnode</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">122&#x202F;&#x219B;&#x202F;123</span><span class="annotate long">line 122 didn't jump to line 123, because the condition on line 122 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">targets</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                        <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Constant</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                            <span class="str">f"cannot extract non Constant variable "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                            <span class="str">f"{target.id} ({type(subnode.value)})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">134&#x202F;&#x219B;&#x202F;137</span><span class="annotate long">line 134 didn't jump to line 137, because the condition on line 134 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">n</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">[</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generic_visit</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="nam">v</span> <span class="op">=</span> <span class="nam">V</span><span class="op">(</span><span class="op">{</span><span class="nam">var</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">143&#x202F;&#x219B;&#x202F;146</span><span class="annotate long">line 143 didn't jump to line 146, because the condition on line 143 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">tree</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">v</span><span class="op">.</span><span class="nam">visit</span><span class="op">(</span><span class="nam">tree</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">    <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span> <span class="key">and</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="key">raise</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="str">f"cannot find {var} in {path}"</span><span class="op">,</span> <span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="key">return</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">var</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="key">def</span> <span class="nam">set_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">create</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="str">"""replace var in path with value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">        value (None or Any): if not None replace var in initfile</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">        create (bool): create path if not present</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="str">        (str, str) the (&lt;previous-var-value|None>, &lt;the new text>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="com"># module level var</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">f"^{var}\\s*=\\s*['\\\"](?P&lt;value>[^\\\"']*)['\\\"]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="nam">fixed</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">    <span class="nam">lines</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse using ast (no code-execution)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">        abort (bool): raise MissingVariable if var is not present</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="str">        None or str: the variable value if found or None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="str">    Raises:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="str">        MissingVariable: if the var is not found and abort is True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">    Notes:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">        this uses ast to parse path, so it doesn't load the module</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="key">class</span> <span class="nam">V</span><span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">NodeVisitor</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">keys</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span> <span class="op">=</span> <span class="nam">keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">result</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="key">def</span> <span class="nam">visit_Module</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: N802</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="com"># we extract the module level variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">for</span> <span class="nam">subnode</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">130&#x202F;&#x219B;&#x202F;131</span><span class="annotate long">line 130 didn't jump to line 131, because the condition on line 130 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">targets</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                        <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="op">(</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Constant</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                            <span class="str">f"cannot extract non Constant variable "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                            <span class="str">f"{target.id} ({type(subnode.value)})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Num</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">142&#x202F;&#x219B;&#x202F;145</span><span class="annotate long">line 142 didn't jump to line 145, because the condition on line 142 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">n</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                        <span class="nam">value</span> <span class="op">=</span> <span class="nam">subnode</span><span class="op">.</span><span class="nam">value</span><span class="op">.</span><span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                    <span class="key">if</span> <span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                        <span class="nam">print</span><span class="op">(</span><span class="str">f">>> {path=}"</span><span class="op">)</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                        <span class="nam">print</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">                        <span class="key">raise</span> <span class="nam">ValidationError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                            <span class="str">f"found multiple repeated variables {target.id}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">result</span><span class="op">[</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generic_visit</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="nam">v</span> <span class="op">=</span> <span class="nam">V</span><span class="op">(</span><span class="op">{</span><span class="nam">var</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">tree</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">v</span><span class="op">.</span><span class="nam">visit</span><span class="op">(</span><span class="nam">tree</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">    <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span> <span class="key">and</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="key">raise</span> <span class="nam">MissingVariableError</span><span class="op">(</span><span class="str">f"cannot find {var} in {path}"</span><span class="op">,</span> <span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="key">return</span> <span class="nam">v</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">var</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="key">def</span> <span class="nam">set_module_var</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">var</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">create</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">    <span class="str">"""replace var in path with value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">    <span class="nam">src</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">src</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">parents</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">touch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="nam">input_lines</span> <span class="op">=</span> <span class="nam">src</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">reversed</span><span class="op">(</span><span class="nam">input_lines</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">if</span> <span class="nam">fixed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">        <span class="nam">match</span> <span class="op">=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">fixed</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"value"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">183&#x202F;&#x219B;&#x202F;186</span><span class="annotate long">line 183 didn't jump to line 186, because the condition on line 183 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">                <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">span</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="nam">x</span><span class="op">]</span> <span class="op">+</span> <span class="nam">value</span> <span class="op">+</span> <span class="nam">line</span><span class="op">[</span><span class="nam">y</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">reversed</span><span class="op">(</span><span class="nam">lines</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">fixed</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">if</span> <span class="nam">txt</span> <span class="key">and</span> <span class="nam">txt</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"\n"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">            <span class="nam">txt</span> <span class="op">+=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">txt</span> <span class="op">+=</span> <span class="str">f'{var} = "{value}"'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">        path (str,Path): python module file to parse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">        var (str): module level variable name to extract</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">        value (None or Any): if not None replace var in initfile</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">        create (bool): create path if not present</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="str">        (str, str) the (&lt;previous-var-value|None>, &lt;the new text>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="com"># validate the var</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">var</span><span class="op">,</span> <span class="nam">abort</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="com"># module level var</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">f"^{var}\\s*=\\s*['\\\"](?P&lt;value>[^\\\"']*)['\\\"]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="nam">fixed</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">lines</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="nam">src</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">src</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">parents</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">src</span><span class="op">.</span><span class="nam">touch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="nam">fp</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">return</span> <span class="nam">fixed</span><span class="op">,</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="key">def</span> <span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">mode</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="str">"""given a version str will bump it according to mode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t"><span class="str">        version: text in the N.M.O form</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="str">        mode: major, minor or micro</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t"><span class="str">        increased text</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "micro")</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="str">    "1.0.4"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "minor")</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">    "1.1.0"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="nam">newver</span> <span class="op">=</span> <span class="op">[</span><span class="nam">int</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span> <span class="key">for</span> <span class="nam">n</span> <span class="key">in</span> <span class="nam">version</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">if</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"major"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">3</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"minor"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"micro"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="key">return</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">newver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">input_lines</span> <span class="op">=</span> <span class="nam">src</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">input_lines</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">        <span class="key">if</span> <span class="nam">fixed</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="nam">match</span> <span class="op">=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="nam">fixed</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"value"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">201&#x202F;&#x219B;&#x202F;204</span><span class="annotate long">line 201 didn't jump to line 204, because the condition on line 201 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">span</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="nam">x</span><span class="op">]</span> <span class="op">+</span> <span class="nam">value</span> <span class="op">+</span> <span class="nam">line</span><span class="op">[</span><span class="nam">y</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="nam">lines</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="nam">txt</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">lines</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">if</span> <span class="op">(</span><span class="nam">fixed</span> <span class="key">is</span> <span class="key">None</span><span class="op">)</span> <span class="key">and</span> <span class="nam">create</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">if</span> <span class="nam">txt</span> <span class="key">and</span> <span class="nam">txt</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"\n"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="nam">txt</span> <span class="op">+=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">        <span class="nam">txt</span> <span class="op">+=</span> <span class="str">f'{var} = "{value}"'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="key">with</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"w"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="nam">fp</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">return</span> <span class="nam">fixed</span><span class="op">,</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="key">def</span> <span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">mode</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="str">"""given a version str will bump it according to mode</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">        version: text in the N.M.O form</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">        mode: major, minor or micro</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">        increased text</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="key">def</span> <span class="nam">update_version</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="nam">initfile</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates initfile in-place</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">initfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">repo</span> <span class="key">or</span> <span class="nam">github_dump</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">242&#x202F;&#x219B;&#x202F;243</span><span class="annotate long">line 242 didn't jump to line 243, because the condition on line 242 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="key">if</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="key">raise</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">InvalidGitRepoError</span><span class="op">(</span><span class="str">f"cannot find a valid git repo for {path}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="key">return</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">github_dump</span> <span class="key">and</span> <span class="nam">repo</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="str">"ref"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">            <span class="str">"sha"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">hex</span><span class="op">[</span><span class="op">:</span><span class="num">7</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">            <span class="str">"run_number"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">repo</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">github_dump</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">    <span class="nam">version</span> <span class="op">=</span> <span class="nam">current</span> <span class="op">=</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"/(?P&lt;what>beta|release)/(?P&lt;version>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">    <span class="nam">expr1</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"(?P&lt;version>\d+([.]\d+)*)(?P&lt;num>b\d+)?$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="key">if</span> <span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">        <span class="com"># setuptools double calls the update_version,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="com"># this fixes the issue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">        <span class="nam">match1</span> <span class="op">=</span> <span class="nam">expr1</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">current</span> <span class="key">or</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">match1</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">267&#x202F;&#x219B;&#x202F;268</span><span class="annotate long">line 267 didn't jump to line 268, because the condition on line 267 was never true</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="str">f"cannot parse current version '{current}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="key">if</span> <span class="nam">match1</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                <span class="str">f"building package for {current} from '{gdata['ref']}' "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="str">f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"what"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">            <span class="nam">version</span> <span class="op">=</span> <span class="str">f"{match1.group('version')}b{gdata['run_number']}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="nam">short</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"sha"</span><span class="op">]</span> <span class="op">+</span> <span class="op">(</span><span class="str">"*"</span> <span class="key">if</span> <span class="nam">dirty</span> <span class="key">else</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">short</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="key">return</span> <span class="nam">version</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "micro")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">    "1.0.4"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">    >>> bump_version("1.0.3", "minor")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">    "1.1.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="nam">newver</span> <span class="op">=</span> <span class="op">[</span><span class="nam">int</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span> <span class="key">for</span> <span class="nam">n</span> <span class="key">in</span> <span class="nam">version</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="key">if</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"major"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">3</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"minor"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">2</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="key">elif</span> <span class="nam">mode</span> <span class="op">==</span> <span class="str">"micro"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="nam">newver</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">    <span class="key">return</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">newver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="key">def</span> <span class="nam">get_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="nam">initfile</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates initfile in-place</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">        dict[str,str|None]: a dict with the current config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">        <span class="str">"version"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="str">"current"</span><span class="op">:</span> <span class="nam">get_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">        <span class="str">"branch"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="str">"hash"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">        <span class="str">"build"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">        <span class="str">"runid"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="str">"workflow"</span><span class="op">:</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="nam">path</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">initfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">lookup</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">repo</span> <span class="key">or</span> <span class="nam">github_dump</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">269&#x202F;&#x219B;&#x202F;270</span><span class="annotate long">line 269 didn't jump to line 270, because the condition on line 269 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">        <span class="key">if</span> <span class="nam">abort</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">            <span class="key">raise</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">InvalidGitRepoError</span><span class="op">(</span><span class="str">f"cannot find a valid git repo for {path}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">github_dump</span> <span class="key">and</span> <span class="nam">repo</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">            <span class="str">"ref"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">            <span class="str">"sha"</span><span class="op">:</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">hex</span><span class="op">[</span><span class="op">:</span><span class="num">7</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">            <span class="str">"run_number"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="str">"run_id"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">dirty</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="nam">gdata</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">github_dump</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">github_dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="nam">dirty</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"/(?P&lt;what>beta|release)/(?P&lt;version>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="nam">expr1</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"(?P&lt;version>\d+([.]\d+)*)(?P&lt;num>b\d+)?$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">lstrip</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">,</span> <span class="str">"refs/heads/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"sha"</span><span class="op">]</span> <span class="op">+</span> <span class="op">(</span><span class="str">"*"</span> <span class="key">if</span> <span class="nam">dirty</span> <span class="key">else</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"build"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_number"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"runid"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">gdata</span><span class="op">[</span><span class="str">"run_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">    <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"branch"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">    <span class="nam">current</span> <span class="op">=</span> <span class="nam">result</span><span class="op">[</span><span class="str">"current"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">    <span class="key">if</span> <span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">gdata</span><span class="op">[</span><span class="str">"ref"</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="com"># setuptools double calls the update_version,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">        <span class="com"># this fixes the issue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">        <span class="nam">match1</span> <span class="op">=</span> <span class="nam">expr1</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">current</span> <span class="key">or</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">match1</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">300&#x202F;&#x219B;&#x202F;301</span><span class="annotate long">line 300 didn't jump to line 301, because the condition on line 300 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span><span class="str">f"cannot parse current version '{current}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">        <span class="key">if</span> <span class="nam">match1</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"version"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">            <span class="key">raise</span> <span class="nam">InvalidVersionError</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                <span class="str">f"building package for {current} from '{gdata['ref']}' "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                <span class="str">f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="key">if</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"what"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"{match1.group('version')}b{gdata['run_number']}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"beta"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"workflow"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"tags"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t"><span class="key">def</span> <span class="nam">update_version</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">    <span class="nam">initfile</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="str">"""extracts version information from github_dump and updates initfile in-place</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">abort</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="key">def</span> <span class="nam">process</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="nam">initfile</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">github_dump</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="nam">paths</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="nam">fixers</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="nam">abort</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="str">"""get version from github_dump and updates initfile/paths</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">        paths (str, Path): path(s) to files jinja2 processeable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t"><span class="str">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="str">        str: the new version for the package</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">        {'branch': 'beta/0.3.1',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">         'build': 0,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">         'current': '0.3.1',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">         'hash': 'c9e484a*',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">         'version': '0.3.1b0',</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">         'runid': 0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">        }</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">    <span class="key">from</span> <span class="nam">argparse</span> <span class="key">import</span> <span class="nam">Namespace</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">    <span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">partial</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="key">from</span> <span class="nam">urllib</span><span class="op">.</span><span class="nam">parse</span> <span class="key">import</span> <span class="nam">quote</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">from</span> <span class="nam">jinja2</span> <span class="key">import</span> <span class="nam">Environment</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="key">class</span> <span class="nam">Context</span><span class="op">(</span><span class="nam">Namespace</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">        <span class="key">def</span> <span class="nam">items</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">                <span class="key">if</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">369&#x202F;&#x219B;&#x202F;370</span><span class="annotate long">line 369 didn't jump to line 370, because the condition on line 369 was never true</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">                <span class="key">yield</span> <span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">get_data</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="nam">github_dump</span><span class="op">,</span> <span class="nam">abort</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"version"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">set_module_var</span><span class="op">(</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__hash__"</span><span class="op">,</span> <span class="nam">data</span><span class="op">[</span><span class="str">"hash"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="nam">env</span> <span class="op">=</span> <span class="nam">Environment</span><span class="op">(</span><span class="nam">autoescape</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="nam">env</span><span class="op">.</span><span class="nam">filters</span><span class="op">[</span><span class="str">"urlquote"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">partial</span><span class="op">(</span><span class="nam">quote</span><span class="op">,</span> <span class="nam">safe</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">    <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">list_of_paths</span><span class="op">(</span><span class="nam">paths</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">path</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">        <span class="key">for</span> <span class="nam">old</span><span class="op">,</span> <span class="nam">new</span> <span class="key">in</span> <span class="op">(</span><span class="nam">fixers</span> <span class="key">or</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">381&#x202F;&#x219B;&#x202F;382</span><span class="annotate long">line 381 didn't jump to line 382, because the loop on line 381 never started</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">            <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="nam">old</span><span class="op">,</span> <span class="nam">new</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">        <span class="nam">tmpl</span> <span class="op">=</span> <span class="nam">env</span><span class="op">.</span><span class="nam">from_string</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">        <span class="nam">path</span><span class="op">.</span><span class="nam">write_text</span><span class="op">(</span><span class="nam">tmpl</span><span class="op">.</span><span class="nam">render</span><span class="op">(</span><span class="nam">ctx</span><span class="op">=</span><span class="nam">Context</span><span class="op">(</span><span class="op">**</span><span class="nam">data</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,308 +5,417 @@
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 156 statements   147 run 9 missing 0 excluded 8 partial *****
+***** 198 statements   187 run 11 missing 0 excluded 9 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
-1from __future__ import annotations 
-2 
-3import ast 
-4import json 
-5import re 
-6from pathlib import Path 
-7from typing import Any 
-8 
-9from . import scm 
+1# see https://pypi.org/project/setuptools-github 
+2# copy of setuptools_github.tools 
+3from __future__ import annotations 
+4 
+5import ast 
+6import json 
+7import re 
+8from pathlib import Path 
+9from typing import Any 
 10 
-11 
-12class ToolsError(Exception): 
-13 pass 
-14 
-15 
-16class ValidationError(ToolsError): 
-17 pass 
-18 
-19 
-20class InvalidVersionError(ToolsError): 
-21 pass 
-22 
-23 
-24class MissingVariableError(ToolsError): 
-25 pass 
-26 
-27 
-28class AbortExecutionError(Exception): 
-29 @staticmethod 
-30 def _strip(txt): 
-31 txt = txt or "" 
-32 txt = txt[1:] if txt.startswith("\n") else txt 
-33 txt = indent(txt, pre="") 
-34 return txt[:-1] if txt.endswith("\n") else txt 
-35 
-36 def __init__( 
-37 self, message: str, explain: str | None = None, hint: str | None = None 
-38 ): 
-39 self.message = message.strip() 
-40 self._explain = explain 
-41 self._hint = hint 
-42 
-43 @property 
-44 def explain(self): 
-45 return self._strip(self._explain) 
-46 
-47 @property 
-48 def hint(self): 
-49 return self._strip(self._hint) 
-50 
-51 def __str__(self): 
-52 result = [self.message] 
-53 if self.explain: 
-54 result.append(indent("\n" + self.explain, pre=" " * 2)[2:]) 
-55 if self.hint: 
-56 result.extend(["\nhint:", indent("\n" + self.hint, pre=" " * 2)[2:]]) 
-57 return "".join(result) 
-58 
-59 
-60def urmtree(path: Path): 
-61 "universal (win|*nix) rmtree" 
-62 from os import name 
-63 from shutil import rmtree 
-64 from stat import S_IWUSR 
-65 
-66 if name == "nt": 66&#x202F;&#x219B;&#x202F;67line 66 didn't jump to line 67,
-because the condition on line 66 was never true
-67 for p in path.rglob("*"): 
-68 p.chmod(S_IWUSR) 
-69 rmtree(path, ignore_errors=True) 
-70 if path.exists(): 70&#x202F;&#x219B;&#x202F;71line 70 didn't jump to line
-71, because the condition on line 70 was never true
-71 raise RuntimeError(f"cannot remove {path=}") 
-72 
-73 
-74def indent(txt: str, pre: str = " " * 2) -> str: 
-75 "simple text indentation" 
-76 
-77 from textwrap import dedent 
+11from . import scm 
+12 
+13 
+14class ToolsError(Exception): 
+15 pass 
+16 
+17 
+18class ValidationError(ToolsError): 
+19 pass 
+20 
+21 
+22class InvalidVersionError(ToolsError): 
+23 pass 
+24 
+25 
+26class MissingVariableError(ToolsError): 
+27 pass 
+28 
+29 
+30class AbortExecutionError(Exception): 
+31 @staticmethod 
+32 def _strip(txt): 
+33 txt = txt or "" 
+34 txt = txt[1:] if txt.startswith("\n") else txt 
+35 txt = indent(txt, pre="") 
+36 return txt[:-1] if txt.endswith("\n") else txt 
+37 
+38 def __init__( 
+39 self, message: str, explain: str | None = None, hint: str | None = None 
+40 ): 
+41 self.message = message.strip() 
+42 self._explain = explain 
+43 self._hint = hint 
+44 
+45 @property 
+46 def explain(self): 
+47 return self._strip(self._explain) 
+48 
+49 @property 
+50 def hint(self): 
+51 return self._strip(self._hint) 
+52 
+53 def __str__(self): 
+54 result = [self.message] 
+55 if self.explain: 
+56 result.append(indent("\n" + self.explain, pre=" " * 2)[2:]) 
+57 if self.hint: 
+58 result.extend(["\nhint:", indent("\n" + self.hint, pre=" " * 2)[2:]]) 
+59 return "".join(result) 
+60 
+61 
+62def urmtree(path: Path): 
+63 "universal (win|*nix) rmtree" 
+64 from os import name 
+65 from shutil import rmtree 
+66 from stat import S_IWUSR 
+67 
+68 if name == "nt": 68&#x202F;&#x219B;&#x202F;69line 68 didn't jump to line 69,
+because the condition on line 68 was never true
+69 for p in path.rglob("*"): 
+70 p.chmod(S_IWUSR) 
+71 rmtree(path, ignore_errors=True) 
+72 if path.exists(): 72&#x202F;&#x219B;&#x202F;73line 72 didn't jump to line
+73, because the condition on line 72 was never true
+73 raise RuntimeError(f"cannot remove {path=}") 
+74 
+75 
+76def indent(txt: str, pre: str = " " * 2) -> str: 
+77 "simple text indentation" 
 78 
-79 txt = dedent(txt) 
-80 if txt.endswith("\n"): 
-81 last_eol = "\n" 
-82 txt = txt[:-1] 
-83 else: 
-84 last_eol = "" 
-85 
-86 result = pre + txt.replace("\n", "\n" + pre) + last_eol 
-87 return result if result.strip() else result.strip() 
-88 
-89 
-90def list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]: 
-91 return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else
+79 from textwrap import dedent 
+80 
+81 txt = dedent(txt) 
+82 if txt.endswith("\n"): 
+83 last_eol = "\n" 
+84 txt = txt[:-1] 
+85 else: 
+86 last_eol = "" 
+87 
+88 result = pre + txt.replace("\n", "\n" + pre) + last_eol 
+89 return result if result.strip() else result.strip() 
+90 
+91 
+92def list_of_paths(paths: str | Path | list[str | Path] | None) -> list[Path]:
+ 
+93 if not paths: 
+94 return [] 
+95 return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else
 paths)] 
-92 
-93 
-94def get_module_var( 
-95 path: Path | str, var: str = "__version__", abort=True 
-96) -> str | None: 
-97 """extract from a python module in path the module level <var> variable 
-98 
-99 Args: 
-100 path (str,Path): python module file to parse using ast (no code-execution) 
-101 var (str): module level variable name to extract 
-102 abort (bool): raise MissingVariable if var is not present 
-103 
-104 Returns: 
-105 None or str: the variable value if found or None 
+96 
+97 
+98def lstrip(txt: str, left: str) -> str: 
+99 return txt[len(left) :] if txt.startswith(left) else txt 
+100 
+101 
+102def get_module_var( 
+103 path: Path | str, var: str = "__version__", abort=True 
+104) -> str | None: 
+105 """extract from a python module in path the module level <var> variable 
 106 
-107 Raises: 
-108 MissingVariable: if the var is not found and abort is True 
-109 
-110 Notes: 
-111 this uses ast to parse path, so it doesn't load the module 
-112 """ 
-113 
-114 class V(ast.NodeVisitor): 
-115 def __init__(self, keys): 
-116 self.keys = keys 
-117 self.result = {} 
-118 
-119 def visit_Module(self, node): # noqa: N802 
-120 # we extract the module level variables 
-121 for subnode in ast.iter_child_nodes(node): 
-122 if not isinstance(subnode, ast.Assign): 122&#x202F;&#x219B;&#x202F;123line
-122 didn't jump to line 123, because the condition on line 122 was never true
-123 continue 
-124 for target in subnode.targets: 
-125 if target.id not in self.keys: 
-126 continue 
-127 if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)): 
-128 raise ValidationError( 
-129 f"cannot extract non Constant variable " 
-130 f"{target.id} ({type(subnode.value)})" 
-131 ) 
-132 if isinstance(subnode.value, ast.Str): 
-133 value = subnode.value.s 
-134 elif isinstance(subnode.value, ast.Num): 134&#x202F;&#x219B;&#x202F;137line
-134 didn't jump to line 137, because the condition on line 134 was never false
-135 value = subnode.value.n 
-136 else: 
-137 value = subnode.value.value 
-138 self.result[target.id] = value 
-139 return self.generic_visit(node) 
-140 
-141 v = V({var}) 
-142 path = Path(path) 
-143 if path.exists(): 143&#x202F;&#x219B;&#x202F;146line 143 didn't jump to
-line 146, because the condition on line 143 was never false
-144 tree = ast.parse(Path(path).read_text()) 
-145 v.visit(tree) 
-146 if var not in v.result and abort: 
-147 raise MissingVariableError(f"cannot find {var} in {path}", path, var) 
-148 return v.result.get(var, None) 
-149 
-150 
-151def set_module_var( 
-152 path: str | Path, var: str, value: Any, create: bool = True 
-153) -> tuple[Any, str]: 
-154 """replace var in path with value 
-155 
-156 Args: 
-157 path (str,Path): python module file to parse 
-158 var (str): module level variable name to extract 
-159 value (None or Any): if not None replace var in initfile 
-160 create (bool): create path if not present 
-161 
-162 Returns: 
-163 (str, str) the (<previous-var-value|None>, <the new text>) 
-164 """ 
-165 # module level var 
-166 expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]") 
-167 fixed = None 
-168 lines = [] 
+107 Args: 
+108 path (str,Path): python module file to parse using ast (no code-execution) 
+109 var (str): module level variable name to extract 
+110 abort (bool): raise MissingVariable if var is not present 
+111 
+112 Returns: 
+113 None or str: the variable value if found or None 
+114 
+115 Raises: 
+116 MissingVariable: if the var is not found and abort is True 
+117 
+118 Notes: 
+119 this uses ast to parse path, so it doesn't load the module 
+120 """ 
+121 
+122 class V(ast.NodeVisitor): 
+123 def __init__(self, keys): 
+124 self.keys = keys 
+125 self.result = {} 
+126 
+127 def visit_Module(self, node): # noqa: N802 
+128 # we extract the module level variables 
+129 for subnode in ast.iter_child_nodes(node): 
+130 if not isinstance(subnode, ast.Assign): 130&#x202F;&#x219B;&#x202F;131line
+130 didn't jump to line 131, because the condition on line 130 was never true
+131 continue 
+132 for target in subnode.targets: 
+133 if target.id not in self.keys: 
+134 continue 
+135 if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)): 
+136 raise ValidationError( 
+137 f"cannot extract non Constant variable " 
+138 f"{target.id} ({type(subnode.value)})" 
+139 ) 
+140 if isinstance(subnode.value, ast.Str): 
+141 value = subnode.value.s 
+142 elif isinstance(subnode.value, ast.Num): 142&#x202F;&#x219B;&#x202F;145line
+142 didn't jump to line 145, because the condition on line 142 was never false
+143 value = subnode.value.n 
+144 else: 
+145 value = subnode.value.value 
+146 if target.id in self.result: 
+147 print(f">>> {path=}") # noqa: T201 
+148 print(path.read_text()) # noqa: T201 
+149 raise ValidationError( 
+150 f"found multiple repeated variables {target.id}" 
+151 ) 
+152 self.result[target.id] = value 
+153 return self.generic_visit(node) 
+154 
+155 v = V({var}) 
+156 path = Path(path) 
+157 if path.exists(): 
+158 tree = ast.parse(Path(path).read_text()) 
+159 v.visit(tree) 
+160 if var not in v.result and abort: 
+161 raise MissingVariableError(f"cannot find {var} in {path}", path, var) 
+162 return v.result.get(var, None) 
+163 
+164 
+165def set_module_var( 
+166 path: str | Path, var: str, value: Any, create: bool = True 
+167) -> tuple[Any, str]: 
+168 """replace var in path with value 
 169 
-170 src = Path(path) 
-171 if not src.exists() and create: 
-172 src.parent.mkdir(parents=True, exist_ok=True) 
-173 src.touch() 
-174 
-175 input_lines = src.read_text().split("\n") 
-176 for line in reversed(input_lines): 
-177 if fixed: 
-178 lines.append(line) 
-179 continue 
-180 match = expr.search(line) 
-181 if match: 
-182 fixed = match.group("value") 
-183 if value is not None: 183&#x202F;&#x219B;&#x202F;186line 183 didn't jump to
-line 186, because the condition on line 183 was never false
-184 x, y = match.span(1) 
-185 line = line[:x] + value + line[y:] 
-186 lines.append(line) 
-187 txt = "\n".join(reversed(lines)) 
-188 if not fixed and create: 
-189 if txt and txt[-1] != "\n": 
-190 txt += "\n" 
-191 txt += f'{var} = "{value}"' 
+170 Args: 
+171 path (str,Path): python module file to parse 
+172 var (str): module level variable name to extract 
+173 value (None or Any): if not None replace var in initfile 
+174 create (bool): create path if not present 
+175 
+176 Returns: 
+177 (str, str) the (<previous-var-value|None>, <the new text>) 
+178 """ 
+179 
+180 # validate the var 
+181 get_module_var(path, var, abort=False) 
+182 
+183 # module level var 
+184 expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]") 
+185 fixed = None 
+186 lines = [] 
+187 
+188 src = Path(path) 
+189 if not src.exists() and create: 
+190 src.parent.mkdir(parents=True, exist_ok=True) 
+191 src.touch() 
 192 
-193 with Path(path).open("w") as fp: 
-194 fp.write(txt) 
-195 return fixed, txt 
-196 
-197 
-198def bump_version(version: str, mode: str) -> str: 
-199 """given a version str will bump it according to mode 
-200 
-201 Arguments: 
-202 version: text in the N.M.O form 
-203 mode: major, minor or micro 
-204 
-205 Returns: 
-206 increased text 
-207 
-208 >>> bump_version("1.0.3", "micro") 
-209 "1.0.4" 
-210 >>> bump_version("1.0.3", "minor") 
-211 "1.1.0" 
-212 """ 
-213 newver = [int(n) for n in version.split(".")] 
-214 if mode == "major": 
-215 newver[-3] += 1 
-216 newver[-2] = 0 
-217 newver[-1] = 0 
-218 elif mode == "minor": 
-219 newver[-2] += 1 
-220 newver[-1] = 0 
-221 elif mode == "micro": 
-222 newver[-1] += 1 
-223 return ".".join(str(v) for v in newver) 
-224 
+193 input_lines = src.read_text().split("\n") 
+194 for line in input_lines: 
+195 if fixed is not None: 
+196 lines.append(line) 
+197 continue 
+198 match = expr.search(line) 
+199 if match: 
+200 fixed = match.group("value") 
+201 if value is not None: 201&#x202F;&#x219B;&#x202F;204line 201 didn't jump to
+line 204, because the condition on line 201 was never false
+202 x, y = match.span(1) 
+203 line = line[:x] + value + line[y:] 
+204 lines.append(line) 
+205 txt = "\n".join(lines) 
+206 if (fixed is None) and create: 
+207 if txt and txt[-1] != "\n": 
+208 txt += "\n" 
+209 txt += f'{var} = "{value}"' 
+210 
+211 with Path(path).open("w") as fp: 
+212 fp.write(txt) 
+213 return fixed, txt 
+214 
+215 
+216def bump_version(version: str, mode: str) -> str: 
+217 """given a version str will bump it according to mode 
+218 
+219 Arguments: 
+220 version: text in the N.M.O form 
+221 mode: major, minor or micro 
+222 
+223 Returns: 
+224 increased text 
 225 
-226def update_version( 
-227 initfile: str | Path, github_dump: str | None = None, abort: bool = True 
-228) -> str | None: 
-229 """extracts version information from github_dump and updates initfile in-
+226 >>> bump_version("1.0.3", "micro") 
+227 "1.0.4" 
+228 >>> bump_version("1.0.3", "minor") 
+229 "1.1.0" 
+230 """ 
+231 newver = [int(n) for n in version.split(".")] 
+232 if mode == "major": 
+233 newver[-3] += 1 
+234 newver[-2] = 0 
+235 newver[-1] = 0 
+236 elif mode == "minor": 
+237 newver[-2] += 1 
+238 newver[-1] = 0 
+239 elif mode == "micro": 
+240 newver[-1] += 1 
+241 return ".".join(str(v) for v in newver) 
+242 
+243 
+244def get_data( 
+245 initfile: str | Path, github_dump: str | None = None, abort: bool = True 
+246) -> dict[str, str | None]: 
+247 """extracts version information from github_dump and updates initfile in-
 place 
-230 
-231 Args: 
-232 initfile (str, Path): path to the __init__.py file with a __version__
+248 
+249 Args: 
+250 initfile (str, Path): path to the __init__.py file with a __version__
 variable 
-233 github_dump (str): the os.getenv("GITHUB_DUMP") value 
-234 
-235 Returns: 
-236 str: the new version for the package 
-237 """ 
-238 
-239 path = Path(initfile) 
-240 repo = scm.lookup(path) 
-241 
-242 if not (repo or github_dump): 242&#x202F;&#x219B;&#x202F;243line 242 didn't
-jump to line 243, because the condition on line 242 was never true
-243 if abort: 
-244 raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}") 
-245 return get_module_var(path, "__version__") 
-246 
-247 if not github_dump and repo: 
-248 gdata = { 
-249 "ref": repo.head.name, 
-250 "sha": repo.head.target.hex[:7], 
-251 "run_number": 0, 
-252 } 
-253 dirty = bool(repo.status()) 
-254 else: 
-255 gdata = json.loads(github_dump) if isinstance(github_dump, str) else
+251 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+252 
+253 Returns: 
+254 dict[str,str|None]: a dict with the current config 
+255 """ 
+256 result = { 
+257 "version": get_module_var(initfile, "__version__"), 
+258 "current": get_module_var(initfile, "__version__"), 
+259 "branch": None, 
+260 "hash": None, 
+261 "build": None, 
+262 "runid": None, 
+263 "workflow": None, 
+264 } 
+265 
+266 path = Path(initfile) 
+267 repo = scm.lookup(path) 
+268 
+269 if not (repo or github_dump): 269&#x202F;&#x219B;&#x202F;270line 269 didn't
+jump to line 270, because the condition on line 269 was never true
+270 if abort: 
+271 raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}") 
+272 return result 
+273 
+274 if not github_dump and repo: 
+275 gdata = { 
+276 "ref": repo.head.name, 
+277 "sha": repo.head.target.hex[:7], 
+278 "run_number": 0, 
+279 "run_id": 0, 
+280 } 
+281 dirty = repo.dirty() 
+282 else: 
+283 gdata = json.loads(github_dump) if isinstance(github_dump, str) else
 github_dump 
-256 dirty = False 
-257 
-258 version = current = get_module_var(path, "__version__") 
-259 
-260 expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$") 
-261 expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$") 
-262 
-263 if match := expr.search(gdata["ref"]): 
-264 # setuptools double calls the update_version, 
-265 # this fixes the issue 
-266 match1 = expr1.search(current or "") 
-267 if not match1: 267&#x202F;&#x219B;&#x202F;268line 267 didn't jump to line
-268, because the condition on line 267 was never true
-268 raise InvalidVersionError(f"cannot parse current version '{current}'") 
-269 if match1.group("version") != match.group("version"): 
-270 raise InvalidVersionError( 
-271 f"building package for {current} from '{gdata['ref']}' " 
-272 f"branch ({match.groupdict()} mismatch {match1.groupdict()})" 
-273 ) 
-274 if match.group("what") == "beta": 
-275 version = f"{match1.group('version')}b{gdata['run_number']}" 
-276 
-277 short = gdata["sha"] + ("*" if dirty else "") 
-278 
-279 set_module_var(path, "__version__", version) 
-280 set_module_var(path, "__hash__", short) 
-281 return version 
+284 dirty = False 
+285 
+286 expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$") 
+287 expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$") 
+288 
+289 result["branch"] = lstrip(gdata["ref"], "refs/heads/") 
+290 result["hash"] = gdata["sha"] + ("*" if dirty else "") 
+291 result["build"] = gdata["run_number"] 
+292 result["runid"] = gdata["run_id"] 
+293 result["workflow"] = result["branch"] 
+294 
+295 current = result["current"] 
+296 if match := expr.search(gdata["ref"]): 
+297 # setuptools double calls the update_version, 
+298 # this fixes the issue 
+299 match1 = expr1.search(current or "") 
+300 if not match1: 300&#x202F;&#x219B;&#x202F;301line 300 didn't jump to line
+301, because the condition on line 300 was never true
+301 raise InvalidVersionError(f"cannot parse current version '{current}'") 
+302 if match1.group("version") != match.group("version"): 
+303 raise InvalidVersionError( 
+304 f"building package for {current} from '{gdata['ref']}' " 
+305 f"branch ({match.groupdict()} mismatch {match1.groupdict()})" 
+306 ) 
+307 if match.group("what") == "beta": 
+308 result["version"] = f"{match1.group('version')}b{gdata['run_number']}" 
+309 result["workflow"] = "beta" 
+310 else: 
+311 result["workflow"] = "tags" 
+312 return result 
+313 
+314 
+315def update_version( 
+316 initfile: str | Path, github_dump: str | None = None, abort: bool = True 
+317) -> str | None: 
+318 """extracts version information from github_dump and updates initfile in-
+place 
+319 
+320 Args: 
+321 initfile (str, Path): path to the __init__.py file with a __version__
+variable 
+322 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+323 
+324 Returns: 
+325 str: the new version for the package 
+326 """ 
+327 
+328 data = get_data(initfile, github_dump, abort) 
+329 set_module_var(initfile, "__version__", data["version"]) 
+330 set_module_var(initfile, "__hash__", data["hash"]) 
+331 return data["version"] 
+332 
+333 
+334def process( 
+335 initfile: str | Path, 
+336 github_dump: str | None = None, 
+337 paths: str | Path | list[str | Path] | None = None, 
+338 fixers: dict[str, str] | None = None, 
+339 abort: bool = True, 
+340) -> dict[str, str | None]: 
+341 """get version from github_dump and updates initfile/paths 
+342 
+343 Args: 
+344 paths (str, Path): path(s) to files jinja2 processeable 
+345 initfile (str, Path): path to the __init__.py file with a __version__
+variable 
+346 github_dump (str): the os.getenv("GITHUB_DUMP") value 
+347 
+348 Returns: 
+349 str: the new version for the package 
+350 
+351 Example: 
+352 {'branch': 'beta/0.3.1', 
+353 'build': 0, 
+354 'current': '0.3.1', 
+355 'hash': 'c9e484a*', 
+356 'version': '0.3.1b0', 
+357 'runid': 0 
+358 } 
+359 """ 
+360 from argparse import Namespace 
+361 from functools import partial 
+362 from urllib.parse import quote 
+363 
+364 from jinja2 import Environment 
+365 
+366 class Context(Namespace): 
+367 def items(self): 
+368 for name, value in self.__dict__.items(): 
+369 if name.startswith("_"): 369&#x202F;&#x219B;&#x202F;370line 369 didn't jump
+to line 370, because the condition on line 369 was never true
+370 continue 
+371 yield (name, value) 
+372 
+373 data = get_data(initfile, github_dump, abort) 
+374 set_module_var(initfile, "__version__", data["version"]) 
+375 set_module_var(initfile, "__hash__", data["hash"]) 
+376 
+377 env = Environment(autoescape=True) 
+378 env.filters["urlquote"] = partial(quote, safe="") 
+379 for path in list_of_paths(paths): 
+380 txt = path.read_text() 
+381 for old, new in (fixers or {}).items(): 381&#x202F;&#x219B;&#x202F;382line
+381 didn't jump to line 382, because the loop on line 381 never started
+382 txt = txt.replace(old, new, 1) 
+383 tmpl = env.from_string(txt) 
+384 path.write_text(tmpl.render(ctx=Context(**data))) 
+385 return data 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
 
 
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
-at 2023-08-01 21:34 +0000
+at 2023-08-03 19:49 +0000
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">58%</span>
+            <span class="pc_cov">62%</span>
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -99,70 +99,70 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_scm_py.html">src/hatch_ci/scm.py</a></td>
-                <td>160</td>
-                <td>31</td>
+                <td>162</td>
+                <td>27</td>
                 <td>0</td>
                 <td>52</td>
-                <td>7</td>
-                <td class="right" data-ratio="166 212">78%</td>
+                <td>8</td>
+                <td class="right" data-ratio="175 214">82%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_script_py.html">src/hatch_ci/script.py</a></td>
-                <td>65</td>
-                <td>65</td>
+                <td>67</td>
+                <td>67</td>
                 <td>2</td>
                 <td>20</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 85">0%</td>
+                <td class="right" data-ratio="0 87">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
-                <td>156</td>
-                <td>9</td>
+                <td>198</td>
+                <td>11</td>
                 <td>0</td>
-                <td>70</td>
-                <td>8</td>
-                <td class="right" data-ratio="205 226">91%</td>
+                <td>82</td>
+                <td>9</td>
+                <td class="right" data-ratio="256 280">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>17</td>
                 <td>17</td>
                 <td>0</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 19">0%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>478</td>
+                <td>524</td>
                 <td>200</td>
                 <td>2</td>
-                <td>162</td>
-                <td>15</td>
-                <td class="right" data-ratio="373 640">58%</td>
+                <td>174</td>
+                <td>17</td>
+                <td class="right" data-ratio="433 698">62%</td>
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
-            created at 2023-08-01 21:34 +0000
+            created at 2023-08-03 19:49 +0000
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
 
-****** Coverage report: 58% ******
+****** Coverage report: 62% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-01 21:34 +0000
+coverage.py_v7.2.7, created at 2023-08-03 19:49 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
 src/hatch_ci/cli.py      72         72      0        18       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
 src/hatch_ci/hooks.py    5          5       0        0        0       0%
-src/hatch_ci/scm.py      160        31      0        52       7       78%
-src/hatch_ci/script.py   65         65      2        20       0       0%
-src/hatch_ci/tools.py    156        9       0        70       8       91%
+src/hatch_ci/scm.py      162        27      0        52       8       82%
+src/hatch_ci/script.py   67         67      2        20       0       0%
+src/hatch_ci/tools.py    198        11      0        82       9       91%
 src/hatch_ci/            17         17      0        2        0       0%
 version_hook.py
-Total                    478        200     2        162      15      58%
+Total                    524        200     2        174      17      62%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-01 21:34 +0000
+coverage.py_v7.2.7, created at 2023-08-03 19:49 +0000
  ____
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/status.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8685763888888889%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_scm_py': {'hash': 'b208d1663706f031c634592ef10b4313', 'index': "*

 * *            "{'nums': {insert: [(2, 162), (4, 27), (6, 8), (7, 12)], delete: [7, 6, 4, 2]}}}, "*

 * *            "'d_7005a4ce5d73f943_script_py': {'hash': '1f1f9597ce7c541f1fe029e8c67db0ee', 'index': "*

 * *            "{'nums': {insert: [(2, 67), (4, 67)], delete: [4, 2]}}}, "*

 * *            "'d_7005a4ce5d73f943_tools_py': {'hash': '38589310877fbebf852e6b6a7d997136', 'index': "*

 * *            "{'nums': {insert: [(2, 198), (4 […]*

```diff
@@ -65,60 +65,60 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "41bce2f71040e14bf267c82fc061941f",
+            "hash": "b208d1663706f031c634592ef10b4313",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
-                    160,
+                    162,
                     0,
-                    31,
+                    27,
                     52,
-                    7,
-                    15
+                    8,
+                    12
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_script_py": {
-            "hash": "728f07121398f0c867cfb108722678ca",
+            "hash": "1f1f9597ce7c541f1fe029e8c67db0ee",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_script_py.html",
                 "nums": [
                     0,
                     1,
-                    65,
+                    67,
                     2,
-                    65,
+                    67,
                     20,
                     0,
                     20
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "a8d6f2dd9ac0362526ec26b96e255458",
+            "hash": "38589310877fbebf852e6b6a7d997136",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
-                    156,
+                    198,
                     0,
+                    11,
+                    82,
                     9,
-                    70,
-                    8,
-                    12
+                    13
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
             "hash": "1796f88df0132c43781f63f1858011e4",
             "index": {
@@ -134,10 +134,10 @@
                     2
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "78efd540b1740235466229ddcdf3f22d",
+    "globals": "67e4af6d5592040c1e4310b56bd8a304",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/junit/junit.html`

 * *Files 2% similar despite different names*

```diff
@@ -435,52 +435,52 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 01-Aug-2023 at 21:34:51 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 03-Aug-2023 at 19:49:08 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>13 tests ran in 0.95 seconds. </p>
-    <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">13 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
+    <p>15 tests ran in 1.38 seconds. </p>
+    <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">15 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
           <th class="sortable" col="duration">Duration</th>
           <th class="sortable links" col="links">Links</th></tr>
         <tr hidden="true" id="not-found-message">
           <th colspan="4">No results found. Try to check the filters</th></tr></thead>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_lookup</td>
-          <td class="col-duration">0.03</td>
+          <td class="col-duration">0.04</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.25</td>
+          <td class="col-duration">0.32</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/KS15M4&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/5MHAHJ&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
@@ -519,23 +519,41 @@
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
-          <td class="col-name">tests/test_tools.py::test_get_module_var</td>
+          <td class="col-name">tests/test_tools.py::test_lstrip</td>
           <td class="col-duration">0.00</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_tools.py::test_get_module_var</td>
+          <td class="col-duration">0.00</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="log"> ------------------------------Captured stdout call------------------------------ <br/>&gt;&gt;&gt; path=PosixPath(&#x27;/tmp/pytest-of-runner/pytest-0/test_get_module_var0/in0.txt&#x27;)
+
+# a test file
+A = 12
+B = 3+5
+C = &quot;hello&quot;
+C = &quot;hello2&quot;
+# end of test
+
+<br/></div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_set_module_var</td>
           <td class="col-duration">0.00</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
@@ -556,36 +574,47 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_master</td>
-          <td class="col-duration">0.05</td>
+          <td class="col-duration">0.06</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_beta</td>
-          <td class="col-duration">0.10</td>
+          <td class="col-duration">0.14</td>
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
-          <td class="col-duration">0.06</td>
+          <td class="col-duration">0.08</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
+<br/></div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_tools.py::test_process</td>
+          <td class="col-duration">0.18</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Updated 1 path from the index
+Switched to a new branch &#x27;beta/1.2.3&#x27;
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,54 +1,65 @@
 ****** junit.html ******
-Report generated on 01-Aug-2023 at 21:34:51 by pytest-html v3.2.0
+Report generated on 03-Aug-2023 at 19:49:08 by pytest-html v3.2.0
 ***** Summary *****
-13 tests ran in 0.95 seconds.
+15 tests ran in 1.38 seconds.
 (Un)check the boxes to filter the results.
-*13 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
+*15 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
-Passed tests/test_scm.py::test_lookup                        0.03
+Passed tests/test_scm.py::test_lookup                        0.04
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.25
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.32
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/KS15M4&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/5MHAHJ&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
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
-Passed tests/test_tools.py::test_get_module_var              0.00
+Passed tests/test_tools.py::test_lstrip                      0.00
 No log output captured.
+Passed tests/test_tools.py::test_get_module_var              0.00
+------------------------------Captured stdout call--------------------------
+----
+>>> path=PosixPath(&#x27;/tmp/pytest-of-runner/pytest-0/
+test_get_module_var0/in0.txt&#x27;) # a test file A = 12 B = 3+5 C = "hello"
+C = "hello2" # end of test
 Passed tests/test_tools.py::test_set_module_var              0.00
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
-Passed tests/test_tools.py::test_update_version_master       0.05
+Passed tests/test_tools.py::test_update_version_master       0.06
 No log output captured.
-Passed tests/test_tools.py::test_update_version_beta         0.10
+Passed tests/test_tools.py::test_update_version_beta         0.14
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.06
+Passed tests/test_tools.py::test_update_version_release      0.08
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
+Passed tests/test_tools.py::test_process                     0.18
+------------------------------Captured stderr call--------------------------
+----
+Updated 1 path from the index Switched to a new branch &#x27;beta/
+1.2.3&#x27;
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/junit/junit.xml`

 * *Files 25% similar despite different names*

#### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,18 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="13" time="0.939" timestamp="2023-08-01T21:34:50.187960" hostname="fv-az306-295">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.032"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.259"/>
-    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.002"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="15" time="1.364" timestamp="2023-08-03T19:49:06.766759" hostname="fv-az336-727">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.042"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.325"/>
+    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
+    <testcase classname="tests.test_tools" name="test_lstrip" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.005"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.051"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.108"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.066"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.060"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.143"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.084"/>
+    <testcase classname="tests.test_tools" name="test_process" time="0.186"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/index.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 <thead><tr class="summary">
 <th class="summary">File</th>
 <th class="summary">Imprecision</th>
 <th class="summary">Lines</th>
 </tr></thead>
 <tfoot><tr class="summary summary-quality-1">
 <th class="summary summary-filename">Total</th>
-<th class="summary summary-precision">18.04% imprecise</th>
-<th class="summary summary-lines">937 LOC</th>
+<th class="summary summary-precision">18.03% imprecise</th>
+<th class="summary summary-lines">1048 LOC</th>
 </tr></tfoot>
 <tbody>
 <tr class="summary summary-quality-0">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/__init__.py.html">hatch_ci</a></td>
 <td class="summary summary-precision">0.00% imprecise</td>
 <td class="summary summary-lines">2 LOC</td>
 </tr>
@@ -36,26 +36,26 @@
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/hooks.py.html">hatch_ci.hooks</a></td>
 <td class="summary summary-precision">37.50% imprecise</td>
 <td class="summary summary-lines">8 LOC</td>
 </tr>
 <tr class="summary summary-quality-1">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/scm.py.html">hatch_ci.scm</a></td>
-<td class="summary summary-precision">9.13% imprecise</td>
-<td class="summary summary-lines">263 LOC</td>
+<td class="summary summary-precision">9.02% imprecise</td>
+<td class="summary summary-lines">266 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/script.py.html">hatch_ci.script</a></td>
-<td class="summary summary-precision">26.35% imprecise</td>
-<td class="summary summary-lines">167 LOC</td>
+<td class="summary summary-precision">26.90% imprecise</td>
+<td class="summary summary-lines">171 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/tools.py.html">hatch_ci.tools</a></td>
-<td class="summary summary-precision">21.71% imprecise</td>
-<td class="summary summary-lines">281 LOC</td>
+<td class="summary summary-precision">20.52% imprecise</td>
+<td class="summary summary-lines">385 LOC</td>
 </tr>
 <tr class="summary summary-quality-1">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/version_hook.py.html">hatch_ci.version_hook</a></td>
 <td class="summary summary-precision">12.66% imprecise</td>
 <td class="summary summary-lines">79 LOC</td>
 </tr>
 </tbody>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
 ****** Mypy Type Check Coverage Summary ******
               Summary from index
 File                  Imprecision      Lines
-Total                 18.04% imprecise 937 LOC
+Total                 18.03% imprecise 1048 LOC
 hatch_ci              0.00% imprecise  2 LOC
 hatch_ci.cli          19.85% imprecise 136 LOC
 hatch_ci.common       0.00% imprecise  1 LOC
 hatch_ci.hooks        37.50% imprecise 8 LOC
-hatch_ci.scm          9.13% imprecise  263 LOC
-hatch_ci.script       26.35% imprecise 167 LOC
-hatch_ci.tools        21.71% imprecise 281 LOC
+hatch_ci.scm          9.02% imprecise  266 LOC
+hatch_ci.script       26.90% imprecise 171 LOC
+hatch_ci.tools        20.52% imprecise 385 LOC
 hatch_ci.version_hook 12.66% imprecise 79 LOC
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -267,14 +267,17 @@
 <span id="L257" class="lineno"><a class="lineno" href="#L257">257</a></span>
 <span id="L258" class="lineno"><a class="lineno" href="#L258">258</a></span>
 <span id="L259" class="lineno"><a class="lineno" href="#L259">259</a></span>
 <span id="L260" class="lineno"><a class="lineno" href="#L260">260</a></span>
 <span id="L261" class="lineno"><a class="lineno" href="#L261">261</a></span>
 <span id="L262" class="lineno"><a class="lineno" href="#L262">262</a></span>
 <span id="L263" class="lineno"><a class="lineno" href="#L263">263</a></span>
+<span id="L264" class="lineno"><a class="lineno" href="#L264">264</a></span>
+<span id="L265" class="lineno"><a class="lineno" href="#L265">265</a></span>
+<span id="L266" class="lineno"><a class="lineno" href="#L266">266</a></span>
 </pre></td>
 <td class="table-code"><pre><span class="line-empty" title="No Anys on this line!"># see https://pypi.org/project/setuptools-github</span>
 <span class="line-empty" title="No Anys on this line!"># copy of setuptools_github.scm</span>
 <span class="line-precise" title="No Anys on this line!">from __future__ import annotations</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">import dataclasses as dc</span>
 <span class="line-precise" title="No Anys on this line!">import io</span>
@@ -473,14 +476,17 @@
 <span class="line-precise" title="No Anys on this line!">            value = mapper[tag]</span>
 <span class="line-precise" title="No Anys on this line!">            if value:</span>
 <span class="line-precise" title="No Anys on this line!">                result[filename] = (</span>
 <span class="line-precise" title="No Anys on this line!">                    (result[filename] | value) if filename in result else value</span>
 <span class="line-empty" title="No Anys on this line!">                )</span>
 <span class="line-precise" title="No Anys on this line!">        return result</span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    def dirty(self) -&gt; bool:</span>
+<span class="line-precise" title="No Anys on this line!">        return bool(self.status(untracked_files="no"))</span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    def commit(</span>
 <span class="line-empty" title="No Anys on this line!">        self,</span>
 <span class="line-empty" title="No Anys on this line!">        paths: ListOfArgs,</span>
 <span class="line-empty" title="No Anys on this line!">        message: str,</span>
 <span class="line-empty" title="No Anys on this line!">    ) -&gt; None:</span>
 <span class="line-precise" title="No Anys on this line!">        all_paths = to_list_of_paths(paths)</span>
 <span class="line-precise" title="No Anys on this line!">        self(["add", *all_paths])</span>
```

#### html2text {}

```diff
@@ -186,90 +186,93 @@
 179             if value:
 180                 result[filename] = (
 181                     (result[filename] | value) if filename in result else
 182 value
 183                 )
 184         return result
 185
-186     def commit(
-187         self,
-188         paths: ListOfArgs,
-189         message: str,
-190     ) -> None:
-191         all_paths = to_list_of_paths(paths)
-192         self(["add", *all_paths])
-193         self(["commit", "-m", message, *all_paths])
-194
-195     def branch(self, name: str | None = None, origin: str = "master") -
-196 > str:
-197         if not name:
-198             name = self.head.name or ""
-199             return name[11:] if name.startswith("refs/heads/") else name
-200         if not (origin or origin is None):
-201             raise RuntimeError(f"invalid {origin=}")
-202         old = self.branch()
-203         self(["checkout", "-b", name, "--track", origin])
-204         return old[11:] if old.startswith("refs/heads/") else old
-205
-206     @property
-207     def branches(self) -> GitRepoBranches:
-208         result = GitRepoBranches([], [])
-209         for line in self(["branch", "-a", "--format", "%(refname)"]).split
-210 ("\n"):
-211             if not line.strip():
-212                 continue
-213             if line.startswith("refs/heads/"):
-214                 result.local.append(line[11:])
-215             elif line.startswith("refs/remotes/"):
-216                 result.remote.append(line[13:])
-217             else:
-218                 raise RuntimeError(f"invalid branch {line}")
-219         return result
-220
-221     @property
-222     def references(self) -> list[str]:
-223         return [
-224             f"refs/tags/{line.strip()}"
-225             for line in self(["tag", "-l"]).split("\n")
-226             if line.strip()
-227         ]
-228
-229     def clone(
-230         self,
-231         dest: str | Path,
-232         force: bool = False,
-233         branch: str | None = None,
-234     ) -> GitRepo:
-235         from shutil import rmtree
-236
-237         workdir = Path(dest).absolute()
-238         if force:
-239             rmtree(workdir, ignore_errors=True)
-240         if workdir.exists():
-241             raise ValueError(f"target directory present {workdir}")
-242
-243         self(
-244             [
-245                 "clone",
-246                 *(["--branch", branch] if branch else []),
-247                 self.workdir.absolute(),
-248                 workdir.absolute(),
-249             ],
-250         )
-251
-252         repo = self.__class__(workdir=workdir)
-253         repo(["config", "user.name", self(["config", "user.name"])])
-254         repo(["config", "user.email", self(["config", "user.email"])])
-255
-256         return repo
-257
+186     def dirty(self) -> bool:
+187         return bool(self.status(untracked_files="no"))
+188
+189     def commit(
+190         self,
+191         paths: ListOfArgs,
+192         message: str,
+193     ) -> None:
+194         all_paths = to_list_of_paths(paths)
+195         self(["add", *all_paths])
+196         self(["commit", "-m", message, *all_paths])
+197
+198     def branch(self, name: str | None = None, origin: str = "master") -
+199 > str:
+200         if not name:
+201             name = self.head.name or ""
+202             return name[11:] if name.startswith("refs/heads/") else name
+203         if not (origin or origin is None):
+204             raise RuntimeError(f"invalid {origin=}")
+205         old = self.branch()
+206         self(["checkout", "-b", name, "--track", origin])
+207         return old[11:] if old.startswith("refs/heads/") else old
+208
+209     @property
+210     def branches(self) -> GitRepoBranches:
+211         result = GitRepoBranches([], [])
+212         for line in self(["branch", "-a", "--format", "%(refname)"]).split
+213 ("\n"):
+214             if not line.strip():
+215                 continue
+216             if line.startswith("refs/heads/"):
+217                 result.local.append(line[11:])
+218             elif line.startswith("refs/remotes/"):
+219                 result.remote.append(line[13:])
+220             else:
+221                 raise RuntimeError(f"invalid branch {line}")
+222         return result
+223
+224     @property
+225     def references(self) -> list[str]:
+226         return [
+227             f"refs/tags/{line.strip()}"
+228             for line in self(["tag", "-l"]).split("\n")
+229             if line.strip()
+230         ]
+231
+232     def clone(
+233         self,
+234         dest: str | Path,
+235         force: bool = False,
+236         branch: str | None = None,
+237     ) -> GitRepo:
+238         from shutil import rmtree
+239
+240         workdir = Path(dest).absolute()
+241         if force:
+242             rmtree(workdir, ignore_errors=True)
+243         if workdir.exists():
+244             raise ValueError(f"target directory present {workdir}")
+245
+246         self(
+247             [
+248                 "clone",
+249                 *(["--branch", branch] if branch else []),
+250                 self.workdir.absolute(),
+251                 workdir.absolute(),
+252             ],
+253         )
+254
+255         repo = self.__class__(workdir=workdir)
+256         repo(["config", "user.name", self(["config", "user.name"])])
+257         repo(["config", "user.email", self(["config", "user.email"])])
 258
-259 def lookup(path: Path) -> GitRepo | None:
-260     cur = path
-261     found = False
-262     while not found:
-263         if (cur / ".git").exists():
+259         return repo
+260
+261
+262 def lookup(path: Path) -> GitRepo | None:
+263     cur = path
+264     found = False
+265     while not found:
+266         if (cur / ".git").exists():
                 return GitRepo(cur)
             if str(cur) == cur.root:
                 break
             cur = cur.parent
         return None
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,18 @@
 <span id="L161" class="lineno"><a class="lineno" href="#L161">161</a></span>
 <span id="L162" class="lineno"><a class="lineno" href="#L162">162</a></span>
 <span id="L163" class="lineno"><a class="lineno" href="#L163">163</a></span>
 <span id="L164" class="lineno"><a class="lineno" href="#L164">164</a></span>
 <span id="L165" class="lineno"><a class="lineno" href="#L165">165</a></span>
 <span id="L166" class="lineno"><a class="lineno" href="#L166">166</a></span>
 <span id="L167" class="lineno"><a class="lineno" href="#L167">167</a></span>
+<span id="L168" class="lineno"><a class="lineno" href="#L168">168</a></span>
+<span id="L169" class="lineno"><a class="lineno" href="#L169">169</a></span>
+<span id="L170" class="lineno"><a class="lineno" href="#L170">170</a></span>
+<span id="L171" class="lineno"><a class="lineno" href="#L171">171</a></span>
 </pre></td>
 <td class="table-code"><pre><span class="line-empty" title="No Anys on this line!">"""create a beta branch or release a beta branch</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">This script will either create a new beta branch:</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">     hatch-ci make-beta ./src/package_name/__init__.py</span>
 <span class="line-empty" title="No Anys on this line!"></span>
@@ -345,21 +349,27 @@
 Explicit (x4)">        local = match.group("beta")</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x2)">        if local != version:</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)
 Explicit (x1)">            options.error(f"wrong version file {version=} != {local}")</span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">        # create an empty commit to mark the release</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x3)">        options.repo(["commit", "--allow-empty", "-m", f"released {version}"])</span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">        # tag</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)">        options.repo(["tag", "-a", f"release/{version}", "-m", f"released {version}"])</span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-empty" title="No Anys on this line!">        # switch to master</span>
+<span class="line-empty" title="No Anys on this line!">        # switch to master (and incorporate the commit message)</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x4)">        options.repo(["checkout", master])</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x3)">        options.repo(["merge", f"beta/{version}"])</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">        # bump version</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">        new_version = tools.bump_version(version, options.mode)</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)
 Unannotated (x2)">        tools.set_module_var(options.initfile, "__version__", new_version)</span>
```

#### html2text {}

```diff
@@ -131,46 +131,51 @@
 125                 f"git checkout beta/{version}",
 126             )
 127             return
 128         local = match.group("beta")
 129         if local != version:
 130             options.error(f"wrong version file {version=} != {local}")
 131
-132         # tag
-133         options.repo(["tag", "-a", f"release/{version}", "-m", f"released
+132         # create an empty commit to mark the release
+133         options.repo(["commit", "--allow-empty", "-m", f"released
 134 {version}"])
 135
-136         # switch to master
-137         options.repo(["checkout", master])
-138
-139         # bump version
-140         new_version = tools.bump_version(version, options.mode)
-141         tools.set_module_var(options.initfile, "__version__", new_version)
-142
-143         # commit
-144         options.repo.commit(
-145             options.initfile, f"version bump {version} -> {new_version}"
-146         )
+136         # tag
+137         options.repo(["tag", "-a", f"release/{version}", "-m", f"released
+138 {version}"])
+139
+140         # switch to master (and incorporate the commit message)
+141         options.repo(["checkout", master])
+142         options.repo(["merge", f"beta/{version}"])
+143
+144         # bump version
+145         new_version = tools.bump_version(version, options.mode)
+146         tools.set_module_var(options.initfile, "__version__", new_version)
 147
-148         print(  # noqa: T201
-149             tools.indent(
-150                 f"""
-151         The release is almost complete.
+148         # commit
+149         options.repo.commit(
+150             options.initfile, f"version bump {version} -> {new_version}"
+151         )
 152
-153         To complete the release:
-154             git push origin release/{version}
-155             git push origin master
-156
-157         To revert this release:
-158             git reset --hard HEAD~1
-159             git tag -d release/{version}
-160         """
-161             ),
-162             file=sys.stderr,
-163         )
-164     else:
-165         options.error(f"unsupported mode {options.mode=}")
-166         raise RuntimeError(f"unsupported mode {options.mode=}")
-167
+153         print(  # noqa: T201
+154             tools.indent(
+155                 f"""
+156         The release is almost complete.
+157
+158         To complete the release:
+159             git push origin release/{version}
+160             git push origin master
+161
+162         To revert this release:
+163             git reset --hard HEAD~1
+164             git tag -d release/{version}
+165         """
+166             ),
+167             file=sys.stderr,
+168         )
+169     else:
+170         options.error(f"unsupported mode {options.mode=}")
+171         raise RuntimeError(f"unsupported mode {options.mode=}")
+
 
     if __name__ == "__main__":
         main()
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files 19% similar despite different names*

```diff
@@ -285,16 +285,122 @@
 <span id="L275" class="lineno"><a class="lineno" href="#L275">275</a></span>
 <span id="L276" class="lineno"><a class="lineno" href="#L276">276</a></span>
 <span id="L277" class="lineno"><a class="lineno" href="#L277">277</a></span>
 <span id="L278" class="lineno"><a class="lineno" href="#L278">278</a></span>
 <span id="L279" class="lineno"><a class="lineno" href="#L279">279</a></span>
 <span id="L280" class="lineno"><a class="lineno" href="#L280">280</a></span>
 <span id="L281" class="lineno"><a class="lineno" href="#L281">281</a></span>
+<span id="L282" class="lineno"><a class="lineno" href="#L282">282</a></span>
+<span id="L283" class="lineno"><a class="lineno" href="#L283">283</a></span>
+<span id="L284" class="lineno"><a class="lineno" href="#L284">284</a></span>
+<span id="L285" class="lineno"><a class="lineno" href="#L285">285</a></span>
+<span id="L286" class="lineno"><a class="lineno" href="#L286">286</a></span>
+<span id="L287" class="lineno"><a class="lineno" href="#L287">287</a></span>
+<span id="L288" class="lineno"><a class="lineno" href="#L288">288</a></span>
+<span id="L289" class="lineno"><a class="lineno" href="#L289">289</a></span>
+<span id="L290" class="lineno"><a class="lineno" href="#L290">290</a></span>
+<span id="L291" class="lineno"><a class="lineno" href="#L291">291</a></span>
+<span id="L292" class="lineno"><a class="lineno" href="#L292">292</a></span>
+<span id="L293" class="lineno"><a class="lineno" href="#L293">293</a></span>
+<span id="L294" class="lineno"><a class="lineno" href="#L294">294</a></span>
+<span id="L295" class="lineno"><a class="lineno" href="#L295">295</a></span>
+<span id="L296" class="lineno"><a class="lineno" href="#L296">296</a></span>
+<span id="L297" class="lineno"><a class="lineno" href="#L297">297</a></span>
+<span id="L298" class="lineno"><a class="lineno" href="#L298">298</a></span>
+<span id="L299" class="lineno"><a class="lineno" href="#L299">299</a></span>
+<span id="L300" class="lineno"><a class="lineno" href="#L300">300</a></span>
+<span id="L301" class="lineno"><a class="lineno" href="#L301">301</a></span>
+<span id="L302" class="lineno"><a class="lineno" href="#L302">302</a></span>
+<span id="L303" class="lineno"><a class="lineno" href="#L303">303</a></span>
+<span id="L304" class="lineno"><a class="lineno" href="#L304">304</a></span>
+<span id="L305" class="lineno"><a class="lineno" href="#L305">305</a></span>
+<span id="L306" class="lineno"><a class="lineno" href="#L306">306</a></span>
+<span id="L307" class="lineno"><a class="lineno" href="#L307">307</a></span>
+<span id="L308" class="lineno"><a class="lineno" href="#L308">308</a></span>
+<span id="L309" class="lineno"><a class="lineno" href="#L309">309</a></span>
+<span id="L310" class="lineno"><a class="lineno" href="#L310">310</a></span>
+<span id="L311" class="lineno"><a class="lineno" href="#L311">311</a></span>
+<span id="L312" class="lineno"><a class="lineno" href="#L312">312</a></span>
+<span id="L313" class="lineno"><a class="lineno" href="#L313">313</a></span>
+<span id="L314" class="lineno"><a class="lineno" href="#L314">314</a></span>
+<span id="L315" class="lineno"><a class="lineno" href="#L315">315</a></span>
+<span id="L316" class="lineno"><a class="lineno" href="#L316">316</a></span>
+<span id="L317" class="lineno"><a class="lineno" href="#L317">317</a></span>
+<span id="L318" class="lineno"><a class="lineno" href="#L318">318</a></span>
+<span id="L319" class="lineno"><a class="lineno" href="#L319">319</a></span>
+<span id="L320" class="lineno"><a class="lineno" href="#L320">320</a></span>
+<span id="L321" class="lineno"><a class="lineno" href="#L321">321</a></span>
+<span id="L322" class="lineno"><a class="lineno" href="#L322">322</a></span>
+<span id="L323" class="lineno"><a class="lineno" href="#L323">323</a></span>
+<span id="L324" class="lineno"><a class="lineno" href="#L324">324</a></span>
+<span id="L325" class="lineno"><a class="lineno" href="#L325">325</a></span>
+<span id="L326" class="lineno"><a class="lineno" href="#L326">326</a></span>
+<span id="L327" class="lineno"><a class="lineno" href="#L327">327</a></span>
+<span id="L328" class="lineno"><a class="lineno" href="#L328">328</a></span>
+<span id="L329" class="lineno"><a class="lineno" href="#L329">329</a></span>
+<span id="L330" class="lineno"><a class="lineno" href="#L330">330</a></span>
+<span id="L331" class="lineno"><a class="lineno" href="#L331">331</a></span>
+<span id="L332" class="lineno"><a class="lineno" href="#L332">332</a></span>
+<span id="L333" class="lineno"><a class="lineno" href="#L333">333</a></span>
+<span id="L334" class="lineno"><a class="lineno" href="#L334">334</a></span>
+<span id="L335" class="lineno"><a class="lineno" href="#L335">335</a></span>
+<span id="L336" class="lineno"><a class="lineno" href="#L336">336</a></span>
+<span id="L337" class="lineno"><a class="lineno" href="#L337">337</a></span>
+<span id="L338" class="lineno"><a class="lineno" href="#L338">338</a></span>
+<span id="L339" class="lineno"><a class="lineno" href="#L339">339</a></span>
+<span id="L340" class="lineno"><a class="lineno" href="#L340">340</a></span>
+<span id="L341" class="lineno"><a class="lineno" href="#L341">341</a></span>
+<span id="L342" class="lineno"><a class="lineno" href="#L342">342</a></span>
+<span id="L343" class="lineno"><a class="lineno" href="#L343">343</a></span>
+<span id="L344" class="lineno"><a class="lineno" href="#L344">344</a></span>
+<span id="L345" class="lineno"><a class="lineno" href="#L345">345</a></span>
+<span id="L346" class="lineno"><a class="lineno" href="#L346">346</a></span>
+<span id="L347" class="lineno"><a class="lineno" href="#L347">347</a></span>
+<span id="L348" class="lineno"><a class="lineno" href="#L348">348</a></span>
+<span id="L349" class="lineno"><a class="lineno" href="#L349">349</a></span>
+<span id="L350" class="lineno"><a class="lineno" href="#L350">350</a></span>
+<span id="L351" class="lineno"><a class="lineno" href="#L351">351</a></span>
+<span id="L352" class="lineno"><a class="lineno" href="#L352">352</a></span>
+<span id="L353" class="lineno"><a class="lineno" href="#L353">353</a></span>
+<span id="L354" class="lineno"><a class="lineno" href="#L354">354</a></span>
+<span id="L355" class="lineno"><a class="lineno" href="#L355">355</a></span>
+<span id="L356" class="lineno"><a class="lineno" href="#L356">356</a></span>
+<span id="L357" class="lineno"><a class="lineno" href="#L357">357</a></span>
+<span id="L358" class="lineno"><a class="lineno" href="#L358">358</a></span>
+<span id="L359" class="lineno"><a class="lineno" href="#L359">359</a></span>
+<span id="L360" class="lineno"><a class="lineno" href="#L360">360</a></span>
+<span id="L361" class="lineno"><a class="lineno" href="#L361">361</a></span>
+<span id="L362" class="lineno"><a class="lineno" href="#L362">362</a></span>
+<span id="L363" class="lineno"><a class="lineno" href="#L363">363</a></span>
+<span id="L364" class="lineno"><a class="lineno" href="#L364">364</a></span>
+<span id="L365" class="lineno"><a class="lineno" href="#L365">365</a></span>
+<span id="L366" class="lineno"><a class="lineno" href="#L366">366</a></span>
+<span id="L367" class="lineno"><a class="lineno" href="#L367">367</a></span>
+<span id="L368" class="lineno"><a class="lineno" href="#L368">368</a></span>
+<span id="L369" class="lineno"><a class="lineno" href="#L369">369</a></span>
+<span id="L370" class="lineno"><a class="lineno" href="#L370">370</a></span>
+<span id="L371" class="lineno"><a class="lineno" href="#L371">371</a></span>
+<span id="L372" class="lineno"><a class="lineno" href="#L372">372</a></span>
+<span id="L373" class="lineno"><a class="lineno" href="#L373">373</a></span>
+<span id="L374" class="lineno"><a class="lineno" href="#L374">374</a></span>
+<span id="L375" class="lineno"><a class="lineno" href="#L375">375</a></span>
+<span id="L376" class="lineno"><a class="lineno" href="#L376">376</a></span>
+<span id="L377" class="lineno"><a class="lineno" href="#L377">377</a></span>
+<span id="L378" class="lineno"><a class="lineno" href="#L378">378</a></span>
+<span id="L379" class="lineno"><a class="lineno" href="#L379">379</a></span>
+<span id="L380" class="lineno"><a class="lineno" href="#L380">380</a></span>
+<span id="L381" class="lineno"><a class="lineno" href="#L381">381</a></span>
+<span id="L382" class="lineno"><a class="lineno" href="#L382">382</a></span>
+<span id="L383" class="lineno"><a class="lineno" href="#L383">383</a></span>
+<span id="L384" class="lineno"><a class="lineno" href="#L384">384</a></span>
+<span id="L385" class="lineno"><a class="lineno" href="#L385">385</a></span>
 </pre></td>
-<td class="table-code"><pre><span class="line-precise" title="No Anys on this line!">from __future__ import annotations</span>
+<td class="table-code"><pre><span class="line-empty" title="No Anys on this line!"># see https://pypi.org/project/setuptools-github</span>
+<span class="line-empty" title="No Anys on this line!"># copy of setuptools_github.tools</span>
+<span class="line-precise" title="No Anys on this line!">from __future__ import annotations</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">import ast</span>
 <span class="line-precise" title="No Anys on this line!">import json</span>
 <span class="line-precise" title="No Anys on this line!">import re</span>
 <span class="line-precise" title="No Anys on this line!">from pathlib import Path</span>
 <span class="line-precise" title="No Anys on this line!">from typing import Any</span>
 <span class="line-empty" title="No Anys on this line!"></span>
@@ -388,19 +494,25 @@
 <span class="line-empty" title="No Anys on this line!">    else:</span>
 <span class="line-precise" title="No Anys on this line!">        last_eol = ""</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    result = pre + txt.replace("\n", "\n" + pre) + last_eol</span>
 <span class="line-precise" title="No Anys on this line!">    return result if result.strip() else result.strip()</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">def list_of_paths(paths: str | Path | list[str | Path]) -&gt; list[Path]:</span>
+<span class="line-precise" title="No Anys on this line!">def list_of_paths(paths: str | Path | list[str | Path] | None) -&gt; list[Path]:</span>
+<span class="line-precise" title="No Anys on this line!">    if not paths:</span>
+<span class="line-empty" title="No Anys on this line!">        return []</span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x2)">    return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">def lstrip(txt: str, left: str) -&gt; str:</span>
+<span class="line-precise" title="No Anys on this line!">    return txt[len(left) :] if txt.startswith(left) else txt</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">def get_module_var(</span>
 <span class="line-precise" title="No Anys on this line!">    path: Path | str, var: str = "__version__", abort=True</span>
 <span class="line-empty" title="No Anys on this line!">) -&gt; str | None:</span>
 <span class="line-empty" title="No Anys on this line!">    """extract from a python module in path the module level &lt;var&gt; variable</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Args:</span>
@@ -458,14 +570,26 @@
 Explicit (x2)">                    elif isinstance(subnode.value, ast.Num):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">                        value = subnode.value.n</span>
 <span class="line-empty" title="No Anys on this line!">                    else:</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)">                        value = subnode.value.value</span>
 <span class="line-any" title="Any Types on this line: 
+Unannotated (x3)">                    if target.id in self.result:</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x5)">                        print(f"&gt;&gt;&gt; {path=}")  # noqa: T201</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x1)
+Error (x1)">                        print(path.read_text())  # noqa: T201</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x1)">                        raise ValidationError(</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x6)">                            f"found multiple repeated variables {target.id}"</span>
+<span class="line-empty" title="No Anys on this line!">                        )</span>
+<span class="line-any" title="Any Types on this line: 
 Unannotated (x4)">                    self.result[target.id] = value</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x3)">            return self.generic_visit(node)</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">    v = V({var})</span>
 <span class="line-precise" title="Any Types on this line: 
@@ -493,46 +617,49 @@
 <span class="line-empty" title="No Anys on this line!">        var (str): module level variable name to extract</span>
 <span class="line-empty" title="No Anys on this line!">        value (None or Any): if not None replace var in initfile</span>
 <span class="line-empty" title="No Anys on this line!">        create (bool): create path if not present</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Returns:</span>
 <span class="line-empty" title="No Anys on this line!">        (str, str) the (&lt;previous-var-value|None&gt;, &lt;the new text&gt;)</span>
 <span class="line-empty" title="No Anys on this line!">    """</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    # validate the var</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x1)">    get_module_var(path, var, abort=False)</span>
+<span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    # module level var</span>
 <span class="line-precise" title="Any Types on this line: 
 Omitted Generics (x4)">    expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P&lt;value&gt;[^\\\"']*)['\\\"]")</span>
 <span class="line-precise" title="No Anys on this line!">    fixed = None</span>
 <span class="line-precise" title="No Anys on this line!">    lines = []</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x1)">    src = Path(path)</span>
 <span class="line-precise" title="No Anys on this line!">    if not src.exists() and create:</span>
 <span class="line-precise" title="No Anys on this line!">        src.parent.mkdir(parents=True, exist_ok=True)</span>
 <span class="line-precise" title="No Anys on this line!">        src.touch()</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    input_lines = src.read_text().split("\n")</span>
-<span class="line-precise" title="Any Types on this line: 
-Omitted Generics (x4)">    for line in reversed(input_lines):</span>
-<span class="line-precise" title="No Anys on this line!">        if fixed:</span>
+<span class="line-precise" title="No Anys on this line!">    for line in input_lines:</span>
+<span class="line-precise" title="No Anys on this line!">        if fixed is not None:</span>
 <span class="line-unanalyzed" title="No Anys on this line!">            lines.append(line)</span>
 <span class="line-precise" title="No Anys on this line!">            continue</span>
 <span class="line-precise" title="No Anys on this line!">        match = expr.search(line)</span>
 <span class="line-precise" title="No Anys on this line!">        if match:</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x4)">            fixed = match.group("value")</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x1)">            if value is not None:</span>
 <span class="line-precise" title="No Anys on this line!">                x, y = match.span(1)</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)">                line = line[:x] + value + line[y:]</span>
 <span class="line-precise" title="No Anys on this line!">        lines.append(line)</span>
-<span class="line-precise" title="Any Types on this line: 
-Omitted Generics (x4)">    txt = "\n".join(reversed(lines))</span>
+<span class="line-precise" title="No Anys on this line!">    txt = "\n".join(lines)</span>
 <span class="line-imprecise" title="Any Types on this line: 
-Explicit (x1)">    if not fixed and create:</span>
+Explicit (x1)">    if (fixed is None) and create:</span>
 <span class="line-precise" title="No Anys on this line!">        if txt and txt[-1] != "\n":</span>
 <span class="line-precise" title="No Anys on this line!">            txt += "\n"</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x1)">        txt += f'{var} = "{value}"'</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x2)">    with Path(path).open("w") as fp:</span>
@@ -565,62 +692,81 @@
 <span class="line-precise" title="No Anys on this line!">        newver[-2] += 1</span>
 <span class="line-precise" title="No Anys on this line!">        newver[-1] = 0</span>
 <span class="line-precise" title="No Anys on this line!">    elif mode == "micro":</span>
 <span class="line-precise" title="No Anys on this line!">        newver[-1] += 1</span>
 <span class="line-precise" title="No Anys on this line!">    return ".".join(str(v) for v in newver)</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="No Anys on this line!">def update_version(</span>
+<span class="line-precise" title="No Anys on this line!">def get_data(</span>
 <span class="line-precise" title="No Anys on this line!">    initfile: str | Path, github_dump: str | None = None, abort: bool = True</span>
-<span class="line-empty" title="No Anys on this line!">) -&gt; str | None:</span>
+<span class="line-empty" title="No Anys on this line!">) -&gt; dict[str, str | None]:</span>
 <span class="line-empty" title="No Anys on this line!">    """extracts version information from github_dump and updates initfile in-place</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Args:</span>
 <span class="line-empty" title="No Anys on this line!">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>
 <span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-empty" title="No Anys on this line!">    Returns:</span>
-<span class="line-empty" title="No Anys on this line!">        str: the new version for the package</span>
+<span class="line-empty" title="No Anys on this line!">        dict[str,str|None]: a dict with the current config</span>
 <span class="line-empty" title="No Anys on this line!">    """</span>
+<span class="line-precise" title="No Anys on this line!">    result = {</span>
+<span class="line-precise" title="Any Types on this line: 
+Unannotated (x1)">        "version": get_module_var(initfile, "__version__"),</span>
+<span class="line-precise" title="Any Types on this line: 
+Unannotated (x1)">        "current": get_module_var(initfile, "__version__"),</span>
+<span class="line-precise" title="No Anys on this line!">        "branch": None,</span>
+<span class="line-precise" title="No Anys on this line!">        "hash": None,</span>
+<span class="line-precise" title="No Anys on this line!">        "build": None,</span>
+<span class="line-precise" title="No Anys on this line!">        "runid": None,</span>
+<span class="line-precise" title="No Anys on this line!">        "workflow": None,</span>
+<span class="line-empty" title="No Anys on this line!">    }</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
 Explicit (x1)">    path = Path(initfile)</span>
 <span class="line-precise" title="No Anys on this line!">    repo = scm.lookup(path)</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    if not (repo or github_dump):</span>
 <span class="line-precise" title="No Anys on this line!">        if abort:</span>
 <span class="line-precise" title="No Anys on this line!">            raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")</span>
-<span class="line-precise" title="Any Types on this line: 
-Unannotated (x1)">        return get_module_var(path, "__version__")</span>
+<span class="line-precise" title="No Anys on this line!">        return result</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="No Anys on this line!">    if not github_dump and repo:</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Unannotated (x1)">        gdata = {</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">            "ref": repo.head.name,</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x4)">            "sha": repo.head.target.hex[:7],</span>
 <span class="line-precise" title="No Anys on this line!">            "run_number": 0,</span>
+<span class="line-precise" title="No Anys on this line!">            "run_id": 0,</span>
 <span class="line-empty" title="No Anys on this line!">        }</span>
-<span class="line-precise" title="No Anys on this line!">        dirty = bool(repo.status())</span>
+<span class="line-precise" title="No Anys on this line!">        dirty = repo.dirty()</span>
 <span class="line-empty" title="No Anys on this line!">    else:</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x12)
 Unannotated (x1)">        gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump</span>
 <span class="line-precise" title="No Anys on this line!">        dirty = False</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-precise" title="Any Types on this line: 
-Unannotated (x1)">    version = current = get_module_var(path, "__version__")</span>
-<span class="line-empty" title="No Anys on this line!"></span>
-<span class="line-precise" title="Any Types on this line: 
 Omitted Generics (x4)">    expr = re.compile(r"/(?P&lt;what&gt;beta|release)/(?P&lt;version&gt;\d+([.]\d+)*)$")</span>
 <span class="line-precise" title="Any Types on this line: 
 Omitted Generics (x4)">    expr1 = re.compile(r"(?P&lt;version&gt;\d+([.]\d+)*)(?P&lt;num&gt;b\d+)?$")</span>
 <span class="line-empty" title="No Anys on this line!"></span>
 <span class="line-any" title="Any Types on this line: 
+Unannotated (x2)">    result["branch"] = lstrip(gdata["ref"], "refs/heads/")</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x3)">    result["hash"] = gdata["sha"] + ("*" if dirty else "")</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x2)">    result["build"] = gdata["run_number"]</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x2)">    result["runid"] = gdata["run_id"]</span>
+<span class="line-precise" title="No Anys on this line!">    result["workflow"] = result["branch"]</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    current = result["current"]</span>
+<span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">    if match := expr.search(gdata["ref"]):</span>
 <span class="line-empty" title="No Anys on this line!">        # setuptools double calls the update_version,</span>
 <span class="line-empty" title="No Anys on this line!">        # this fixes the issue</span>
 <span class="line-precise" title="No Anys on this line!">        match1 = expr1.search(current or "")</span>
 <span class="line-precise" title="No Anys on this line!">        if not match1:</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(f"cannot parse current version '{current}'")</span>
 <span class="line-imprecise" title="Any Types on this line: 
@@ -632,23 +778,102 @@
 Omitted Generics (x4)">                f"building package for {current} from '{gdata['ref']}' "</span>
 <span class="line-empty" title="No Anys on this line!">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
 <span class="line-empty" title="No Anys on this line!">            )</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x4)">        if match.group("what") == "beta":</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x3)
-Unannotated (x2)">            version = f"{match1.group('version')}b{gdata['run_number']}"</span>
+Unannotated (x2)">            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"</span>
+<span class="line-precise" title="No Anys on this line!">            result["workflow"] = "beta"</span>
+<span class="line-empty" title="No Anys on this line!">        else:</span>
+<span class="line-precise" title="No Anys on this line!">            result["workflow"] = "tags"</span>
+<span class="line-precise" title="No Anys on this line!">    return result</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">def update_version(</span>
+<span class="line-precise" title="No Anys on this line!">    initfile: str | Path, github_dump: str | None = None, abort: bool = True</span>
+<span class="line-empty" title="No Anys on this line!">) -&gt; str | None:</span>
+<span class="line-empty" title="No Anys on this line!">    """extracts version information from github_dump and updates initfile in-place</span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    Args:</span>
+<span class="line-empty" title="No Anys on this line!">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>
+<span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    Returns:</span>
+<span class="line-empty" title="No Anys on this line!">        str: the new version for the package</span>
+<span class="line-empty" title="No Anys on this line!">    """</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    data = get_data(initfile, github_dump, abort)</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">    set_module_var(initfile, "__version__", data["version"])</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x4)">    short = gdata["sha"] + ("*" if dirty else "")</span>
+Explicit (x3)">    set_module_var(initfile, "__hash__", data["hash"])</span>
+<span class="line-precise" title="No Anys on this line!">    return data["version"]</span>
 <span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">def process(</span>
+<span class="line-empty" title="No Anys on this line!">    initfile: str | Path,</span>
+<span class="line-precise" title="No Anys on this line!">    github_dump: str | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    paths: str | Path | list[str | Path] | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    fixers: dict[str, str] | None = None,</span>
+<span class="line-precise" title="No Anys on this line!">    abort: bool = True,</span>
+<span class="line-empty" title="No Anys on this line!">) -&gt; dict[str, str | None]:</span>
+<span class="line-empty" title="No Anys on this line!">    """get version from github_dump and updates initfile/paths</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    Args:</span>
+<span class="line-empty" title="No Anys on this line!">        paths (str, Path): path(s) to files jinja2 processeable</span>
+<span class="line-empty" title="No Anys on this line!">        initfile (str, Path): path to the __init__.py file with a __version__ variable</span>
+<span class="line-empty" title="No Anys on this line!">        github_dump (str): the os.getenv("GITHUB_DUMP") value</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    Returns:</span>
+<span class="line-empty" title="No Anys on this line!">        str: the new version for the package</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-empty" title="No Anys on this line!">    Example:</span>
+<span class="line-empty" title="No Anys on this line!">        {'branch': 'beta/0.3.1',</span>
+<span class="line-empty" title="No Anys on this line!">         'build': 0,</span>
+<span class="line-empty" title="No Anys on this line!">         'current': '0.3.1',</span>
+<span class="line-empty" title="No Anys on this line!">         'hash': 'c9e484a*',</span>
+<span class="line-empty" title="No Anys on this line!">         'version': '0.3.1b0',</span>
+<span class="line-empty" title="No Anys on this line!">         'runid': 0</span>
+<span class="line-empty" title="No Anys on this line!">        }</span>
+<span class="line-empty" title="No Anys on this line!">    """</span>
+<span class="line-precise" title="No Anys on this line!">    from argparse import Namespace</span>
+<span class="line-precise" title="No Anys on this line!">    from functools import partial</span>
+<span class="line-precise" title="No Anys on this line!">    from urllib.parse import quote</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    from jinja2 import Environment</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    class Context(Namespace):</span>
+<span class="line-any" title="No Anys on this line!">        def items(self):</span>
 <span class="line-any" title="Any Types on this line: 
-Explicit (x3)">    set_module_var(path, "__version__", version)</span>
+Unannotated (x5)">            for name, value in self.__dict__.items():</span>
 <span class="line-any" title="Any Types on this line: 
-Explicit (x3)
-Unannotated (x1)">    set_module_var(path, "__hash__", short)</span>
-<span class="line-precise" title="No Anys on this line!">    return version</span>
+Unannotated (x3)">                if name.startswith("_"):</span>
+<span class="line-any" title="No Anys on this line!">                    continue</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x2)">                yield (name, value)</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="No Anys on this line!">    data = get_data(initfile, github_dump, abort)</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">    set_module_var(initfile, "__version__", data["version"])</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">    set_module_var(initfile, "__hash__", data["hash"])</span>
+<span class="line-empty" title="No Anys on this line!"></span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x3)">    env = Environment(autoescape=True)</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x4)
+Explicit (x4)">    env.filters["urlquote"] = partial(quote, safe="")</span>
+<span class="line-precise" title="No Anys on this line!">    for path in list_of_paths(paths):</span>
+<span class="line-precise" title="No Anys on this line!">        txt = path.read_text()</span>
+<span class="line-precise" title="No Anys on this line!">        for old, new in (fixers or {}).items():</span>
+<span class="line-precise" title="No Anys on this line!">            txt = txt.replace(old, new, 1)</span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x1)">        tmpl = env.from_string(txt)</span>
+<span class="line-any" title="Any Types on this line: 
+Explicit (x3)">        path.write_text(tmpl.render(ctx=Context(**data)))</span>
+<span class="line-precise" title="No Anys on this line!">    return data</span>
 </pre></td>
 </tr></tbody>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,298 +1,409 @@
 
 ***** hatch_ci.tools *****
                              src/hatch_ci/tools.py
+    # see https://pypi.org/project/setuptools-github
+    # copy of setuptools_github.tools
     from __future__ import annotations
 
     import ast
     import json
     import re
     from pathlib import Path
     from typing import Any
-1
-2   from . import scm
+
+1   from . import scm
+2
 3
-4
-5   class ToolsError(Exception):
-6       pass
+4   class ToolsError(Exception):
+5       pass
+6
 7
-8
-9   class ValidationError(ToolsError):
-10      pass
+8   class ValidationError(ToolsError):
+9       pass
+10
 11
-12
-13  class InvalidVersionError(ToolsError):
-14      pass
+12  class InvalidVersionError(ToolsError):
+13      pass
+14
 15
-16
-17  class MissingVariableError(ToolsError):
-18      pass
+16  class MissingVariableError(ToolsError):
+17      pass
+18
 19
-20
-21  class AbortExecutionError(Exception):
-22      @staticmethod
-23      def _strip(txt):
-24          txt = txt or ""
-25          txt = txt[1:] if txt.startswith("\n") else txt
-26          txt = indent(txt, pre="")
-27          return txt[:-1] if txt.endswith("\n") else txt
-28
-29      def __init__(
-30          self, message: str, explain: str | None = None, hint: str | None =
-31  None
-32      ):
-33          self.message = message.strip()
-34          self._explain = explain
-35          self._hint = hint
-36
-37      @property
-38      def explain(self):
-39          return self._strip(self._explain)
-40
-41      @property
-42      def hint(self):
-43          return self._strip(self._hint)
-44
-45      def __str__(self):
-46          result = [self.message]
-47          if self.explain:
-48              result.append(indent("\n" + self.explain, pre=" " * 2)[2:])
-49          if self.hint:
-50              result.extend(["\nhint:", indent("\n" + self.hint, pre=" " * 2)
-51  [2:]])
-52          return "".join(result)
+20  class AbortExecutionError(Exception):
+21      @staticmethod
+22      def _strip(txt):
+23          txt = txt or ""
+24          txt = txt[1:] if txt.startswith("\n") else txt
+25          txt = indent(txt, pre="")
+26          return txt[:-1] if txt.endswith("\n") else txt
+27
+28      def __init__(
+29          self, message: str, explain: str | None = None, hint: str | None =
+30  None
+31      ):
+32          self.message = message.strip()
+33          self._explain = explain
+34          self._hint = hint
+35
+36      @property
+37      def explain(self):
+38          return self._strip(self._explain)
+39
+40      @property
+41      def hint(self):
+42          return self._strip(self._hint)
+43
+44      def __str__(self):
+45          result = [self.message]
+46          if self.explain:
+47              result.append(indent("\n" + self.explain, pre=" " * 2)[2:])
+48          if self.hint:
+49              result.extend(["\nhint:", indent("\n" + self.hint, pre=" " * 2)
+50  [2:]])
+51          return "".join(result)
+52
 53
-54
-55  def urmtree(path: Path):
-56      "universal (win|*nix) rmtree"
-57      from os import name
-58      from shutil import rmtree
-59      from stat import S_IWUSR
-60
-61      if name == "nt":
-62          for p in path.rglob("*"):
-63              p.chmod(S_IWUSR)
-64      rmtree(path, ignore_errors=True)
-65      if path.exists():
-66          raise RuntimeError(f"cannot remove {path=}")
+54  def urmtree(path: Path):
+55      "universal (win|*nix) rmtree"
+56      from os import name
+57      from shutil import rmtree
+58      from stat import S_IWUSR
+59
+60      if name == "nt":
+61          for p in path.rglob("*"):
+62              p.chmod(S_IWUSR)
+63      rmtree(path, ignore_errors=True)
+64      if path.exists():
+65          raise RuntimeError(f"cannot remove {path=}")
+66
 67
-68
-69  def indent(txt: str, pre: str = " " * 2) -> str:
-70      "simple text indentation"
-71
-72      from textwrap import dedent
-73
-74      txt = dedent(txt)
-75      if txt.endswith("\n"):
-76          last_eol = "\n"
-77          txt = txt[:-1]
-78      else:
-79          last_eol = ""
-80
-81      result = pre + txt.replace("\n", "\n" + pre) + last_eol
-82      return result if result.strip() else result.strip()
+68  def indent(txt: str, pre: str = " " * 2) -> str:
+69      "simple text indentation"
+70
+71      from textwrap import dedent
+72
+73      txt = dedent(txt)
+74      if txt.endswith("\n"):
+75          last_eol = "\n"
+76          txt = txt[:-1]
+77      else:
+78          last_eol = ""
+79
+80      result = pre + txt.replace("\n", "\n" + pre) + last_eol
+81      return result if result.strip() else result.strip()
+82
 83
-84
-85  def list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]:
-86      return [Path(s) for s in ([paths] if isinstance(paths, (str, Path))
-87  else paths)]
-88
-89
-90  def get_module_var(
-91      path: Path | str, var: str = "__version__", abort=True
-92  ) -> str | None:
-93      """extract from a python module in path the module level <var> variable
+84  def list_of_paths(paths: str | Path | list[str | Path] | None) -> list
+85  [Path]:
+86      if not paths:
+87          return []
+88      return [Path(s) for s in ([paths] if isinstance(paths, (str, Path))
+89  else paths)]
+90
+91
+92  def lstrip(txt: str, left: str) -> str:
+93      return txt[len(left) :] if txt.startswith(left) else txt
 94
-95      Args:
-96          path (str,Path): python module file to parse using ast (no code-
-97  execution)
-98          var (str): module level variable name to extract
-99          abort (bool): raise MissingVariable if var is not present
+95
+96  def get_module_var(
+97      path: Path | str, var: str = "__version__", abort=True
+98  ) -> str | None:
+99      """extract from a python module in path the module level <var> variable
 100
-101     Returns:
-102         None or str: the variable value if found or None
-103
-104     Raises:
-105         MissingVariable: if the var is not found and abort is True
+101     Args:
+102         path (str,Path): python module file to parse using ast (no code-
+103 execution)
+104         var (str): module level variable name to extract
+105         abort (bool): raise MissingVariable if var is not present
 106
-107     Notes:
-108         this uses ast to parse path, so it doesn't load the module
-109     """
-110
-111     class V(ast.NodeVisitor):
-112         def __init__(self, keys):
-113             self.keys = keys
-114             self.result = {}
-115
-116         def visit_Module(self, node):  # noqa: N802
-117             # we extract the module level variables
-118             for subnode in ast.iter_child_nodes(node):
-119                 if not isinstance(subnode, ast.Assign):
-120                     continue
-121                 for target in subnode.targets:
-122                     if target.id not in self.keys:
-123                         continue
-124                     if not isinstance(subnode.value, (ast.Num, ast.Str,
-125 ast.Constant)):
-126                         raise ValidationError(
-127                             f"cannot extract non Constant variable "
-128                             f"{target.id} ({type(subnode.value)})"
-129                         )
-130                     if isinstance(subnode.value, ast.Str):
-131                         value = subnode.value.s
-132                     elif isinstance(subnode.value, ast.Num):
-133                         value = subnode.value.n
-134                     else:
-135                         value = subnode.value.value
-136                     self.result[target.id] = value
-137             return self.generic_visit(node)
-138
-139     v = V({var})
-140     path = Path(path)
-141     if path.exists():
-142         tree = ast.parse(Path(path).read_text())
-143         v.visit(tree)
-144     if var not in v.result and abort:
-145         raise MissingVariableError(f"cannot find {var} in {path}", path,
-146 var)
-147     return v.result.get(var, None)
-148
-149
-150 def set_module_var(
-151     path: str | Path, var: str, value: Any, create: bool = True
-152 ) -> tuple[Any, str]:
-153     """replace var in path with value
-154
-155     Args:
-156         path (str,Path): python module file to parse
-157         var (str): module level variable name to extract
-158         value (None or Any): if not None replace var in initfile
-159         create (bool): create path if not present
-160
-161     Returns:
-162         (str, str) the (<previous-var-value|None>, <the new text>)
-163     """
-164     # module level var
-165     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
-166     fixed = None
-167     lines = []
-168
-169     src = Path(path)
-170     if not src.exists() and create:
-171         src.parent.mkdir(parents=True, exist_ok=True)
-172         src.touch()
+107     Returns:
+108         None or str: the variable value if found or None
+109
+110     Raises:
+111         MissingVariable: if the var is not found and abort is True
+112
+113     Notes:
+114         this uses ast to parse path, so it doesn't load the module
+115     """
+116
+117     class V(ast.NodeVisitor):
+118         def __init__(self, keys):
+119             self.keys = keys
+120             self.result = {}
+121
+122         def visit_Module(self, node):  # noqa: N802
+123             # we extract the module level variables
+124             for subnode in ast.iter_child_nodes(node):
+125                 if not isinstance(subnode, ast.Assign):
+126                     continue
+127                 for target in subnode.targets:
+128                     if target.id not in self.keys:
+129                         continue
+130                     if not isinstance(subnode.value, (ast.Num, ast.Str,
+131 ast.Constant)):
+132                         raise ValidationError(
+133                             f"cannot extract non Constant variable "
+134                             f"{target.id} ({type(subnode.value)})"
+135                         )
+136                     if isinstance(subnode.value, ast.Str):
+137                         value = subnode.value.s
+138                     elif isinstance(subnode.value, ast.Num):
+139                         value = subnode.value.n
+140                     else:
+141                         value = subnode.value.value
+142                     if target.id in self.result:
+143                         print(f">>> {path=}")  # noqa: T201
+144                         print(path.read_text())  # noqa: T201
+145                         raise ValidationError(
+146                             f"found multiple repeated variables
+147 {target.id}"
+148                         )
+149                     self.result[target.id] = value
+150             return self.generic_visit(node)
+151
+152     v = V({var})
+153     path = Path(path)
+154     if path.exists():
+155         tree = ast.parse(Path(path).read_text())
+156         v.visit(tree)
+157     if var not in v.result and abort:
+158         raise MissingVariableError(f"cannot find {var} in {path}", path,
+159 var)
+160     return v.result.get(var, None)
+161
+162
+163 def set_module_var(
+164     path: str | Path, var: str, value: Any, create: bool = True
+165 ) -> tuple[Any, str]:
+166     """replace var in path with value
+167
+168     Args:
+169         path (str,Path): python module file to parse
+170         var (str): module level variable name to extract
+171         value (None or Any): if not None replace var in initfile
+172         create (bool): create path if not present
 173
-174     input_lines = src.read_text().split("\n")
-175     for line in reversed(input_lines):
-176         if fixed:
-177             lines.append(line)
-178             continue
-179         match = expr.search(line)
-180         if match:
-181             fixed = match.group("value")
-182             if value is not None:
-183                 x, y = match.span(1)
-184                 line = line[:x] + value + line[y:]
-185         lines.append(line)
-186     txt = "\n".join(reversed(lines))
-187     if not fixed and create:
-188         if txt and txt[-1] != "\n":
-189             txt += "\n"
-190         txt += f'{var} = "{value}"'
-191
-192     with Path(path).open("w") as fp:
-193         fp.write(txt)
-194     return fixed, txt
-195
-196
-197 def bump_version(version: str, mode: str) -> str:
-198     """given a version str will bump it according to mode
-199
-200     Arguments:
-201         version: text in the N.M.O form
-202         mode: major, minor or micro
-203
-204     Returns:
-205         increased text
-206
-207     >>> bump_version("1.0.3", "micro")
-208     "1.0.4"
-209     >>> bump_version("1.0.3", "minor")
-210     "1.1.0"
-211     """
-212     newver = [int(n) for n in version.split(".")]
-213     if mode == "major":
-214         newver[-3] += 1
-215         newver[-2] = 0
-216         newver[-1] = 0
-217     elif mode == "minor":
-218         newver[-2] += 1
-219         newver[-1] = 0
-220     elif mode == "micro":
-221         newver[-1] += 1
-222     return ".".join(str(v) for v in newver)
+174     Returns:
+175         (str, str) the (<previous-var-value|None>, <the new text>)
+176     """
+177
+178     # validate the var
+179     get_module_var(path, var, abort=False)
+180
+181     # module level var
+182     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
+183     fixed = None
+184     lines = []
+185
+186     src = Path(path)
+187     if not src.exists() and create:
+188         src.parent.mkdir(parents=True, exist_ok=True)
+189         src.touch()
+190
+191     input_lines = src.read_text().split("\n")
+192     for line in input_lines:
+193         if fixed is not None:
+194             lines.append(line)
+195             continue
+196         match = expr.search(line)
+197         if match:
+198             fixed = match.group("value")
+199             if value is not None:
+200                 x, y = match.span(1)
+201                 line = line[:x] + value + line[y:]
+202         lines.append(line)
+203     txt = "\n".join(lines)
+204     if (fixed is None) and create:
+205         if txt and txt[-1] != "\n":
+206             txt += "\n"
+207         txt += f'{var} = "{value}"'
+208
+209     with Path(path).open("w") as fp:
+210         fp.write(txt)
+211     return fixed, txt
+212
+213
+214 def bump_version(version: str, mode: str) -> str:
+215     """given a version str will bump it according to mode
+216
+217     Arguments:
+218         version: text in the N.M.O form
+219         mode: major, minor or micro
+220
+221     Returns:
+222         increased text
 223
-224
-225 def update_version(
-226     initfile: str | Path, github_dump: str | None = None, abort: bool =
-227 True
-228 ) -> str | None:
-229     """extracts version information from github_dump and updates initfile
-230 in-place
-231
-232     Args:
-233         initfile (str, Path): path to the __init__.py file with a
-234 __version__ variable
-235         github_dump (str): the os.getenv("GITHUB_DUMP") value
-236
-237     Returns:
-238         str: the new version for the package
-239     """
+224     >>> bump_version("1.0.3", "micro")
+225     "1.0.4"
+226     >>> bump_version("1.0.3", "minor")
+227     "1.1.0"
+228     """
+229     newver = [int(n) for n in version.split(".")]
+230     if mode == "major":
+231         newver[-3] += 1
+232         newver[-2] = 0
+233         newver[-1] = 0
+234     elif mode == "minor":
+235         newver[-2] += 1
+236         newver[-1] = 0
+237     elif mode == "micro":
+238         newver[-1] += 1
+239     return ".".join(str(v) for v in newver)
 240
-241     path = Path(initfile)
-242     repo = scm.lookup(path)
-243
-244     if not (repo or github_dump):
-245         if abort:
-246             raise scm.InvalidGitRepoError(f"cannot find a valid git repo
-247 for {path}")
-248         return get_module_var(path, "__version__")
-249
-250     if not github_dump and repo:
-251         gdata = {
-252             "ref": repo.head.name,
-253             "sha": repo.head.target.hex[:7],
-254             "run_number": 0,
-255         }
-256         dirty = bool(repo.status())
-257     else:
-258         gdata = json.loads(github_dump) if isinstance(github_dump, str)
-259 else github_dump
-260         dirty = False
-261
-262     version = current = get_module_var(path, "__version__")
-263
-264     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+(
-265 [.]\d+)*)$")
-266     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
-267
-268     if match := expr.search(gdata["ref"]):
-269         # setuptools double calls the update_version,
-270         # this fixes the issue
-271         match1 = expr1.search(current or "")
-272         if not match1:
-273             raise InvalidVersionError(f"cannot parse current version '
-274 {current}'")
-275         if match1.group("version") != match.group("version"):
-276             raise InvalidVersionError(
-277                 f"building package for {current} from '{gdata['ref']}' "
-278                 f"branch ({match.groupdict()} mismatch {match1.groupdict
-279 ()})"
-280             )
-281         if match.group("what") == "beta":
-                version = f"{match1.group('version')}b{gdata['run_number']}"
-
-        short = gdata["sha"] + ("*" if dirty else "")
+241
+242 def get_data(
+243     initfile: str | Path, github_dump: str | None = None, abort: bool =
+244 True
+245 ) -> dict[str, str | None]:
+246     """extracts version information from github_dump and updates initfile
+247 in-place
+248
+249     Args:
+250         initfile (str, Path): path to the __init__.py file with a
+251 __version__ variable
+252         github_dump (str): the os.getenv("GITHUB_DUMP") value
+253
+254     Returns:
+255         dict[str,str|None]: a dict with the current config
+256     """
+257     result = {
+258         "version": get_module_var(initfile, "__version__"),
+259         "current": get_module_var(initfile, "__version__"),
+260         "branch": None,
+261         "hash": None,
+262         "build": None,
+263         "runid": None,
+264         "workflow": None,
+265     }
+266
+267     path = Path(initfile)
+268     repo = scm.lookup(path)
+269
+270     if not (repo or github_dump):
+271         if abort:
+272             raise scm.InvalidGitRepoError(f"cannot find a valid git repo
+273 for {path}")
+274         return result
+275
+276     if not github_dump and repo:
+277         gdata = {
+278             "ref": repo.head.name,
+279             "sha": repo.head.target.hex[:7],
+280             "run_number": 0,
+281             "run_id": 0,
+282         }
+283         dirty = repo.dirty()
+284     else:
+285         gdata = json.loads(github_dump) if isinstance(github_dump, str)
+286 else github_dump
+287         dirty = False
+288
+289     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+(
+290 [.]\d+)*)$")
+291     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
+292
+293     result["branch"] = lstrip(gdata["ref"], "refs/heads/")
+294     result["hash"] = gdata["sha"] + ("*" if dirty else "")
+295     result["build"] = gdata["run_number"]
+296     result["runid"] = gdata["run_id"]
+297     result["workflow"] = result["branch"]
+298
+299     current = result["current"]
+300     if match := expr.search(gdata["ref"]):
+301         # setuptools double calls the update_version,
+302         # this fixes the issue
+303         match1 = expr1.search(current or "")
+304         if not match1:
+305             raise InvalidVersionError(f"cannot parse current version '
+306 {current}'")
+307         if match1.group("version") != match.group("version"):
+308             raise InvalidVersionError(
+309                 f"building package for {current} from '{gdata['ref']}' "
+310                 f"branch ({match.groupdict()} mismatch {match1.groupdict
+311 ()})"
+312             )
+313         if match.group("what") == "beta":
+314             result["version"] = f"{match1.group('version')}b{gdata
+315 ['run_number']}"
+316             result["workflow"] = "beta"
+317         else:
+318             result["workflow"] = "tags"
+319     return result
+320
+321
+322 def update_version(
+323     initfile: str | Path, github_dump: str | None = None, abort: bool =
+324 True
+325 ) -> str | None:
+326     """extracts version information from github_dump and updates initfile
+327 in-place
+328
+329     Args:
+330         initfile (str, Path): path to the __init__.py file with a
+331 __version__ variable
+332         github_dump (str): the os.getenv("GITHUB_DUMP") value
+333
+334     Returns:
+335         str: the new version for the package
+336     """
+337
+338     data = get_data(initfile, github_dump, abort)
+339     set_module_var(initfile, "__version__", data["version"])
+340     set_module_var(initfile, "__hash__", data["hash"])
+341     return data["version"]
+342
+343
+344 def process(
+345     initfile: str | Path,
+346     github_dump: str | None = None,
+347     paths: str | Path | list[str | Path] | None = None,
+348     fixers: dict[str, str] | None = None,
+349     abort: bool = True,
+350 ) -> dict[str, str | None]:
+351     """get version from github_dump and updates initfile/paths
+352
+353     Args:
+354         paths (str, Path): path(s) to files jinja2 processeable
+355         initfile (str, Path): path to the __init__.py file with a
+356 __version__ variable
+357         github_dump (str): the os.getenv("GITHUB_DUMP") value
+358
+359     Returns:
+360         str: the new version for the package
+361
+362     Example:
+363         {'branch': 'beta/0.3.1',
+364          'build': 0,
+365          'current': '0.3.1',
+366          'hash': 'c9e484a*',
+367          'version': '0.3.1b0',
+368          'runid': 0
+369         }
+370     """
+371     from argparse import Namespace
+372     from functools import partial
+373     from urllib.parse import quote
+374
+375     from jinja2 import Environment
+376
+377     class Context(Namespace):
+378         def items(self):
+379             for name, value in self.__dict__.items():
+380                 if name.startswith("_"):
+381                     continue
+382                 yield (name, value)
+383
+384     data = get_data(initfile, github_dump, abort)
+385     set_module_var(initfile, "__version__", data["version"])
+        set_module_var(initfile, "__hash__", data["hash"])
 
-        set_module_var(path, "__version__", version)
-        set_module_var(path, "__hash__", short)
-        return version
+        env = Environment(autoescape=True)
+        env.filters["urlquote"] = partial(quote, safe="")
+        for path in list_of_paths(paths):
+            txt = path.read_text()
+            for old, new in (fixers or {}).items():
+                txt = txt.replace(old, new, 1)
+            tmpl = env.from_string(txt)
+            path.write_text(tmpl.render(ctx=Context(**data)))
+        return data
```

### Comparing `hatch_ci-0.0.3b13/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.3b23/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/src/hatch_ci/cli.py` & `hatch_ci-0.0.3b23/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/src/hatch_ci/scm.py` & `hatch_ci-0.0.3b23/src/hatch_ci/scm.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,17 @@
             value = mapper[tag]
             if value:
                 result[filename] = (
                     (result[filename] | value) if filename in result else value
                 )
         return result
 
+    def dirty(self) -> bool:
+        return bool(self.status(untracked_files="no"))
+
     def commit(
         self,
         paths: ListOfArgs,
         message: str,
     ) -> None:
         all_paths = to_list_of_paths(paths)
         self(["add", *all_paths])
```

### Comparing `hatch_ci-0.0.3b13/src/hatch_ci/script.py` & `hatch_ci-0.0.3b23/src/hatch_ci/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,19 +123,23 @@
                 f"git checkout beta/{version}",
             )
             return
         local = match.group("beta")
         if local != version:
             options.error(f"wrong version file {version=} != {local}")
 
+        # create an empty commit to mark the release
+        options.repo(["commit", "--allow-empty", "-m", f"released {version}"])
+
         # tag
         options.repo(["tag", "-a", f"release/{version}", "-m", f"released {version}"])
 
-        # switch to master
+        # switch to master (and incorporate the commit message)
         options.repo(["checkout", master])
+        options.repo(["merge", f"beta/{version}"])
 
         # bump version
         new_version = tools.bump_version(version, options.mode)
         tools.set_module_var(options.initfile, "__version__", new_version)
 
         # commit
         options.repo.commit(
```

### Comparing `hatch_ci-0.0.3b13/src/hatch_ci/tools.py` & `hatch_ci-0.0.3b23/src/hatch_ci/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# see https://pypi.org/project/setuptools-github
+# copy of setuptools_github.tools
 from __future__ import annotations
 
 import ast
 import json
 import re
 from pathlib import Path
 from typing import Any
@@ -83,18 +85,24 @@
     else:
         last_eol = ""
 
     result = pre + txt.replace("\n", "\n" + pre) + last_eol
     return result if result.strip() else result.strip()
 
 
-def list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]:
+def list_of_paths(paths: str | Path | list[str | Path] | None) -> list[Path]:
+    if not paths:
+        return []
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
+def lstrip(txt: str, left: str) -> str:
+    return txt[len(left) :] if txt.startswith(left) else txt
+
+
 def get_module_var(
     path: Path | str, var: str = "__version__", abort=True
 ) -> str | None:
     """extract from a python module in path the module level <var> variable
 
     Args:
         path (str,Path): python module file to parse using ast (no code-execution)
@@ -131,14 +139,20 @@
                         )
                     if isinstance(subnode.value, ast.Str):
                         value = subnode.value.s
                     elif isinstance(subnode.value, ast.Num):
                         value = subnode.value.n
                     else:
                         value = subnode.value.value
+                    if target.id in self.result:
+                        print(f">>> {path=}")  # noqa: T201
+                        print(path.read_text())  # noqa: T201
+                        raise ValidationError(
+                            f"found multiple repeated variables {target.id}"
+                        )
                     self.result[target.id] = value
             return self.generic_visit(node)
 
     v = V({var})
     path = Path(path)
     if path.exists():
         tree = ast.parse(Path(path).read_text())
@@ -158,38 +172,42 @@
         var (str): module level variable name to extract
         value (None or Any): if not None replace var in initfile
         create (bool): create path if not present
 
     Returns:
         (str, str) the (<previous-var-value|None>, <the new text>)
     """
+
+    # validate the var
+    get_module_var(path, var, abort=False)
+
     # module level var
     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
     fixed = None
     lines = []
 
     src = Path(path)
     if not src.exists() and create:
         src.parent.mkdir(parents=True, exist_ok=True)
         src.touch()
 
     input_lines = src.read_text().split("\n")
-    for line in reversed(input_lines):
-        if fixed:
+    for line in input_lines:
+        if fixed is not None:
             lines.append(line)
             continue
         match = expr.search(line)
         if match:
             fixed = match.group("value")
             if value is not None:
                 x, y = match.span(1)
                 line = line[:x] + value + line[y:]
         lines.append(line)
-    txt = "\n".join(reversed(lines))
-    if not fixed and create:
+    txt = "\n".join(lines)
+    if (fixed is None) and create:
         if txt and txt[-1] != "\n":
             txt += "\n"
         txt += f'{var} = "{value}"'
 
     with Path(path).open("w") as fp:
         fp.write(txt)
     return fixed, txt
@@ -219,63 +237,149 @@
         newver[-2] += 1
         newver[-1] = 0
     elif mode == "micro":
         newver[-1] += 1
     return ".".join(str(v) for v in newver)
 
 
-def update_version(
+def get_data(
     initfile: str | Path, github_dump: str | None = None, abort: bool = True
-) -> str | None:
+) -> dict[str, str | None]:
     """extracts version information from github_dump and updates initfile in-place
 
     Args:
         initfile (str, Path): path to the __init__.py file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
-        str: the new version for the package
+        dict[str,str|None]: a dict with the current config
     """
+    result = {
+        "version": get_module_var(initfile, "__version__"),
+        "current": get_module_var(initfile, "__version__"),
+        "branch": None,
+        "hash": None,
+        "build": None,
+        "runid": None,
+        "workflow": None,
+    }
 
     path = Path(initfile)
     repo = scm.lookup(path)
 
     if not (repo or github_dump):
         if abort:
             raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")
-        return get_module_var(path, "__version__")
+        return result
 
     if not github_dump and repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
+            "run_id": 0,
         }
-        dirty = bool(repo.status())
+        dirty = repo.dirty()
     else:
         gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
         dirty = False
 
-    version = current = get_module_var(path, "__version__")
-
     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$")
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
+    result["branch"] = lstrip(gdata["ref"], "refs/heads/")
+    result["hash"] = gdata["sha"] + ("*" if dirty else "")
+    result["build"] = gdata["run_number"]
+    result["runid"] = gdata["run_id"]
+    result["workflow"] = result["branch"]
+
+    current = result["current"]
     if match := expr.search(gdata["ref"]):
         # setuptools double calls the update_version,
         # this fixes the issue
         match1 = expr1.search(current or "")
         if not match1:
             raise InvalidVersionError(f"cannot parse current version '{current}'")
         if match1.group("version") != match.group("version"):
             raise InvalidVersionError(
                 f"building package for {current} from '{gdata['ref']}' "
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
             )
         if match.group("what") == "beta":
-            version = f"{match1.group('version')}b{gdata['run_number']}"
+            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"
+            result["workflow"] = "beta"
+        else:
+            result["workflow"] = "tags"
+    return result
+
+
+def update_version(
+    initfile: str | Path, github_dump: str | None = None, abort: bool = True
+) -> str | None:
+    """extracts version information from github_dump and updates initfile in-place
+
+    Args:
+        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        github_dump (str): the os.getenv("GITHUB_DUMP") value
+
+    Returns:
+        str: the new version for the package
+    """
+
+    data = get_data(initfile, github_dump, abort)
+    set_module_var(initfile, "__version__", data["version"])
+    set_module_var(initfile, "__hash__", data["hash"])
+    return data["version"]
+
 
-    short = gdata["sha"] + ("*" if dirty else "")
+def process(
+    initfile: str | Path,
+    github_dump: str | None = None,
+    paths: str | Path | list[str | Path] | None = None,
+    fixers: dict[str, str] | None = None,
+    abort: bool = True,
+) -> dict[str, str | None]:
+    """get version from github_dump and updates initfile/paths
+
+    Args:
+        paths (str, Path): path(s) to files jinja2 processeable
+        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        github_dump (str): the os.getenv("GITHUB_DUMP") value
+
+    Returns:
+        str: the new version for the package
+
+    Example:
+        {'branch': 'beta/0.3.1',
+         'build': 0,
+         'current': '0.3.1',
+         'hash': 'c9e484a*',
+         'version': '0.3.1b0',
+         'runid': 0
+        }
+    """
+    from argparse import Namespace
+    from functools import partial
+    from urllib.parse import quote
+
+    from jinja2 import Environment
+
+    class Context(Namespace):
+        def items(self):
+            for name, value in self.__dict__.items():
+                if name.startswith("_"):
+                    continue
+                yield (name, value)
 
-    set_module_var(path, "__version__", version)
-    set_module_var(path, "__hash__", short)
-    return version
+    data = get_data(initfile, github_dump, abort)
+    set_module_var(initfile, "__version__", data["version"])
+    set_module_var(initfile, "__hash__", data["hash"])
+
+    env = Environment(autoescape=True)
+    env.filters["urlquote"] = partial(quote, safe="")
+    for path in list_of_paths(paths):
+        txt = path.read_text()
+        for old, new in (fixers or {}).items():
+            txt = txt.replace(old, new, 1)
+        tmpl = env.from_string(txt)
+        path.write_text(tmpl.render(ctx=Context(**data)))
+    return data
```

### Comparing `hatch_ci-0.0.3b13/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.3b23/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/tests/conftest.py` & `hatch_ci-0.0.3b23/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
+import collections
+import contextlib
 import os
-import sys
 import pathlib
 import shutil
-import contextlib
-import collections
 import subprocess
+import sys
 
 import pytest
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent.parent / "src"))
 from hatch_ci import scm  # noqa F401,E402
 
 
@@ -58,15 +58,15 @@
         def run(self, args, cwd=None, load_data=True):
             cmd = [str(a) for a in [self.exe, self.script, *args]]
 
             with contextlib.ExitStack() as stack:
                 fpout = stack.enter_context((self.workdir / "stdout.txt").open("w"))
                 fperr = stack.enter_context((self.workdir / "stderr.txt").open("w"))
                 self.p = subprocess.Popen(
-                    cmd,
+                    cmd,  # noqa: S603
                     cwd=self.workdir if cwd is True else cwd,
                     stdout=fpout,
                     stderr=fperr,
                 )
                 self.p.communicate()
             out = (self.workdir / "stdout.txt").read_text()
             err = (self.workdir / "stderr.txt").read_text()
@@ -115,30 +115,31 @@
         # clone from repo
         repo2 = git_project_factory().create(clone=repo)
 
         assert repo.workdir != repo1.workdir
         assert repo.workdir != repo1.workdir
 
     """
+
     class GitRepoBase(scm.GitRepo):
-        def init(
-            self,
-            force: bool = False,
-            nobranch: bool = False
-        ) -> GitRepoBase:
+        def init(self, force: bool = False, nobranch: bool = False) -> GitRepoBase:
             from shutil import rmtree
 
             if force:
                 rmtree(self.workdir, ignore_errors=True)
             self.workdir.mkdir(parents=True, exist_ok=True if force else False)
 
             if not nobranch:
                 self(["init", "-b", "master"])
             else:
-                self(["init",])
+                self(
+                    [
+                        "init",
+                    ]
+                )
 
             self(["config", "user.name", "First Last"])
             self(["config", "user.email", "user@email"])
 
             if not nobranch:
                 self(["commit", "-m", "initial", "--allow-empty"])
             return self
@@ -172,22 +173,25 @@
                 clone.clone(self.workdir, force=force)
             else:
                 self.init(force=force, nobranch=nobranch)
             self.version(version)
             return self
 
     def id_generator(size=6):
-        from string import ascii_uppercase, digits
         from random import choice
+        from string import ascii_uppercase, digits
 
-        return "".join(choice(ascii_uppercase + digits) for _ in range(size))
+        return "".join(
+            choice(ascii_uppercase + digits) for _ in range(size)  # noqa: S311
+        )
 
     return lambda subdir="": Project(tmp_path / (subdir or id_generator()))
     # or request.node.name
 
+
 #####################
 # Main flags/config #
 #####################
 
 
 def pytest_configure(config):
     config.addinivalue_line("markers", "manual: test intented to run manually")
@@ -197,8 +201,7 @@
     if config.option.keyword or config.option.markexpr:
         return  # let pytest handle this
 
     for item in items:
         if "manual" not in item.keywords:
             continue
         item.add_marker(pytest.mark.skip(reason="manual not selected"))
-
```

### Comparing `hatch_ci-0.0.3b13/tests/test_scm.py` & `hatch_ci-0.0.3b23/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/tests/test_tools.py` & `hatch_ci-0.0.3b23/tests/test_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 
 # this is the output from ${{ toJson(github) }}
 GITHUB = {
     "beta": {
         "ref": "refs/heads/beta/0.0.4",
         "sha": "2169f90c22e",
         "run_number": "8",
+        "run_id": 123,
     },
     "release": {
         "ref": "refs/tags/release/0.0.3",
         "sha": "5547365c82",
         "run_number": "3",
+        "run_id": 456,
     },
     "master": {
         "ref": "refs/heads/master",
         "sha": "2169f90c",
         "run_number": "20",
+        "run_id": 789,
     },
 }
 
 
 def T(txt):  # noqa: N802
     from textwrap import dedent
 
@@ -125,14 +128,18 @@
     assert tools.list_of_paths("hello") == [Path("hello")]
     assert tools.list_of_paths(["hello", Path("world")]) == [
         Path("hello"),
         Path("world"),
     ]
 
 
+def test_lstrip():
+    assert tools.lstrip("/a/b/c/d/e", "/a/b") == "/c/d/e"
+
+
 def test_get_module_var(tmp_path):
     "pulls variables from a file"
     path = tmp_path / "in0.txt"
     path.write_text(
         """
 # a test file
 A = 12
@@ -142,29 +149,53 @@
 """
     )
     assert 12 == tools.get_module_var(path, "A")
     assert "hello" == tools.get_module_var(path, "C")
     pytest.raises(tools.ValidationError, tools.get_module_var, path, "B")
     pytest.raises(tools.MissingVariableError, tools.get_module_var, path, "X1")
 
+    path.write_text(
+        """
+# a test file
+A = 12
+B = 3+5
+C = "hello"
+C = "hello2"
+# end of test
+"""
+    )
+    pytest.raises(tools.ValidationError, tools.get_module_var, path, "C")
+
 
 def test_set_module_var(tmp_path):
     "handles set_module_var cases"
     path = tmp_path / "in2.txt"
 
     path.write_text(
         """
 # a fist comment line
 __hash__ = "4.5.6"
 # end of test
 """
     )
 
+    version, txt = tools.set_module_var(path, "__version__", "")
+    assert version is None
+    assert (
+        txt.rstrip()
+        == """
+# a fist comment line
+__hash__ = "4.5.6"
+# end of test
+__version__ = ""
+""".rstrip()
+    )
+
     version, txt = tools.set_module_var(path, "__version__", "1.2.3")
-    assert not version
+    assert version == ""
     assert (
         txt.rstrip()
         == """
 # a fist comment line
 __hash__ = "4.5.6"
 # end of test
 __version__ = "1.2.3"
@@ -191,14 +222,26 @@
 # a fist comment line
 __hash__ = "9.10.11"
 # end of test
 __version__ = "6.7.8"
 """.rstrip()
     )
 
+    version, txt = tools.set_module_var(path, "__version__", "9.10.11")
+    assert version == "6.7.8"
+    assert (
+        txt.rstrip()
+        == """
+# a fist comment line
+__hash__ = "9.10.11"
+# end of test
+__version__ = "9.10.11"
+""".rstrip()
+    )
+
 
 def test_set_module_var_empty_file(tmp_path):
     "check if the set_module_var will create a bew file"
     path = tmp_path / "in1.txt"
 
     assert not path.exists()
     tools.set_module_var(path, "__version__", "1.2.3")
@@ -304,7 +347,54 @@
 
     assert (
         tools.update_version(repo.initfile, GITHUB["release"], abort=False) == "0.0.3"
     )
     assert tools.get_module_var(repo.initfile) == "0.0.3"
     assert tools.get_module_var(repo.initfile, "__hash__") == "5547365c82"
     repo.revert(repo.initfile)
+
+
+def test_process(git_project_factory):
+    def write_tfile(tfile):
+        tfile.write_text("""
+{% for k, v in ctx.items() | sort -%}
+Key[{{k}}] = {{v}}
+{% endfor %}
+""")
+        return tfile
+
+    repo = git_project_factory().create("1.2.3")
+
+    # tfile won't appear in the repo.status() because is untracked
+    tfile = write_tfile(repo.workdir / "test.txt")
+
+    data = tools.process(repo.initfile, None, tfile)
+
+    assert data["hash"][-1] != "*"
+
+    assert tfile.read_text() == f"""
+Key[branch] = master
+Key[build] = 0
+Key[current] = 1.2.3
+Key[hash] = {data['hash']}
+Key[runid] = 0
+Key[version] = 1.2.3
+Key[workflow] = master
+"""
+
+    # clean and switch to new branch
+    repo.revert(repo.initfile)
+    write_tfile(tfile)
+    repo.branch("beta/1.2.3", "master")
+
+    data = tools.process(repo.initfile, None, tfile)
+    assert data["hash"][-1] != "*"
+
+    assert tfile.read_text() == f"""
+Key[branch] = beta/1.2.3
+Key[build] = 0
+Key[current] = 1.2.3
+Key[hash] = {data['hash']}
+Key[runid] = 0
+Key[version] = 1.2.3b0
+Key[workflow] = beta
+"""
```

### Comparing `hatch_ci-0.0.3b13/LICENSE.txt` & `hatch_ci-0.0.3b23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.3b13/README.md` & `hatch_ci-0.0.3b23/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions)
-[![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](Coverage)
-
-[![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
------
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/workflows/master.yml)
+[![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](https://app.codecov.io/gh/cav71/hatch-ci/tree/master)
+
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
+[![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 
 This provides a plugin to [Hatch](https://github.com/pypa/hatch) leveraging a CI/CD system (github at the moment)
 to deliver packages to [PyPi](https://pypi.org).
 
 > **NOTE**: this is heavily inspired from  [hatch-vcs](https://github.com/ofek/hatch-vcs)
```

### Comparing `hatch_ci-0.0.3b13/pyproject.toml` & `hatch_ci-0.0.3b23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.1.0", "hatch-ci", "typing-extensions"]
+requires = ["hatchling>=1.1.0", "typing-extensions", "hatch-ci"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-ci"
 dynamic = ["version"]
 description = "Hatch plugin for ci system versioning"
 readme = "README.md"
```

### Comparing `hatch_ci-0.0.3b13/PKG-INFO` & `hatch_ci-0.0.3b23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.3b13
+Version: 0.0.3b23
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
@@ -21,21 +21,23 @@
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions)
-[![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](Coverage)
-
-[![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
------
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/workflows/master.yml)
+[![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](https://app.codecov.io/gh/cav71/hatch-ci/tree/master)
+
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
+[![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 
 This provides a plugin to [Hatch](https://github.com/pypa/hatch) leveraging a CI/CD system (github at the moment)
 to deliver packages to [PyPi](https://pypi.org).
 
 > **NOTE**: this is heavily inspired from  [hatch-vcs](https://github.com/ofek/hatch-vcs)
```

