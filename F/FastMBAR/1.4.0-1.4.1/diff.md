# Comparing `tmp/fastmbar-1.4.0.tar.gz` & `tmp/fastmbar-1.4.1.tar.gz`

## Comparing `fastmbar-1.4.0.tar` & `fastmbar-1.4.1.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastmbar-1.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.4.0/.travis.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastmbar-1.4.0/build.sh
--rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.4.0/energy_matrix.pdf
--rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.0/energy_matrix.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fastmbar-1.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.4.0/FastMBAR/__init__.py
--rw-r--r--   0        0        0    29168 2020-02-02 00:00:00.000000 fastmbar-1.4.0/FastMBAR/fastmbar.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.4.0/FastMBAR/test_FastMBAR.py
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.4.0/FastMBAR/utils/analyzer.py
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.4.0/FastMBAR/utils/fastmbartools.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/.gitignore
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/Makefile
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/requirements.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.buildinfo
--rw-r--r--   0        0        0    30535 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/API.html
--rw-r--r--   0        0        0    56378 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/butane_PMF.html
--rw-r--r--   0        0        0    67565 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/dialanine_PMF.html
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/examples.html
--rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/genindex.html
--rw-r--r--   0        0        0    16014 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/index.html
--rw-r--r--   0        0        0    36805 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/installation.html
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/objects.inv
--rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/references.html
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/search.html
--rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/searchindex.js
--rw-r--r--   0        0        0    26667 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/usage.html
--rw-r--r--   0        0        0    68887 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/API.doctree
--rw-r--r--   0        0        0    41990 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/butane_PMF.doctree
--rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/dialanine_PMF.doctree
--rw-r--r--   0        0        0    61703 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/environment.pickle
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/examples.doctree
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/index.doctree
--rw-r--r--   0        0        0    33251 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/installation.doctree
--rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/references.doctree
--rw-r--r--   0        0        0    28287 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/.doctrees/usage.doctree
--rw-r--r--   0        0        0   187708 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/Fig_1.png
--rw-r--r--   0        0        0   211402 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/Fig_11.png
--rw-r--r--   0        0        0   172324 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/Fig_2.png
--rw-r--r--   0        0        0   193626 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/Fig_21.png
--rw-r--r--   0        0        0   156671 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/PMF.png
--rw-r--r--   0        0        0   116954 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/PMF1.png
--rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_images/energy_matrix.png
--rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_modules/index.html
--rw-r--r--   0        0        0   125331 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_modules/FastMBAR/fastmbar.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/API.rst
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/butane_PMF.rst
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/dialanine_PMF.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/examples.rst
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/index.rst
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/installation.rst
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/references.rst
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_sources/usage.rst
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/basic.css
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/clipboard.min.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/copy-button.svg
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/copybutton.css
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/copybutton.js
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/doctools.js
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/language_data.js
--rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/logo.ai
--rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/logo.eps
--rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/logo.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/plus.png
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    17088 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/underscore.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/webpack-macros.html
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/styles/bootstrap.css
--rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/API.rst
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/butane_PMF.rst
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/conf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/dialanine_PMF.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/examples.rst
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/index.rst
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/references.rst
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/usage.rst
--rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/_static/logo.ai
--rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/_static/logo.eps
--rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.0/docs/source/_static/logo.png
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.4.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.4.0/LICENSE
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastmbar-1.4.0/README.rst
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fastmbar-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastmbar-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastmbar-1.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.4.1/.travis.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastmbar-1.4.1/build.sh
+-rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.4.1/energy_matrix.pdf
+-rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.1/energy_matrix.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fastmbar-1.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.4.1/FastMBAR/__init__.py
+-rw-r--r--   0        0        0    29951 2020-02-02 00:00:00.000000 fastmbar-1.4.1/FastMBAR/fastmbar.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.4.1/FastMBAR/test_FastMBAR.py
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.4.1/FastMBAR/utils/analyzer.py
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.4.1/FastMBAR/utils/fastmbartools.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/.gitignore
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/Makefile
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/requirements.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.buildinfo
+-rw-r--r--   0        0        0    30535 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/API.html
+-rw-r--r--   0        0        0    56378 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/butane_PMF.html
+-rw-r--r--   0        0        0    67565 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/dialanine_PMF.html
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/examples.html
+-rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/genindex.html
+-rw-r--r--   0        0        0    16014 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/index.html
+-rw-r--r--   0        0        0    36805 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/installation.html
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/objects.inv
+-rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/references.html
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/search.html
+-rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/searchindex.js
+-rw-r--r--   0        0        0    26667 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/usage.html
+-rw-r--r--   0        0        0    68887 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/API.doctree
+-rw-r--r--   0        0        0    41990 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/butane_PMF.doctree
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/dialanine_PMF.doctree
+-rw-r--r--   0        0        0    61703 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/examples.doctree
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/index.doctree
+-rw-r--r--   0        0        0    33251 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/installation.doctree
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/references.doctree
+-rw-r--r--   0        0        0    28287 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/.doctrees/usage.doctree
+-rw-r--r--   0        0        0   187708 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/Fig_1.png
+-rw-r--r--   0        0        0   211402 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/Fig_11.png
+-rw-r--r--   0        0        0   172324 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/Fig_2.png
+-rw-r--r--   0        0        0   193626 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/Fig_21.png
+-rw-r--r--   0        0        0   156671 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/PMF.png
+-rw-r--r--   0        0        0   116954 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/PMF1.png
+-rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_images/energy_matrix.png
+-rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_modules/index.html
+-rw-r--r--   0        0        0   125331 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_modules/FastMBAR/fastmbar.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/API.rst
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/butane_PMF.rst
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/dialanine_PMF.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/examples.rst
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/index.rst
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/installation.rst
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/references.rst
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_sources/usage.rst
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/doctools.js
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/language_data.js
+-rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/logo.ai
+-rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/logo.eps
+-rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/logo.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/plus.png
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    17088 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/underscore.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/webpack-macros.html
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/API.rst
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/butane_PMF.rst
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/conf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/dialanine_PMF.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/examples.rst
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/index.rst
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/references.rst
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/usage.rst
+-rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/_static/logo.ai
+-rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/_static/logo.eps
+-rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.1/docs/source/_static/logo.png
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.4.1/LICENSE
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastmbar-1.4.1/README.rst
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fastmbar-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastmbar-1.4.1/PKG-INFO
```

### Comparing `fastmbar-1.4.0/.readthedocs.yaml` & `fastmbar-1.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/energy_matrix.pdf` & `fastmbar-1.4.1/energy_matrix.pdf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/energy_matrix.png` & `fastmbar-1.4.1/energy_matrix.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/FastMBAR/fastmbar.py` & `fastmbar-1.4.1/FastMBAR/fastmbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             raise TypeError("method has to be a string.")
         if method not in ["Newton", "L-BFGS-B"]:
             raise ValueError("method has to be Newton or L-BFGS-B.")
         self.method = method
 
         ## solve the MBAR equation
         if self.bootstrap is False:
