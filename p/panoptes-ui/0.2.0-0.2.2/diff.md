# Comparing `tmp/panoptes-ui-0.2.0.tar.gz` & `tmp/panoptes-ui-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panoptes-ui-0.2.0.tar", last modified: Sun Jan 31 21:45:06 2021, max compression
+gzip compressed data, was "panoptes-ui-0.2.2.tar", last modified: Thu Aug  3 14:12:10 2023, max compression
```

## Comparing `panoptes-ui-0.2.0.tar` & `panoptes-ui-0.2.2.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.636437 panoptes-ui-0.2.0/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       48 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/MANIFEST.in
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      619 2021-01-31 21:45:06.633436 panoptes-ui-0.2.0/PKG-INFO
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     5088 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/README.md
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.478085 panoptes-ui-0.2.0/panoptes/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       27 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/__init__.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4743 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/app.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      739 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/database.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4649 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/models.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1095 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/panoptes.py
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.516082 panoptes-ui-0.2.0/panoptes/routes/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       86 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/routes/__init__.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     3985 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/routes/api.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      672 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/schema_forms.py
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.554268 panoptes-ui-0.2.0/panoptes/server_utilities/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/server_utilities/__init__.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     5707 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/server_utilities/db_queries.py
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.573420 panoptes-ui-0.2.0/panoptes/static/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/__init__.py
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.764756 panoptes-ui-0.2.0/panoptes/static/src/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1011 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/404.html
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/__init__.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1641 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/about.html
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.904384 panoptes-ui-0.2.0/panoptes/static/src/css/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)   336236 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/css/style.css
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)   773634 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/css/style.css.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)   276087 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/css/style.min.css
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)  1044838 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/css/style.min.css.map
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.952150 panoptes-ui-0.2.0/panoptes/static/src/img/
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:05.216149 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1913 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/1.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2105 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/2.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1645 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/3.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2580 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/4.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    19058 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/5.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1608 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/6.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2059 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/7.jpg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    20466 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/avatars/8.jpg
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:05.459174 panoptes-ui-0.2.0/panoptes/static/src/img/brand/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4391 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/logo.svg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2019 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes.png
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)  1201622 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes.svg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4287 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes_eye.png
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4698 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes_logo.svg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1460 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/brand/sygnet.svg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4286 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/img/favicon.ico
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    10610 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/index.html
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1837 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/job.html
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:05.818200 panoptes-ui-0.2.0/panoptes/static/src/js/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4312 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/charts.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     9421 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/charts.js.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      777 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/colors.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1162 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/colors.js.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     8623 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/main.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    20520 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/main.js.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      422 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/popovers.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      675 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/popovers.js.map
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.048081 panoptes-ui-0.2.0/panoptes/static/src/js/src/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     4429 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/charts.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      720 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/colors.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     9344 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/init.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     8755 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/main.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      394 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/popovers.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      340 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/tooltips.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    11320 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/src/widgets.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      367 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/tooltips.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      527 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/tooltips.js.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    11143 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/widgets.js
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    27173 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/js/widgets.js.map
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.139057 panoptes-ui-0.2.0/panoptes/static/src/notifications/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    36471 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/notifications/alerts.html
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    35530 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/notifications/badge.html
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)    41078 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/notifications/modals.html
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.225065 panoptes-ui-0.2.0/panoptes/static/src/scss/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       33 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/scss/_custom.scss
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       22 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/scss/_variables.scss
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      200 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/scss/style.scss
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.259109 panoptes-ui-0.2.0/panoptes/static/src/scss/vendors/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      155 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/scss/vendors/_variables.scss
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.296109 panoptes-ui-0.2.0/panoptes/static/src/scss/vendors/pace-progress/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     3134 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/scss/vendors/pace-progress/pace.scss
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2857 2021-01-31 21:43:32.000000 panoptes-ui-0.2.0/panoptes/static/src/searchResults.html
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.345274 panoptes-ui-0.2.0/panoptes/static/src/vendors/
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:04.348538 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.452120 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2110 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.css
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)   117500 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.css.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1731 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.min.css
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)   117477 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     3159 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/workflow.html
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1664 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/static/src/workflows.html
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.522494 panoptes-ui-0.2.0/panoptes/tests/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/tests/__init__.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     7469 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/tests/api_test.py
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1425 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/panoptes/tests/api_test_helper.py
-drwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        0 2021-01-31 21:45:06.616853 panoptes-ui-0.2.0/panoptes_ui.egg-info/
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      619 2021-01-31 21:44:57.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/PKG-INFO
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     2903 2021-01-31 21:44:58.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/SOURCES.txt
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        1 2021-01-31 21:44:57.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/dependency_links.txt
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       44 2021-01-31 21:44:57.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/entry_points.txt
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)      101 2021-01-31 21:44:57.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/requires.txt
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)        9 2021-01-31 21:44:57.000000 panoptes-ui-0.2.0/panoptes_ui.egg-info/top_level.txt
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)       38 2021-01-31 21:45:06.637437 panoptes-ui-0.2.0/setup.cfg
--rwxrwxrwx   0 argardelakos  (1000) argardelakos  (1000)     1147 2021-01-31 21:43:33.000000 panoptes-ui-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.301707 panoptes-ui-0.2.2/panoptes/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/panoptes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.301707 panoptes-ui-0.2.2/panoptes/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/routes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/schema_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/server_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/server_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/server_utilities/db_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/static/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.309707 panoptes-ui-0.2.2/panoptes/static/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   336236 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   773634 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   276087 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1044838 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.309707 panoptes-ui-0.2.2/panoptes/static/src/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.313707 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/8.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.317707 panoptes-ui-0.2.2/panoptes/static/src/img/brand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1201622 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/sygnet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/job.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/charts.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/colors.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/colors.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/colors.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    36471 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35530 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/modals.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/_custom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/pace.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/searchResults.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.297707 panoptes-ui-0.2.2/panoptes/static/src/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.297707 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117500 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117477 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/workflows.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/api_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/panoptes_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/setup.py
```

### Comparing `panoptes-ui-0.2.0/README.md` & `panoptes-ui-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/app.py` & `panoptes-ui-0.2.2/panoptes/app.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/database.py` & `panoptes-ui-0.2.2/panoptes/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import scoped_session, sessionmaker
 
