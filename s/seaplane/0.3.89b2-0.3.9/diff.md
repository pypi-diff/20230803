# Comparing `tmp/seaplane-0.3.89b2.tar.gz` & `tmp/seaplane-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.3.89b2.tar", max compression
+gzip compressed data, was "seaplane-0.3.9.tar", max compression
```

## Comparing `seaplane-0.3.89b2.tar` & `seaplane-0.3.9.tar`

### file list

```diff
@@ -1,70 +1,68 @@
--rw-r--r--   0        0        0     1538 2023-07-21 14:25:12.219270 seaplane-0.3.89b2/README.md
--rw-r--r--   0        0        0     2931 2023-08-03 11:40:08.858657 seaplane-0.3.89b2/pyproject.toml
--rw-r--r--   0        0        0      778 2023-07-28 12:14:29.242045 seaplane-0.3.89b2/src/seaplane/__init__.py
--rw-r--r--   0        0        0       66 2023-07-21 14:25:14.742200 seaplane-0.3.89b2/src/seaplane/__main__.py
--rw-r--r--   0        0        0        0 2023-07-26 11:44:50.864621 seaplane-0.3.89b2/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-07-21 14:25:14.717240 seaplane-0.3.89b2/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2797 2023-07-21 14:25:14.717997 seaplane-0.3.89b2/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     1491 2023-08-03 11:13:50.755979 seaplane-0.3.89b2/src/seaplane/api/api_substation.py
--rw-r--r--   0        0        0     5806 2023-07-21 14:25:14.717640 seaplane-0.3.89b2/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     1552 2023-07-21 14:25:14.722296 seaplane-0.3.89b2/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3487 2023-07-21 14:25:14.717435 seaplane-0.3.89b2/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0      252 2023-07-28 13:21:29.634374 seaplane-0.3.89b2/src/seaplane/apps/__init__.py
--rw-r--r--   0        0        0     1939 2023-07-21 14:25:14.740411 seaplane-0.3.89b2/src/seaplane/apps/app.py
--rw-r--r--   0        0        0     2511 2023-07-21 14:25:14.727611 seaplane-0.3.89b2/src/seaplane/apps/build.py
--rw-r--r--   0        0        0     3121 2023-07-21 14:25:14.740237 seaplane-0.3.89b2/src/seaplane/apps/cli.py
--rw-r--r--   0        0        0     2952 2023-08-02 16:52:20.209197 seaplane-0.3.89b2/src/seaplane/apps/datasources/__init__.py
--rw-r--r--   0        0        0     1883 2023-07-21 14:25:14.727419 seaplane-0.3.89b2/src/seaplane/apps/datasources/request_data_source.py
--rw-r--r--   0        0        0     2368 2023-07-21 14:25:14.725497 seaplane-0.3.89b2/src/seaplane/apps/datasources/sql_executor.py
--rw-r--r--   0        0        0     6179 2023-08-01 13:22:44.607938 seaplane-0.3.89b2/src/seaplane/apps/decorators.py
--rw-r--r--   0        0        0    12169 2023-07-28 14:33:00.952645 seaplane-0.3.89b2/src/seaplane/apps/deploy.py
--rw-r--r--   0        0        0       52 2023-07-21 14:25:14.740972 seaplane-0.3.89b2/src/seaplane/apps/entry_points/__init__.py
--rw-r--r--   0        0        0     9553 2023-07-26 11:44:50.865394 seaplane-0.3.89b2/src/seaplane/apps/entry_points/entry_point.py
--rw-r--r--   0        0        0     2194 2023-07-21 14:25:14.730843 seaplane-0.3.89b2/src/seaplane/apps/event_handler.py
--rw-r--r--   0        0        0     1947 2023-07-21 14:25:14.741836 seaplane-0.3.89b2/src/seaplane/apps/executor.py
--rw-r--r--   0        0        0     3583 2023-08-01 14:05:40.003728 seaplane-0.3.89b2/src/seaplane/apps/task.py
--rw-r--r--   0        0        0      217 2023-08-01 13:22:46.265456 seaplane-0.3.89b2/src/seaplane/apps/tasks/__init__.py
--rw-r--r--   0        0        0     3230 2023-07-21 14:25:14.730035 seaplane-0.3.89b2/src/seaplane/apps/tasks/openai.py
--rw-r--r--   0        0        0     3150 2023-07-21 14:25:14.728391 seaplane-0.3.89b2/src/seaplane/apps/tasks/replicate.py
--rw-r--r--   0        0        0     1094 2023-07-21 14:25:14.730325 seaplane-0.3.89b2/src/seaplane/apps/tasks/sql.py
--rw-r--r--   0        0        0     1161 2023-08-03 11:12:24.112385 seaplane-0.3.89b2/src/seaplane/apps/tasks/substation.py
--rw-r--r--   0        0        0     3110 2023-08-03 11:39:56.415371 seaplane-0.3.89b2/src/seaplane/apps/tasks/vectordb.py
--rw-r--r--   0        0        0       33 2023-07-21 14:25:14.733884 seaplane-0.3.89b2/src/seaplane/apps/website/.gitignore
--rw-r--r--   0        0        0     1750 2023-07-21 14:25:14.732095 seaplane-0.3.89b2/src/seaplane/apps/website/README.md
--rw-r--r--   0        0        0       77 2023-07-21 14:25:14.731529 seaplane-0.3.89b2/src/seaplane/apps/website/jsconfig.json
--rw-r--r--   0        0        0      118 2023-07-21 14:25:14.731911 seaplane-0.3.89b2/src/seaplane/apps/website/next.config.js
--rw-r--r--   0        0        0      644 2023-07-21 14:25:14.734019 seaplane-0.3.89b2/src/seaplane/apps/website/package.json
--rw-r--r--   0        0        0       82 2023-07-21 14:25:14.734168 seaplane-0.3.89b2/src/seaplane/apps/website/postcss.config.js
--rw-r--r--   0        0        0      717 2023-07-21 14:25:14.732539 seaplane-0.3.89b2/src/seaplane/apps/website/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-07-21 14:25:14.733701 seaplane-0.3.89b2/src/seaplane/apps/website/public/next.svg
--rw-r--r--   0        0        0    39147 2023-07-21 14:25:14.732701 seaplane-0.3.89b2/src/seaplane/apps/website/public/openai.png
--rw-r--r--   0        0        0    11580 2023-07-21 14:25:14.732841 seaplane-0.3.89b2/src/seaplane/apps/website/public/seaplane_logo.svg
--rw-r--r--   0        0        0     2296 2023-07-21 14:25:14.732974 seaplane-0.3.89b2/src/seaplane/apps/website/public/seaplane_logo_mark.svg
--rw-r--r--   0        0        0   195272 2023-07-21 14:25:14.733365 seaplane-0.3.89b2/src/seaplane/apps/website/public/stabilityai.png
--rw-r--r--   0        0        0      629 2023-07-21 14:25:14.733551 seaplane-0.3.89b2/src/seaplane/apps/website/public/vercel.svg
--rw-r--r--   0        0        0     3691 2023-07-21 14:25:14.736701 seaplane-0.3.89b2/src/seaplane/apps/website/src/components/Header.jsx
--rw-r--r--   0        0        0    10691 2023-07-21 14:25:14.736851 seaplane-0.3.89b2/src/seaplane/apps/website/src/components/SmartPipe.jsx
--rw-r--r--   0        0        0     4191 2023-07-21 14:25:14.736999 seaplane-0.3.89b2/src/seaplane/apps/website/src/components/SmartPipesList.jsx
--rw-r--r--   0        0        0      127 2023-07-21 14:25:14.737294 seaplane-0.3.89b2/src/seaplane/apps/website/src/pages/_app.js
--rw-r--r--   0        0        0      231 2023-07-21 14:25:14.737714 seaplane-0.3.89b2/src/seaplane/apps/website/src/pages/_document.js
--rw-r--r--   0        0        0     1841 2023-07-21 14:25:14.737434 seaplane-0.3.89b2/src/seaplane/apps/website/src/pages/index.js
--rw-r--r--   0        0        0     2377 2023-07-21 14:25:14.737575 seaplane-0.3.89b2/src/seaplane/apps/website/src/pages/tutorial.js
--rw-r--r--   0        0        0      228 2023-07-21 14:25:14.736265 seaplane-0.3.89b2/src/seaplane/apps/website/src/styles/globals.css
--rw-r--r--   0        0        0      528 2023-07-21 14:25:14.731769 seaplane-0.3.89b2/src/seaplane/apps/website/tailwind.config.js
--rw-r--r--   0        0        0       58 2023-07-21 14:25:14.723206 seaplane-0.3.89b2/src/seaplane/carrier/__init__.py
--rw-r--r--   0        0        0     4463 2023-07-21 14:25:14.723452 seaplane-0.3.89b2/src/seaplane/carrier/processor.py
--rw-r--r--   0        0        0     9173 2023-08-01 13:22:44.591564 seaplane-0.3.89b2/src/seaplane/configuration.py
--rw-r--r--   0        0        0     2480 2023-08-01 13:52:27.711636 seaplane-0.3.89b2/src/seaplane/integrations/langchain.py
--rw-r--r--   0        0        0     1815 2023-07-21 14:25:14.742466 seaplane-0.3.89b2/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      267 2023-08-01 14:15:30.094731 seaplane-0.3.89b2/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0      540 2023-07-21 14:25:14.715240 seaplane-0.3.89b2/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3560 2023-07-21 14:25:14.715566 seaplane-0.3.89b2/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      478 2023-07-21 14:25:14.711223 seaplane-0.3.89b2/src/seaplane/model/region.py
--rw-r--r--   0        0        0       86 2023-07-26 11:44:50.865910 seaplane-0.3.89b2/src/seaplane/model/secrets/__init__.py
--rw-r--r--   0        0        0      530 2023-07-21 14:25:14.716316 seaplane-0.3.89b2/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      393 2023-08-01 14:05:41.644489 seaplane-0.3.89b2/src/seaplane/model/vector/__init__.py
--rw-r--r--   0        0        0      559 2023-07-21 14:25:14.704688 seaplane-0.3.89b2/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-07-21 14:25:14.704383 seaplane-0.3.89b2/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0       67 2023-08-01 13:22:44.503811 seaplane-0.3.89b2/src/seaplane/vector/__init__.py
--rw-r--r--   0        0        0     4414 2023-08-01 14:16:37.295485 seaplane-0.3.89b2/src/seaplane/vector/vector_store.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 seaplane-0.3.89b2/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.9/README.md
+-rw-r--r--   0        0        0     2682 2023-06-08 16:33:33.572139 seaplane-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1178 2023-06-08 15:19:56.475350 seaplane-0.3.9/src/seaplane/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-07 13:57:55.120996 seaplane-0.3.9/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.9/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2558 2023-06-07 11:17:31.773475 seaplane-0.3.9/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-06-07 11:17:31.773747 seaplane-0.3.9/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-06-07 11:17:31.774043 seaplane-0.3.9/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-06-07 11:17:31.774348 seaplane-0.3.9/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-06-07 11:17:31.774586 seaplane-0.3.9/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-06-07 11:17:31.774882 seaplane-0.3.9/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-06-07 11:17:31.775138 seaplane-0.3.9/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.9/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0       57 2023-06-08 15:27:56.714791 seaplane-0.3.9/src/seaplane/carrier/__init__.py
+-rw-r--r--   0        0        0     2401 2023-06-08 15:27:17.021086 seaplane-0.3.9/src/seaplane/carrier/processor.py
+-rw-r--r--   0        0        0     8148 2023-06-08 16:06:32.018960 seaplane-0.3.9/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1818 2023-06-05 16:13:40.927293 seaplane-0.3.9/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-07 13:57:55.121524 seaplane-0.3.9/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.9/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.9/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.9/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.9/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-06-07 11:17:31.775418 seaplane-0.3.9/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-06-07 11:17:31.775652 seaplane-0.3.9/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.9/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.9/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-06-07 11:17:31.775895 seaplane-0.3.9/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.9/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-08 15:19:30.007796 seaplane-0.3.9/src/seaplane/smartpipes/__init__.py
+-rw-r--r--   0        0        0     1521 2023-06-08 15:18:22.874342 seaplane-0.3.9/src/seaplane/smartpipes/build.py
+-rw-r--r--   0        0        0     2756 2023-06-07 14:00:21.738111 seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py
+-rw-r--r--   0        0        0      166 2023-06-07 13:57:55.122029 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-07 13:57:55.122241 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/bloom.py
+-rw-r--r--   0        0        0     3242 2023-06-07 13:57:55.122396 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/openai.py
+-rw-r--r--   0        0        0     4054 2023-06-07 13:57:55.122622 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/pinecone.py
+-rw-r--r--   0        0        0     3164 2023-06-07 13:57:55.122771 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py
+-rw-r--r--   0        0        0     7131 2023-06-08 06:15:04.301952 seaplane-0.3.9/src/seaplane/smartpipes/decorators.py
+-rw-r--r--   0        0        0     6081 2023-06-08 16:19:46.270911 seaplane-0.3.9/src/seaplane/smartpipes/deploy.py
+-rw-r--r--   0        0        0     2364 2023-06-07 14:02:48.693793 seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py
+-rw-r--r--   0        0        0     1639 2023-06-07 14:17:11.058070 seaplane-0.3.9/src/seaplane/smartpipes/executor.py
+-rw-r--r--   0        0        0     3495 2023-06-08 16:33:17.244291 seaplane-0.3.9/src/seaplane/smartpipes/smartapi.py
+-rw-r--r--   0        0        0     2090 2023-06-07 13:59:40.996093 seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py
+-rw-r--r--   0        0        0       33 2023-06-05 16:13:40.929884 seaplane-0.3.9/src/seaplane/smartpipes/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-06-05 16:13:40.930353 seaplane-0.3.9/src/seaplane/smartpipes/website/README.md
+-rw-r--r--   0        0        0       77 2023-06-05 16:13:40.930859 seaplane-0.3.9/src/seaplane/smartpipes/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-06-05 16:13:40.931524 seaplane-0.3.9/src/seaplane/smartpipes/website/next.config.js
+-rw-r--r--   0        0        0      650 2023-06-05 16:13:40.932082 seaplane-0.3.9/src/seaplane/smartpipes/website/package.json
+-rw-r--r--   0        0        0       82 2023-06-05 16:13:40.932489 seaplane-0.3.9/src/seaplane/smartpipes/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-06-05 16:13:40.933215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-06-05 16:13:40.933596 seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-06-05 16:13:40.934215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-06-05 16:13:40.934926 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-06-05 16:13:40.935333 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-06-05 16:13:40.938647 seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-06-05 16:13:40.939528 seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-06-05 16:13:40.943187 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10990 2023-06-05 16:13:40.944429 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     4317 2023-06-07 13:59:40.996261 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-06-05 16:13:40.945730 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-06-05 16:13:40.946888 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_document.js
+-rw-r--r--   0        0        0     1962 2023-06-05 16:13:40.947276 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/index.js
+-rw-r--r--   0        0        0     2643 2023-06-07 13:57:55.123829 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/tutorial.js
+-rw-r--r--   0        0        0      228 2023-06-05 16:13:40.947900 seaplane-0.3.9/src/seaplane/smartpipes/website/src/styles/globals.css
+-rw-r--r--   0        0        0      528 2023-06-05 16:13:40.948083 seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js
+-rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.9/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.9/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     5883 2023-06-08 16:34:11.748651 seaplane-0.3.9/setup.py
+-rw-r--r--   0        0        0     3182 2023-06-08 16:34:11.748974 seaplane-0.3.9/PKG-INFO
```

### Comparing `seaplane-0.3.89b2/README.md` & `seaplane-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/pyproject.toml` & `seaplane-0.3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.3.89-beta.2"
+version = "0.3.9"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
-attrs = "^22.2.0"
-certifi = "^2022.6.15"
-charset-normalizer = "^2.1.0"
-idna = "^3.3"
-iniconfig = "^1.1.1"
-packaging = "^21.3"
-pluggy = "^1.0.0"
-py = "^1.11.0"
-pyparsing = "^3.0.9"
-requests = "^2.31.0"
-tomli = "^2.0.1"
+python = ">=3.10.*,<4.0"
+attrs = "21.4.0"
+certifi = "2022.6.15"
+charset-normalizer = "2.1.0"
+idna = "3.3"
+iniconfig = "1.1.1"
+packaging = "21.3"
+pluggy = "1.0.0"
+py = "1.11.0"
+pyparsing = "3.0.9"
+requests = "2.28.1"
+tomli = "2.0.1"
+urllib3 = "1.26.9"
 types-requests = "^2.28.0"
 returns = "^0.19.0"
 requests-mock = "^1.9.3"
 simplejson = "^3.17.6"
 types-simplejson = "^3.17.7"
 Flask-Cors = "^3.0.10"
 Flask-SocketIO = "^5.3.4"
 openai = "^0.27.7"
 tqdm = "^4.65.0"
