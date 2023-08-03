# Comparing `tmp/ixbrl-viewer-1.3.0.tar.gz` & `tmp/ixbrl-viewer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-viewer-1.3.0.tar", last modified: Thu Jul 27 19:45:32 2023, max compression
+gzip compressed data, was "ixbrl-viewer-1.4.0.tar", last modified: Thu Aug  3 00:07:09 2023, max compression
```

## Comparing `ixbrl-viewer-1.3.0.tar` & `ixbrl-viewer-1.4.0.tar`

### file list

```diff
@@ -1,237 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.babelrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.204800 ixbrl-viewer-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.204800 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/questions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.208800 ixbrl-viewer-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/node-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/npm-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/puppeteer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.208800 ixbrl-viewer-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.216801 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
--rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
--rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
--rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
--rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.224801 ixbrl-viewer-1.3.0/examples/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/example-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/extended-viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/ixbrl-viewer-demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/review-mode.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.224801 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 19:45:31.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25873 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/stubviewer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   859288 2023-07-27 19:45:12.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-27 19:45:12.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/i18next-parser.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/inspector.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.232801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.236801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/accordian.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.js
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/calculations.js
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.js
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/dialog.js
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.js
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.js
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/footnote.js
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    44285 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.js
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.js
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.js
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/qname.js
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.js
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.js
--rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.js
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/test-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.js
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.js
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js
--rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/accordian.less
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/block-list.less
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/chart.less
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/clearfix.less
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/colours.less
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/common.less
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/components.less
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/core.less
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/dialog.less
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/fonts.less
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/icons.less
--rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/inspector.less
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/loader.less
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/menu.less
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/summary.less
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/tabs.less
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/validation-report.less
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.common.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.dev.js
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.prod.js
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/xhtmlserialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   492586 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/Makefile-src
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/build-viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/fetch-sample-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/sample-files.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/samples/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/samples/src/continuation/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/continuation/continuation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/ixds-test/
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/document1.html
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/faurecia.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/valeo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/scrollable-div/
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/scrollable-div/scrollable-div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/core_elements.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/doc_frame.js
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/fact_details_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/search_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/toolbar.js
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/viewer_page.js
--rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/
--rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
--rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/highlights.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/fact_properties.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/highlight.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/search.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tools/generate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
--rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.babelrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.386339 ixbrl-viewer-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.386339 ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/questions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.390339 ixbrl-viewer-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/node-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/npm-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/puppeteer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.390339 ixbrl-viewer-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.398339 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
+-rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.402339 ixbrl-viewer-1.4.0/examples/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/example-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/extended-viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/example_plugin/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/ixbrl-viewer-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/review-mode.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.402339 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.402339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13689 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/featureConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/stubviewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   859316 2023-08-03 00:06:55.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-03 00:06:55.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/i18next-parser.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.382339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/inspector.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.382339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.406339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.410339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.414339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/accordian.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/aspect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/calculations.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/concept.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/dialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/fact.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/factset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/inspector.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/outline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/period.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/period.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/qname.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/report.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/search.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/summary.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/test-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/unit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/util.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/accordian.less
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/block-list.less
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/chart.less
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/clearfix.less
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/colours.less
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/common.less
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/components.less
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/core.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/dialog.less
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/fonts.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/icons.less
+-rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/inspector.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/loader.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/menu.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/summary.less
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/tabs.less
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/validation-report.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/webpack.common.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/webpack.dev.js
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/webpack.prod.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/iXBRLViewerPlugin/xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 00:07:09.000000 ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   492445 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/Makefile-src
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4323 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/build-viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/fetch-sample-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/sample-files.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.382339 ixbrl-viewer-1.4.0/samples/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/samples/src/continuation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/continuation/continuation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/samples/src/ixds-test/
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/ixds-test/document1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/ixds-test/faurecia.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/ixds-test/valeo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/samples/src/scrollable-div/
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/scrollable-div/scrollable-div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/samples/src/xbrl-invalid-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/tests/puppeteer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/tests/puppeteer/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/core_elements.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.418339 ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/doc_frame.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/fact_details_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/search_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/toolbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/framework/viewer_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/tests/puppeteer/test_filings/
+-rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/test_filings/highlights.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/tests/puppeteer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/tests/fact_properties.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/tests/highlight.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/tests/search.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/tests/puppeteer/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/puppeteer/tools/generate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:07:09.422339 ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-08-03 00:06:21.000000 ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
```

### Comparing `ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/bug.yml` & `ixbrl-viewer-1.4.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/dependabot.yml` & `ixbrl-viewer-1.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/workflows/node-tests.yml` & `ixbrl-viewer-1.4.0/.github/workflows/node-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/workflows/npm-package.yml` & `ixbrl-viewer-1.4.0/.github/workflows/npm-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/workflows/puppeteer.yml` & `ixbrl-viewer-1.4.0/.github/workflows/puppeteer.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/workflows/python-package.yml` & `ixbrl-viewer-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/.github/workflows/python-tests.yml` & `ixbrl-viewer-1.4.0/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/LICENSE` & `ixbrl-viewer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/Makefile` & `ixbrl-viewer-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/NOTICE` & `ixbrl-viewer-1.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/PKG-INFO` & `ixbrl-viewer-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.3.0
+Version: 1.4.0
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.3.0/PLUGINS.md` & `ixbrl-viewer-1.4.0/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/README.md` & `ixbrl-viewer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/README.md` & `ixbrl-viewer-1.4.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.4.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/example_plugin/README.md` & `ixbrl-viewer-1.4.0/examples/example_plugin/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/example_plugin/example-plugin.gif` & `ixbrl-viewer-1.4.0/examples/example_plugin/example-plugin.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/example_plugin/extended-viewer.js` & `ixbrl-viewer-1.4.0/examples/example_plugin/extended-viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/example_plugin/package-lock.json` & `ixbrl-viewer-1.4.0/examples/example_plugin/package-lock.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/example_plugin/webpack.config.js` & `ixbrl-viewer-1.4.0/examples/example_plugin/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/ixbrl-viewer-demo.gif` & `ixbrl-viewer-1.4.0/examples/ixbrl-viewer-demo.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/review-mode.png` & `ixbrl-viewer-1.4.0/examples/review-mode.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml` & `ixbrl-viewer-1.4.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/__init__.py` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 from typing import Optional, Union
 
 from arelle import Cntlr
 from arelle.LocalViewer import LocalViewer
 from arelle.ModelDocument import Type
 from arelle.webserver.bottle import static_file
 
-from iXBRLViewerPlugin.constants import DEFAULT_VIEWER_PATH
-from .iXBRLViewer import IXBRLViewerBuilder, IXBRLViewerBuilderError, VIEWER_FEATURES_AND_DESCRIPTIONS
+from .constants import CONFIG_FEATURE_PREFIX, CONFIG_LAUNCH_ON_LOAD, \
+    CONFIG_SCRIPT_URL, DEFAULT_LAUNCH_ON_LOAD, DEFAULT_OUTPUT_NAME, \
+    DEFAULT_VIEWER_PATH, FEATURE_CONFIGS
+from .iXBRLViewer import IXBRLViewerBuilder, IXBRLViewerBuilderError
 
 
 #
 # GUI operation:
 #
 #     if submenu View->iXBRL Viewer->Launch viewer on load is checkmarked, a local viewer is automatically opened to view
 #
@@ -77,17 +79,17 @@
     parser.add_option("--zip-viewer-output",
                       action="store_true",
                       default=False,
                       dest="zipViewerOutput",
                       help="Converts the viewer output into a self contained zip")
     featureGroup = OptionGroup(parser, "Viewer Features",
                             "See viewer README for information on enabling/disabling features.")
-    for featureName, featureDescription in VIEWER_FEATURES_AND_DESCRIPTIONS.items():
-        arg = f'--viewer-feature-{featureName}'
-        featureGroup.add_option(arg, arg.lower(), action="store_true", default=False, help=featureDescription)
+    for featureConfig in FEATURE_CONFIGS:
+        arg = f'--viewer-feature-{featureConfig.key}'
+        featureGroup.add_option(arg, arg.lower(), action="store_true", default=False, help=featureConfig.description)
     parser.add_option_group(featureGroup)
 
 
 def generateViewer(
         cntlr: Cntlr,
         saveViewerDest: Union[io.BytesIO, str],
         viewerURL: str = DEFAULT_VIEWER_PATH,
@@ -159,17 +161,17 @@
     if os.path.isfile(saveViewerDir):
         saveViewerDir = os.path.dirname(os.path.join(os.getcwd(), saveViewerDir))
     return os.path.join(saveViewerDir, relativeViewerPath)
 
 
 def getFeaturesFromOptions(options: Union[argparse.Namespace, OptionParser]):
     return [
-        featureName
-        for featureName in VIEWER_FEATURES_AND_DESCRIPTIONS.keys()
-        if getattr(options, f'viewer_feature_{featureName}') or getattr(options, f'viewer_feature_{featureName.lower()}')
+        featureConfig.key
+        for featureConfig in FEATURE_CONFIGS
+        if getattr(options, f'viewer_feature_{featureConfig.key}') or getattr(options, f'viewer_feature_{featureConfig.key.lower()}')
     ]
 
 
 def iXBRLViewerCommandLineXbrlRun(cntlr, options, *args, **kwargs):
     generateViewer(
         cntlr,
         options.saveViewerDest or kwargs.get("responseZipStream"),
@@ -178,65 +180,69 @@
         options.useStubViewer,
         options.zipViewerOutput,
         getFeaturesFromOptions(options),
         options.packageDownloadURL,
     )
 
 
-def iXBRLViewerMenuCommand(cntlr):
+def iXBRLViewerSaveCommand(cntlr):
     from .ui import SaveViewerDialog
     if cntlr.modelManager is None or cntlr.modelManager.modelXbrl is None:
         cntlr.addToLog("No document loaded.")
         return
     modelXbrl = cntlr.modelManager.modelXbrl
     if modelXbrl.modelDocument.type not in (Type.INLINEXBRL, Type.INLINEXBRLDOCUMENTSET):
         cntlr.addToLog("No inline XBRL document loaded.")
         return
     dialog = SaveViewerDialog(cntlr)
+    dialog.render()
     if dialog.accepted and dialog.filename():
         generateViewer(
             cntlr,
             dialog.filename(),
             dialog.scriptUrl(),
             zipViewerOutput=dialog.zipViewerOutput(),
+            features=dialog.features()
         )
 
 
+def iXBRLViewerSettingsCommand(cntlr):
+    from .ui import SettingsDialog
+    SettingsDialog(cntlr).render()
+
+
 def iXBRLViewerToolsMenuExtender(cntlr, menu, *args, **kwargs):
-    # Extend menu with an item for the savedts plugin
-    menu.add_command(label="Save iXBRL Viewer Instance",
-                     underline=0,
-                     command=lambda: iXBRLViewerMenuCommand(cntlr))
+    # Add Tools menu
+    from tkinter import Menu  # must only import if GUI present (no tkinter on GUI-less servers)
+    viewerMenu = Menu(cntlr.menubar, tearoff=0)
+    menu.add_cascade(label=_("iXBRL Viewer"), menu=viewerMenu, underline=0)
+
+    # Extend menu with settings and save dialogs
+    viewerMenu.add_command(
+        label="Settings...",
+        underline=0,
+        command=lambda: iXBRLViewerSettingsCommand(cntlr))
+    viewerMenu.add_command(
+        label="Save Viewer...",
+        underline=0,
+        command=lambda: iXBRLViewerSaveCommand(cntlr))
 
 
 def toolsMenuExtender(cntlr, menu, *args, **kwargs):
     iXBRLViewerToolsMenuExtender(cntlr, menu, *args, **kwargs)
 
 
 def commandLineOptionExtender(*args, **kwargs):
     iXBRLViewerCommandLineOptionExtender(*args, **kwargs)
 
 
 def commandLineRun(*args, **kwargs):
     iXBRLViewerCommandLineXbrlRun(*args, **kwargs)
 
 
-def viewMenuExtender(cntlr, viewMenu, *args, **kwargs):
-    # persist menu selections for showing filing data and tables menu
-    from tkinter import Menu, BooleanVar  # must only import if GUI present (no tkinter on GUI-less servers)
-    def setLaunchIXBRLViewer(self, *args):
-        cntlr.config["LaunchIXBRLViewer"] = cntlr.launchIXBRLViewer.get()
-        cntlr.saveConfig()
-    erViewMenu = Menu(cntlr.menubar, tearoff=0)
-    viewMenu.add_cascade(label=_("iXBRL Viewer"), menu=erViewMenu, underline=0)
-    cntlr.launchIXBRLViewer = BooleanVar(value=cntlr.config.get("LaunchIXBRLViewer", True))
-    cntlr.launchIXBRLViewer.trace("w", setLaunchIXBRLViewer)
-    erViewMenu.add_checkbutton(label=_("Launch viewer on load"), underline=0, variable=cntlr.launchIXBRLViewer, onvalue=True, offvalue=False)
-
-
 class iXBRLViewerLocalViewer(LocalViewer):
     # plugin-specific local file handler
     def getLocalFile(self, file, relpath, request):
         _report, _sep, _file = file.partition("/")
         if file == 'ixbrlviewer.js':
             return static_file('ixbrlviewer.js', os.path.dirname(DEFAULT_VIEWER_PATH))
         elif _report.isnumeric():  # in reportsFolder folder
@@ -253,20 +259,34 @@
                 self.cntlr.addToLog("http://localhost:{}/{}".format(self.port, file), messageCode="localViewer:fileNotFound", level=logging.DEBUG)
             return static_file(_file, root=_fileDir, headers=self.noCacheHeaders)  # extra_headers modification to py-bottle
         return static_file(file, root="/")  # probably can't get here unless path is wrong
 
 
 def guiRun(cntlr, modelXbrl, attach, *args, **kwargs):
     """ run iXBRL Viewer using GUI interactions for a single instance or testcases """
+    if not cntlr.config.setdefault(CONFIG_LAUNCH_ON_LOAD, DEFAULT_LAUNCH_ON_LOAD):
+        # Don't run on launch if the option has been disabled
+        return
     try:
         import webbrowser
         global tempViewer
         tempViewer = tempfile.TemporaryDirectory()
-        viewer_file_name = 'ixbrlviewer.html'
-        generateViewer(cntlr, tempViewer.name, useStubViewer=True)
+        viewer_file_name = DEFAULT_OUTPUT_NAME
+        features = [
+            c.key
+            for c in FEATURE_CONFIGS
+            if cntlr.config.setdefault(f'{CONFIG_FEATURE_PREFIX}{c.key}', False)
+        ]
+        generateViewer(
+            cntlr,
+            saveViewerDest=tempViewer.name,
+            viewerURL=cntlr.config.setdefault(CONFIG_SCRIPT_URL, DEFAULT_VIEWER_PATH),
+            useStubViewer=True,
+            features=features
+        )
         localViewer = iXBRLViewerLocalViewer("iXBRL Viewer",  os.path.dirname(__file__))
         localhost = localViewer.init(cntlr, tempViewer.name)
         webbrowser.open(f'{localhost}/{viewer_file_name}')
     except Exception as ex:
         modelXbrl.error(
             "viewer:exception",
             "Exception %(exception)s \sTraceback %(traceback)s",
@@ -284,10 +304,9 @@
     'description': "iXBRL Viewer creator",
     'license': 'License :: OSI Approved :: Apache License, Version 2.0 (Apache-2.0)',
     'author': 'Paul Warren',
     'copyright': 'Copyright :: Workiva Inc. :: 2019',
     'CntlrCmdLine.Options': commandLineOptionExtender,
     'CntlrCmdLine.Xbrl.Run': commandLineRun,
     'CntlrWinMain.Menu.Tools': toolsMenuExtender,
-    'CntlrWinMain.Menu.View': viewMenuExtender,
     'CntlrWinMain.Xbrl.Loaded': guiRun,
 }
```

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/iXBRLViewer.py` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/iXBRLViewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,29 @@
 from arelle.ModelDocument import Type
 from arelle.ModelRelationshipSet import ModelRelationshipSet
 from arelle.ModelValue import QName, INVALIDixVALUE
 from arelle.UrlUtil import isHttpUrl
 from arelle.ValidateXbrlCalcs import inferredDecimals
 from lxml import etree
 
-from iXBRLViewerPlugin.constants import DEFAULT_VIEWER_PATH
+from .constants import DEFAULT_OUTPUT_NAME, DEFAULT_VIEWER_PATH, FEATURE_CONFIGS
 from .xhtmlserialize import XHTMLSerializer
 
 
 UNRECOGNIZED_LINKBASE_LOCAL_DOCUMENTS_TYPE = 'unrecognizedLinkbase'
 LINK_QNAME_TO_LOCAL_DOCUMENTS_LINKBASE_TYPE = {
     XbrlConst.qnLinkCalculationLink: 'calcLinkbase',
     XbrlConst.qnLinkDefinitionLink: 'defLinkbase',
     XbrlConst.qnLinkLabelLink: 'labelLinkbase',
     XbrlConst.qnLinkPresentationLink: 'presLinkbase',
     XbrlConst.qnLinkReferenceLink: 'refLinkbase',
 }
 
 WIDER_NARROWER_ARCROLE = 'http://www.esma.europa.eu/xbrl/esef/arcrole/wider-narrower'
 
-VIEWER_FEATURES_AND_DESCRIPTIONS = {
-    "review": "Enables highlighting of untagged numbers and dates.",
-}
-
 class NamespaceMap:
     """
     Class for building a 1:1 map of prefixes to namespace URIs
     Will attempt to use a provided, preferred prefix, but will uniquify as
     required.
     """
 
@@ -98,16 +94,17 @@
         }
         self.footnoteRelationshipSet = ModelRelationshipSet(dts, "XBRL-footnotes")
         self.basenameSuffix = basenameSuffix
 
     def enableFeature(self, featureName: str):
         if featureName in self.taxonomyData["features"]:
             return
-        assert featureName in VIEWER_FEATURES_AND_DESCRIPTIONS, \
-            f'Given feature name `{featureName}` does not match any defined features: {VIEWER_FEATURES_AND_DESCRIPTIONS.keys()}'
+        featureNames = [c.key for c in FEATURE_CONFIGS]
+        assert featureName in featureNames, \
+            f'Given feature name `{featureName}` does not match any defined features: {featureNames}'
         self.taxonomyData["features"].append(featureName)
 
     def outputFilename(self, filename):
         (base, ext) = os.path.splitext(filename)
         return base + self.basenameSuffix + ext
 
     def lineWrap(self, s, n = 80):
@@ -416,26 +413,26 @@
                 os.path.basename(self.outputFilename(doc.filepath)): deepcopy(doc.xmlDocument)
                 for doc in sorted(dts.modelDocument.referencesDocument.keys(), key=lambda x: x.objectIndex)
             }
             docSetFiles = list(xmlDocsByFilename.keys())
 
             if useStubViewer:
                 xmlDocument = self.getStubDocument()
-                iv.addFile(iXBRLViewerFile("ixbrlviewer.html", xmlDocument))
+                iv.addFile(iXBRLViewerFile(DEFAULT_OUTPUT_NAME, xmlDocument))
             else:
                 xmlDocument = next(iter(xmlDocsByFilename.values()))
 
             for filename, docSetXMLDoc in xmlDocsByFilename.items():
                 iv.addFile(iXBRLViewerFile(filename, docSetXMLDoc))
 
         elif useStubViewer:
             xmlDocument = self.getStubDocument()
             filename = self.outputFilename(os.path.basename(dts.modelDocument.filepath))
             docSetFiles = [ filename ]
-            iv.addFile(iXBRLViewerFile("ixbrlviewer.html", xmlDocument))
+            iv.addFile(iXBRLViewerFile(DEFAULT_OUTPUT_NAME, xmlDocument))
             iv.addFile(iXBRLViewerFile(filename, dts.modelDocument.xmlDocument))
 
         else:
             xmlDocument = deepcopy(dts.modelDocument.xmlDocument)
             iv.addFile(iXBRLViewerFile('xbrlviewer.html', xmlDocument))
 
         if packageDownloadURL is not None:
```

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27208,23 +27208,25 @@
                     calcLinkbase: r,
                     defLinkbase: o,
                     labelLinkbase: a,
                     presLinkbase: s,
                     refLinkbase: l,
                     unrecognizedLinkbase: c
                 } = this.summary.getLocalDocuments(), u = e.find(".files-summary");
