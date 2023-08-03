# Comparing `tmp/junifer-0.0.4.dev15.tar.gz` & `tmp/junifer-0.0.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.4.dev15.tar", last modified: Thu Aug  3 10:23:22 2023, max compression
+gzip compressed data, was "junifer-0.0.4.dev8.tar", last modified: Mon Jul 24 13:44:20 2023, max compression
```

## Comparing `junifer-0.0.4.dev15.tar` & `junifer-0.0.4.dev8.tar`

### file list

```diff
@@ -1,376 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.069723 junifer-0.0.4.dev15/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.069723 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.069723 junifer-0.0.4.dev15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34354 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.057722 junifer-0.0.4.dev15/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.073724 junifer-0.0.4.dev15/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/changes/newsfragments/233.bugfix
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/changes/newsfragments/247.doc
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/changes/newsfragments/248.change
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.077724 junifer-0.0.4.dev15/docs/using/
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.081724 junifer-0.0.4.dev15/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.081724 junifer-0.0.4.dev15/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.081724 junifer-0.0.4.dev15/junifer/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24632 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.085724 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.089725 junifer-0.0.4.dev15/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.061723 junifer-0.0.4.dev15/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.089725 junifer-0.0.4.dev15/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.061723 junifer-0.0.4.dev15/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.089725 junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    48818 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.089725 junifer-0.0.4.dev15/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/datalad_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.093725 junifer-0.0.4.dev15/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.065723 junifer-0.0.4.dev15/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16142 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.097725 junifer-0.0.4.dev15/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.101726 junifer-0.0.4.dev15/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.101726 junifer-0.0.4.dev15/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.101726 junifer-0.0.4.dev15/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.105726 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.105726 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.105726 junifer-0.0.4.dev15/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.105726 junifer-0.0.4.dev15/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.109727 junifer-0.0.4.dev15/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.113727 junifer-0.0.4.dev15/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.113727 junifer-0.0.4.dev15/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21922 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.113727 junifer-0.0.4.dev15/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.113727 junifer-0.0.4.dev15/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.113727 junifer-0.0.4.dev15/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35520 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.117727 junifer-0.0.4.dev15/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29337 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28318 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.117727 junifer-0.0.4.dev15/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.117727 junifer-0.0.4.dev15/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.117727 junifer-0.0.4.dev15/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.117727 junifer-0.0.4.dev15/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.081724 junifer-0.0.4.dev15/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-08-03 10:23:22.000000 junifer-0.0.4.dev15/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 10:23:21.000000 junifer-0.0.4.dev15/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:22.121728 junifer-0.0.4.dev15/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-03 10:22:51.000000 junifer-0.0.4.dev15/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34354 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.053328 junifer-0.0.4.dev8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.061328 junifer-0.0.4.dev8/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/changes/newsfragments/247.doc
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.065328 junifer-0.0.4.dev8/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/junifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24632 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.073328 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.077328 junifer-0.0.4.dev8/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.053328 junifer-0.0.4.dev8/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.077328 junifer-0.0.4.dev8/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.053328 junifer-0.0.4.dev8/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.077328 junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48818 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.077328 junifer-0.0.4.dev8/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.077328 junifer-0.0.4.dev8/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/datalad_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.057328 junifer-0.0.4.dev8/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-24 13:44:07.000000 junifer-0.0.4.dev8/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-07-24 13:44:07.000000 junifer-0.0.4.dev8/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 13:44:07.000000 junifer-0.0.4.dev8/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-24 13:44:07.000000 junifer-0.0.4.dev8/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-24 13:44:07.000000 junifer-0.0.4.dev8/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16142 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.081328 junifer-0.0.4.dev8/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.085328 junifer-0.0.4.dev8/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.085328 junifer-0.0.4.dev8/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.085328 junifer-0.0.4.dev8/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.085328 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.085328 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.089328 junifer-0.0.4.dev8/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21922 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35520 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29337 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28318 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.093329 junifer-0.0.4.dev8/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.069328 junifer-0.0.4.dev8/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-24 13:44:20.000000 junifer-0.0.4.dev8/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 13:44:19.000000 junifer-0.0.4.dev8/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:20.097329 junifer-0.0.4.dev8/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-24 13:44:06.000000 junifer-0.0.4.dev8/tox.ini
```

### Comparing `junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.4.dev8/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/workflows/ci-docs.yml` & `junifer-0.0.4.dev8/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/workflows/ci.yml` & `junifer-0.0.4.dev8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/workflows/docs-preview.yml` & `junifer-0.0.4.dev8/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/workflows/docs.yml` & `junifer-0.0.4.dev8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.github/workflows/pypi.yml` & `junifer-0.0.4.dev8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.gitignore` & `junifer-0.0.4.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/.pre-commit-config.yaml` & `junifer-0.0.4.dev8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/LICENSE.md` & `junifer-0.0.4.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/PKG-INFO` & `junifer-0.0.4.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev15
+Version: 0.0.4.dev8
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.4.dev15/README.md` & `junifer-0.0.4.dev8/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/codecov.yml` & `junifer-0.0.4.dev8/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/conda-env.yml` & `junifer-0.0.4.dev8/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/Makefile` & `junifer-0.0.4.dev8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/_static/css/custom.css` & `junifer-0.0.4.dev8/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/_templates/versions.html` & `junifer-0.0.4.dev8/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/builtin.rst` & `junifer-0.0.4.dev8/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/changes/contributors.inc` & `junifer-0.0.4.dev8/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/conf.py` & `junifer-0.0.4.dev8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/contribution.rst` & `junifer-0.0.4.dev8/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/coordinates.rst` & `junifer-0.0.4.dev8/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/datagrabber.rst` & `junifer-0.0.4.dev8/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/extension.rst` & `junifer-0.0.4.dev8/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/index.rst` & `junifer-0.0.4.dev8/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/marker.rst` & `junifer-0.0.4.dev8/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/masks.rst` & `junifer-0.0.4.dev8/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/extending/parcellations.rst` & `junifer-0.0.4.dev8/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/faq.rst` & `junifer-0.0.4.dev8/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/help.rst` & `junifer-0.0.4.dev8/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/images/junifer_logo.png` & `junifer-0.0.4.dev8/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/index.rst` & `junifer-0.0.4.dev8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/installation.rst` & `junifer-0.0.4.dev8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/links.inc` & `junifer-0.0.4.dev8/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/maintaining.rst` & `junifer-0.0.4.dev8/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.4.dev8/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/starting.rst` & `junifer-0.0.4.dev8/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/data.rst` & `junifer-0.0.4.dev8/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/datagrabber.rst` & `junifer-0.0.4.dev8/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/datareader.rst` & `junifer-0.0.4.dev8/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/index.rst` & `junifer-0.0.4.dev8/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/marker.rst` & `junifer-0.0.4.dev8/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/pipeline.rst` & `junifer-0.0.4.dev8/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/preprocess.rst` & `junifer-0.0.4.dev8/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/understanding/storage.rst` & `junifer-0.0.4.dev8/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/using/codeless.rst` & `junifer-0.0.4.dev8/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/using/index.rst` & `junifer-0.0.4.dev8/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/using/masks.rst` & `junifer-0.0.4.dev8/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/using/queueing.rst` & `junifer-0.0.4.dev8/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/using/running.rst` & `junifer-0.0.4.dev8/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/docs/whats_new.rst` & `junifer-0.0.4.dev8/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/norun_hcpfc_pearson.py` & `junifer-0.0.4.dev8/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/norun_ukbvm_gmd.py` & `junifer-0.0.4.dev8/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/run_compute_parcel_mean.py` & `junifer-0.0.4.dev8/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.4.dev8/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/run_ets_rss_marker.py` & `junifer-0.0.4.dev8/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/run_junifer_julearn.py` & `junifer-0.0.4.dev8/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/run_run_gmd_mean.py` & `junifer-0.0.4.dev8/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/yamls/gmd_mean.yaml` & `junifer-0.0.4.dev8/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.4.dev8/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/cli.py` & `junifer-0.0.4.dev8/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/decorators.py` & `junifer-0.0.4.dev8/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/functions.py` & `junifer-0.0.4.dev8/junifer/api/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,20 +528,18 @@
             for i_job, _ in enumerate(elements):
                 dag_file.write(f"run{i_job} ")
             dag_file.write("CHILD collect\n\n")
 
     # Submit job(s)
     if submit is True:
         logger.info("Submitting HTCondor job")