+pinecone-client = "^2.2.1"
 tiktoken = "^0.4.0"
 pypdf = "^3.9.0"
-langchain = "^0.0.195"
-nats-py="^2.3.1"
-psycopg2-binary = "^2.9.6"
-nkeys = "^0.1.0"
-toml = "^0.10.2"
-cookiecutter = "^2.1.1"
-types-toml = "^0.10.8.6"
-urllib3 = "^1.26.16"
-python-dotenv = "^1.0.0"
-qdrant-client = "^1.3.2"
-langchainplus-sdk = "^0.0.20"
-
-[tool.poetry.scripts]
-seaplane = "seaplane.apps.cli:main"
+langchain = "^0.0.183"
+boto3 = "^1.26.142"
 
 [tool.poetry.dev-dependencies]
 nox-poetry = "*"
 
 # Testing.
 pytest = "*"
 pytest-cov = "*"
@@ -61,23 +51,24 @@
 # Linting.
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-broken-line = "*"
 flake8-comprehensions = "*"
 pep8-naming = "*"
 # TODO: Remove this when flake8 adds native support for pyproject.toml.
-pyproject-flake8 = "^6.0.0.post1"
+pyproject-flake8 = "*"
 
 # Formatting.
 black = "*"
 isort = "*"
 Sphinx = "^5.2.3"
 sphinx-autodoc-typehints = "^1.19.4"
 myst-parser = "^0.18.1"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