-engine = create_engine('sqlite:///.panoptes.db?check_same_thread=False', convert_unicode=True)
+engine = create_engine('sqlite:///.panoptes.db?check_same_thread=False')
 db_session = scoped_session(sessionmaker(autocommit=False,
                                          autoflush=False,
                                          bind=engine))
 Base = declarative_base()
 Base.query = db_session.query_property()
```

### Comparing `panoptes-ui-0.2.0/panoptes/models.py` & `panoptes-ui-0.2.2/panoptes/models.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/panoptes.py` & `panoptes-ui-0.2.2/panoptes/panoptes.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/routes/api.py` & `panoptes-ui-0.2.2/panoptes/routes/api.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/schema_forms.py` & `panoptes-ui-0.2.2/panoptes/schema_forms.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/server_utilities/db_queries.py` & `panoptes-ui-0.2.2/panoptes/server_utilities/db_queries.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/404.html` & `panoptes-ui-0.2.2/panoptes/static/src/404.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/about.html` & `panoptes-ui-0.2.2/panoptes/static/src/about.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/css/style.css` & `panoptes-ui-0.2.2/panoptes/static/src/css/style.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/css/style.css.map` & `panoptes-ui-0.2.2/panoptes/static/src/css/style.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/css/style.min.css` & `panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/css/style.min.css.map` & `panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/1.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/1.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/2.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/2.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/3.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/3.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/4.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/4.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/5.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/5.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/6.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/6.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/7.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/7.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/avatars/8.jpg` & `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/8.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/logo.svg` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/logo.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes.png` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.png`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes.svg` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes_eye.png` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_eye.png`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/panoptes_logo.svg` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_logo.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/brand/sygnet.svg` & `panoptes-ui-0.2.2/panoptes/static/src/img/brand/sygnet.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/img/favicon.ico` & `panoptes-ui-0.2.2/panoptes/static/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/index.html` & `panoptes-ui-0.2.2/panoptes/static/src/index.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/job.html` & `panoptes-ui-0.2.2/panoptes/static/src/job.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/charts.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/charts.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/charts.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/charts.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/colors.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/colors.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/colors.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/colors.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/main.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/main.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/main.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/main.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/popovers.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/src/charts.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/src/charts.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/src/colors.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/src/colors.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/src/init.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/src/init.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/src/main.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/src/main.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/src/widgets.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/src/widgets.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/tooltips.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/widgets.js` & `panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/js/widgets.js.map` & `panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/notifications/alerts.html` & `panoptes-ui-0.2.2/panoptes/static/src/notifications/alerts.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/notifications/badge.html` & `panoptes-ui-0.2.2/panoptes/static/src/notifications/badge.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/notifications/modals.html` & `panoptes-ui-0.2.2/panoptes/static/src/notifications/modals.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/scss/vendors/pace-progress/pace.scss` & `panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/pace.scss`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/searchResults.html` & `panoptes-ui-0.2.2/panoptes/static/src/searchResults.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.css` & `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.css.map` & `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.min.css` & `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map` & `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/workflow.html` & `panoptes-ui-0.2.2/panoptes/static/src/workflow.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/static/src/workflows.html` & `panoptes-ui-0.2.2/panoptes/static/src/workflows.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/tests/api_test.py` & `panoptes-ui-0.2.2/panoptes/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes/tests/api_test_helper.py` & `panoptes-ui-0.2.2/panoptes/tests/api_test_helper.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.0/panoptes_ui.egg-info/SOURCES.txt` & `panoptes-ui-0.2.2/panoptes_ui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 panoptes/__init__.py
 panoptes/app.py
 panoptes/database.py
 panoptes/models.py
```

### Comparing `panoptes-ui-0.2.0/setup.py` & `panoptes-ui-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 if sys.version_info < (3, 6):
     sys.exit('Sorry, panoptes requires Python >= 3.6')
 
 setup(
     name='panoptes-ui',
-    version='0.2.0',
+    version='0.2.2',
     url='https://github.com/panoptes-organization/panoptes',
     license='MIT',
     author='panoptes-organization',
     author_email='georgekostoulas@gmail.com, agardelakos@gmail.com, fgypas@gmail.com, gntalaperas@gmail.com, dimitris.afe@gmail.com, rekoumisd@gmail.com, vsochat@stanford.edu',
     description="panoptes: monitor computational workflows in real time",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