-            dF_init = self.energy.new_zeros(self.M - 1)
+            dF_init = self._initialize_dF(self.energy, self.num_conf)
             dF = _solve_mbar(
                 dF_init.to(self.device),
                 self.energy.to(self.device),
                 self.num_conf.to(self.device),
                 self.method,
                 self._batch_size,
                 verbose=self.verbose,
@@ -249,15 +249,15 @@
                 - 2 * self._F_cov
             )
             self._DeltaF_std = self._DeltaF_cov.sqrt()
 
         elif self.bootstrap is True:
             dFs = []
             log_prob_mix = []
-            dF_init = self.energy.new_zeros(self.M - 1)
+            dF_init = self._initialize_dF(self.energy, self.num_conf)
             self._conf_idx = []
             for _ in range(self.bootstrap_num_rep):
                 conf_idx = _bootstrap_conf_idx(
                     self.num_conf.to(torch.int64), self.bootstrap_block_size
                 )
                 dF = _solve_mbar(
                     dF_init.to(self.device),
@@ -337,14 +337,29 @@
         return self._DeltaF_std.cpu().numpy()
 
     @property
     def log_prob_mix(self) -> np.ndarray:
         """the log probability density of conformations in the mixture distribution."""
         return self._log_prob_mix.cpu().numpy()
 
+    def _initialize_dF(self, energy, num_conf):
+        ## Initilize dF by self-consistent iteration
+        ## this is only required by the Newton's method, becuase when the inital guess
+        ## is far away from the true solution, the Hessian matrix can be very close to
+        ## singular due to underflow. This can be avoided by using a good initial guess.
+        dF_init = energy.new_zeros(self.M - 1)
+        for _ in range(10):
+            F_init = torch.cat([dF_init.new_zeros(1), dF_init])
+            b = - F_init - torch.log(num_conf)
+            log_prob_mix = torch.logsumexp(-(energy + b[:, None]), dim=0)
+            du = energy + log_prob_mix
+            F = -torch.logsumexp(-du, dim=1)
+            dF_init = F[1:] - F[0]
+        return dF_init
+
     def calculate_free_energies_of_perturbed_states(self, energy_perturbed):
         """calculate free energies for perturbed states.
 
         Parameters
         -----------
         energy_perturbed: 2-D float ndarray with size of (L,N)
             each row of the energy_perturbed matrix represents a state and
@@ -354,19 +369,19 @@
         Returns
         -------
         results: dict
             a dictionary containing the following keys:
 
             **F** - the free energy of the perturbed states.
 
-            **F_std** - the standard deviation of the free energy of the perturbed states. 
+            **F_std** - the standard deviation of the free energy of the perturbed states.
 
             **F_cov** - the covariance between the free energies of the perturbed states.
 
-            **DeltaF** - :math:`\mathrm{DeltaF}[k,l]` is the free energy difference between state            
+            **DeltaF** - :math:`\mathrm{DeltaF}[k,l]` is the free energy difference between state
             :math:`k` and state :math:`l`, i.e., :math:`\mathrm{DeltaF}[k,l] = F[l] - F[k]` .
 
             **DeltaF_std** - the standard deviation of the free energy difference.
         """
 
         if isinstance(energy_perturbed, np.ndarray):
             energy_perturbed = energy_perturbed.astype(np.float64)
@@ -430,14 +445,15 @@
             "F_cov": F_cov.numpy(),
             "DeltaF": DeltaF.numpy(),
             "DeltaF_std": DeltaF_std.numpy(),
         }
 
         return results
 