```

### Comparing `seaplane-0.3.89b2/src/seaplane/api/api_http.py` & `seaplane-0.3.9/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/api/api_request.py` & `seaplane-0.3.9/src/seaplane/api/api_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,21 +33,15 @@
     """
 
     def handle_request(request: Callable[[str], Response], token: str) -> Result[Any, HTTPError]:
         try:
             response = request(token)
 
             if response.ok:
-                data = None
-                if response.headers.get("content-type") == "application/json":
-                    data = response.json()
-                else:
-                    data = response.text
-
-                return Success(data)
+                return Success(response.json())
             else:
                 body_error = response.text
                 log.error(f"Request Error: {body_error}")
                 return Failure(HTTPError(response.status_code, body_error))
         except requests.exceptions.RequestException as err:
             log.error(f"Request exception: {str(err)}")
             return Failure(HTTPError(SDK_HTTP_ERROR_CODE, str(err)))
@@ -67,14 +61,14 @@
 
     def req(request: Callable[[str], Response]) -> Result[Any, HTTPError]:
         access_token: Result[str, HTTPError]
 
         if token_api.access_token is not None:
             access_token = Success(token_api.access_token)
         else:
-            access_token = token_api._request_access_token().map(lambda result: result["token"])
+            access_token = token_api._request_access_token()
 
         return access_token.bind(lambda token: handle_request(request, token)).lash(
             lambda error: renew_if_fails(token_api, request, error)
         )
 
     return req
```

### Comparing `seaplane-0.3.89b2/src/seaplane/api/metadata_api.py` & `seaplane-0.3.9/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/api/sql_api.py` & `seaplane-0.3.9/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/api/token_api.py` & `seaplane-0.3.9/src/seaplane/api/token_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Optional
 
 import requests
 from returns.result import Failure, Result, Success
 
 from ..logging import log
 from ..model.errors import HTTPError
 from ..util import unwrap
@@ -21,15 +21,14 @@
     """
 
     def __init__(self, configuration) -> None:  # type: ignore
         self.url = f"{configuration.identify_endpoint}/token"
         self.api_key = configuration.seaplane_api_key
         self.access_token = configuration._current_access_token
         self.auto_renew = configuration._token_auto_renew