-        subprocess.run(
-            ["condor_submit_dag", "-include_env", "HOME", dag_fname]
-        )
+        subprocess.run(["condor_submit_dag", dag_fname])
         logger.info("HTCondor job submitted")
     else:
-        cmd = f"condor_submit_dag -include_env 'HOME' {dag_fname.absolute()!s}"
+        cmd = f"condor_submit_dag {dag_fname.absolute()!s}"
         logger.info(
             f"HTCondor job files created, to submit the job, run `{cmd}`"
         )
 
 
 def _queue_slurm(
     jobname: str,
```

### Comparing `junifer-0.0.4.dev15/junifer/api/parser.py` & `junifer-0.0.4.dev8/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.4.dev8/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/tests/test_api_utils.py` & `junifer-0.0.4.dev8/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/tests/test_cli.py` & `junifer-0.0.4.dev8/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/tests/test_functions.py` & `junifer-0.0.4.dev8/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/tests/test_parser.py` & `junifer-0.0.4.dev8/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/api/utils.py` & `junifer-0.0.4.dev8/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.4.dev8/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.4.dev8/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.4.dev8/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.4.dev8/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.4.dev8/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/coordinates.py` & `junifer-0.0.4.dev8/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.4.dev8/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/masks.py` & `junifer-0.0.4.dev8/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/parcellations.py` & `junifer-0.0.4.dev8/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/tests/test_coordinates.py` & `junifer-0.0.4.dev8/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/tests/test_data_utils.py` & `junifer-0.0.4.dev8/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/tests/test_masks.py` & `junifer-0.0.4.dev8/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/tests/test_parcellations.py` & `junifer-0.0.4.dev8/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/data/utils.py` & `junifer-0.0.4.dev8/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/__init__.py` & `junifer-0.0.4.dev8/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.4.dev8/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/base.py` & `junifer-0.0.4.dev8/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/datalad_base.py` & `junifer-0.0.4.dev8/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.4.dev8/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/multiple.py` & `junifer-0.0.4.dev8/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/pattern.py` & `junifer-0.0.4.dev8/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.4.dev8/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.4.dev8/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datagrabber/utils.py` & `junifer-0.0.4.dev8/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datareader/default.py` & `junifer-0.0.4.dev8/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.4.dev8/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.4.dev8/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.4.dev8/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.4.dev8/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.4.dev8/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.4.dev8/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/__init__.py` & `junifer-0.0.4.dev8/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/base.py` & `junifer-0.0.4.dev8/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/collection.py` & `junifer-0.0.4.dev8/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/ets_rss.py` & `junifer-0.0.4.dev8/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/falff_base.py` & `junifer-0.0.4.dev8/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.4.dev8/junifer/markers/falff/falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/parcel_aggregation.py` & `junifer-0.0.4.dev8/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/reho_base.py` & `junifer-0.0.4.dev8/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.4.dev8/junifer/markers/reho/reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/sphere_aggregation.py` & `junifer-0.0.4.dev8/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.4.dev8/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_collection.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.4.dev8/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/markers/utils.py` & `junifer-0.0.4.dev8/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/onthefly/read_transform.py` & `junifer-0.0.4.dev8/junifer/onthefly/read_transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,30 @@
 
 if TYPE_CHECKING:
     from junifer.storage import BaseFeatureStorage
 
 
 def read_transform(
     storage: Type["BaseFeatureStorage"],
+    feature_name: str,
     transform: str,
-    feature_name: Optional[str] = None,
-    feature_md5: Optional[str] = None,
     transform_args: Optional[Tuple] = None,
     transform_kw_args: Optional[Dict] = None,
 ) -> pd.DataFrame:
     """Read stored feature and transform to specific statistical output.
 
     Parameters
     ----------
     storage : storage-like
         The storage class, for example, SQLiteFeatureStorage.
+    feature_name : str
+        Name of the feature to read.
     transform : str
         The kind of transform formatted as ``<package>_<function>``,
         for example, ``bctpy_degrees_und``.
-    feature_name : str, optional
-        Name of the feature to read (default None).
-    feature_md5 : str, optional
-        MD5 hash of the feature to read (default None).
     transform_args : tuple, optional
         The positional arguments for the callable of ``transform``
         (default None).
     transform_kw_args : dict, optional
         The keyword arguments for the callable of ``transform``
         (default None).
 
@@ -61,17 +58,15 @@
 
     """
     # Set default values for args and kwargs
     transform_args = transform_args or ()
     transform_kw_args = transform_kw_args or {}
 
     # Read storage
-    stored_data = storage.read(
-        feature_name=feature_name, feature_md5=feature_md5
-    )  # type: ignore
+    stored_data = storage.read(feature_name=feature_name)  # type: ignore
     # Retrieve package and function
     package, func_str = transform.split("_", 1)
     # Condition for package
     if package == "bctpy":
         # Check that "matrix" is the feature data kind
         if stored_data["kind"] != "matrix":
             raise_error(
@@ -106,31 +101,29 @@
             func = getattr(bct, func_str)
         except AttributeError as err:
             raise_error(msg=str(err), klass=AttributeError)
 
         # Apply function and store subject-wise
         output_list = []
         logger.debug(
-            f"Computing '{package}.{func_str}' for feature "
-            f"{feature_name or feature_md5} ..."
+            f"Computing '{package}.{func_str}' for feature {feature_name} ..."
         )
         for subject in range(stored_data["data"].shape[2]):
             output = func(
                 stored_data["data"][:, :, subject],
                 *transform_args,
                 **transform_kw_args,
             )
             output_list.append(output)
 
         # Create dataframe for index
         idx_df = pd.DataFrame(data=stored_data["element"])
         # Create multiindex from dataframe
         logger.debug(
-            "Generating pandas.MultiIndex for feature "
-            f"{feature_name or feature_md5} ..."
+            f"Generating pandas.MultiIndex for feature {feature_name} ..."
         )
         data_idx = pd.MultiIndex.from_frame(df=idx_df)
 
         # Create dataframe
         df = pd.DataFrame(
             data=output_list,
             index=data_idx,
```

### Comparing `junifer-0.0.4.dev15/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.4.dev8/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.4.dev8/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/registry.py` & `junifer-0.0.4.dev8/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.4.dev8/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.4.dev8/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.4.dev8/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.4.dev8/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/pipeline/utils.py` & `junifer-0.0.4.dev8/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/preprocess/base.py` & `junifer-0.0.4.dev8/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.4.dev8/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.4.dev8/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.4.dev8/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/stats.py` & `junifer-0.0.4.dev8/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/base.py` & `junifer-0.0.4.dev8/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/hdf5.py` & `junifer-0.0.4.dev8/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/pandas_base.py` & `junifer-0.0.4.dev8/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/sqlite.py` & `junifer-0.0.4.dev8/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.4.dev8/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.4.dev8/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.4.dev8/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.4.dev8/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/tests/test_utils.py` & `junifer-0.0.4.dev8/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/storage/utils.py` & `junifer-0.0.4.dev8/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.4.dev8/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/datagrabbers.py` & `junifer-0.0.4.dev8/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/registry.py` & `junifer-0.0.4.dev8/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.4.dev8/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.4.dev8/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.4.dev8/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.4.dev8/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/testing/utils.py` & `junifer-0.0.4.dev8/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/tests/test_stats.py` & `junifer-0.0.4.dev8/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/utils/logging.py` & `junifer-0.0.4.dev8/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/utils/tests/test_fs.py` & `junifer-0.0.4.dev8/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer/utils/tests/test_logging.py` & `junifer-0.0.4.dev8/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/junifer.egg-info/PKG-INFO` & `junifer-0.0.4.dev8/junifer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev15
+Version: 0.0.4.dev8
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.4.dev15/junifer.egg-info/SOURCES.txt` & `junifer-0.0.4.dev8/junifer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 docs/api/preprocessing.rst
 docs/api/stats.rst
 docs/api/storage.rst
 docs/api/testing.rst
 docs/api/utils.rst
 docs/changes/contributors.inc
 docs/changes/newsfragments/.gitignore
-docs/changes/newsfragments/233.bugfix
 docs/changes/newsfragments/247.doc
-docs/changes/newsfragments/248.change
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
 docs/extending/parcellations.rst
```

### Comparing `junifer-0.0.4.dev15/pyproject.toml` & `junifer-0.0.4.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.4.dev8/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.4.dev8/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.4.dev8/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_bids_example_dataset.py` & `junifer-0.0.4.dev8/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.4.dev8/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.4.dev8/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev15/tox.ini` & `junifer-0.0.4.dev8/tox.ini`

 * *Files identical despite different names*