+                let d = 0;
 
-                function d(e, n) {
+                function h(e, n) {
                     if (0 === e.length) u.find(n).hide();
                     else {
                         const i = u.find(n + " ul");
+                        d += 1;
                         for (const n of e) i.append(t()("<li></li>").text(n))
                     }
                 }
-                d(n, ".inline-docs"), d(i, ".schemas"), d(s, ".pres-links"), d(r, ".calc-links"), d(o, ".def-links"), d(a, ".label-links"), d(l, ".ref-links"), d(c, ".other-links")
+                h(n, ".inline-docs"), h(i, ".schemas"), h(s, ".pres-links"), h(r, ".calc-links"), h(o, ".def-links"), h(a, ".label-links"), h(l, ".ref-links"), h(c, ".other-links"), 0 == d && u.hide()
             }
             createOutline() {
                 if (this.outline.hasOutline()) {
                     t()(".outline .no-outline-overlay").hide();
                     const e = t()('<div class="fact-list"></div>').appendTo(t()(".outline .body"));
                     for (const n of this.outline.sortedSections()) t()('<div class="fact-list-item"></div>').text(this._report.getRoleLabel(n)).click((() => this.selectItem(this.outline.sections[n].id))).dblclick((() => t()("#inspector").removeClass("outline-mode"))).mousedown((e => {
                         e.detail > 1 && e.preventDefault()
@@ -27493,15 +27495,15 @@
         }, hr.prototype.isReviewModeEnabled = function() {
             return this.isFeatureEnabled("review")
         }, hr.prototype._loadInspectorHTML = function() {
             t()(n(845)).prependTo("body");
             var e = n(610).toString();
             t()('<style id="ixv-style"></style>').prop("type", "text/css").text(e).appendTo("head"), t()('<link id="ixv-favicon" type="image/x-icon" rel="shortcut icon" />').attr("href", n(688)).appendTo("head");
             try {
-                t()(".inspector-foot .version").text("1.3.0")
+                t()(".inspector-foot .version").text("1.4.0")
             } catch (e) {}
         }, hr.prototype._reparentDocument = function() {
             var e = t()("#ixv #iframe-container"),
                 n = t()('<iframe title="iXBRL document view"/>').appendTo(e)[0],
                 i = n.contentDocument || n.contentWindow.document;
             i.open(), i.write("<!DOCTYPE html><html><head><title></title></head><body></body></html>"), i.close();
             var r = t()("title").text();
```

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/inspector.html` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/html/inspector.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/accordian.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/accordian.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/aspect.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/calculations.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/calculations.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/concept.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/dialog.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/dialog.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/fact.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/factset.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/footnote.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/footnote.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/inspector.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -560,34 +560,39 @@
             labelLinkbase,
             presLinkbase,
             refLinkbase,
             unrecognizedLinkbase
         } = this.summary.getLocalDocuments();
 
         const summaryFilesContent = summaryDom.find(".files-summary");
+        let visibleItems = 0;
 
         function insertFileSummary(docs, classSelector) {
             if (docs.length === 0) {
                 summaryFilesContent.find(classSelector).hide();
             } else {
                 const ul = summaryFilesContent.find(classSelector + ' ul')
+                visibleItems += 1;
                 for (const doc of docs) {
                     ul.append($("<li></li>").text(doc));
                 }
             }
         }
 
         insertFileSummary(inline, ".inline-docs");
         insertFileSummary(schema, ".schemas");
         insertFileSummary(presLinkbase, ".pres-links");
         insertFileSummary(calcLinkbase, ".calc-links");
         insertFileSummary(defLinkbase, ".def-links");
         insertFileSummary(labelLinkbase, ".label-links");
         insertFileSummary(refLinkbase, ".ref-links");
         insertFileSummary(unrecognizedLinkbase, ".other-links");
+        if (visibleItems == 0) {
+            summaryFilesContent.hide();
+        }
     };
 
     createOutline() {
         if (this.outline.hasOutline()) {
             $('.outline .no-outline-overlay').hide();
             const container = $('<div class="fact-list"></div>').appendTo($('.outline .body'));
             for (const elr of this.outline.sortedSections()) {
```

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/menu.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/menu.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/outline.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/period.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/period.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/report.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/report.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/search.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/summary.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/unit.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/util.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.test.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/util.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewer.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/js/viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/accordian.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/accordian.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/chart.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/chart.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/colours.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/colours.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/dialog.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/dialog.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/icons.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/icons.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/inspector.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/inspector.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/loader.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/loader.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/menu.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/menu.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/summary.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/summary.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/tabs.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/tabs.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/viewer.less` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/src/less/viewer.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.common.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/webpack.common.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.dev.js` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/viewer/webpack.dev.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/xhtmlserialize.py` & `ixbrl-viewer-1.4.0/iXBRLViewerPlugin/xhtmlserialize.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/PKG-INFO` & `ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.3.0
+Version: 1.4.0
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/SOURCES.txt` & `ixbrl-viewer-1.4.0/ixbrl_viewer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
 examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
 examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
 examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
 iXBRLViewerPlugin/__init__.py
 iXBRLViewerPlugin/_version.py
 iXBRLViewerPlugin/constants.py
+iXBRLViewerPlugin/featureConfig.py
 iXBRLViewerPlugin/iXBRLViewer.py
 iXBRLViewerPlugin/stubviewer.html
 iXBRLViewerPlugin/ui.py
 iXBRLViewerPlugin/xhtmlserialize.py
 iXBRLViewerPlugin/viewer/i18next-parser.config.js
 iXBRLViewerPlugin/viewer/version.js
 iXBRLViewerPlugin/viewer/webpack.common.js
```

### Comparing `ixbrl-viewer-1.3.0/package-lock.json` & `ixbrl-viewer-1.4.0/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994805369263263%*

 * *Differences: {"'packages'": "{'node_modules/@jest/console': {'version': '29.6.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/@jest/console/-/console-29.6.2.tgz', 'integrity': "*

 * *               "'sha512-0N0yZof5hi44HAR2pPS+ikJ3nzKNoZdVu8FffRf3wy47I7Dm7etk/3KetMdRUqzVd16V4O2m2ISpNTbnIuqy1w==', "*

 * *               "'dependencies': {'jest-message-util': '^29.6.2', 'jest-util': '^29.6.2'}}, "*

 * *               "'node_modules/@jest/core': {'version': '29.6.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/ […]*

```diff
@@ -1158,25 +1158,25 @@
             "version": "0.1.3"
         },
         "node_modules/@jest/console": {
             "dependencies": {
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
-                "jest-message-util": "^29.6.1",
-                "jest-util": "^29.6.1",
+                "jest-message-util": "^29.6.2",
+                "jest-util": "^29.6.2",
                 "slash": "^3.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-Aj772AYgwTSr5w8qnyoJ0eDYvN6bMsH3ORH1ivMotrInHLKdUz6BDlaEXHdM6kODaBIkNIyQGzsMvRdOv7VG7Q==",
-            "resolved": "https://registry.npmjs.org/@jest/console/-/console-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-0N0yZof5hi44HAR2pPS+ikJ3nzKNoZdVu8FffRf3wy47I7Dm7etk/3KetMdRUqzVd16V4O2m2ISpNTbnIuqy1w==",
+            "resolved": "https://registry.npmjs.org/@jest/console/-/console-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/console/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -1245,58 +1245,58 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/@jest/core": {
             "dependencies": {
-                "@jest/console": "^29.6.1",
-                "@jest/reporters": "^29.6.1",
-                "@jest/test-result": "^29.6.1",
-                "@jest/transform": "^29.6.1",
+                "@jest/console": "^29.6.2",
+                "@jest/reporters": "^29.6.2",
+                "@jest/test-result": "^29.6.2",
+                "@jest/transform": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "ansi-escapes": "^4.2.1",
                 "chalk": "^4.0.0",
                 "ci-info": "^3.2.0",
                 "exit": "^0.1.2",
                 "graceful-fs": "^4.2.9",
                 "jest-changed-files": "^29.5.0",
-                "jest-config": "^29.6.1",
-                "jest-haste-map": "^29.6.1",
-                "jest-message-util": "^29.6.1",
+                "jest-config": "^29.6.2",
+                "jest-haste-map": "^29.6.2",
+                "jest-message-util": "^29.6.2",
                 "jest-regex-util": "^29.4.3",
-                "jest-resolve": "^29.6.1",
-                "jest-resolve-dependencies": "^29.6.1",
-                "jest-runner": "^29.6.1",
-                "jest-runtime": "^29.6.1",
-                "jest-snapshot": "^29.6.1",
-                "jest-util": "^29.6.1",
-                "jest-validate": "^29.6.1",
-                "jest-watcher": "^29.6.1",
+                "jest-resolve": "^29.6.2",
+                "jest-resolve-dependencies": "^29.6.2",
+                "jest-runner": "^29.6.2",
+                "jest-runtime": "^29.6.2",
+                "jest-snapshot": "^29.6.2",
+                "jest-util": "^29.6.2",
+                "jest-validate": "^29.6.2",
+                "jest-watcher": "^29.6.2",
                 "micromatch": "^4.0.4",
-                "pretty-format": "^29.6.1",
+                "pretty-format": "^29.6.2",
                 "slash": "^3.0.0",
                 "strip-ansi": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-CcowHypRSm5oYQ1obz1wfvkjZZ2qoQlrKKvlfPwh5jUXVU12TWr2qMeH8chLMuTFzHh5a1g2yaqlqDICbr+ukQ==",
+            "integrity": "sha512-Oj+5B+sDMiMWLhPFF+4/DvHOf+U10rgvCLGPHP8Xlsy/7QxS51aU/eBngudHlJXnaWD5EohAgJ4js+T6pa+zOg==",
             "peerDependencies": {
                 "node-notifier": "^8.0.1 || ^9.0.0 || ^10.0.0"
             },
             "peerDependenciesMeta": {
                 "node-notifier": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@jest/core/-/core-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/@jest/core/-/core-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/core/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -1365,126 +1365,126 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/@jest/environment": {
             "dependencies": {
-                "@jest/fake-timers": "^29.6.1",
+                "@jest/fake-timers": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
-                "jest-mock": "^29.6.1"
+                "jest-mock": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-RMMXx4ws+Gbvw3DfLSuo2cfQlK7IwGbpuEWXCqyYDcqYTI+9Ju3a5hDnXaxjNsa6uKh9PQF2v+qg+RLe63tz5A==",
-            "resolved": "https://registry.npmjs.org/@jest/environment/-/environment-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-AEcW43C7huGd/vogTddNNTDRpO6vQ2zaQNrttvWV18ArBx9Z56h7BIsXkNFJVOO4/kblWEQz30ckw0+L3izc+Q==",
+            "resolved": "https://registry.npmjs.org/@jest/environment/-/environment-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/expect": {
             "dependencies": {
-                "expect": "^29.6.1",
-                "jest-snapshot": "^29.6.1"
+                "expect": "^29.6.2",
+                "jest-snapshot": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-N5xlPrAYaRNyFgVf2s9Uyyvr795jnB6rObuPx4QFvNJz8aAjpZUDfO4bh5G/xuplMID8PrnuF1+SfSyDxhsgYg==",
-            "resolved": "https://registry.npmjs.org/@jest/expect/-/expect-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-m6DrEJxVKjkELTVAztTLyS/7C92Y2b0VYqmDROYKLLALHn8T/04yPs70NADUYPrV3ruI+H3J0iUIuhkjp7vkfg==",
+            "resolved": "https://registry.npmjs.org/@jest/expect/-/expect-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/expect-utils": {
             "dependencies": {
                 "jest-get-type": "^29.4.3"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-o319vIf5pEMx0LmzSxxkYYxo4wrRLKHq9dP1yJU7FoPTB0LfAKSz8SWD6D/6U3v/O52t9cF5t+MeJiRsfk7zMw==",
-            "resolved": "https://registry.npmjs.org/@jest/expect-utils/-/expect-utils-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-6zIhM8go3RV2IG4aIZaZbxwpOzz3ZiM23oxAlkquOIole+G6TrbeXnykxWYlqF7kz2HlBjdKtca20x9atkEQYg==",
+            "resolved": "https://registry.npmjs.org/@jest/expect-utils/-/expect-utils-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/fake-timers": {
             "dependencies": {
                 "@jest/types": "^29.6.1",
                 "@sinonjs/fake-timers": "^10.0.2",
                 "@types/node": "*",
-                "jest-message-util": "^29.6.1",
-                "jest-mock": "^29.6.1",
-                "jest-util": "^29.6.1"
+                "jest-message-util": "^29.6.2",
+                "jest-mock": "^29.6.2",
+                "jest-util": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-RdgHgbXyosCDMVYmj7lLpUwXA4c69vcNzhrt69dJJdf8azUrpRh3ckFCaTPNjsEeRi27Cig0oKDGxy5j7hOgHg==",
-            "resolved": "https://registry.npmjs.org/@jest/fake-timers/-/fake-timers-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-euZDmIlWjm1Z0lJ1D0f7a0/y5Kh/koLFMUBE5SUYWrmy8oNhJpbTBDAP6CxKnadcMLDoDf4waRYCe35cH6G6PA==",
+            "resolved": "https://registry.npmjs.org/@jest/fake-timers/-/fake-timers-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/globals": {
             "dependencies": {
-                "@jest/environment": "^29.6.1",
-                "@jest/expect": "^29.6.1",
+                "@jest/environment": "^29.6.2",
+                "@jest/expect": "^29.6.2",
                 "@jest/types": "^29.6.1",
-                "jest-mock": "^29.6.1"
+                "jest-mock": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-2VjpaGy78JY9n9370H8zGRCFbYVWwjY6RdDMhoJHa1sYfwe6XM/azGN0SjY8kk7BOZApIejQ1BFPyH7FPG0w3A==",
-            "resolved": "https://registry.npmjs.org/@jest/globals/-/globals-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-cjuJmNDjs6aMijCmSa1g2TNG4Lby/AeU7/02VtpW+SLcZXzOLK2GpN2nLqcFjmhy3B3AoPeQVx7BnyOf681bAw==",
+            "resolved": "https://registry.npmjs.org/@jest/globals/-/globals-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/reporters": {
             "dependencies": {
                 "@bcoe/v8-coverage": "^0.2.3",
-                "@jest/console": "^29.6.1",
-                "@jest/test-result": "^29.6.1",
-                "@jest/transform": "^29.6.1",
+                "@jest/console": "^29.6.2",
+                "@jest/test-result": "^29.6.2",
+                "@jest/transform": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@jridgewell/trace-mapping": "^0.3.18",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
                 "collect-v8-coverage": "^1.0.0",
                 "exit": "^0.1.2",
                 "glob": "^7.1.3",
                 "graceful-fs": "^4.2.9",
                 "istanbul-lib-coverage": "^3.0.0",
                 "istanbul-lib-instrument": "^5.1.0",
                 "istanbul-lib-report": "^3.0.0",
                 "istanbul-lib-source-maps": "^4.0.0",
                 "istanbul-reports": "^3.1.3",
-                "jest-message-util": "^29.6.1",
-                "jest-util": "^29.6.1",
-                "jest-worker": "^29.6.1",
+                "jest-message-util": "^29.6.2",
+                "jest-util": "^29.6.2",
+                "jest-worker": "^29.6.2",
                 "slash": "^3.0.0",
                 "string-length": "^4.0.1",
                 "strip-ansi": "^6.0.0",
                 "v8-to-istanbul": "^9.0.1"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-9zuaI9QKr9JnoZtFQlw4GREQbxgmNYXU6QuWtmuODvk5nvPUeBYapVR/VYMyi2WSx3jXTLJTJji8rN6+Cm4+FA==",
+            "integrity": "sha512-sWtijrvIav8LgfJZlrGCdN0nP2EWbakglJY49J1Y5QihcQLfy7ovyxxjJBRXMNltgt4uPtEcFmIMbVshEDfFWw==",
             "peerDependencies": {
                 "node-notifier": "^8.0.1 || ^9.0.0 || ^10.0.0"
             },
             "peerDependenciesMeta": {
                 "node-notifier": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@jest/reporters/-/reporters-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/@jest/reporters/-/reporters-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/reporters/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -1579,41 +1579,41 @@
             },
             "integrity": "sha512-oA+I2SHHQGxDCZpbrsCQSoMLb3Bz547JnM+jUr9qEbuw0vQlWZfpPS7CO9J7XiwKicEz9OFn/IYoLkkiUD7bzA==",
             "resolved": "https://registry.npmjs.org/@jest/source-map/-/source-map-29.6.0.tgz",
             "version": "29.6.0"
         },
         "node_modules/@jest/test-result": {
             "dependencies": {
-                "@jest/console": "^29.6.1",
+                "@jest/console": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/istanbul-lib-coverage": "^2.0.0",
                 "collect-v8-coverage": "^1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-Ynr13ZRcpX6INak0TPUukU8GWRfm/vAytE3JbJNGAvINySWYdfE7dGZMbk36oVuK4CigpbhMn8eg1dixZ7ZJOw==",
-            "resolved": "https://registry.npmjs.org/@jest/test-result/-/test-result-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-3VKFXzcV42EYhMCsJQURptSqnyjqCGbtLuX5Xxb6Pm6gUf1wIRIl+mandIRGJyWKgNKYF9cnstti6Ls5ekduqw==",
+            "resolved": "https://registry.npmjs.org/@jest/test-result/-/test-result-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/test-sequencer": {
             "dependencies": {
-                "@jest/test-result": "^29.6.1",
+                "@jest/test-result": "^29.6.2",
                 "graceful-fs": "^4.2.9",
-                "jest-haste-map": "^29.6.1",
+                "jest-haste-map": "^29.6.2",
                 "slash": "^3.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-oBkC36PCDf/wb6dWeQIhaviU0l5u6VCsXa119yqdUosYAt7/FbQU2M2UoziO3igj/HBDEgp57ONQ3fm0v9uyyg==",
-            "resolved": "https://registry.npmjs.org/@jest/test-sequencer/-/test-sequencer-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-GVYi6PfPwVejO7slw6IDO0qKVum5jtrJ3KoLGbgBWyr2qr4GaxFV6su+ZAjdTX75Sr1DkMFRk09r2ZVa+wtCGw==",
+            "resolved": "https://registry.npmjs.org/@jest/test-sequencer/-/test-sequencer-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/test-sequencer/node_modules/slash": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-g9Q1haeby36OSStwb4ntCGGGaKsaVSjQ68fBxoQcutl5fS1vuY18H3wSt3jFyFtrkx+Kz0V1G85A4MyAdDMi2Q==",
@@ -1626,29 +1626,29 @@
                 "@jest/types": "^29.6.1",
                 "@jridgewell/trace-mapping": "^0.3.18",
                 "babel-plugin-istanbul": "^6.1.1",
                 "chalk": "^4.0.0",
                 "convert-source-map": "^2.0.0",
                 "fast-json-stable-stringify": "^2.1.0",
                 "graceful-fs": "^4.2.9",
-                "jest-haste-map": "^29.6.1",
+                "jest-haste-map": "^29.6.2",
                 "jest-regex-util": "^29.4.3",
-                "jest-util": "^29.6.1",
+                "jest-util": "^29.6.2",
                 "micromatch": "^4.0.4",
                 "pirates": "^4.0.4",
                 "slash": "^3.0.0",
                 "write-file-atomic": "^4.0.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-URnTneIU3ZjRSaf906cvf6Hpox3hIeJXRnz3VDSw5/X93gR8ycdfSIEy19FlVx8NFmpN7fe3Gb1xF+NjXaQLWg==",
-            "resolved": "https://registry.npmjs.org/@jest/transform/-/transform-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-ZqCqEISr58Ce3U+buNFJYUktLJZOggfyvR+bZMaiV1e8B1SIvJbwZMrYz3gx/KAPn9EXmOmN+uB08yLCjWkQQg==",
+            "resolved": "https://registry.npmjs.org/@jest/transform/-/transform-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/@jest/transform/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -2125,20 +2125,14 @@
         },
         "node_modules/@types/normalize-package-data": {
             "dev": true,
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
-        "node_modules/@types/prettier": {
-            "dev": true,
-            "integrity": "sha512-+68kP9yzs4LMp7VNh8gdzMSPZFL44MLGqiHWvttYJe+6qnuVr4Ek9wSBQoveqY/r+LwjCcU29kNVkidwim+kYA==",
-            "resolved": "https://registry.npmjs.org/@types/prettier/-/prettier-2.7.3.tgz",
-            "version": "2.7.3"
-        },
         "node_modules/@types/stack-utils": {
             "dev": true,
             "integrity": "sha512-Hl219/BT5fLAaz6NDkSuhzasy49dwQS/DSdu4MdggFB8zcXv7vflBI3xp7FEmkmdDkBUI2bPUNeMttp2knYdxw==",
             "resolved": "https://registry.npmjs.org/@types/stack-utils/-/stack-utils-2.0.1.tgz",
             "version": "2.0.1"
         },
         "node_modules/@types/symlink-or-copy": {
@@ -2916,32 +2910,32 @@
             "dev": true,
             "integrity": "sha512-n7pFrqQm44TCYvrCDb0MqabAF+JUBq+ijBvNMUxpkLjJaAu32faIexewMumrH5KLLJ1HDyT0PTEqRyAe/GwwuQ==",
             "resolved": "https://registry.npmjs.org/babel-helpers/-/babel-helpers-6.24.1.tgz",
             "version": "6.24.1"
         },
         "node_modules/babel-jest": {
             "dependencies": {
-                "@jest/transform": "^29.6.1",
+                "@jest/transform": "^29.6.2",
                 "@types/babel__core": "^7.1.14",
                 "babel-plugin-istanbul": "^6.1.1",
                 "babel-preset-jest": "^29.5.0",
                 "chalk": "^4.0.0",
                 "graceful-fs": "^4.2.9",
                 "slash": "^3.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-qu+3bdPEQC6KZSPz+4Fyjbga5OODNcp49j6GKzG1EKbkfyJBxEYGVUmVGpwCSeGouG52R4EgYMLb6p9YeEEQ4A==",
+            "integrity": "sha512-BYCzImLos6J3BH/+HvUCHG1dTf2MzmAB4jaVxHV+29RZLjR29XuYTmsf2sdDwkrb+FczkGo3kOhE7ga6sI0P4A==",
             "peerDependencies": {
                 "@babel/core": "^7.8.0"
             },
-            "resolved": "https://registry.npmjs.org/babel-jest/-/babel-jest-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/babel-jest/-/babel-jest-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/babel-jest/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -4699,17 +4693,25 @@
             "dev": true,
             "integrity": "sha512-VBBaLc1MgL5XpzgIP7ny5Z6Nx3UrRkIViUkPUdtl9aya5amy3De1gsUUSB1g3+3sExYNjCAsAznmukyxCb1GRA==",
             "resolved": "https://registry.npmjs.org/decimal.js/-/decimal.js-10.4.3.tgz",
             "version": "10.4.3"
         },
         "node_modules/dedent": {
             "dev": true,
-            "integrity": "sha512-Q6fKUPqnAHAyhiUgFU7BUzLiv0kd8saH9al7tnu5Q/okj6dnupxyTgFIBjVzJATdfIAm9NAsvXNzjaKa+bxVyA==",
-            "resolved": "https://registry.npmjs.org/dedent/-/dedent-0.7.0.tgz",
-            "version": "0.7.0"
+            "integrity": "sha512-3sSQTYoWKGcRHmHl6Y6opLpRJH55bxeGQ0Y1LCI5pZzUXvokVkj0FC4bi7uEwazxA9FQZ0Nv067Zt5kSUvXxEA==",
+            "peerDependencies": {
+                "babel-plugin-macros": "^3.1.0"
+            },
+            "peerDependenciesMeta": {
+                "babel-plugin-macros": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/dedent/-/dedent-1.5.0.tgz",
+            "version": "1.5.0"
         },
         "node_modules/deepmerge": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-3sUqbMEc77XqpdNO7FRyRog+eW3ph+GYCbj+rK+uYyRMuwsVy0rMiVtPn+QJlKFvWP/1PYpapqYn0Me2knFn+A==",
@@ -5219,28 +5221,28 @@
             },
             "integrity": "sha512-Zk/eNKV2zbjpKzrsQ+n1G6poVbErQxJ0LBOJXaKZ1EViLzH+hrLu9cdXI4zw9dBQJslwBEpbQ2P1oS7nDxs6jQ==",
             "resolved": "https://registry.npmjs.org/exit/-/exit-0.1.2.tgz",
             "version": "0.1.2"
         },
         "node_modules/expect": {
             "dependencies": {
-                "@jest/expect-utils": "^29.6.1",
+                "@jest/expect-utils": "^29.6.2",
                 "@types/node": "*",
                 "jest-get-type": "^29.4.3",
-                "jest-matcher-utils": "^29.6.1",
-                "jest-message-util": "^29.6.1",
-                "jest-util": "^29.6.1"
+                "jest-matcher-utils": "^29.6.2",
+                "jest-message-util": "^29.6.2",
+                "jest-util": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-XEdDLonERCU1n9uR56/Stx9OqojaLAQtZf9PrCHH9Hl8YXiEIka3H4NXJ3NOIBmQJTg7+j7buh34PMHfJujc8g==",
-            "resolved": "https://registry.npmjs.org/expect/-/expect-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-iAErsLxJ8C+S02QbLAwgSGSezLQK+XXRDt8IuFXFpwCNw2ECmzZSmjKcCaFVp5VRMk+WAvz6h6jokzEzBFZEuA==",
+            "resolved": "https://registry.npmjs.org/expect/-/expect-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/extend": {
             "dev": true,
             "integrity": "sha512-fjquC59cD7CyW6urNXK0FBufkZcoiGG80wTuPujX590cB5Ttln20E2UB4S/WARVqhXffZl2LNgS+gQdPIIim/g==",
             "resolved": "https://registry.npmjs.org/extend/-/extend-3.0.2.tgz",
             "version": "3.0.2"
         },
@@ -7054,34 +7056,34 @@
             "version": "3.1.6"
         },
         "node_modules/jest": {
             "bin": {
                 "jest": "bin/jest.js"
             },
             "dependencies": {
-                "@jest/core": "^29.6.1",
+                "@jest/core": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "import-local": "^3.0.2",
-                "jest-cli": "^29.6.1"
+                "jest-cli": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-Nirw5B4nn69rVUZtemCQhwxOBhm0nsp3hmtF4rzCeWD7BkjAXRIji7xWQfnTNbz9g0aVsBX6aZK3n+23LM6uDw==",
+            "integrity": "sha512-8eQg2mqFbaP7CwfsTpCxQ+sHzw1WuNWL5UUvjnWP4hx2riGz9fPSzYOaU5q8/GqWn1TfgZIVTqYJygbGbWAANg==",
             "peerDependencies": {
                 "node-notifier": "^8.0.1 || ^9.0.0 || ^10.0.0"
             },
             "peerDependenciesMeta": {
                 "node-notifier": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/jest/-/jest-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/jest/-/jest-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-changed-files": {
             "dependencies": {
                 "execa": "^5.0.0",
                 "p-limit": "^3.1.0"
             },
             "dev": true,
@@ -7090,42 +7092,42 @@
             },
             "integrity": "sha512-IFG34IUMUaNBIxjQXF/iu7g6EcdMrGRRxaUSw92I/2g2YC6vCdTltl4nHvt7Ci5nSJwXIkCu8Ka1DKF+X7Z1Ag==",
             "resolved": "https://registry.npmjs.org/jest-changed-files/-/jest-changed-files-29.5.0.tgz",
             "version": "29.5.0"
         },
         "node_modules/jest-circus": {
             "dependencies": {
-                "@jest/environment": "^29.6.1",
-                "@jest/expect": "^29.6.1",
-                "@jest/test-result": "^29.6.1",
+                "@jest/environment": "^29.6.2",
+                "@jest/expect": "^29.6.2",
+                "@jest/test-result": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
                 "co": "^4.6.0",
-                "dedent": "^0.7.0",
+                "dedent": "^1.0.0",
                 "is-generator-fn": "^2.0.0",
-                "jest-each": "^29.6.1",
-                "jest-matcher-utils": "^29.6.1",
-                "jest-message-util": "^29.6.1",
-                "jest-runtime": "^29.6.1",
-                "jest-snapshot": "^29.6.1",
-                "jest-util": "^29.6.1",
+                "jest-each": "^29.6.2",
+                "jest-matcher-utils": "^29.6.2",
+                "jest-message-util": "^29.6.2",
+                "jest-runtime": "^29.6.2",
+                "jest-snapshot": "^29.6.2",
+                "jest-util": "^29.6.2",
                 "p-limit": "^3.1.0",
-                "pretty-format": "^29.6.1",
+                "pretty-format": "^29.6.2",
                 "pure-rand": "^6.0.0",
                 "slash": "^3.0.0",
                 "stack-utils": "^2.0.3"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-tPbYLEiBU4MYAL2XoZme/bgfUeotpDBd81lgHLCbDZZFaGmECk0b+/xejPFtmiBP87GgP/y4jplcRpbH+fgCzQ==",
-            "resolved": "https://registry.npmjs.org/jest-circus/-/jest-circus-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-G9mN+KOYIUe2sB9kpJkO9Bk18J4dTDArNFPwoZ7WKHKel55eKIS/u2bLthxgojwlf9NLCVQfgzM/WsOVvoC6Fw==",
+            "resolved": "https://registry.npmjs.org/jest-circus/-/jest-circus-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-circus/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7197,42 +7199,42 @@
             "version": "7.2.0"
         },
         "node_modules/jest-cli": {
             "bin": {
                 "jest": "bin/jest.js"
             },
             "dependencies": {
-                "@jest/core": "^29.6.1",
-                "@jest/test-result": "^29.6.1",
+                "@jest/core": "^29.6.2",
+                "@jest/test-result": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "chalk": "^4.0.0",
                 "exit": "^0.1.2",
                 "graceful-fs": "^4.2.9",
                 "import-local": "^3.0.2",
-                "jest-config": "^29.6.1",
-                "jest-util": "^29.6.1",
-                "jest-validate": "^29.6.1",
+                "jest-config": "^29.6.2",
+                "jest-util": "^29.6.2",
+                "jest-validate": "^29.6.2",
                 "prompts": "^2.0.1",
                 "yargs": "^17.3.1"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-607dSgTA4ODIN6go9w6xY3EYkyPFGicx51a69H7yfvt7lN53xNswEVLovq+E77VsTRi5fWprLH0yl4DJgE8Ing==",
+            "integrity": "sha512-TT6O247v6dCEX2UGHGyflMpxhnrL0DNqP2fRTKYm3nJJpCTfXX3GCMQPGFjXDoj0i5/Blp3jriKXFgdfmbYB6Q==",
             "peerDependencies": {
                 "node-notifier": "^8.0.1 || ^9.0.0 || ^10.0.0"
             },
             "peerDependenciesMeta": {
                 "node-notifier": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/jest-cli/-/jest-cli-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/jest-cli/-/jest-cli-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-cli/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7293,55 +7295,55 @@
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-config": {
             "dependencies": {
                 "@babel/core": "^7.11.6",
-                "@jest/test-sequencer": "^29.6.1",
+                "@jest/test-sequencer": "^29.6.2",
                 "@jest/types": "^29.6.1",
-                "babel-jest": "^29.6.1",
+                "babel-jest": "^29.6.2",
                 "chalk": "^4.0.0",
                 "ci-info": "^3.2.0",
                 "deepmerge": "^4.2.2",
                 "glob": "^7.1.3",
                 "graceful-fs": "^4.2.9",
-                "jest-circus": "^29.6.1",
-                "jest-environment-node": "^29.6.1",
+                "jest-circus": "^29.6.2",
+                "jest-environment-node": "^29.6.2",
                 "jest-get-type": "^29.4.3",
                 "jest-regex-util": "^29.4.3",
-                "jest-resolve": "^29.6.1",
-                "jest-runner": "^29.6.1",
-                "jest-util": "^29.6.1",
-                "jest-validate": "^29.6.1",
+                "jest-resolve": "^29.6.2",
+                "jest-runner": "^29.6.2",
+                "jest-util": "^29.6.2",
+                "jest-validate": "^29.6.2",
                 "micromatch": "^4.0.4",
                 "parse-json": "^5.2.0",
-                "pretty-format": "^29.6.1",
+                "pretty-format": "^29.6.2",
                 "slash": "^3.0.0",
                 "strip-json-comments": "^3.1.1"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-XdjYV2fy2xYixUiV2Wc54t3Z4oxYPAELUzWnV6+mcbq0rh742X2p52pii5A3oeRzYjLnQxCsZmp0qpI6klE2cQ==",
+            "integrity": "sha512-VxwFOC8gkiJbuodG9CPtMRjBUNZEHxwfQXmIudSTzFWxaci3Qub1ddTRbFNQlD/zUeaifLndh/eDccFX4wCMQw==",
             "peerDependencies": {
                 "@types/node": "*",
                 "ts-node": ">=9.0.0"
             },
             "peerDependenciesMeta": {
                 "@types/node": {
                     "optional": true
                 },
                 "ts-node": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/jest-config/-/jest-config-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/jest-config/-/jest-config-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-config/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7413,23 +7415,23 @@
             "version": "7.2.0"
         },
         "node_modules/jest-diff": {
             "dependencies": {
                 "chalk": "^4.0.0",
                 "diff-sequences": "^29.4.3",
                 "jest-get-type": "^29.4.3",
-                "pretty-format": "^29.6.1"
+                "pretty-format": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-FsNCvinvl8oVxpNLttNQX7FAq7vR+gMDGj90tiP7siWw1UdakWUGqrylpsYrpvj908IYckm5Y0Q7azNAozU1Kg==",
-            "resolved": "https://registry.npmjs.org/jest-diff/-/jest-diff-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-t+ST7CB9GX5F2xKwhwCf0TAR17uNDiaPTZnVymP9lw0lssa9vG+AFyDZoeIHStU3WowFFwT+ky+er0WVl2yGhA==",
+            "resolved": "https://registry.npmjs.org/jest-diff/-/jest-diff-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-diff/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7504,24 +7506,24 @@
             "version": "29.4.3"
         },
         "node_modules/jest-each": {
             "dependencies": {
                 "@jest/types": "^29.6.1",
                 "chalk": "^4.0.0",
                 "jest-get-type": "^29.4.3",
-                "jest-util": "^29.6.1",
-                "pretty-format": "^29.6.1"
+                "jest-util": "^29.6.2",
+                "pretty-format": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-n5eoj5eiTHpKQCAVcNTT7DRqeUmJ01hsAL0Q1SMiBHcBcvTKDELixQOGMCpqhbIuTcfC4kMfSnpmDqRgRJcLNQ==",
-            "resolved": "https://registry.npmjs.org/jest-each/-/jest-each-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-MsrsqA0Ia99cIpABBc3izS1ZYoYfhIy0NNWqPSE0YXbQjwchyt6B1HD2khzyPe1WiJA7hbxXy77ZoUQxn8UlSw==",
+            "resolved": "https://registry.npmjs.org/jest-each/-/jest-each-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-each/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7581,55 +7583,55 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-environment-jsdom": {
             "dependencies": {
-                "@jest/environment": "^29.6.1",
-                "@jest/fake-timers": "^29.6.1",
+                "@jest/environment": "^29.6.2",
+                "@jest/fake-timers": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/jsdom": "^20.0.0",
                 "@types/node": "*",
-                "jest-mock": "^29.6.1",
-                "jest-util": "^29.6.1",
+                "jest-mock": "^29.6.2",
+                "jest-util": "^29.6.2",
                 "jsdom": "^20.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-PoY+yLaHzVRhVEjcVKSfJ7wXmJW4UqPYNhR05h7u/TK0ouf6DmRNZFBL/Z00zgQMyWGMBXn69/FmOvhEJu8cIw==",
+            "integrity": "sha512-7oa/+266AAEgkzae8i1awNEfTfjwawWKLpiw2XesZmaoVVj9u9t8JOYx18cG29rbPNtkUlZ8V4b5Jb36y/VxoQ==",
             "peerDependencies": {
                 "canvas": "^2.5.0"
             },
             "peerDependenciesMeta": {
                 "canvas": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/jest-environment-jsdom/-/jest-environment-jsdom-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/jest-environment-jsdom/-/jest-environment-jsdom-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-environment-node": {
             "dependencies": {
-                "@jest/environment": "^29.6.1",
-                "@jest/fake-timers": "^29.6.1",
+                "@jest/environment": "^29.6.2",
+                "@jest/fake-timers": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
-                "jest-mock": "^29.6.1",
-                "jest-util": "^29.6.1"
+                "jest-mock": "^29.6.2",
+                "jest-util": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-ZNIfAiE+foBog24W+2caIldl4Irh8Lx1PUhg/GZ0odM1d/h2qORAsejiFc7zb+SEmYPn1yDZzEDSU5PmDkmVLQ==",
-            "resolved": "https://registry.npmjs.org/jest-environment-node/-/jest-environment-node-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-YGdFeZ3T9a+/612c5mTQIllvWkddPbYcN2v95ZH24oWMbGA4GGS2XdIF92QMhUhvrjjuQWYgUGW2zawOyH63MQ==",
+            "resolved": "https://registry.npmjs.org/jest-environment-node/-/jest-environment-node-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-get-type": {
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
             "integrity": "sha512-J5Xez4nRRMjk8emnTpWrlkyb9pfRQQanDrvWHhsR1+VUfbwxi30eVcZFlcdGInRibU4G5LwHXpI7IRHU0CY+gg==",
@@ -7641,57 +7643,57 @@
                 "@jest/types": "^29.6.1",
                 "@types/graceful-fs": "^4.1.3",
                 "@types/node": "*",
                 "anymatch": "^3.0.3",
                 "fb-watchman": "^2.0.0",
                 "graceful-fs": "^4.2.9",
                 "jest-regex-util": "^29.4.3",
-                "jest-util": "^29.6.1",
-                "jest-worker": "^29.6.1",
+                "jest-util": "^29.6.2",
+                "jest-worker": "^29.6.2",
                 "micromatch": "^4.0.4",
                 "walker": "^1.0.8"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-0m7f9PZXxOCk1gRACiVgX85knUKPKLPg4oRCjLoqIm9brTHXaorMA0JpmtmVkQiT8nmXyIVoZd/nnH1cfC33ig==",
+            "integrity": "sha512-+51XleTDAAysvU8rT6AnS1ZJ+WHVNqhj1k6nTvN2PYP+HjU3kqlaKQ1Lnw3NYW3bm2r8vq82X0Z1nDDHZMzHVA==",
             "optionalDependencies": {
                 "fsevents": "^2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/jest-haste-map/-/jest-haste-map-29.6.1.tgz",
-            "version": "29.6.1"
+            "resolved": "https://registry.npmjs.org/jest-haste-map/-/jest-haste-map-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-leak-detector": {
             "dependencies": {
                 "jest-get-type": "^29.4.3",
-                "pretty-format": "^29.6.1"
+                "pretty-format": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-OrxMNyZirpOEwkF3UHnIkAiZbtkBWiye+hhBweCHkVbCgyEy71Mwbb5zgeTNYWJBi1qgDVfPC1IwO9dVEeTLwQ==",
-            "resolved": "https://registry.npmjs.org/jest-leak-detector/-/jest-leak-detector-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-aNqYhfp5uYEO3tdWMb2bfWv6f0b4I0LOxVRpnRLAeque2uqOVVMLh6khnTcE2qJ5wAKop0HcreM1btoysD6bPQ==",
+            "resolved": "https://registry.npmjs.org/jest-leak-detector/-/jest-leak-detector-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-matcher-utils": {
             "dependencies": {
                 "chalk": "^4.0.0",
-                "jest-diff": "^29.6.1",
+                "jest-diff": "^29.6.2",
                 "jest-get-type": "^29.4.3",
-                "pretty-format": "^29.6.1"
+                "pretty-format": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-SLaztw9d2mfQQKHmJXKM0HCbl2PPVld/t9Xa6P9sgiExijviSp7TnZZpw2Fpt+OI3nwUO/slJbOfzfUMKKC5QA==",
-            "resolved": "https://registry.npmjs.org/jest-matcher-utils/-/jest-matcher-utils-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-4LiAk3hSSobtomeIAzFTe+N8kL6z0JtF3n6I4fg29iIW7tt99R7ZcIFW34QkX+DuVrf+CUe6wuVOpm7ZKFJzZQ==",
+            "resolved": "https://registry.npmjs.org/jest-matcher-utils/-/jest-matcher-utils-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-matcher-utils/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7757,25 +7759,25 @@
             "dependencies": {
                 "@babel/code-frame": "^7.12.13",
                 "@jest/types": "^29.6.1",
                 "@types/stack-utils": "^2.0.0",
                 "chalk": "^4.0.0",
                 "graceful-fs": "^4.2.9",
                 "micromatch": "^4.0.4",
-                "pretty-format": "^29.6.1",
+                "pretty-format": "^29.6.2",
                 "slash": "^3.0.0",
                 "stack-utils": "^2.0.3"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-KoAW2zAmNSd3Gk88uJ56qXUWbFk787QKmjjJVOjtGFmmGSZgDBrlIL4AfQw1xyMYPNVD7dNInfIbur9B2rd/wQ==",
-            "resolved": "https://registry.npmjs.org/jest-message-util/-/jest-message-util-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-vnIGYEjoPSuRqV8W9t+Wow95SDp6KPX2Uf7EoeG9G99J2OVh7OSwpS4B6J0NfpEIpfkBNHlBZpA2rblEuEFhZQ==",
+            "resolved": "https://registry.npmjs.org/jest-message-util/-/jest-message-util-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-message-util/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7846,23 +7848,23 @@
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-mock": {
             "dependencies": {
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
-                "jest-util": "^29.6.1"
+                "jest-util": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-brovyV9HBkjXAEdRooaTQK42n8usKoSRR3gihzUpYeV/vwqgSoNfrksO7UfSACnPmxasO/8TmHM3w9Hp3G1dgw==",
-            "resolved": "https://registry.npmjs.org/jest-mock/-/jest-mock-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-hoSv3lb3byzdKfwqCuT6uTscan471GUECqgNYykg6ob0yiAw3zYc7OrPnI9Qv8Wwoa4lC7AZ9hyS4AiIx5U2zg==",
+            "resolved": "https://registry.npmjs.org/jest-mock/-/jest-mock-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-pnp-resolver": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-+3NpwQEnRoIBtx4fyhblQDPgJI0H1IEIkX7ShLUjPGA7TtUTvI1oiKi3SR4oBR0hQhQR80l4WAe5RrXBwWMA8w==",
@@ -7886,42 +7888,42 @@
             "resolved": "https://registry.npmjs.org/jest-regex-util/-/jest-regex-util-29.4.3.tgz",
             "version": "29.4.3"
         },
         "node_modules/jest-resolve": {
             "dependencies": {
                 "chalk": "^4.0.0",
                 "graceful-fs": "^4.2.9",
-                "jest-haste-map": "^29.6.1",
+                "jest-haste-map": "^29.6.2",
                 "jest-pnp-resolver": "^1.2.2",
-                "jest-util": "^29.6.1",
-                "jest-validate": "^29.6.1",
+                "jest-util": "^29.6.2",
+                "jest-validate": "^29.6.2",
                 "resolve": "^1.20.0",
                 "resolve.exports": "^2.0.0",
                 "slash": "^3.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-AeRkyS8g37UyJiP9w3mmI/VXU/q8l/IH52vj/cDAyScDcemRbSBhfX/NMYIGilQgSVwsjxrCHf3XJu4f+lxCMg==",
-            "resolved": "https://registry.npmjs.org/jest-resolve/-/jest-resolve-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-G/iQUvZWI5e3SMFssc4ug4dH0aZiZpsDq9o1PtXTV1210Ztyb2+w+ZgQkB3iOiC5SmAEzJBOHWz6Hvrd+QnNPw==",
+            "resolved": "https://registry.npmjs.org/jest-resolve/-/jest-resolve-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-resolve-dependencies": {
             "dependencies": {
                 "jest-regex-util": "^29.4.3",
-                "jest-snapshot": "^29.6.1"
+                "jest-snapshot": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-BbFvxLXtcldaFOhNMXmHRWx1nXQO5LoXiKSGQcA1LxxirYceZT6ch8KTE1bK3X31TNG/JbkI7OkS/ABexVahiw==",
-            "resolved": "https://registry.npmjs.org/jest-resolve-dependencies/-/jest-resolve-dependencies-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-LGqjDWxg2fuQQm7ypDxduLu/m4+4Lb4gczc13v51VMZbVP5tSBILqVx8qfWcsdP8f0G7aIqByIALDB0R93yL+w==",
+            "resolved": "https://registry.npmjs.org/jest-resolve-dependencies/-/jest-resolve-dependencies-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-resolve/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -7990,43 +7992,43 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-runner": {
             "dependencies": {
-                "@jest/console": "^29.6.1",
-                "@jest/environment": "^29.6.1",
-                "@jest/test-result": "^29.6.1",
-                "@jest/transform": "^29.6.1",
+                "@jest/console": "^29.6.2",
+                "@jest/environment": "^29.6.2",
+                "@jest/test-result": "^29.6.2",
+                "@jest/transform": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
                 "emittery": "^0.13.1",
                 "graceful-fs": "^4.2.9",
                 "jest-docblock": "^29.4.3",
-                "jest-environment-node": "^29.6.1",
-                "jest-haste-map": "^29.6.1",
-                "jest-leak-detector": "^29.6.1",
-                "jest-message-util": "^29.6.1",
-                "jest-resolve": "^29.6.1",
-                "jest-runtime": "^29.6.1",
-                "jest-util": "^29.6.1",
-                "jest-watcher": "^29.6.1",
-                "jest-worker": "^29.6.1",
+                "jest-environment-node": "^29.6.2",
+                "jest-haste-map": "^29.6.2",
+                "jest-leak-detector": "^29.6.2",
+                "jest-message-util": "^29.6.2",
+                "jest-resolve": "^29.6.2",
+                "jest-runtime": "^29.6.2",
+                "jest-util": "^29.6.2",
+                "jest-watcher": "^29.6.2",
+                "jest-worker": "^29.6.2",
                 "p-limit": "^3.1.0",
                 "source-map-support": "0.5.13"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-tw0wb2Q9yhjAQ2w8rHRDxteryyIck7gIzQE4Reu3JuOBpGp96xWgF0nY8MDdejzrLCZKDcp8JlZrBN/EtkQvPQ==",
-            "resolved": "https://registry.npmjs.org/jest-runner/-/jest-runner-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-wXOT/a0EspYgfMiYHxwGLPCZfC0c38MivAlb2lMEAlwHINKemrttu1uSbcGbfDV31sFaPWnWJPmb2qXM8pqZ4w==",
+            "resolved": "https://registry.npmjs.org/jest-runner/-/jest-runner-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-runner/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8105,44 +8107,44 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-runtime": {
             "dependencies": {
-                "@jest/environment": "^29.6.1",
-                "@jest/fake-timers": "^29.6.1",
-                "@jest/globals": "^29.6.1",
+                "@jest/environment": "^29.6.2",
+                "@jest/fake-timers": "^29.6.2",
+                "@jest/globals": "^29.6.2",
                 "@jest/source-map": "^29.6.0",
-                "@jest/test-result": "^29.6.1",
-                "@jest/transform": "^29.6.1",
+                "@jest/test-result": "^29.6.2",
+                "@jest/transform": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
                 "cjs-module-lexer": "^1.0.0",
                 "collect-v8-coverage": "^1.0.0",
                 "glob": "^7.1.3",
                 "graceful-fs": "^4.2.9",
-                "jest-haste-map": "^29.6.1",
-                "jest-message-util": "^29.6.1",
-                "jest-mock": "^29.6.1",
+                "jest-haste-map": "^29.6.2",
+                "jest-message-util": "^29.6.2",
+                "jest-mock": "^29.6.2",
                 "jest-regex-util": "^29.4.3",
-                "jest-resolve": "^29.6.1",
-                "jest-snapshot": "^29.6.1",
-                "jest-util": "^29.6.1",
+                "jest-resolve": "^29.6.2",
+                "jest-snapshot": "^29.6.2",
+                "jest-util": "^29.6.2",
                 "slash": "^3.0.0",
                 "strip-bom": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-D6/AYOA+Lhs5e5il8+5pSLemjtJezUr+8zx+Sn8xlmOux3XOqx4d8l/2udBea8CRPqqrzhsKUsN/gBDE/IcaPQ==",
-            "resolved": "https://registry.npmjs.org/jest-runtime/-/jest-runtime-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-2X9dqK768KufGJyIeLmIzToDmsN0m7Iek8QNxRSI/2+iPFYHF0jTwlO3ftn7gdKd98G/VQw9XJCk77rbTGZnJg==",
+            "resolved": "https://registry.npmjs.org/jest-runtime/-/jest-runtime-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-runtime/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8216,38 +8218,37 @@
         "node_modules/jest-snapshot": {
             "dependencies": {
                 "@babel/core": "^7.11.6",
                 "@babel/generator": "^7.7.2",
                 "@babel/plugin-syntax-jsx": "^7.7.2",
                 "@babel/plugin-syntax-typescript": "^7.7.2",
                 "@babel/types": "^7.3.3",
-                "@jest/expect-utils": "^29.6.1",
-                "@jest/transform": "^29.6.1",
+                "@jest/expect-utils": "^29.6.2",
+                "@jest/transform": "^29.6.2",
                 "@jest/types": "^29.6.1",
-                "@types/prettier": "^2.1.5",
                 "babel-preset-current-node-syntax": "^1.0.0",
                 "chalk": "^4.0.0",
-                "expect": "^29.6.1",
+                "expect": "^29.6.2",
                 "graceful-fs": "^4.2.9",
-                "jest-diff": "^29.6.1",
+                "jest-diff": "^29.6.2",
                 "jest-get-type": "^29.4.3",
-                "jest-matcher-utils": "^29.6.1",
-                "jest-message-util": "^29.6.1",
-                "jest-util": "^29.6.1",
+                "jest-matcher-utils": "^29.6.2",
+                "jest-message-util": "^29.6.2",
+                "jest-util": "^29.6.2",
                 "natural-compare": "^1.4.0",
-                "pretty-format": "^29.6.1",
+                "pretty-format": "^29.6.2",
                 "semver": "^7.5.3"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-G4UQE1QQ6OaCgfY+A0uR1W2AY0tGXUPQpoUClhWHq1Xdnx1H6JOrC2nH5lqnOEqaDgbHFgIwZ7bNq24HpB180A==",
-            "resolved": "https://registry.npmjs.org/jest-snapshot/-/jest-snapshot-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-1OdjqvqmRdGNvWXr/YZHuyhh5DeaLp1p/F8Tht/MrMw4Kr1Uu/j4lRG+iKl1DAqUJDWxtQBMk41Lnf/JETYBRA==",
+            "resolved": "https://registry.npmjs.org/jest-snapshot/-/jest-snapshot-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-snapshot/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8351,17 +8352,17 @@
                 "graceful-fs": "^4.2.9",
                 "picomatch": "^2.2.3"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-NRFCcjc+/uO3ijUVyNOQJluf8PtGCe/W6cix36+M3cTFgiYqFOOW5MgN4JOOcvbUhcKTYVd1CvHz/LWi8d16Mg==",
-            "resolved": "https://registry.npmjs.org/jest-util/-/jest-util-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-3eX1qb6L88lJNCFlEADKOkjpXJQyZRiavX1INZ4tRnrBVr2COd3RgcTLyUiEXMNBlDU/cgYq6taUS0fExrWW4w==",
+            "resolved": "https://registry.npmjs.org/jest-util/-/jest-util-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-util/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8426,23 +8427,23 @@
         "node_modules/jest-validate": {
             "dependencies": {
                 "@jest/types": "^29.6.1",
                 "camelcase": "^6.2.0",
                 "chalk": "^4.0.0",
                 "jest-get-type": "^29.4.3",
                 "leven": "^3.1.0",
-                "pretty-format": "^29.6.1"
+                "pretty-format": "^29.6.2"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-r3Ds69/0KCN4vx4sYAbGL1EVpZ7MSS0vLmd3gV78O+NAx3PDQQukRU5hNHPXlyqCgFY8XUk7EuTMLugh0KzahA==",
-            "resolved": "https://registry.npmjs.org/jest-validate/-/jest-validate-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-vGz0yMN5fUFRRbpJDPwxMpgSXW1LDKROHfBopAvDcmD6s+B/s8WJrwi+4bfH4SdInBA5C3P3BI19dBtKzx1Arg==",
+            "resolved": "https://registry.npmjs.org/jest-validate/-/jest-validate-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-validate/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8514,30 +8515,30 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-watcher": {
             "dependencies": {
-                "@jest/test-result": "^29.6.1",
+                "@jest/test-result": "^29.6.2",
                 "@jest/types": "^29.6.1",
                 "@types/node": "*",
                 "ansi-escapes": "^4.2.1",
                 "chalk": "^4.0.0",
                 "emittery": "^0.13.1",
-                "jest-util": "^29.6.1",
+                "jest-util": "^29.6.2",
                 "string-length": "^4.0.1"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-d4wpjWTS7HEZPaaj8m36QiaP856JthRZkrgcIY/7ISoUWPIillrXM23WPboZVLbiwZBt4/qn2Jke84Sla6JhFA==",
-            "resolved": "https://registry.npmjs.org/jest-watcher/-/jest-watcher-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-GZitlqkMkhkefjfN/p3SJjrDaxPflqxEAv3/ik10OirZqJGYH5rPiIsgVcfof0Tdqg3shQGdEIxDBx+B4tuLzA==",
+            "resolved": "https://registry.npmjs.org/jest-watcher/-/jest-watcher-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-watcher/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -8598,25 +8599,25 @@
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/jest-worker": {
             "dependencies": {
                 "@types/node": "*",
-                "jest-util": "^29.6.1",
+                "jest-util": "^29.6.2",
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-U+Wrbca7S8ZAxAe9L6nb6g8kPdia5hj32Puu5iOqBCMTMWFHXuK6dOV2IFrpedbTV8fjMFLdWNttQTBL6u2MRA==",
-            "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-l3ccBOabTdkng8I/ORCkADz4eSMKejTYv1vB/Z83UiubqhC1oQ5Li6dWCyqOIvSifGjUBxuvxvlm6KGK2DtuAQ==",
+            "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/jest-worker/node_modules/has-flag": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
@@ -10293,17 +10294,17 @@
                 "ansi-styles": "^5.0.0",
                 "react-is": "^18.0.0"
             },
             "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
-            "integrity": "sha512-7jRj+yXO0W7e4/tSJKoR7HRIHLPPjtNaUGG2xxKQnGvPNRkgWcQ0AZX6P4KBRJN4FcTBWb3sa7DVUJmocYuoog==",
-            "resolved": "https://registry.npmjs.org/pretty-format/-/pretty-format-29.6.1.tgz",
-            "version": "29.6.1"
+            "integrity": "sha512-1q0oC8eRveTg5nnBEWMXAU2qpv65Gnuf2eCQzSjxpWFkPaPARwqZZDGuNE0zPAZfTCHzIk3A8dIjwlQKKLphyg==",
+            "resolved": "https://registry.npmjs.org/pretty-format/-/pretty-format-29.6.2.tgz",
+            "version": "29.6.2"
         },
         "node_modules/pretty-format/node_modules/ansi-styles": {
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "funding": {
```

### Comparing `ixbrl-viewer-1.3.0/package.json` & `ixbrl-viewer-1.4.0/package.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/pyproject.toml` & `ixbrl-viewer-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/Makefile` & `ixbrl-viewer-1.4.0/samples/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/Makefile-src` & `ixbrl-viewer-1.4.0/samples/Makefile-src`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/build-viewer.py` & `ixbrl-viewer-1.4.0/samples/build-viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from arelle.ModelFormulaObject import FormulaOptions
 import os
 import sys
 import glob
 import argparse
 import iXBRLViewerPlugin.iXBRLViewer
 from arelle.plugin import inlineXbrlDocumentSet
-from iXBRLViewerPlugin import generateViewer, getFeaturesFromOptions, VIEWER_FEATURES_AND_DESCRIPTIONS
+from iXBRLViewerPlugin import generateViewer, getFeaturesFromOptions, FEATURE_CONFIGS
 
 class CntlrCreateViewer(Cntlr.Cntlr):
 
     def __init__(self):
         super(CntlrCreateViewer, self).__init__(hasGui=False)
 
     def loadPackagesFromDir(self, directory):
@@ -67,17 +67,17 @@
 parser.add_argument("--out", "-o", help="File or directory to write output to", default="viewer.html")
 parser.add_argument("--use-stub-viewer",
                     action="store_true",
                     help="Use stub viewer for faster loading of inspector (requires web server)")
 parser.add_argument('files', metavar='FILES', nargs='+',
                     help='Files to process')
 featureGroup = parser.add_argument_group('Viewer Features')
-for featureName, featureDescription in VIEWER_FEATURES_AND_DESCRIPTIONS.items():
-    arg = f'--viewer-feature-{featureName}'
-    featureGroup.add_argument(arg, arg.lower(), action="store_true", default=False, help=featureDescription)
+for featureConfig in FEATURE_CONFIGS:
+    arg = f'--viewer-feature-{featureConfig.key}'
+    featureGroup.add_argument(arg, arg.lower(), action="store_true", default=False, help=featureConfig.description)
 
 args = parser.parse_args()
 
 cntlr = CntlrCreateViewer()
 cntlr.startLogging(
     logFileName='logToPrint',
     logFormat="[%(messageCode)s] %(message)s - %(file)s",
```

### Comparing `ixbrl-viewer-1.3.0/samples/fetch-sample-files.py` & `ixbrl-viewer-1.4.0/samples/fetch-sample-files.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/sample-files.list` & `ixbrl-viewer-1.4.0/samples/sample-files.list`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/continuation/continuation.html` & `ixbrl-viewer-1.4.0/samples/src/continuation/continuation.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/ixds-test/document1.html` & `ixbrl-viewer-1.4.0/samples/src/ixds-test/document1.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/ixds-test/faurecia.html` & `ixbrl-viewer-1.4.0/samples/src/ixds-test/faurecia.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/ixds-test/valeo.html` & `ixbrl-viewer-1.4.0/samples/src/ixds-test/valeo.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/scrollable-div/scrollable-div.html` & `ixbrl-viewer-1.4.0/samples/src/scrollable-div/scrollable-div.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html` & `ixbrl-viewer-1.4.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/core_elements.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/core_elements.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/doc_frame.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/doc_frame.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/fact_details_panel.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/fact_details_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/search_panel.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/search_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/toolbar.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/page_objects/toolbar.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/framework/viewer_page.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/framework/viewer_page.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg` & `ixbrl-viewer-1.4.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip` & `ixbrl-viewer-1.4.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/highlights.zip` & `ixbrl-viewer-1.4.0/tests/puppeteer/test_filings/highlights.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/tests/fact_properties.test.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/tests/fact_properties.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/tests/highlight.test.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/tests/highlight.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/puppeteer/tests/search.test.js` & `ixbrl-viewer-1.4.0/tests/puppeteer/tests/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py` & `ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py` & `ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py` & `ixbrl-viewer-1.4.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py`

 * *Files identical despite different names*