-        self.tenant: Optional[str] = None
 
     def set_url(self, url: str) -> None:
         self.url = url
 
     def set_token(self, access_token: Optional[str]) -> None:
         """Set a valid Seaplane Token.
 
@@ -69,44 +68,33 @@
         """Request a new token.
 
         Returns
         -------
         str
             Returns the token.
         """
-        return unwrap(self._request_access_token())["token"]
+        return unwrap(self._request_access_token())
 
-    def get_tenant(self) -> str:
-        """Request the current tenant
-
-        Returns
-        -------
-        str
-            Returns the tenant.
-        """
-        return self.tenant if self.tenant else unwrap(self._request_access_token())["tenant"]
-
-    def _request_access_token(self) -> Result[Dict[str, str], HTTPError]:
+    def _request_access_token(self) -> Result[str, HTTPError]:
         try:
             log.info("Requesting access token...")
-            if not self.api_key:
-                log.error("API KEY not set, use sea.config.set_api_key")
-
             response = requests.post(self.url, json={}, headers=headers(self.api_key))
 
             if response.ok:
-                token = response.json()
-                self.access_token = token["token"]
-                self.tenant = token["tenant"]
+                token = response.json()["token"]
+                self.access_token = token
                 return Success(token)
             else:
                 self._current_access_token = None
-                error_body = response.text
+                error_body = response.json()
                 log.error(
                     f"Bad Access token request code {response.status_code}, error {error_body}"
                 )
                 return Failure(HTTPError(response.status_code, error_body))
 
         except requests.exceptions.RequestException as err:
             self._current_access_token = None
-            log.error(f"Request access token exception: {str(err)}")
+            if not self.api_key:
+                log.error("API KEY not set, use sea.config.set_api_key")
+            else:
+                log.error(f"Request access token exception: {str(err)}")
             return Failure(HTTPError(SDK_HTTP_ERROR_CODE, str(err)))
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/app.py` & `seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 import secrets
 import string
 from typing import Any, Callable, List, Optional
 
 from ..logging import log
-from .task import Task, TaskEvent
+from .coprocessor import Coprocessor, CoprocessorEvent
 
 
 def random_id() -> str:
     alphabet = string.ascii_letters + string.digits
     random_string = "".join(secrets.choice(alphabet) for i in range(10))
     return random_string
 
 
-class AppEvent:
-    def __init__(self, app_id: str, input: Any) -> None:
+class SmartPipeEvent:
+    def __init__(self, smart_pipe_id: str, input: Any) -> None:
         self.id = random_id()
-        self.app_id = app_id
+        self.smart_pipe_id = smart_pipe_id
         self.status = "in_progress"
         self.input: Any = input
         self.output: Optional[Any] = None
-        self.tasks: List[TaskEvent] = []
+        self.coprocessors: List[CoprocessorEvent] = []
         self.error: Optional[Any] = None
 
-    def add_task_event(self, event: TaskEvent) -> None:
-        for i, cp in enumerate(self.tasks):
+    def add_coprocessor_event(self, event: CoprocessorEvent) -> None:
+        for i, cp in enumerate(self.coprocessors):
             if cp.id == event.id:
-                self.tasks[i] = event
+                self.coprocessors[i] = event
                 return
-        self.tasks.append(event)
+        self.coprocessors.append(event)
 
-    def set_output(self, output: Any) -> None:
+    def set_ouput(self, output: Any) -> None:
         self.output = output
         self.status = "completed"
 
     def set_error(self, error: Any) -> None:
         self.error = error
         self.status = "error"
 
 
-class App:
+class SmartPipe:
     def __init__(
         self,
         func: Callable[[Any], Any],
         path: str,
         method: str,
         id: str,
         parameters: Optional[List[str]],
     ) -> None:
         self.func = func
         self.path = path
         self.method = method
         self.id = id
         self.parameters = parameters
-        self.tasks: List[Task] = []
-        self.events: List[AppEvent] = []
-        self.return_source = None
+        self.coprocessors: List[Coprocessor] = []
+        self.events: List[SmartPipeEvent] = []
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.func(*args, *kwargs)
 
-    def add_task(self, task: Task) -> None:
-        for i, cp in enumerate(self.tasks):
-            if cp.id == task.id:
-                self.tasks[i] = task
+    def add_coprocessor(self, coprocessor: Coprocessor) -> None:
+        for i, cp in enumerate(self.coprocessors):
+            if cp.id == coprocessor.id:
+                self.coprocessors[i] = coprocessor
                 return
-        self.tasks.append(task)
+        self.coprocessors.append(coprocessor)
 
     def print(self) -> None:
         log.info(f"id: {self.id}, path: {self.path}, method: {self.method}")
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/event_handler.py` & `seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 import traceback
 from typing import Any, Callable, Dict, List, Optional
 
-from .app import AppEvent
-from .task import TaskEvent
+from .coprocessor import CoprocessorEvent
+from .smartpipe import SmartPipeEvent
 
 
 def format_exception(e: Optional[Exception]) -> Optional[List[str]]:
     if e is None:
         return None
 
     return traceback.format_exception(type(e), e, e.__traceback__)
 
 
-def task_event_json(event: TaskEvent) -> Dict[str, Any]:
+def coprocessor_event_json(event: CoprocessorEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
     }
 
 
-def event_json(event: AppEvent) -> Dict[str, Any]:
+def event_json(event: SmartPipeEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
-        "app_id": event.app_id,
+        "smart_pipe_id": event.smart_pipe_id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
-        "tasks": [task_event_json(task) for task in event.tasks],
+        "coprocessors": [
+            coprocessor_event_json(coprocessor) for coprocessor in event.coprocessors
+        ],
     }
 
 
 class EventHandler:
     def __init__(self) -> None:
         self.on_change_event: Callable[[Dict[str, Any]], None] = lambda x: None
-        self.events: List[AppEvent] = []
+        self.events: List[SmartPipeEvent] = []
         self.active_event: List[str] = ["none"]
 
     def set_event(self, callback: Callable[[Dict[str, Any]], None]) -> None:
         self.on_change_event = callback
 
     def on_change(self, message: Dict[str, Any]) -> None:
         self.on_change_event(message)
 
-    def add_event(self, event: AppEvent) -> None:
+    def add_event(self, event: SmartPipeEvent) -> None:
         self.active_event[0] = event.id
         self.events.append(event)
 
         self.on_change_event({"type": "add_request", "payload": event_json(event)})
 
-    def update_event(self, event: AppEvent) -> None:
+    def update_event(self, event: SmartPipeEvent) -> None:
         for i, e in enumerate(self.events):
             if e.id == self.active_event[0]:
                 self.events[i] = event
 
                 self.on_change_event({"type": "update_request", "payload": event_json(event)})
                 break
 
-    def task_event(self, task_event: TaskEvent) -> None:
+    def coprocessor_event(self, coprocessor_event: CoprocessorEvent) -> None:
         for i, event in enumerate(self.events):
             if event.id == self.active_event[0]:
-                event.add_task_event(task_event)
+                event.add_coprocessor_event(coprocessor_event)
 
                 self.events[i] = event
 
                 self.on_change_event({"type": "update_request", "payload": event_json(event)})
                 break
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/executor.py` & `seaplane-0.3.9/src/seaplane/smartpipes/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,55 @@
 import json
 from typing import Any
 
 from ..logging import log
 from ..model.errors import HTTPError
-from .app import App
+from .coprocessor import Coprocessor, CoprocessorEvent
 from .event_handler import EventHandler
-from .task import Task, TaskEvent
 
 
-class TaskExecutor:
-    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
+class CoprocessorExecutor:
+    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
         pass
 
 
-class RealTaskExecutor(TaskExecutor):
+class RealCoProcessorExecutor(CoprocessorExecutor):
     def __init__(self, event_handler: EventHandler) -> None:
         self.event_handler = event_handler
 
-    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
+    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
         args_str = tuple(arg.decode() if isinstance(arg, bytes) else arg for arg in args)
         args_json = json.dumps(args_str)
 
-        event = TaskEvent(task.id, args_json)
-        self.event_handler.task_event(event)
+        event = CoprocessorEvent(coprocessor.id, args_json)
+        self.event_handler.coprocessor_event(event)
         result = None
 
         try:
-            result = task.process(*args, **kwargs)
-            event.set_output(result)
+            result = coprocessor.process(*args, **kwargs)
+            event.set_ouput(result)
         except HTTPError as err:
-            log.error(f"Task HTTPError: {err}")
+            log.error(f"Coprocessor HTTPError: {err}")
             event.set_error(err)
         except Exception as e:
-            log.error(f"Task error: {e}")
+            log.error(f"Coprocessor error: {e}")
             event.set_error(e)
 
-        self.event_handler.task_event(event)
+        self.event_handler.coprocessor_event(event)
 
         if event.error is not None:
             raise event.error
 
         return result
 
 
-class SchemaExecutor(TaskExecutor):
+class SchemaExecutor(CoprocessorExecutor):
     def __init__(self) -> None:
         ...
 
-    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
+    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
         arguments = []
         for arg in args:
             arguments.append(arg)
 
-        task.called_from(arguments)
-        return task.id
-
-
-class AppExecutor:
-    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
-        pass
-
-
-class ProductionAppExecutor(AppExecutor):
-    def __init__(self) -> None:
-        ...
-
-    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
-        pass
-
-
-class DevelopmentAppExecutor(AppExecutor):
-    def __init__(self) -> None:
-        ...
-
-    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
-        pass
+        coprocessor.called_from(arguments)
+        return coprocessor.id
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/task.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,80 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from ..logging import log
-from ..model.errors import SeaplaneError
-from .tasks import OpenAI, Replicate, Sql, Store, SubstationTask
+from .coprocessors import Bloom, OpenAI, Replicate, Store
 
 
-class TaskEvent:
+class CoprocessorEvent:
     def __init__(self, id: str, input: Any) -> None:
         self.id = id
         self.status = "in_progress"
         self.input = input
         self.output: Optional[Any] = None
         self.error: Optional[Any] = None
 
-    def set_output(self, output: Any) -> None:
+    def set_ouput(self, output: Any) -> None:
         self.output = output
         self.status = "completed"
 
     def set_error(self, error: Any) -> None:
         self.error = error
         self.status = "error"
 
 
 SEAPLANE_API_KEY_NAME = "SEAPLANE_API_KEY"
 OPENAI_API_KEY_NAME = "OPENAI_API_KEY"
 REPLICATE_API_KEY_NAME = "REPLICATE_API_KEY"
 
 
-class Task:
+class Coprocessor:
     def __init__(
-        self,
-        func: Callable[[Any], Any],
-        type: str,
-        id: Optional[str] = None,
-        model: Optional[str] = None,
-        sql_access: Optional[Dict[str, str]] = None,
-        index_name: Optional[str] = None,
+        self, func: Callable[[Any], Any], type: str, id: Optional[str], model: Optional[str]
     ) -> None:
         self.func = func
         self.args: Optional[Tuple[Any, ...]] = None
         self.kwargs: Optional[Dict[str, Any]] = None
         self.type = type
         self.model = model
         self.sources: List[str] = []
-        self.sql_access = sql_access
-        self.sql: Optional[Sql] = None
         self.name = func.__name__
-        self.index_name = index_name
 
         if id is not None:
             self.id = id
         else:
             self.id = func.__name__
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
-        log.info(f"Task type '{self.type}' Model ID {self.model}")
-
-        if self.type == "sql":
-            if self.sql_access is None:
-                raise SeaplaneError("Task of type SQL without sql attribute.")
-
-            if not self.sql:
-                self.sql = Sql(self.func, self.id, self.sql_access)
-
-            return self.sql.process(*self.args, **self.kwargs)
+        log.info(f"Coprocessor type '{self.type}' Model ID {self.model}")
 
         if self.type == "vectordb":
-            log.info("Accessing Vector DB task...")
-
-            if not self.index_name:
-                raise SeaplaneError("Missing index_name attribute on vectordb Task.")
-
-            self.args = self.args + (Store(self.index_name),)
+            log.info("Accessing Vector DB coprocessor...")
+            self.args = self.args + (Store(),)
             return self.func(*self.args, **self.kwargs)
 
-        model = None
-
-        if self.model:
-            model = self.model.lower()
-        else:
-            model = self.model
-
-        if model == "mpt-30b":
-            substation = SubstationTask(self.func, self.id, model)
-            return substation.process(*self.args, **self.kwargs)
-        elif model == "gpt-3.5":
-            openai = OpenAI(self.func, self.id, model)
+        if self.model == "bloom":
+            bloom = Bloom(self.func, self.id, self.model)
+            return bloom.process(*self.args, **self.kwargs)
+        elif self.model == "gpt-3.5":
+            openai = OpenAI(self.func, self.id, self.model)
             return openai.process(*self.args, **self.kwargs)
-        elif model == "gpt-3":
-            openai = OpenAI(self.func, self.id, model)
+        elif self.model == "gpt-3":
+            openai = OpenAI(self.func, self.id, self.model)
             return openai.process(*self.args, **self.kwargs)
-        elif model == "stable-diffusion":
-            replicate = Replicate(self.func, self.type, self.id, model)
+        elif self.model == "stable-diffusion":
+            replicate = Replicate(self.func, self.type, self.id, self.model)
             return replicate.process(*self.args, **self.kwargs)
-        elif model:
-            replicate = Replicate(self.func, self.type, self.id, model)
+        elif self.model:
+            replicate = Replicate(self.func, self.type, self.id, self.model)
             return replicate.process(*self.args, **self.kwargs)
         else:
-            log.info("Compute task type...")
+            log.info("Unknown coprocessor...")
             return self.func(*self.args, **self.kwargs)
 
     def called_from(self, sources: List[str]) -> None:
         self.sources = sources
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/tasks/openai.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,24 +88,24 @@
         self.id = id
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
         if self.model == "gpt-3.5":
-            log.info("Processing GPT-3.5 Model...")
+            log.info("Procesing GPT-3.5 Model...")
             self.args = self.args + (_gpt_3_5(),)
 
             return self.func(*self.args, **self.kwargs)
         elif self.model == "gpt-3":
-            log.info("Processing GPT-3 Model...")
+            log.info("Procesing GPT-3 Model...")
             self.args = self.args + (_gpt_3(),)
 
             return self.func(*self.args, **self.kwargs)
         else:
             raise SeaplaneError(
-                "OPENAI Task Not recognised , the model \
-                    doesn't match with any current OPEN AI task."
+                "OPENAI Coprocessor Not recognised , the model \
+                    doesn't match with any current OPEN AI coprocessor."
             )
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/tasks/replicate.py` & `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,21 @@
         self.id = id
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
         if self.model == "stable-diffusion":
-            log.info("Accessing Replicate stable-diffusion task...")
+            log.info("Accessing Replicate stable-diffusion coprocessor...")
             self.args = self.args + (
                 inference("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478"),
             )
 
             return self.func(*self.args, **self.kwargs)
         elif self.model:
-            log.info(f"Accessing Replicate {self.model} task...")
+            log.info(f"Accessing Replicate {self.model} coprocessor...")
             self.args = self.args + (inference(self.model),)
 
             return self.func(*self.args, **self.kwargs)
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/README.md` & `seaplane-0.3.9/src/seaplane/smartpipes/website/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/package.json` & `seaplane-0.3.9/src/seaplane/smartpipes/website/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'name'": "'smartpipes'"}*

```diff
@@ -11,15 +11,15 @@
         "react": "18.2.0",
         "react-dom": "18.2.0",
         "react-markdown": "^8.0.7",
         "react-syntax-highlighter": "^15.5.0",
         "socket.io-client": "^4.6.1",
         "tailwindcss": "3.3.2"
     },
-    "name": "apps",
+    "name": "smartpipes",
     "private": true,
     "scripts": {
         "build": "next build",
         "dev": "next dev",
         "lint": "next lint",
         "start": "next start"
     },
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/favicon.ico` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/next.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/openai.png` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/seaplane_logo.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/seaplane_logo_mark.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/stabilityai.png` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/public/vercel.svg` & `seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/src/components/Header.jsx` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/src/components/SmartPipe.jsx` & `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx`

 * *Files 11% similar despite different names*

```diff
@@ -61,18 +61,18 @@
   return error.reduce((prev, cur) => prev + cur + "\n", "")
 }
 
 function classNames(...classes) {
   return classes.filter(Boolean).join(' ')
 }
 
-const onClick = (app, body) => {
-  console.log(`Request to ${app.path} with body: ${JSON.stringify(body)}`)
-  fetch(`http://localhost:1337${app.path}`, {
-    method: app.method,    
+const onClick = (smartPipe, body) => {
+  console.log(`Request to ${smartPipe.path} with body: ${JSON.stringify(body)}`)
+  fetch(`http://localhost:1337${smartPipe.path}`, {
+    method: smartPipe.method,    
     headers: {
       'Content-Type': 'application/json'
     },
     body: body ? JSON.stringify(body) : null
   })
   .then((res) => console.log(res))
 }
@@ -82,30 +82,30 @@
   POST: 'text-purple-700 bg-purple-50 ring-purple-600/20',
   in_progress: 'text-gray-600 bg-gray-50 ring-gray-500/10',
   GET: 'text-yellow-800 bg-yellow-50 ring-yellow-600/20',  
   error: 'text-red-800 bg-red-50 ring-red-600/20',  
   completed: 'text-green-800 bg-green-50 ring-green-600/20',  
 }
 
-const getTaskEvent = (currentRequest, task) => {  
+const getCoprocessorEvent = (currentRequest, coprocessor) => {  
   if(currentRequest === undefined) return undefined
 
-  const res = currentRequest.tasks.filter(co => co.id === task.id)
+  const res = currentRequest.coprocessors.filter(co => co.id === coprocessor.id)
   return res.length > 0 ? res[0] : undefined
 }
 
-export default function App({currentRequest, app}) {
+export default function SmartPipe({currentRequest, smartPipe}) {
   const [body, setBody] = useState(undefined)
 
   return (
     <div className="flow-root">
         
-      {app?.method === 'POST' ? (<div className='mb-4'>
+      {smartPipe?.method === 'POST' ? (<div className='mb-4'>
         <label htmlFor="comment" className="block text-sm font-medium leading-6 text-gray-900">
-          Make a request to {app.method} {app.path} 
+          Make a request to {smartPipe.method} {smartPipe.path} 
         </label>
         <div className="mt-2">
           <textarea
             rows={3}
             name="comment"
             id="comment"
             placeholder=' POST body request'
@@ -114,22 +114,22 @@
             defaultValue={''}
           />
         </div>
       </div>) : null}
       <div className="flex mb-10 justify-end">        
            
                   <a
-                        onClick={() => {onClick(app, body)}}
+                        onClick={() => {onClick(smartPipe, body)}}
                         className="hidden rounded-md bg-[#00bda5] px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 hover:text-black sm:block"
                       >
                         Make Request
                       </a>            
         </div>
       <ul role="list" className="-mb-8">
-      <li key={app.id}>
+      <li key={smartPipe.id}>
             <div className="relative pb-8">
               <span className="absolute left-4 top-4 -ml-px h-full w-0.5 bg-gray-200" aria-hidden="true" />
               <div className="relative flex space-x-3">
                 <div>
                   <span
                     className={classNames(
                       'bg-[#00bda5]',
@@ -140,21 +140,21 @@
                   </span>
                 </div>
                 <div className="flex min-w-0 flex-1 justify-between space-x-4 pt-1.5">
                   <div>                    
                     <div className="flex items-start gap-x-3">                      
                         <p
                           className={classNames(
-                            statuses[app.method],
+                            statuses[smartPipe.method],
                             'rounded-md whitespace-nowrap mt-0.5 px-1.5 py-0.5 text-xs font-medium ring-1 ring-inset'
                           )}
                         >
-                          {app.method}
+                          {smartPipe.method}
                         </p>                        
-                        <p className="text-sm font-semibold leading-6 text-gray-900">{' '+ app.id }</p>
+                        <p className="text-sm font-semibold leading-6 text-gray-900">{' '+ smartPipe.id }</p>
                                                
                       </div>                      
                       {currentRequest !== undefined ? (
                         <div className="flex my-5">
                           <p>Request input: {currentRequest.input}</p>                          
                         </div>
                       ): null}                      
@@ -169,70 +169,70 @@
                             {currentRequest.status}
                           </p>                                                  
                         </div>) : null}
                 </div>
               </div>
             </div>
           </li>
-        {app.tasks.map((task, eventIdx) => (
-          <li key={task.id}>
+        {smartPipe.coprocessors.map((coprocessor, eventIdx) => (
+          <li key={coprocessor.id}>
             <div className="relative pb-8">
-              {eventIdx !== app.tasks.length - 1 ? (
+              {eventIdx !== smartPipe.coprocessors.length - 1 ? (
                 <span className="absolute left-4 top-4 -ml-px h-full w-0.5 bg-gray-200" aria-hidden="true" />
               ) : null}
               <div className="relative flex space-x-3">
                 <div>
                   <span
                     className={classNames(
-                      icons(task.model).color,
+                      icons(coprocessor.model).color,
                       'h-8 w-8 rounded-full flex items-center justify-center ring-8 ring-white'
                     )}
                   >
-                    <Image src={icons(task.model).icon} width={24} height={24} alt="OpenAI logo" />
+                    <Image src={icons(coprocessor.model).icon} width={24} height={24} alt="OpenAI logo" />
                   </span>
                 </div>
                 <div className="flex min-w-0 flex-1 justify-between space-x-4 pt-1.5">                  
                   <div>                                                               
                     <p className="text-sm text-gray-500">
-                      {task.type === 'compute' ? 'Compute' : <span className='text-sm font-semibold'>{'Model: ' + task.model}</span> }{' '}<span className='text-sm font-semibold'>{'ID: ' + task.id} </span>
+                      {coprocessor.type === 'compute' ? 'Compute' : <span className='text-sm font-semibold'>{'Model: ' + coprocessor.model}</span> }{' '}<span className='text-sm font-semibold'>{'ID: ' + coprocessor.id} </span>
                     </p>                                                       
-                    {getTaskEvent(currentRequest, task) !== undefined ? (
+                    {getCoprocessorEvent(currentRequest, coprocessor) !== undefined ? (
                         <div>                          
                           <div className="my-5">
                             <p className="font-semibold">Input:</p>
                             <div className="bg-white border rounded-md p-4">
-                              <p className="">{getTaskEvent(currentRequest, task).input}</p>
+                              <p className="">{getCoprocessorEvent(currentRequest, coprocessor).input}</p>
                             </div>
                           </div>                           
-                          {getTaskEvent(currentRequest, task).status !== 'error' ? (
+                          {getCoprocessorEvent(currentRequest, coprocessor).status !== 'error' ? (
                             <div className="my-5">
                             <p className="font-semibold">Output:</p>
                             <div className="bg-white border rounded-md p-4">
-                              <p className="">{JSON.stringify(getTaskEvent(currentRequest, task).output, null, 2)}</p>
+                              <p className="">{JSON.stringify(getCoprocessorEvent(currentRequest, coprocessor).output, null, 2)}</p>
                             </div>
                           </div>                         
                           ): (<div className="my-5">
                           <p className="text-red-500 font-semibold">Error:</p>
                           <div className="bg-gray-300 border rounded-md p-4">
-                            <pre className="whitespace-pre-wrap break-word">{showError(getTaskEvent(currentRequest, task).error)}</pre>
+                            <pre className="whitespace-pre-wrap break-word">{showError(getCoprocessorEvent(currentRequest, coprocessor).error)}</pre>
                           </div>
                         </div>)}
                           
                         </div>
                       ): null}    
                   </div>                  
                   <div className="whitespace-nowrap text-right text-sm text-gray-500">
-                    {getTaskEvent(currentRequest, task) !== undefined ?  (<div className="whitespace-nowrap text-right text-sm text-gray-500">
+                    {getCoprocessorEvent(currentRequest, coprocessor) !== undefined ?  (<div className="whitespace-nowrap text-right text-sm text-gray-500">
                           <p
                             className={classNames(
-                              statuses[getTaskEvent(currentRequest, task).status],
+                              statuses[getCoprocessorEvent(currentRequest, coprocessor).status],
                               'rounded-md whitespace-nowrap mt-0.5 px-1.5 py-0.5 text-xs font-medium ring-1 ring-inset'
                             )}
                           >
-                            {getTaskEvent(currentRequest, task).status}
+                            {getCoprocessorEvent(currentRequest, coprocessor).status}
                           </p>                                                  
                         </div>) : null} 
                   </div>
                 </div>
               </div>
             </div>
           </li>
```

### Comparing `seaplane-0.3.89b2/src/seaplane/apps/website/tailwind.config.js` & `seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/configuration.py` & `seaplane-0.3.9/src/seaplane/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,33 @@
 import os
 from typing import Dict, Optional
 
-from dotenv import load_dotenv
-
 from .api.token_api import TokenAPI
 from .logging import log
 from .model.errors import SeaplaneError
 
-env_file = load_dotenv("./.env")
-if env_file:
-    log.debug("👀 Found .env config file")
-
 _SEAPLANE_COMPUTE_API_ENDPOINT = "https://compute.cplane.cloud/v2beta"
 _SEAPLANE_COORDINATION_API_ENDPOINT = "https://metadata.cplane.cloud/v1"
 _SEAPLANE_IDENTIFY_API_ENDPOINT = "https://flightdeck.cplane.cloud/v1"
 _SEAPLANE_GLOBAL_SQL_API_ENDPOINT = "https://sql.cplane.cloud/v1"
-_SEAPLANE_CARRIER_API_ENDPOINT = "https://carrier.cplane.cloud/v1"
+_SEAPLANE_CARRIER_API_ENDPOINT = "https://carrier.staging.cplane.dev/v1"
 _SEAPLANE_SUBSTATION_API_ENDPOINT = "https://substation.dev.cplane.cloud/v1"
-_SEAPLANE_SUBSTATION_EMBED_API_ENDPOINT = "https://embed.substation.cplane.cloud/v1/embed"
-_SEAPLANE_VECTOR_DB_API_ENDPOINT = "https://vector.cplane.cloud"
-
-_SEAPLANE_ENV_VAR_PRODUCTION = "SEAPLANE_APPS_PRODUCTION"
 
-api_key_names = ["SEAPLANE_API_KEY", "OPENAI_API_KEY", "REPLICATE_API_KEY"]
+_SEAPLANE_ENV_VAR_PRODUCTION = "SMARTPIPES_PRODUCTION"
 
 
-def get_env(key: str) -> Optional[str]:
+def get_env(key: str) -> str:
     env = os.getenv(key)
 
     if not env:
-        return None
+        return ""
     else:
         return env
 
 
-def get_api_keys() -> Dict[str, str]:
-    api_keys = {}
-
-    for api_key_env_name in api_key_names:
-        api_key = get_env(api_key_env_name)
-        if api_key:
-            api_keys[api_key_env_name] = api_key
-
-    return api_keys
-
-
 class Configuration:
     """
     Seaplane SDK Configuration.
 
     Everytime the configuration is changed,
     It'll clear local configurations to the default Auth module.
     """
@@ -57,20 +36,23 @@
         self.seaplane_api_key: Optional[str] = None
         self.identify_endpoint = _SEAPLANE_IDENTIFY_API_ENDPOINT
         self.compute_endpoint = _SEAPLANE_COMPUTE_API_ENDPOINT
         self.coordination_endpoint = _SEAPLANE_COORDINATION_API_ENDPOINT
         self.global_sql_endpoint = _SEAPLANE_GLOBAL_SQL_API_ENDPOINT
         self.substation_endpoint = _SEAPLANE_SUBSTATION_API_ENDPOINT
         self.carrier_endpoint = _SEAPLANE_CARRIER_API_ENDPOINT
-        self.vector_db_endpoint = _SEAPLANE_VECTOR_DB_API_ENDPOINT
-        self.substation_embed_endpoint = _SEAPLANE_SUBSTATION_EMBED_API_ENDPOINT
         self._current_access_token: Optional[str] = None
         self._token_auto_renew = True
-        self.seaplane_api_key = get_env("SEAPLANE_API_KEY")
-        self._api_keys: Dict[str, str] = get_api_keys()
+        self._api_keys: Dict[str, str] = {
+            "SEAPLANE_API_KEY": get_env("SEAPLANE_API_KEY"),
+            "OPENAI_API_KEY": get_env("OPENAI_API_KEY"),
+            "REPLICATE_API_KEY": get_env("REPLICATE_API_KEY"),
+            "PINECONE_API_KEY": get_env("PINECONE_API_KEY"),
+            "PINECONE_API_ENV": get_env("PINECONE_API_ENV"),
+        }
         self._production = False
         self._update_token_api()
 
     def set_api_key(self, api_key: str) -> None:
         """Set the Seaplane API Key.
 
         The API Key is needed for the Seaplane Python SDK usage.