+
 def _compute_logp_of_F(F, energy, num_conf):
     logp = (
         torch.sum(num_conf * F)
         - torch.logsumexp(-(energy.T - torch.log(num_conf) - F), dim=1).sum()
     )
     return logp
```

### Comparing `fastmbar-1.4.0/FastMBAR/test_FastMBAR.py` & `fastmbar-1.4.1/FastMBAR/test_FastMBAR.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/FastMBAR/utils/analyzer.py` & `fastmbar-1.4.1/FastMBAR/utils/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/FastMBAR/utils/fastmbartools.py` & `fastmbar-1.4.1/FastMBAR/utils/fastmbartools.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/Makefile` & `fastmbar-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/API.html` & `fastmbar-1.4.1/docs/build/API.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/butane_PMF.html` & `fastmbar-1.4.1/docs/build/butane_PMF.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/dialanine_PMF.html` & `fastmbar-1.4.1/docs/build/dialanine_PMF.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/examples.html` & `fastmbar-1.4.1/docs/build/examples.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/genindex.html` & `fastmbar-1.4.1/docs/build/genindex.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/index.html` & `fastmbar-1.4.1/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/installation.html` & `fastmbar-1.4.1/docs/build/installation.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/references.html` & `fastmbar-1.4.1/docs/build/references.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/search.html` & `fastmbar-1.4.1/docs/build/search.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/searchindex.js` & `fastmbar-1.4.1/docs/build/searchindex.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/usage.html` & `fastmbar-1.4.1/docs/build/usage.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/API.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/API.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/butane_PMF.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/butane_PMF.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/dialanine_PMF.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/dialanine_PMF.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/environment.pickle` & `fastmbar-1.4.1/docs/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/examples.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/index.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/installation.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/references.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/references.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/.doctrees/usage.doctree` & `fastmbar-1.4.1/docs/build/.doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/Fig_1.png` & `fastmbar-1.4.1/docs/build/_images/Fig_1.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/Fig_11.png` & `fastmbar-1.4.1/docs/build/_images/Fig_11.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/Fig_2.png` & `fastmbar-1.4.1/docs/build/_images/Fig_2.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/Fig_21.png` & `fastmbar-1.4.1/docs/build/_images/Fig_21.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/PMF.png` & `fastmbar-1.4.1/docs/build/_images/PMF.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/PMF1.png` & `fastmbar-1.4.1/docs/build/_images/PMF1.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_images/energy_matrix.png` & `fastmbar-1.4.1/docs/build/_images/energy_matrix.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_modules/index.html` & `fastmbar-1.4.1/docs/build/_modules/index.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_modules/FastMBAR/fastmbar.html` & `fastmbar-1.4.1/docs/build/_modules/FastMBAR/fastmbar.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/butane_PMF.rst` & `fastmbar-1.4.1/docs/build/_sources/butane_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/dialanine_PMF.rst` & `fastmbar-1.4.1/docs/build/_sources/dialanine_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/examples.rst` & `fastmbar-1.4.1/docs/build/_sources/examples.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/index.rst` & `fastmbar-1.4.1/docs/build/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/installation.rst` & `fastmbar-1.4.1/docs/build/_sources/installation.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/references.rst` & `fastmbar-1.4.1/docs/build/_sources/references.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_sources/usage.rst` & `fastmbar-1.4.1/docs/build/_sources/usage.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/_sphinx_javascript_frameworks_compat.js` & `fastmbar-1.4.1/docs/build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/basic.css` & `fastmbar-1.4.1/docs/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/clipboard.min.js` & `fastmbar-1.4.1/docs/build/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/copybutton.css` & `fastmbar-1.4.1/docs/build/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/copybutton.js` & `fastmbar-1.4.1/docs/build/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/copybutton_funcs.js` & `fastmbar-1.4.1/docs/build/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/doctools.js` & `fastmbar-1.4.1/docs/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/jquery-3.6.0.js` & `fastmbar-1.4.1/docs/build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/jquery.js` & `fastmbar-1.4.1/docs/build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/language_data.js` & `fastmbar-1.4.1/docs/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/logo.ai` & `fastmbar-1.4.1/docs/build/_static/logo.ai`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/logo.eps` & `fastmbar-1.4.1/docs/build/_static/logo.eps`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/logo.png` & `fastmbar-1.4.1/docs/build/_static/logo.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/pygments.css` & `fastmbar-1.4.1/docs/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/searchtools.js` & `fastmbar-1.4.1/docs/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/underscore-1.13.1.js` & `fastmbar-1.4.1/docs/build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/underscore.js` & `fastmbar-1.4.1/docs/build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/webpack-macros.html` & `fastmbar-1.4.1/docs/build/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/images/logo_binder.svg` & `fastmbar-1.4.1/docs/build/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/images/logo_colab.png` & `fastmbar-1.4.1/docs/build/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/images/logo_deepnote.svg` & `fastmbar-1.4.1/docs/build/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/images/logo_jupyterhub.svg` & `fastmbar-1.4.1/docs/build/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo` & `fastmbar-1.4.1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `fastmbar-1.4.1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/bootstrap.js` & `fastmbar-1.4.1/docs/build/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/bootstrap.js.map` & `fastmbar-1.4.1/docs/build/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/pydata-sphinx-theme.js` & `fastmbar-1.4.1/docs/build/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/pydata-sphinx-theme.js.map` & `fastmbar-1.4.1/docs/build/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/sphinx-book-theme.js` & `fastmbar-1.4.1/docs/build/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/scripts/sphinx-book-theme.js.map` & `fastmbar-1.4.1/docs/build/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/styles/bootstrap.css` & `fastmbar-1.4.1/docs/build/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/styles/pydata-sphinx-theme.css` & `fastmbar-1.4.1/docs/build/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/styles/sphinx-book-theme.css` & `fastmbar-1.4.1/docs/build/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `fastmbar-1.4.1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/butane_PMF.rst` & `fastmbar-1.4.1/docs/source/butane_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/conf.py` & `fastmbar-1.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/dialanine_PMF.rst` & `fastmbar-1.4.1/docs/source/dialanine_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/examples.rst` & `fastmbar-1.4.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/index.rst` & `fastmbar-1.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/installation.rst` & `fastmbar-1.4.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/references.rst` & `fastmbar-1.4.1/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/usage.rst` & `fastmbar-1.4.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/_static/logo.ai` & `fastmbar-1.4.1/docs/source/_static/logo.ai`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/_static/logo.eps` & `fastmbar-1.4.1/docs/source/_static/logo.eps`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/docs/source/_static/logo.png` & `fastmbar-1.4.1/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/LICENSE` & `fastmbar-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/README.rst` & `fastmbar-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.0/pyproject.toml` & `fastmbar-1.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FastMBAR"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Xinqiang Ding", email="Xinqiang.Ding@tufts.edu" }
 ]
 description = "A fast solver for large scale MBAR/UWHAM equations"
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `fastmbar-1.4.0/PKG-INFO` & `fastmbar-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastMBAR
-Version: 1.4.0
+Version: 1.4.1
 Summary: A fast solver for large scale MBAR/UWHAM equations
 Project-URL: Homepage, https://fastmbar.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/BrooksResearchGroup-UM/FastMBAR/issues
 Author-email: Xinqiang Ding <Xinqiang.Ding@tufts.edu>
 License: MIT License
         
         Copyright (c) 2018 Xinqiang Ding, Charles L. Brooks III
```