@@ -80,25 +62,25 @@
         api_key : str
             Seaplane API Key.
         """
         self.seaplane_api_key = api_key
         self._update_token_api()
 
     def set_api_keys(self, api_keys: Dict[str, str]) -> None:
-        """Set the Seaplane API Keys for Apps.
+        """Set the Seaplane API Keys for SmartPipes.
 
-        The API Keys is needed for some of the Tasks.
+        The API Keys is needed for some of the Coprocessors.
 
-        Supported Tasks API Keys:
+        Supported Coprocessors API Keys:
 
         Seaplane: SEAPLANE_API_KEY
         Open AI: OPENAI_API_KEY
         Replicate: REPLICATE_API_KEY
 
-        For example, for use an OpenAI Task,
+        For example, for use an OpenAI Coprocessor,
         you need to provide the Key - Value, of the API Key.
 
             $ from seaplane import sea
 
             $ api_keys = {"OPENAI_API_KEY": "sp-api-key-test" }
             $ sea.config.set_api_keys(api_keys)
 
@@ -212,30 +194,14 @@
         if endpoint[-1] == "/":
             self.carrier_endpoint = endpoint.rstrip(endpoint[-1])
         else:
             self.carrier_endpoint = endpoint
 
         self._update_token_api()
 
-    def set_vector_endpoint(self, endpoint: str) -> None:
-        if endpoint[-1] == "/":
-            self.vector_db_endpoint = endpoint.rstrip(endpoint[-1])
-        else:
-            self.vector_db_endpoint = endpoint
-
-        self._update_token_api()
-
-    def set_substation_embed_endpoint(self, endpoint: str) -> None:
-        if endpoint[-1] == "/":
-            self.substation_embed_endpoint = endpoint.rstrip(endpoint[-1])
-        else:
-            self.substation_embed_endpoint = endpoint
-
-        self._update_token_api()
-
     def _update_token_api(self) -> None:
         self._token_api = TokenAPI(self)
 
     def log_level(self, level: int) -> None:
         """Change logging level.
 
         Seaplane uses Python logging module for internal logs.
@@ -271,15 +237,15 @@
         if enable:
             log.enable()
         else:
             log.disable()
 
     def is_production(self) -> bool:
         if not self._production:
-            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION, "").lower() == "true"
+            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION) is not None
 
         return self._production
 
     def set_production(self, is_production: bool) -> None:
         self._production = is_production
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `seaplane-0.3.89b2/src/seaplane/logging/__init__.py` & `seaplane-0.3.9/src/seaplane/logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     INFO = logging.INFO
     DEBUG = logging.DEBUG
     NOTSET = logging.NOTSET
 
     def __init__(self) -> None:
         logging.basicConfig(format=self.FORMAT)
         self.logger = logging.getLogger("Seaplane")
-        self.logger.setLevel(logging.INFO)
+        self.logger.setLevel(logging.WARNING)
 
     def debug(self, message: str) -> None:
         self.logger.debug(message)
 
     def info(self, message: str) -> None:
         self.logger.info(message)
```

### Comparing `seaplane-0.3.89b2/src/seaplane/model/metadata/__init__.py` & `seaplane-0.3.9/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/src/seaplane/model/sql/__init__.py` & `seaplane-0.3.9/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.89b2/PKG-INFO` & `seaplane-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,44 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.3.89b2
+Version: 0.3.9
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-SocketIO (>=5.3.4,<6.0.0)
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
-Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
-Requires-Dist: charset-normalizer (>=2.1.0,<3.0.0)
-Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
-Requires-Dist: idna (>=3.3,<4.0)
-Requires-Dist: iniconfig (>=1.1.1,<2.0.0)
-Requires-Dist: langchain (>=0.0.195,<0.0.196)
-Requires-Dist: langchainplus-sdk (>=0.0.20,<0.0.21)
-Requires-Dist: nats-py (>=2.3.1,<3.0.0)
-Requires-Dist: nkeys (>=0.1.0,<0.2.0)
+Requires-Dist: attrs (==21.4.0)
+Requires-Dist: boto3 (>=1.26.142,<2.0.0)
+Requires-Dist: certifi (==2022.6.15)
+Requires-Dist: charset-normalizer (==2.1.0)
+Requires-Dist: idna (==3.3)
+Requires-Dist: iniconfig (==1.1.1)
+Requires-Dist: langchain (>=0.0.183,<0.0.184)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
-Requires-Dist: py (>=1.11.0,<2.0.0)
-Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
+Requires-Dist: packaging (==21.3)
+Requires-Dist: pinecone-client (>=2.2.1,<3.0.0)
+Requires-Dist: pluggy (==1.0.0)
+Requires-Dist: py (==1.11.0)
+Requires-Dist: pyparsing (==3.0.9)
 Requires-Dist: pypdf (>=3.9.0,<4.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: qdrant-client (>=1.3.2,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (==2.28.1)
 Requires-Dist: requests-mock (>=1.9.3,<2.0.0)
 Requires-Dist: returns (>=0.19.0,<0.20.0)
 Requires-Dist: simplejson (>=3.17.6,<4.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tomli (==2.0.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: types-requests (>=2.28.0,<3.0.0)
 Requires-Dist: types-simplejson (>=3.17.7,<4.0.0)
-Requires-Dist: types-toml (>=0.10.8.6,<0.11.0.0)
-Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
+Requires-Dist: urllib3 (==1.26.9)
 Project-URL: Documentation, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Project-URL: Repository, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Description-Content-Type: text/markdown
 
 # Seaplane Python SDK
 [![PyPI](https://badge.fury.io/py/seaplane.svg)](https://badge.fury.io/py/seaplane)
 [![Python](https://img.shields.io/pypi/pyversions/seaplane.svg?style=plastic)](https://badge.fury.io/py/seaplane)
```

