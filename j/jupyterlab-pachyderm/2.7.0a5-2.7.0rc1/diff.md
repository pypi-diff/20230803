# Comparing `tmp/jupyterlab_pachyderm-2.7.0a5.tar.gz` & `tmp/jupyterlab_pachyderm-2.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.7.0a5.tar", last modified: Wed Jul 12 20:56:47 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.7.0rc1.tar", last modified: Wed Jul 26 23:18:54 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.7.0a5.tar` & `jupyterlab_pachyderm-2.7.0rc1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.136294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.136294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   161098 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8296 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9596 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17560 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 20:56:16.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-07-12 20:54:18.000000 jupyterlab_pachyderm-2.7.0a5/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.120399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.128399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.128399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.136399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163203 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8290 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10621 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17660 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 23:18:25.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-07-26 23:16:19.000000 jupyterlab_pachyderm-2.7.0rc1/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8762 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2920 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/LICENSE` & `jupyterlab_pachyderm-2.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/MANIFEST.in` & `jupyterlab_pachyderm-2.7.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/PKG-INFO` & `jupyterlab_pachyderm-2.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.7.0a5
+Version: 2.7.0rc1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/README.md` & `jupyterlab_pachyderm-2.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.7.0-rc.1'"}*

```diff
@@ -66,19 +66,14 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.b44c82c4e0aece4113cd.js",
-            "style": "./style"
-        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -133,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.5"
+    "version": "2.7.0-rc.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.62cd8a8c852e71b919b6.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'2.7.0-rc.1'"}*

```diff
@@ -66,14 +66,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.62cd8a8c852e71b919b6.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -128,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.5"
+    "version": "2.7.0-rc.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunkjupyterlab_pachyderm = self.webpackChunkjupyterlab_pachyderm || []).push([
-    [829], {
-        7363: (e, t, a) => {
+    [199], {
+        843: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Ee
+                default: () => _e
             });
             var n = a(3279),
                 r = a.n(n),
                 l = a(4234);
             const s = r()((e => {
                     const t = e.target.getAttribute("data-testid");
                     t && (0, l.track)("notebook:click", {
@@ -252,30 +252,30 @@
             }), o.createElement("path", {
                 fill: "#D06868",
                 d: "m66.471 0-1.376 5.72-11.262 11.995 1.344-5.686z"
             }), o.createElement("path", {
                 fill: "#A5597E",
                 d: "m65.127 5.686 12.678 11.713-11.294 12.029-12.678-11.713z"
             })));
-            var h;
+            var p;
             ! function(e) {
                 e.openDocs = "jupyterlab-pachyderm:open-docs", e.contactSupport = "jupyterlab-pachyderm:contact-support"
-            }(h || (h = {}));
-            const p = {
+            }(p || (p = {}));
+            const h = {
                 id: "jupyterlab-pachyderm:help",
                 autoStart: !0,
                 requires: [c.IMainMenu],
                 activate: (e, t) => {
                     ((e, t) => {
-                        t && (e.commands.addCommand(h.openDocs, {
+                        t && (e.commands.addCommand(p.openDocs, {
                             label: "Pachyderm Docs",
                             execute: () => {
                                 window.open("https://docs.pachyderm.com/latest/getting_started/")
                             }
-                        }), e.commands.addCommand(h.contactSupport, {
+                        }), e.commands.addCommand(p.contactSupport, {
                             label: "Contact Pachyderm Support",
                             execute: () => {
                                 const e = m().createElement("div", {
                                         className: "pachyderm-help-title"
                                     }, m().createElement(u, {
                                         className: "pachyderm-help-title-logo"
                                     }), " ", m().createElement("h2", null, "Pachyderm Support")),
@@ -294,17 +294,17 @@
                                     buttons: [d.Dialog.createButton({
                                         label: "Dismiss",
                                         className: "jp-About-button jp-mod-reject jp-mod-styled"
                                     })]
                                 })
                             }
                         }), t.helpMenu.addGroup([{
-                            command: h.openDocs
+                            command: p.openDocs
                         }, {
-                            command: h.contactSupport
+                            command: p.contactSupport
                         }], 20))
                     })(e, t)
                 }
             };
             var f = a(9071),
                 E = a(344),
                 _ = a(5139),
@@ -395,15 +395,15 @@
                 S = a(122),
                 z = a(8299),
                 L = a(127),
                 N = a(1840),
                 B = a(8832),
                 O = a(3114);
 
-            function D(e = "", t = "GET", a = null, n = "pachyderm/v2") {
+            function A(e = "", t = "GET", a = null, n = "pachyderm/v2") {
                 return r = this, l = void 0, i = function*() {
                     const r = _.ServerConnection.makeSettings(),
                         l = E.URLExt.join(r.baseUrl, n, e),
                         s = {
                             method: t,
                             body: a ? JSON.stringify(a) : void 0
                         };
@@ -450,15 +450,15 @@
                             e(r)
                         }))).then(a, n)
                     }
                     c((i = i.apply(r, l || [])).next())
                 }));
                 var r, l, s, i
             }
-            var A = function(e, t, a, n) {
+            var D = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -487,23 +487,23 @@
                         code: 999,
                         message: ""
                     }, this._config = {
                         pachd_address: "",
                         cluster_status: "INVALID"
                     }, this._mountedSignal = new N.Signal(this), this._unmountedSignal = new N.Signal(this), this._projectSignal = new N.Signal(this), this._statusSignal = new N.Signal(this), this._configSignal = new N.Signal(this), this._dataPoll = new O.n_({
                         auto: !0,
-                        factory: () => A(this, void 0, void 0, (function*() {
+                        factory: () => D(this, void 0, void 0, (function*() {
                             return this.getData()
                         })),
                         frequency: {
                             interval: 2e3,
                             backoff: !0,
                             max: 5e3
                         }
-                    }), this.refresh = () => A(this, void 0, void 0, (function*() {
+                    }), this.refresh = () => D(this, void 0, void 0, (function*() {
                         yield this._dataPoll.refresh(), yield this._dataPoll.tick
                     })), this.updateData = e => {
                         JSON.stringify(e) !== JSON.stringify(this._rawData) && (this._rawData = e, this.mounted = Array.from(Object.values(e.mounted)), this.unmounted = Array.from(Object.values(e.unmounted)))
                     }, this.updateProjects = e => {
                         JSON.stringify(e) !== JSON.stringify(this.projects) && (this.projects = e)
                     }, this.name = e
                 }
@@ -552,23 +552,23 @@
                 get configSignal() {
                     return this._configSignal
                 }
                 get poll() {
                     return this._dataPoll
                 }
                 getData() {
-                    return A(this, void 0, void 0, (function*() {
+                    return D(this, void 0, void 0, (function*() {
                         try {
-                            const e = yield D("config", "GET");
+                            const e = yield A("config", "GET");
                             if (this.config = e, "INVALID" !== e.cluster_status) {
-                                const e = yield D("mounts", "GET");
+                                const e = yield A("mounts", "GET");
                                 this.status = {
                                     code: 200
                                 }, this.updateData(e);
-                                const t = yield D("projects", "GET");
+                                const t = yield A("projects", "GET");
                                 this.updateProjects(t)
                             }
                         } catch (e) {
                             e instanceof _.ServerConnection.ResponseError && (this.status = {
                                 code: e.response.status,
                                 message: e.response.statusText
                             })
@@ -593,15 +593,15 @@
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get(e, t) {
                     return a = this, n = void 0, l = function*() {
                         try {
-                            return yield D(E.URLExt.join("pfs", e), "GET")
+                            return yield A(E.URLExt.join("pfs", e), "GET")
                         } catch (e) {
                             return console.log("/pfs not found"), {
                                 name: "",
                                 path: "",
                                 last_modified: "2022-04-26T16:28:48.015858Z",
                                 created: "2022-04-26T16:28:48.015858Z",
                                 content: [],
@@ -2366,28 +2366,28 @@
                 }) => {
                     const {
                         addressField: s,
                         setAddressField: i,
                         errorMessage: c,
                         setErrorMessage: d,
                         shouldShowAddressInput: u,
-                        setShouldShowAddressInput: h,
-                        updatePachdAddress: p,
+                        setShouldShowAddressInput: p,
+                        updatePachdAddress: h,
                         callLogin: f,
                         callLogout: E,
                         shouldShowLogin: _,
                         loading: v,
                         showAdvancedOptions: k,
                         setShowAdvancedOptions: b,
                         serverCa: w,
                         setServerCa: x
                     } = ((e, t, a, n, r, l) => {
-                        const [s, i] = (0, o.useState)(!1), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(!1), [f, E] = (0, o.useState)(!1), [_, g] = (0, o.useState)(!1), [v, k] = (0, o.useState)("");
+                        const [s, i] = (0, o.useState)(!1), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [p, h] = (0, o.useState)(!1), [f, E] = (0, o.useState)(!1), [_, g] = (0, o.useState)(!1), [v, k] = (0, o.useState)("");
                         (0, o.useEffect)((() => {
-                            e && (p("AUTH_ENABLED" === n.cluster_status), E("INVALID" === n.cluster_status)), u(""), m(""), k(""), g(!1)
+                            e && (h("AUTH_ENABLED" === n.cluster_status), E("INVALID" === n.cluster_status)), u(""), m(""), k(""), g(!1)
                         }), [e, n]);
                         const y = (e => {
                             const t = (0, o.useRef)();
                             return (0, o.useEffect)((() => {
                                 t.current = e
                             })), t.current
                         })(l);
@@ -2401,52 +2401,52 @@
                             shouldShowAddressInput: f,
                             setShouldShowAddressInput: E,
                             updatePachdAddress: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
                                     const e = c.trim();
                                     if (/^((grpc|grpcs|http|https|unix):\/\/)/.test(e)) {
-                                        const t = yield D("config", "PUT", v ? {
+                                        const t = yield A("config", "PUT", v ? {
                                             pachd_address: e,
                                             server_cas: v
                                         } : {
                                             pachd_address: e
                                         });
-                                        "INVALID" === t.cluster_status ? u("Invalid address.") : (a(t), p("AUTH_ENABLED" === t.cluster_status))
+                                        "INVALID" === t.cluster_status ? u("Invalid address.") : (a(t), h("AUTH_ENABLED" === t.cluster_status))
                                     } else u("Cluster address should start with grpc://, grpcs://, http://, https:// or unix://")
                                 } catch (e) {
                                     u("Unable to connect to cluster."), console.log(e)
                                 }
                                 i(!1)
                             })),
                             callLogin: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    const e = yield D("auth/_login", "PUT");
+                                    const e = yield A("auth/_login", "PUT");
                                     if (e.auth_url) {
                                         const t = `width=500,height=500,left=${window.screenX+(window.outerWidth-500)/2},top=${window.screenY+(window.outerHeight-500)/2.5}`;
                                         window.open(e.auth_url, "", t)
                                     }
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 setTimeout((() => {
                                     i(!1)
                                 }), 2e3)
                             })),
                             callLogout: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    yield D("auth/_logout", "PUT"), yield r()
+                                    yield A("auth/_logout", "PUT"), yield r()
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 i(!1)
                             })),
-                            shouldShowLogin: h,
+                            shouldShowLogin: p,
                             loading: s,
                             showAdvancedOptions: _,
                             setShowAdvancedOptions: g,
                             serverCa: v,
                             setServerCa: k
                         }
                     })(e, t, n, r, l, a);
@@ -2472,15 +2472,15 @@
                         className: "pachyderm-mount-config-address-label"
                     }, "Cluster Address"), m().createElement("span", {
                         "data-testid": "Config__pachdAddress",
                         className: "pachyderm-mount-config-address"
                     }, r.pachd_address), m().createElement("button", {
                         "data-testid": "Config__pachdAddressUpdate",
                         className: "pachyderm-button-link",
-                        onClick: () => h(!0)
+                        onClick: () => p(!0)
                     }, "Change Address")) : m().createElement("div", {
                         style: {
                             width: "100%",
                             display: "flex",
                             flexDirection: "column"
                         }
                     }, m().createElement("div", {
@@ -2493,15 +2493,15 @@
                     }, m().createElement("span", {
                         className: "pachyderm-mount-config-subheading"
                     }, r.pachd_address ? "Update Configuration" : "Connect To a Cluster"), r.pachd_address && m().createElement("button", {
                         "data-testid": "Config__pachdAddressCancel",
                         className: "pachyderm-button-link",
                         disabled: v,
                         onClick: () => {
-                            d(""), i(""), x(""), h(!1), b(!1)
+                            d(""), i(""), x(""), p(!1), b(!1)
                         }
                     }, m().createElement(g.closeIcon.react, {
                         tag: "span"
                     }))), m().createElement("label", {
                         htmlFor: "pachd",
                         className: "pachyderm-mount-config-address-label"
                     }, "Cluster Address"), m().createElement("input", {
@@ -2561,15 +2561,15 @@
                     }, k ? "Clear Advanced Settings" : "Use Advanced Settings"), m().createElement("button", {
                         "data-testid": "Config__pachdAddressSubmit",
                         className: "pachyderm-button pachyderm-mount-config-set-address",
                         style: {
                             width: "100px"
                         },
                         disabled: v || !s,
-                        onClick: p
+                        onClick: h
                     }, "Set Address")))), _ && !u && m().createElement("div", {
                         className: "pachyderm-mount-login-container"
                     }, 200 === a ? m().createElement("button", {
                         "data-testid": "Config__logout",
                         className: "pachyderm-button",
                         style: {
                             width: "100px"
@@ -2633,35 +2633,35 @@
                 currentDatumInfo: s,
                 repoViewInputSpec: i
             }) => {
                 const c = (0, o.useRef)(null),
                     {
                         loading: d,
                         shouldShowCycler: u,
-                        currDatum: h,
-                        currIdx: p,
+                        currDatum: p,
+                        currIdx: h,
                         setCurrIdx: f,
                         inputSpec: E,
                         setInputSpec: v,
                         callMountDatums: k,
                         callUnmountAll: y,
                         errorMessage: b,
                         saveInputSpec: w,
                         initialInputSpec: x
                     } = ((e, t, a, n, r, l, s) => {
-                        const [i, c] = (0, o.useState)(!1), [m, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(-1), [p, f] = (0, o.useState)({
+                        const [i, c] = (0, o.useState)(!1), [m, d] = (0, o.useState)(!1), [u, p] = (0, o.useState)(-1), [h, f] = (0, o.useState)({
                             id: "",
                             idx: -1,
                             num_datums: 0
                         }), [E, g] = (0, o.useState)(""), [v, k] = (0, o.useState)({}), [y, b] = (0, o.useState)(""), [w, x] = (0, o.useState)({});
                         (0, o.useEffect)((() => {
                             e && -1 !== u && S()
                         }), [u, e]), (0, o.useEffect)((() => {
                             if (e)
-                                if (t || z(), t && s) d(!0), h(s.curr_idx), f({
+                                if (t || z(), t && s) d(!0), p(s.curr_idx), f({
                                     id: "",
                                     idx: s.curr_idx,
                                     num_datums: s.num_datums
                                 }), g(M(s.input)), a(!1);
                                 else if ("string" == typeof w) g(w);
                             else {
                                 let e = {};
@@ -2685,50 +2685,50 @@
                                 } catch (t) {
                                     return T().stringify(e, null, 2)
                                 }
                             },
                             S = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    const e = yield D(`_show_datum?idx=${u}`, "PUT");
+                                    const e = yield A(`_show_datum?idx=${u}`, "PUT");
                                     n(""), f(e)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 c(!1)
                             })),
                             z = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    n(""), yield D("_unmount_all", "PUT"), n(""), yield r(), h(-1), f({
+                                    n(""), yield A("_unmount_all", "PUT"), n(""), yield r(), p(-1), f({
                                         id: "",
                                         idx: -1,
                                         num_datums: 0
                                     }), d(!1)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 b(""), c(!1)
                             }));
                         return {
                             loading: i,
                             shouldShowCycler: m,
-                            currDatum: p,
+                            currDatum: h,
                             currIdx: u,
-                            setCurrIdx: h,
+                            setCurrIdx: p,
                             inputSpec: E,
                             setInputSpec: g,
                             callMountDatums: () => $(void 0, void 0, void 0, (function*() {
                                 c(!0), b("");
                                 try {
                                     const e = C(),
-                                        t = yield D("_mount_datums", "PUT", {
+                                        t = yield A("_mount_datums", "PUT", {
                                             input: e
                                         });
-                                    n(""), h(0), f(t), d(!0), g(M(e))
+                                    n(""), p(0), f(t), d(!0), g(M(e))
                                 } catch (e) {
                                     console.log(e), e instanceof T().YAMLParseError ? b("Poorly formatted input spec- must be either YAML or JSON") : e instanceof _.ServerConnection.ResponseError ? b("Bad data in input spec") : b("Error mounting datums")
                                 }
                                 c(!1)
                             })),
                             callUnmountAll: z,
                             errorMessage: y,
@@ -2831,34 +2831,38 @@
                 }, "Datum", m().createElement("div", {
                     style: {
                         display: "flex"
                     }
                 }, m().createElement("button", {
                     className: "pachyderm-button-link",
                     "data-testid": "Datum__cyclerLeft",
-                    disabled: p <= 0,
+                    disabled: h <= 0,
                     onClick: () => {
-                        p >= 1 && f(p - 1)
+                        h >= 1 && f(h - 1)
                     }
                 }, m().createElement(g.caretLeftIcon.react, {
                     tag: "span",
                     className: "pachyderm-mount-datum-left"
-                })), "(" + (p + 1) + "/" + h.num_datums + ")", m().createElement("button", {
+                })), "(" + (h + 1) + "/" + p.num_datums + ")", m().createElement("button", {
                     className: "pachyderm-button-link",
                     "data-testid": "Datum__cyclerRight",
-                    disabled: p >= h.num_datums - 1,
+                    disabled: h >= p.num_datums - 1,
                     onClick: () => {
-                        p < h.num_datums - 1 && f(p + 1)
+                        h < p.num_datums - 1 && f(h + 1)
                     }
                 }, m().createElement(g.caretRightIcon.react, {
                     tag: "span",
                     className: "pachyderm-mount-datum-right"
                 }))))))
             };
-            var J = function(e, t, a, n) {
+            var J;
+            ! function(e) {
+                e.None = "None", e.Simple = "Simple", e.Advanced = "Advanced"
+            }(J || (J = {}));
+            var q = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -2877,98 +2881,113 @@
                         e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
-            const q = "default",
-                Y = ({
+            const Y = "default",
+                X = ({
                     ppsContext: e,
                     settings: t,
                     setShowPipeline: a,
                     saveNotebookMetadata: n,
                     saveNotebookToDisk: r
                 }) => {
                     const {
                         loading: l,
                         pipelineName: s,
                         setPipelineName: i,
                         pipelineProject: c,
                         setPipelineProject: d,
                         imageName: u,
-                        setImageName: h,
-                        inputSpec: p,
+                        setImageName: p,
+                        inputSpec: h,
                         setInputSpec: f,
-                        requirements: E,
-                        setRequirements: v,
-                        callCreatePipeline: k,
-                        currentNotebook: y,
-                        errorMessage: b,
-                        responseMessage: w
+                        pipelinePort: E,
+                        setPipelinePort: v,
+                        gpuMode: k,
+                        setGpuMode: y,
+                        resourceSpec: b,
+                        setResourceSpec: w,
+                        requirements: x,
+                        setRequirements: C,
+                        callCreatePipeline: M,
+                        currentNotebook: S,
+                        errorMessage: z,
+                        responseMessage: L
                     } = ((e, t, a, n) => {
-                        const [r, l] = (0, o.useState)(!1), [s, i] = (0, o.useState)(""), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(""), [f, E] = (0, o.useState)(""), [g, v] = (0, o.useState)(""), [k, y] = (0, o.useState)(""), [b, w] = (0, o.useState)("None");
-                        let x;
+                        const [r, l] = (0, o.useState)(!1), [s, i] = (0, o.useState)(""), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [p, h] = (0, o.useState)(""), [f, E] = (0, o.useState)(""), [g, v] = (0, o.useState)(J.None), [k, y] = (0, o.useState)(""), [b, w] = (0, o.useState)(""), [x, C] = (0, o.useState)(""), [M, S] = (0, o.useState)(""), [z, L] = (0, o.useState)("None");
+                        let N;
                         if ((0, o.useEffect)((() => {
-                                var a, n, r, l, s, c, o, d, h, f, _, g;
-                                u(null !== (n = null === (a = null == e ? void 0 : e.metadata) || void 0 === a ? void 0 : a.config.image) && void 0 !== n ? n : t.defaultPipelineImage), i(null !== (l = null === (r = null == e ? void 0 : e.metadata) || void 0 === r ? void 0 : r.config.pipeline.name) && void 0 !== l ? l : ""), m(null !== (o = null === (c = null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.config.pipeline.project) || void 0 === c ? void 0 : c.name) && void 0 !== o ? o : ""), E(null !== (h = null === (d = null == e ? void 0 : e.metadata) || void 0 === d ? void 0 : d.config.requirements) && void 0 !== h ? h : ""), y(""), (null === (f = null == e ? void 0 : e.metadata) || void 0 === f ? void 0 : f.config.input_spec) ? p(e.metadata.config.input_spec) : p(""), w(null !== (g = null === (_ = null == e ? void 0 : e.notebookModel) || void 0 === _ ? void 0 : _.name) && void 0 !== g ? g : "None")
+                                var a, n, r, l, s, c, o, d, p, f, _, g, k, b, x, C, M, z;
+                                u(null !== (n = null === (a = null == e ? void 0 : e.metadata) || void 0 === a ? void 0 : a.config.image) && void 0 !== n ? n : t.defaultPipelineImage), i(null !== (l = null === (r = null == e ? void 0 : e.metadata) || void 0 === r ? void 0 : r.config.pipeline.name) && void 0 !== l ? l : ""), m(null !== (o = null === (c = null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.config.pipeline.project) || void 0 === c ? void 0 : c.name) && void 0 !== o ? o : ""), w(null !== (p = null === (d = null == e ? void 0 : e.metadata) || void 0 === d ? void 0 : d.config.requirements) && void 0 !== p ? p : ""), S(""), (null === (f = null == e ? void 0 : e.metadata) || void 0 === f ? void 0 : f.config.input_spec) ? h(e.metadata.config.input_spec) : h(""), L(null !== (g = null === (_ = null == e ? void 0 : e.notebookModel) || void 0 === _ ? void 0 : _.name) && void 0 !== g ? g : "None"), E(null !== (b = null === (k = null == e ? void 0 : e.metadata) || void 0 === k ? void 0 : k.config.port) && void 0 !== b ? b : ""), v(null !== (C = null === (x = null == e ? void 0 : e.metadata) || void 0 === x ? void 0 : x.config.gpu_mode) && void 0 !== C ? C : J.None), y(null !== (z = null === (M = null == e ? void 0 : e.metadata) || void 0 === M ? void 0 : M.config.resource_spec) && void 0 !== z ? z : "")
                             }), [e]), (0, o.useEffect)((() => {
-                                const e = C();
+                                const e = B();
                                 a(e)
-                            }), [s, c, d, f, h]), null == e ? void 0 : e.notebookModel) {
+                            }), [s, c, d, b, p, f, g, k]), null == e ? void 0 : e.notebookModel) {
                             const t = e.notebookModel;
-                            x = () => J(void 0, void 0, void 0, (function*() {
-                                l(!0), v(""), y("");
-                                const e = C();
+                            N = () => q(void 0, void 0, void 0, (function*() {
+                                l(!0), C(""), S("");
+                                const e = B();
                                 a(e);
                                 const r = yield n();
                                 try {
-                                    const e = yield D(`pps/_create/${encodeURI(t.path)}`, "PUT", {
+                                    const e = yield A(`pps/_create/${encodeURI(t.path)}`, "PUT", {
                                         last_modified_time: null != r ? r : t.last_modified
                                     });
-                                    null !== e.message && y(e.message)
+                                    null !== e.message && S(e.message)
                                 } catch (e) {
                                     if (!(e instanceof _.ServerConnection.ResponseError)) throw e;
-                                    v("Error creating pipeline: " + e.response.statusText)
+                                    C("Error creating pipeline: " + e.response.statusText)
                                 }
                                 l(!1)
                             }))
-                        } else x = () => J(void 0, void 0, void 0, (function*() {
-                            v("Error: No notebook in focus")
+                        } else N = () => q(void 0, void 0, void 0, (function*() {
+                            C("Error: No notebook in focus")
                         }));
-                        const C = () => ({
+                        const B = () => ({
                             version: "v1.0.0",
                             config: {
                                 pipeline: {
                                     name: s,
                                     project: {
                                         name: c
                                     }
                                 },
                                 image: d,
-                                requirements: f,
-                                input_spec: h
+                                requirements: b,
+                                input_spec: p,
+                                port: f,
+                                gpu_mode: g,
+                                resource_spec: k
                             }
                         });
                         return {
                             loading: r,
                             pipelineName: s,
                             setPipelineName: i,
                             pipelineProject: c,
                             setPipelineProject: m,
                             imageName: d,
                             setImageName: u,
-                            inputSpec: h,
-                            setInputSpec: p,
-                            requirements: f,
-                            setRequirements: E,
-                            callCreatePipeline: x,
-                            currentNotebook: b,
-                            errorMessage: g,
-                            responseMessage: k
+                            inputSpec: p,
+                            setInputSpec: h,
+                            pipelinePort: f,
+                            setPipelinePort: E,
+                            gpuMode: g,
+                            setGpuMode: v,
+                            resourceSpec: k,
+                            setResourceSpec: y,
+                            requirements: b,
+                            setRequirements: w,
+                            callCreatePipeline: N,
+                            currentNotebook: z,
+                            errorMessage: x,
+                            responseMessage: M
                         }
                     })(e, t, n, r);
                     return m().createElement("div", {
                         className: "pachyderm-mount-pipeline-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-pipeline-back"
                     }, m().createElement("button", {
@@ -3013,15 +3032,15 @@
                         className: "pachyderm-pipeline-current-notebook-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-current-notebook-label",
                         htmlFor: "currentNotebook"
                     }, "Current Notebook:", "  "), m().createElement("span", {
                         className: "pachyderm-pipeline-current-notebook-value",
                         "data-testid": "Pipeline__currentNotebookValue"
-                    }, y)), m().createElement("div", {
+                    }, S)), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "pipelineName"
                     }, "*Pipeline Name:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputPipelineName",
@@ -3041,87 +3060,131 @@
                         "data-testid": "Pipeline__inputPipelineProjectName",
                         name: "pipelineName",
                         value: c,
                         onChange: e => {
                             d(e.target.value)
                         },
                         disabled: l,
-                        placeholder: q
+                        placeholder: Y
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "imageName"
                     }, "*Container Image Name:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputImageName",
                         name: "imageName",
                         value: u,
                         onChange: e => {
-                            h(e.target.value)
+                            p(e.target.value)
                         },
                         disabled: l
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "requirements"
                     }, "Requirements File:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputRequirements",
                         name: "requirements",
-                        value: E,
+                        value: x,
                         onChange: e => {
-                            v(e.target.value)
+                            C(e.target.value)
                         },
                         disabled: l,
                         placeholder: "./requirements.txt"
                     })), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "port"
+                    }, "Port:", "  "), m().createElement("input", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__inputPort",
+                        name: "port",
+                        value: E,
+                        onChange: e => {
+                            v(e.target.value)
+                        },
+                        disabled: l
+                    })), m().createElement("div", {
                         className: "pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-textarea-label",
                         htmlFor: "inputSpec"
                     }, "Pipeline Input Spec:"), m().createElement("textarea", {
                         className: "pachyderm-pipeline-textarea pachyderm-input",
                         "data-testid": "Pipeline__inputSpecInput",
                         name: "inputSpec",
-                        value: p,
+                        value: h,
                         onChange: e => {
                             f(e.target.value)
                         },
                         disabled: l,
                         placeholder: "# example:\npfs:\n  repo: images\n  branch: dev\n  glob: /*\n"
                     })), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "gpuMode"
+                    }, "*Gpu Mode:", "  "), m().createElement("select", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__gpuMode",
+                        name: "gpuMode",
+                        value: k,
+                        onChange: e => {
+                            y(e.target.value)
+                        }
+                    }, Object.keys(J).map((e => m().createElement("option", {
+                        value: e
+                    }, e))))), k === J.Advanced && m().createElement("div", {
+                        className: "pachyderm-pipeline-textarea-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-textarea-label",
+                        htmlFor: "resourceSpec"
+                    }, "Pipeline Resource Spec:"), m().createElement("textarea", {
+                        className: "pachyderm-pipeline-textarea pachyderm-input",
+                        "data-testid": "Pipeline__resourceSpecInput",
+                        name: "resourceSpec",
+                        value: b,
+                        onChange: e => {
+                            w(e.target.value)
+                        },
+                        disabled: l,
+                        placeholder: "# example:\ngpu:\n  type: nvidia.com/gpu\n  number: 1\n"
+                    })), m().createElement("div", {
                         className: "pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-preview-label"
                     }, "Pipeline Spec Preview: ", "  "), m().createElement("textarea", {
                         className: "pachyderm-pipeline-spec-preview-textarea",
                         style: {
                             backgroundColor: "#80808080"
                         },
                         "data-testid": "Pipeline__specPreview",
                         name: "specPreview",
-                        value: `pipeline:\n  name: ${s}\n  project: ${c||q}\ntransform:\n  image: ${u}\ninput:\n${p.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
+                        value: `pipeline:\n  name: ${s}\n  project: ${c||Y}\ntransform:\n  image: ${u}\ninput:\n${h.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n${k===J.None?"":"resource_limits:\n"+(k===J.Simple?"gpu:\n  type: nvidia.com/gpu\n  number: 1\n":k===J.Advanced?b:"").split("\n").map(((e,t,a)=>"  "+e)).join("\n")}`,
                         readOnly: !0
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-buttons"
                     }, m().createElement("button", {
                         "data-testid": "Pipeline__create_pipeline",
                         className: "pachyderm-button",
-                        onClick: k
+                        onClick: M
                     }, "Run")), m().createElement("span", {
                         className: "pachyderm-pipeline-error",
                         "data-testid": "Pipeline__errorMessage"
-                    }, b), m().createElement("span", {
+                    }, z), m().createElement("span", {
                         className: "pachyderm-pipeline-response",
                         "data-testid": "Pipeline__responseMessage"
-                    }, w))
+                    }, L))
                 };
-            const X = ({
+            const K = ({
                     setShowPipeline: e
                 }) => m().createElement("div", {
                     className: "pachyderm-mount-pipeline-base"
                 }, m().createElement("div", {
                     className: "pachyderm-mount-pipeline-back"
                 }, m().createElement("button", {
                     "data-testid": "Pipeline__back",
@@ -3160,51 +3223,51 @@
                     tag: "span",
                     className: "pachyderm-mount-icon-padding"
                 }))), m().createElement("span", {
                     className: "pachyderm-mount-pipeline-subheading"
                 }, "Publish as Pipeline"), m().createElement("div", {
                     className: "pachyderm-mount-pipeline-splash"
                 }, m().createElement("span", null, "Open a notebook to create a pipeline"))),
-                K = (e, t) => e > t ? 1 : e < t ? -1 : 0,
-                Q = (e, t) => e - t;
-            var ee = a(4184),
-                te = a.n(ee);
-            const ae = e => {
+                Q = (e, t) => e > t ? 1 : e < t ? -1 : 0,
+                ee = (e, t) => e - t;
+            var te = a(4184),
+                ae = a.n(te);
+            const ne = e => {
                 var {
                     children: t,
                     className: a,
                     color: n = "gray"
                 } = e, r = function(e, t) {
                     var a = {};
                     for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
                     if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                         var r = 0;
                         for (n = Object.getOwnPropertySymbols(e); r < n.length; r++) t.indexOf(n[r]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[r]) && (a[n[r]] = e[n[r]])
                     }
                     return a
                 }(e, ["children", "className", "color"]);
-                const l = te()("jp-circle-base", a, {
+                const l = ae()("jp-circle-base", a, {
                     "jp-circle-green": "green" === n,
                     "jp-circle-red": "red" === n,
                     "jp-circle-yellow": "yellow" === n,
                     "jp-circle-gray": "gray" === n
                 });
                 return m().createElement("div", Object.assign({
                     className: l
                 }, r), t)
             };
-            const ne = ["unmounting", "mounting", "error"],
-                re = ({
+            const re = ["unmounting", "mounting", "error"],
+                le = ({
                     item: e,
                     open: t,
                     updateData: a
                 }) => {
                     const [n, r] = (0, o.useState)(!1), l = e.branch, s = "Unmount", i = e.how_many_commits_behind;
                     return (0, o.useEffect)((() => {
-                        r(ne.includes(e.state))
+                        r(re.includes(e.state))
                     }), [e]), m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name-branch-wrapper " + (n ? "pachyderm-mount-sortableList-disabled" : ""),
                         onClick: () => {
                             t(e.name)
@@ -3225,15 +3288,15 @@
                         className: "pachyderm-mount-list-item-action"
                     }, m().createElement("button", {
                         disabled: n,
                         onClick: () => {
                             return t = void 0, n = void 0, s = function*() {
                                 r(!0);
                                 try {
-                                    const t = yield D("_unmount", "PUT", {
+                                    const t = yield A("_unmount", "PUT", {
                                         mounts: [`${e.name}`]
                                     });
                                     a(t)
                                 } catch (e) {
                                     console.log("error unmounting repo")
                                 }
                             }, new((l = void 0) || (l = Promise))((function(e, a) {
@@ -3278,44 +3341,44 @@
                             case "unmounting":
                             case "mounting":
                                 a = "yellow";
                                 break;
                             case "error":
                                 a = "red"
                         }
-                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(ae, {
+                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(ne, {
                             color: a,
                             className: "pachyderm-mount-list-item-status-circle"
                         }), m().createElement("div", {
                             "data-testid": "ListItem__statusIcon",
                             className: "pachyderm-mount-list-item-status-icon",
                             title: n
                         }, m().createElement(y.react, {
                             tag: "span"
                         })))
                     })(e.state, e.status))))
                 };
-            const le = ({
+            const se = ({
                     item: e,
                     updateData: t,
                     mountedItems: a
                 }) => {
                     var n;
-                    const [r, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(!1), p = (null === (n = null == e ? void 0 : e.branches) || void 0 === n ? void 0 : n.length) > 0, f = "Mount";
+                    const [r, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, p] = (0, o.useState)(!1), h = (null === (n = null == e ? void 0 : e.branches) || void 0 === n ? void 0 : n.length) > 0, f = "Mount";
                     return (0, o.useEffect)((() => {
-                        h("none" !== e.authorization)
+                        p("none" !== e.authorization)
                     }), [e]), (0, o.useEffect)((() => {
                         const t = a.find((t => t.repo === e.repo && t.project === e.project && t.branch === r));
                         i(!!t)
                     }), [a, r]), (0, o.useEffect)((() => {
-                        if (p) {
+                        if (h) {
                             const t = e.branches.find((e => "master" === e));
                             l(t || e.branches[0]), d(!1)
                         }
-                    }), [e]), u ? p ? m().createElement("li", {
+                    }), [e]), u ? h ? m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name-branch-wrapper " + (c ? "pachyderm-mount-sortableList-disabled" : "")
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
@@ -3338,15 +3401,15 @@
                     }, m().createElement("button", {
                         disabled: c || s,
                         onClick: () => {
                             return a = void 0, n = void 0, s = function*() {
                                 d(!0);
                                 try {
                                     if (r) {
-                                        const a = yield D("_mount", "PUT", {
+                                        const a = yield A("_mount", "PUT", {
                                             mounts: [{
                                                 name: "master" === r ? `${e.project}_${e.repo}` : `${e.project}_${e.repo}_${r}`,
                                                 repo: e.repo,
                                                 branch: r,
                                                 project: e.project,
                                                 mode: "ro"
                                             }]
@@ -3408,34 +3471,34 @@
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
                     }, `${e.project}_${e.repo}`), m().createElement("span", {
                         className: "pachyderm-mount-list-item-branch"
                     }, "No read access")))
                 },
-                se = {
+                ie = {
                     name: "Name",
-                    func: K,
+                    func: Q,
                     accessor: e => "name" in e ? e.name : `${e.project}_${e.repo}`
                 },
-                ie = ({
+                ce = ({
                     open: e,
                     items: t,
                     updateData: a,
                     mountedItems: n,
                     type: r,
                     projects: l
                 }) => {
                     const s = "All projects",
                         i = l.map((e => e.project.name)),
                         [c, d] = (0, o.useState)(s),
                         {
                             sortedData: u,
-                            setComparator: h,
-                            reversed: p
+                            setComparator: p,
+                            reversed: h
                         } = (({
                             data: e,
                             initialSort: t = {
                                 func: () => 1,
                                 name: "",
                                 accessor: e => e
                             },
@@ -3445,25 +3508,25 @@
                                 s((t => (e.name === t.name || e.reverse ? r(-1 * n) : r(1), e)))
                             }), [n]);
                             return {
                                 sortedData: (0, o.useMemo)((() => [...e].sort(((e, t) => n * l.func(l.accessor(e), l.accessor(t))))), [l, e, n]),
                                 reversed: -1 === n,
                                 setComparator: i,
                                 comparatorName: l.name,
-                                numberComparator: Q,
-                                stringComparator: K
+                                numberComparator: ee,
+                                stringComparator: Q
                             }
                         })({
                             data: t,
-                            initialSort: se,
+                            initialSort: ie,
                             initialDirection: 1
                         }),
                         f = (0, o.useCallback)((() => {
-                            h(se)
-                        }), [h]);
+                            p(ie)
+                        }), [p]);
                     return m().createElement("div", {
                         className: "pachyderm-mount-sortableList"
                     }, "unmounted" === r && m().createElement("div", {
                         className: "pachyderm-mount-sortableList-projectFilter"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-projectFilter-headerItem"
                     }, m().createElement("span", null, "Project: "), m().createElement("select", {
@@ -3481,29 +3544,29 @@
                         key: e,
                         value: e
                     }, e)))))), m().createElement("div", {
                         className: "pachyderm-mount-sortableList-header"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-sortableList-headerItem",
                         onClick: f
-                    }, m().createElement("span", null, "Name"), m().createElement("span", null, p ? m().createElement(g.caretDownIcon.react, null) : m().createElement(g.caretUpIcon.react, null)))), m().createElement("ul", {
+                    }, m().createElement("span", null, "Name"), m().createElement("span", null, h ? m().createElement(g.caretDownIcon.react, null) : m().createElement(g.caretUpIcon.react, null)))), m().createElement("ul", {
                         className: "pachyderm-mount-sortableList-content"
-                    }, u && u.map((t => "name" in t ? m().createElement(re, {
+                    }, u && u.map((t => "name" in t ? m().createElement(le, {
                         item: t,
                         key: t.name,
                         open: e,
                         updateData: a
-                    }) : (c === t.project || c === s) && m().createElement(le, {
+                    }) : (c === t.project || c === s) && m().createElement(se, {
                         item: t,
                         key: `${t.project}_${t.repo}`,
                         updateData: a,
                         mountedItems: n
                     })))))
                 },
-                ce = e => o.createElement("svg", Object.assign({
+                oe = e => o.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 400,
                     height: 180,
                     viewBox: "320 -20 180 270",
                     xmlnsXlink: "http://www.w3.org/1999/xlink"
                 }, e), o.createElement("defs", null, o.createElement("path", {
                     id: "genericError_svg__b",
@@ -4018,56 +4081,56 @@
                     d: "M142.52 208.32 154 228.48h-22.96z"
                 }), o.createElement("path", {
                     d: "M607.04 74.706c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5zm-5.6-11.2c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5z",
                     stroke: "#26101A",
                     strokeWidth: 1.4,
                     fill: "#C3E5D7"
                 }))),
-                oe = e => o.createElement("svg", Object.assign({
+                me = e => o.createElement("svg", Object.assign({
                     width: 20,
                     height: 20,
                     xmlns: "http://www.w3.org/2000/svg",
                     viewBox: "0 0 16 16"
                 }, e), o.createElement("g", {
                     fill: "none",
                     fillRule: "evenodd"
                 }, o.createElement("path", {
                     d: "M0 0h16v16H0z"
                 }), o.createElement("path", {
                     d: "M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0Zm0 11.65a1.2 1.2 0 1 0 0 2.4 1.2 1.2 0 0 0 0-2.4Zm0-9.7a1.2 1.2 0 0 0-1.2 1.2v5.6a1.2 1.2 0 1 0 2.4 0v-5.6A1.2 1.2 0 0 0 8 1.95Z",
                     fill: "#BF444F"
                 }))),
-                me = ({
+                de = ({
                     status: e
                 }) => m().createElement("div", {
                     className: "pachyderm-mount-base",
                     style: {
                         display: "flex",
                         flexDirection: "column",
                         alignItems: "center",
                         justifyContent: "center"
                     }
-                }, m().createElement("div", null, m().createElement(ce, {
+                }, m().createElement("div", null, m().createElement(oe, {
                     width: "280px",
                     height: "130px"
                 })), m().createElement("div", {
                     style: {
                         display: "flex",
                         flexDirection: "row",
                         alignItems: "center",
                         paddingBottom: "1rem"
                     }
-                }, m().createElement(oe, null), m().createElement("span", {
+                }, m().createElement(me, null), m().createElement("span", {
                     style: {
                         paddingLeft: ".5rem"
                     }
                 }, "Looks like there was an error")), m().createElement("div", {
                     "data-testid": "FullPageError__message"
                 }, e.message));
-            var de = function(e, t, a, n) {
+            var ue = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -4086,61 +4149,61 @@
                         e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
-            const ue = "mount-browser:",
+            const pe = "mount-browser:",
                 he = "pachyderm_pps";
-            class pe {
+            class fe {
                 constructor(e, t, a, n, r, l) {
                     this._showConfig = !1, this._showConfigSignal = new N.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new N.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new N.Signal(this), this._showPipelineSignal = new N.Signal(this), this._ppsContextSignal = new N.Signal(this), this.isCurrentWidgetNotebook = e => (e = null != e ? e : this._widgetTracker.currentWidget) instanceof L.NotebookPanel, this.getActiveNotebook = () => {
                         const e = this._widgetTracker.currentWidget;
                         return this.isCurrentWidgetNotebook(e) ? e : null
-                    }, this.handleWidgetChanged = (e, t) => de(this, void 0, void 0, (function*() {
+                    }, this.handleWidgetChanged = (e, t) => ue(this, void 0, void 0, (function*() {
                         this.isCurrentWidgetNotebook(t.newValue) && (yield this.handleNotebookChanged(t.newValue)), this.setShowPipeline(this._showPipeline), yield Promise.resolve()
-                    })), this.handleNotebookChanged = e => de(this, void 0, void 0, (function*() {
+                    })), this.handleNotebookChanged = e => ue(this, void 0, void 0, (function*() {
                         yield e.sessionContext.ready, e.context.fileChanged.connect(this.handleNotebookReload);
                         const t = {
                             metadata: this.getNotebookMetadata(e),
                             notebookModel: e.context.contentsModel
                         };
                         this._ppsContextSignal.emit(t), yield Promise.resolve()
-                    })), this.handleNotebookReload = (e, t) => de(this, void 0, void 0, (function*() {
+                    })), this.handleNotebookReload = (e, t) => ue(this, void 0, void 0, (function*() {
                         const e = {
                             metadata: this.getNotebookMetadata(),
                             notebookModel: t
                         };
                         this._ppsContextSignal.emit(e), yield Promise.resolve()
                     })), this.getNotebookMetadata = e => {
                         var t;
                         return null === (t = null == (e = null != e ? e : this.getActiveNotebook()) ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(he)
                     }, this.saveNotebookMetadata = e => {
                         var t;
                         const a = this.getActiveNotebook();
                         null !== a ? (null === (t = null == a ? void 0 : a.model) || void 0 === t || t.metadata.set(he, e), console.log("notebook metadata saved")) : console.log("No active notebook")
-                    }, this.saveNotebookToDisk = () => de(this, void 0, void 0, (function*() {
+                    }, this.saveNotebookToDisk = () => ue(this, void 0, void 0, (function*() {
                         const e = this.getActiveNotebook();
                         return null !== e ? (yield e.context.ready, yield e.context.save(), yield e.context.ready, e.context.contentsModel.last_modified) : null
                     })), this.open = e => {
                         this._app.commands.execute("filebrowser:open-path", {
-                            path: ue + e
+                            path: pe + e
                         })
-                    }, this.refresh = (e, t) => de(this, void 0, void 0, (function*() {
+                    }, this.refresh = (e, t) => ue(this, void 0, void 0, (function*() {
                         yield this._mountBrowser.model.refresh()
                     })), this.verifyBrowserPath = (e, t) => {
                         this._mountBrowser.model.path !== this._mountBrowser.model.rootPath && (this.isValidBrowserPath(this._mountBrowser.model.path, t) || this.open(""))
                     }, this.isValidBrowserPath = (e, t) => {
-                        const a = e.split(ue)[1].split("/")[0];
+                        const a = e.split(pe)[1].split("/")[0];
                         if ("out" === a) return !0;
                         for (let e = 0; e < t.length; e++)
                             if (a === t[e].name) return !0;
                         return !1
-                    }, this.setShowDatum = e => de(this, void 0, void 0, (function*() {
+                    }, this.setShowDatum = e => ue(this, void 0, void 0, (function*() {
                         e ? (this._datum.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this.saveMountedReposList()) : (this._datum.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), yield this.restoreMountedReposList()), this._mountBrowser.setHidden(!1), this._config.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showDatum = e, this._showDatumSignal.emit(e)
                     })), this.saveMountedReposList = () => {
                         const e = this._poller.mounted,
                             t = [];
                         for (let a = 0; a < e.length; a++) {
                             const n = {
                                 pfs: Object.assign(Object.assign(Object.assign(Object.assign(Object.assign({
@@ -4158,15 +4221,15 @@
                                 })
                             };
                             t.push(n)
                         }
                         0 === e.length ? this._repoViewInputSpec = {} : 1 === e.length ? this._repoViewInputSpec = t[0] : this._repoViewInputSpec = {
                             cross: t
                         }, this._saveInputSpecSignal.emit(this._repoViewInputSpec)
-                    }, this.restoreMountedReposList = () => de(this, void 0, void 0, (function*() {
+                    }, this.restoreMountedReposList = () => ue(this, void 0, void 0, (function*() {
                         const e = [];
                         if (Object.prototype.hasOwnProperty.call(this._repoViewInputSpec, "cross") && Array.isArray(this._repoViewInputSpec.cross))
                             for (let t = 0; t < this._repoViewInputSpec.cross.length; t++) {
                                 const a = this._repoViewInputSpec.cross[t].pfs;
                                 e.push({
                                     name: a.name ? a.name : a.repo,
                                     repo: a.repo,
@@ -4180,15 +4243,15 @@
                                     name: t.name ? t.name : t.repo,
                                     repo: t.repo,
                                     project: t.project ? t.project : "default",
                                     branch: t.branch ? t.branch : "master",
                                     mode: "ro"
                                 })
                             } if (e.length > 0) {
-                            const t = yield D("_mount", "PUT", {
+                            const t = yield A("_mount", "PUT", {
                                 mounts: e
                             });
                             this._poller.updateData(t)
                         }
                         this.open("")
                     })), this.setShowPipeline = e => {
                         e ? this.isCurrentWidgetNotebook() ? (this._pipeline.setHidden(!1), this._pipelineSplash.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._pipeline.setHidden(!0), this._pipelineSplash.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._pipeline.setHidden(!0), this._pipelineSplash.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._config.setHidden(!0), this._datum.setHidden(!0), this._fullPageError.setHidden(!0), this._showPipeline = e, this._showPipelineSignal.emit(e)
@@ -4196,18 +4259,18 @@
                         this._keepMounted = e
                     }, this.setShowConfig = e => {
                         e ? (this._config.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._config.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showConfig = e, this._showConfigSignal.emit(e)
                     }, this.setShowFullPageError = e => {
                         e ? (this._fullPageError.setHidden(!1), this._config.setHidden(!0), this._datum.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0), this._pipeline.setHidden(!0)) : (this._fullPageError.setHidden(!0), this._config.setHidden(!1), this._datum.setHidden(!1), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1), this._pipeline.setHidden(!1))
                     }, this.updateConfig = e => {
                         this._poller.config = e
-                    }, this.setup = () => de(this, void 0, void 0, (function*() {
+                    }, this.setup = () => ue(this, void 0, void 0, (function*() {
                         if (yield this._poller.refresh(), 500 === this._poller.status.code) this.setShowFullPageError(!0);
                         else if (this.setShowConfig("INVALID" === this._poller.config.cluster_status || 200 !== this._poller.status.code), 200 === this._poller.status.code) try {
-                            const e = yield D("datums", "GET");
+                            const e = yield A("datums", "GET");
                             e.num_datums > 0 && (this._keepMounted = !0, this._currentDatumInfo = e, yield this.setShowDatum(!0))
                         } catch (e) {
                             console.log(e)
                         }
                         this._loader.setHidden(!0)
                     })), this._app = e, this._poller = new F("PollMounts"), this._repoViewInputSpec = {}, this._widgetTracker = l, this._poller.configSignal.connect(((e, t) => {
                         "INVALID" !== t.cluster_status || this._showConfig || this.setShowConfig(!0)
@@ -4248,30 +4311,30 @@
                         className: "pachyderm-button-alpha-notice"
                     }, "Alpha")), m().createElement("button", {
                         className: "pachyderm-button-link",
                         onClick: () => this.setShowConfig(!0)
                     }, m().createElement(g.settingsIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
-                    }))), m().createElement(ie, {
+                    }))), m().createElement(ce, {
                         open: this.open,
                         items: t || this._poller.mounted,
                         updateData: this._poller.updateData,
                         mountedItems: [],
                         type: "mounted",
                         projects: []
                     }))))), this._mountedList.addClass("pachyderm-mount-react-wrapper"), this._unmountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.unmountedSignal
                     }, ((e, t) => m().createElement(d.UseSignal, {
                         signal: this._poller.projectSignal
                     }, ((e, a) => m().createElement("div", {
                         className: "pachyderm-mount-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-base-title"
-                    }, "Unmounted Repositories"), m().createElement(ie, {
+                    }, "Unmounted Repositories"), m().createElement(ce, {
                         open: this.open,
                         items: t || this._poller.unmounted,
                         updateData: this._poller.updateData,
                         mountedItems: this._poller.mounted,
                         type: "unmounted",
                         projects: a || this._poller.projects
                     }))))))), this._unmountedList.addClass("pachyderm-mount-react-wrapper"), this._datum = d.ReactWidget.create(m().createElement(d.UseSignal, {
@@ -4285,25 +4348,25 @@
                         setKeepMounted: this.setKeepMounted,
                         open: this.open,
                         pollRefresh: this._poller.refresh,
                         currentDatumInfo: this._currentDatumInfo,
                         repoViewInputSpec: a || this._repoViewInputSpec
                     })))))), this._datum.addClass("pachyderm-mount-datum-wrapper"), this._pipeline = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._ppsContextSignal
-                    }, ((e, a) => m().createElement(Y, {
+                    }, ((e, a) => m().createElement(X, {
                         ppsContext: a,
                         settings: t,
                         setShowPipeline: this.setShowPipeline,
                         saveNotebookMetadata: this.saveNotebookMetadata,
                         saveNotebookToDisk: this.saveNotebookToDisk
-                    })))), this._pipelineSplash = d.ReactWidget.create(m().createElement(X, {
+                    })))), this._pipelineSplash = d.ReactWidget.create(m().createElement(K, {
                         setShowPipeline: this.setShowPipeline
                     })), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._pipelineSplash.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(W, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
-                    }, ((e, t) => m().createElement(me, {
+                    }, ((e, t) => m().createElement(de, {
                         status: t || this._poller.status
                     })))), this._fullPageError.addClass("pachyderm-mount-react-wrapper"), this._mountBrowser = ((e, t, a) => {
                         var n;
                         const r = new H(e.docRegistry);
                         t.services.contents.addDrive(r);
                         const l = a.createFileBrowser("jupyterlab-pachyderm-browser", {
                             driveName: r.name,
@@ -4335,15 +4398,15 @@
                                     }
                                 }), e.addCommand("copy-path", {
                                     label: "Copy Path",
                                     icon: "fa fa-file",
                                     mnemonic: 0,
                                     execute: () => {
                                         (0, P.each)(l.selectedItems(), (e => {
-                                            d.Clipboard.copyToSystem(e.path.replace(ue, "/pfs/"))
+                                            d.Clipboard.copyToSystem(e.path.replace(pe, "/pfs/"))
                                         }))
                                     }
                                 });
                                 const a = new B.Menu({
                                     commands: e
                                 });
                                 a.addItem({
@@ -4376,27 +4439,27 @@
                 get layout() {
                     return this._panel
                 }
                 get ready() {
                     return this._readyPromise
                 }
             }
-            const fe = "jupyterlab-pachyderm:mount",
-                Ee = [{
-                    id: fe,
+            const Ee = "jupyterlab-pachyderm:mount",
+                _e = [{
+                    id: Ee,
                     autoStart: !0,
                     requires: [M.IDocumentManager, S.IFileBrowserFactory, C.ILayoutRestorer, C.ILabShell, z.ISettingRegistry],
                     activate: (e, t, a, n, r, l) => {
                         const s = {
                                 defaultPipelineImage: ""
                             },
                             i = e => {
                                 s.defaultPipelineImage = e.get("defaultPipelineImage").composite
                             };
-                        return Promise.all([l.load(fe), e.restored]).then((([e]) => {
+                        return Promise.all([l.load(Ee), e.restored]).then((([e]) => {
                             i(e), e.changed.connect(i)
-                        })), new pe(e, s, t, a, n, r)
+                        })), new fe(e, s, t, a, n, r)
                     }
-                }, i, p, x]
+                }, i, h, x]
         }
     }
 ]);
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, u, i, d, f, s, p, c, h, b, v, m, y = {
             6334: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(371), t.e(829)]).then((() => () => t(7363))),
-                        "./extension": () => Promise.all([t.e(371), t.e(829)]).then((() => () => t(7363))),
+                        "./index": () => Promise.all([t.e(371), t.e(199)]).then((() => () => t(843))),
+                        "./extension": () => Promise.all([t.e(371), t.e(199)]).then((() => () => t(843))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -45,26 +45,26 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         67: "9d3e2934cfe0e102619e",
+        199: "6f6cc83faa1bc2d85def",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
-        747: "b62f963856036a13fba1",
-        829: "7feefb314c4865d398d2"
+        747: "b62f963856036a13fba1"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
+        199: "6f6cc83faa1bc2d85def",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
-        747: "b62f963856036a13fba1",
-        829: "7feefb314c4865d398d2"
+        747: "b62f963856036a13fba1"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.5", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-rc.1", (() => Promise.all([j.e(371), j.e(199)]).then((() => () => j(843))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -242,15 +242,15 @@
         7638: () => c("default", "@jupyterlab/application", [1, 3, 6, 5]),
         8299: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 5]),
         8535: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
         8832: () => c("default", "@lumino/widgets", [1, 1, 37, 2]),
         8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
         9071: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 5])
     }, m = {
-        829: [122, 127, 344, 930, 931, 1526, 1745, 1840, 4234, 4439, 5139, 6057, 6271, 6303, 7638, 8299, 8535, 8832, 8918, 9071]
+        199: [122, 127, 344, 930, 931, 1526, 1745, 1840, 4234, 4439, 5139, 6057, 6271, 6303, 7638, 8299, 8535, 8832, 8918, 9071]
     }, j.f.consumes = (e, r) => {
         j.o(m, e) && m[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pps_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -129,14 +129,17 @@
 @dataclass
 class PpsConfig:
 
     notebook_path: Path
     pipeline: Pipeline
     image: str
     requirements: Optional[str]
+    port: str
+    gpu_mode: str
+    resource_spec: dict
     input_spec: dict  # We may be able to use the pachyderm SDK to parse and validate.
 
     @classmethod
     def from_notebook(cls, notebook_path: Union[str, Path]) -> "PpsConfig":
         """Parses a config from the metadata of a notebook file.
 
         Raises ValueError if required field is not specified.
@@ -168,21 +171,31 @@
 
         requirements = config.get('requirements')
 
         input_spec_str = config.get('input_spec')
         if input_spec_str is None:
             raise ValueError("field input_spec not set")
         input_spec = yaml.safe_load(input_spec_str)
+        
+        port = config.get('port')
+
+        gpu_mode = config.get('gpu_mode')
+        resource_spec_str = config.get('resource_spec')
+
+        resource_spec = dict() if resource_spec_str is None else yaml.safe_load(resource_spec_str)
 
         return cls(
             notebook_path=notebook_path,
             pipeline=pipeline,
             image=image,
             requirements=requirements,
-            input_spec=input_spec
+            input_spec=input_spec,
+            port=port,
+            gpu_mode=gpu_mode,
+            resource_spec=resource_spec,
         )
 
     def to_dict(self):
         data = asdict(self)
         del data['notebook_path']
         return data
 
@@ -201,25 +214,46 @@
                 )
             )
         ]
     )
     pipeline = dict(name=config.pipeline.name)
     if config.pipeline.project and config.pipeline.project.name:
         pipeline['project'] = dict(name=config.pipeline.project.name)
-    return dict(
+    pipelineSpec =  dict(
         pipeline=pipeline,
         description="Auto-generated from notebook",
         transform=dict(
             cmd=["python3", "-u", f"/pfs/{companion_repo}/entrypoint.py"],
             image=config.image
         ),
+
         input=input_spec,
         update=True,
         reprocess=True,
     )
+    if config.port:
+        pipelineSpec['service'] = dict(
+            external_port=config.port,
+            internal_port=config.port,
+            type="LoadBalancer"
+        )
+    
+    if config.gpu_mode == "Simple":
+        pipelineSpec['resource_limits'] = dict(
+            gpu=dict(
+                type="nvidia.com/gpu",
+                number="1",
+            )
+        )
+    elif config.gpu_mode == "Advanced":
+        pipelineSpec['resource_limits'] = config.resource_spec
+        pass
+
+
+    return pipelineSpec
 
 
 def upload_environment(
         client: python_pachyderm.Client, repo: str, config: PpsConfig, script: bytes
 ) -> str:
     """Manages the pipeline's "environment" through a companion repo.
 
@@ -242,15 +276,17 @@
 
         from pathlib import Path
         from subprocess import run
 
         reqs = Path(__file__).parent.joinpath("requirements.txt")
         if reqs.exists():
             run(["pip", "--disable-pip-version-check", "install", "-r", reqs.as_posix()])
-
+            print("Finished installing requirements")
+        
+        print("running user code")
         import user_code  # This runs the user's code.
 
     entrypoint_script = (
         f'{dedent(getsource(entrypoint))}\n\n'
         'if __name__ == "__main__":\n'
         '    entrypoint()\n'
     )
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,14 +420,15 @@
     Returns a serialized JSON object that can be written to a file.
     """
     notebook_data = json.loads(notebook.read_bytes())
     config = PpsConfig.from_notebook(notebook)
     config.pipeline = dict(name=pipeline_name, project=dict(name=project_name))
     # sub in repo_name
     config.input_spec = f"pfs:\n  repo: {repo_name}\n  glob: \"/*\""
+    config.resource_spec = "" # this is currently not being tested so it is set to the empty string
     config.requirements = str(notebook.with_name(config.requirements).relative_to(os.getcwd()))
     notebook_data['metadata'][METADATA_KEY]['config'] = config.to_dict()
     return json.dumps(notebook_data)
 
 
 @pytest.fixture
 def notebook_path(simple_pachyderm_env) -> Path:
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.7.0a5
+Version: 2.7.0rc1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 jupyterlab_pachyderm.egg-info/top_level.txt
 jupyterlab_pachyderm/labextension/package.json
 jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
 jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
 jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
 jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
 jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
-jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/package.json` & `jupyterlab_pachyderm-2.7.0rc1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-rc.1'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.5"
+    "version": "2.7.0-rc.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/pyproject.toml` & `jupyterlab_pachyderm-2.7.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/setup.cfg` & `jupyterlab_pachyderm-2.7.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/setup.py` & `jupyterlab_pachyderm-2.7.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/handler.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import React from 'react';
 import {closeIcon} from '@jupyterlab/ui-components';
 import {usePipeline} from './hooks/usePipeline';
-import {PpsContext, PpsMetadata, MountSettings} from '../../types';
+import {PpsContext, PpsMetadata, MountSettings, GpuMode} from '../../types';
 
 type PipelineProps = {
   ppsContext: PpsContext | undefined;
   settings: MountSettings;
   setShowPipeline: (shouldShow: boolean) => void;
   saveNotebookMetadata: (metadata: PpsMetadata) => void;
   saveNotebookToDisk: () => Promise<string | null>;
 };
 
+const placeholderAdvancedResourceSpec = `# example:
+gpu:
+  type: nvidia.com/gpu
+  number: 1
+`;
+const placeholderSimpleResourceSpec = `gpu:
+  type: nvidia.com/gpu
+  number: 1
+`;
 const placeholderInputSpec = `# example:
 pfs:
   repo: images
   branch: dev
   glob: /*
 `;
 const placeholderRequirements = './requirements.txt';
@@ -33,14 +42,20 @@
     setPipelineName,
     pipelineProject,
     setPipelineProject,
     imageName,
     setImageName,
     inputSpec,
     setInputSpec,
+    pipelinePort,
+    setPipelinePort,
+    gpuMode,
+    setGpuMode,
+    resourceSpec,
+    setResourceSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
     currentNotebook,
     errorMessage,
     responseMessage,
   } = usePipeline(
@@ -153,14 +168,29 @@
           onChange={(e: any) => {
             setRequirements(e.target.value);
           }}
           disabled={loading}
           placeholder={placeholderRequirements}
         ></input>
       </div>
+      <div className="pachyderm-pipeline-input-wrapper">
+        <label className="pachyderm-pipeline-input-label" htmlFor="port">
+          Port:{'  '}
+        </label>
+        <input
+          className="pachyderm-pipeline-input"
+          data-testid="Pipeline__inputPort"
+          name="port"
+          value={pipelinePort}
+          onChange={(e: any) => {
+            setPipelinePort(e.target.value);
+          }}
+          disabled={loading}
+        ></input>
+      </div>
       <div className="pachyderm-pipeline-textarea-wrapper">
         <label
           className="pachyderm-pipeline-textarea-label"
           htmlFor="inputSpec"
         >
           Pipeline Input Spec:
         </label>
@@ -172,15 +202,53 @@
           onChange={(e: any) => {
             setInputSpec(e.target.value);
           }}
           disabled={loading}
           placeholder={placeholderInputSpec}
         ></textarea>
       </div>
-
+      <div className="pachyderm-pipeline-input-wrapper">
+        <label className="pachyderm-pipeline-input-label" htmlFor="gpuMode">
+          *Gpu Mode:{'  '}
+        </label>
+        <select
+          className="pachyderm-pipeline-input"
+          data-testid="Pipeline__gpuMode"
+          name="gpuMode"
+          value={gpuMode}
+          onChange={(e: any) => {
+            setGpuMode(e.target.value);
+          }}
+        >
+          {(Object.keys(GpuMode) as Array<GpuMode>).map((mode) => (
+            <option value={mode}>{mode}</option>
+          ))}
+        </select>
+      </div>
+      {gpuMode === GpuMode.Advanced && (
+        <div className="pachyderm-pipeline-textarea-wrapper">
+          <label
+            className="pachyderm-pipeline-textarea-label"
+            htmlFor="resourceSpec"
+          >
+            Pipeline Resource Spec:
+          </label>
+          <textarea
+            className="pachyderm-pipeline-textarea pachyderm-input"
+            data-testid="Pipeline__resourceSpecInput"
+            name="resourceSpec"
+            value={resourceSpec}
+            onChange={(e: any) => {
+              setResourceSpec(e.target.value);
+            }}
+            disabled={loading}
+            placeholder={placeholderAdvancedResourceSpec}
+          ></textarea>
+        </div>
+      )}
       <div className="pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper">
         <label className="pachyderm-pipeline-preview-label">
           Pipeline Spec Preview: {'  '}
         </label>
         <textarea
           className="pachyderm-pipeline-spec-preview-textarea"
           style={{backgroundColor: '#80808080'}}
@@ -192,15 +260,28 @@
 transform:
   image: ${imageName}
 input:
 ${inputSpec
   .split('\n')
   .map((line, _, __) => '  ' + line)
   .join('\n')}
-`}
+${
+  gpuMode === GpuMode.None
+    ? ''
+    : 'resource_limits:\n' +
+      (gpuMode === GpuMode.Simple
+        ? placeholderSimpleResourceSpec
+        : gpuMode === GpuMode.Advanced
+        ? resourceSpec
+        : ''
+      )
+        .split('\n')
+        .map((line, _, __) => '  ' + line)
+        .join('\n')
+}`}
           readOnly={true}
         ></textarea>
       </div>
 
       <div className="pachyderm-pipeline-buttons">
         <button
           data-testid="Pipeline__create_pipeline"
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import {useEffect, useState} from 'react';
 import {ServerConnection} from '@jupyterlab/services';
 
 import {
   CreatePipelineResponse,
+  GpuMode,
   MountSettings,
   PpsContext,
   PpsMetadata,
 } from '../../../types';
 import {requestAPI} from '../../../../../handler';
 
 export const PPS_VERSION = 'v1.0.0';
@@ -17,14 +18,20 @@
   setPipelineName: (input: string) => void;
   pipelineProject: string;
   setPipelineProject: (input: string) => void;
   imageName: string;
   setImageName: (input: string) => void;
   inputSpec: string;
   setInputSpec: (input: string) => void;
+  pipelinePort: string;
+  setPipelinePort: (input: string) => void;
+  gpuMode: GpuMode;
+  setGpuMode: (input: GpuMode) => void;
+  resourceSpec: string;
+  setResourceSpec: (input: string) => void;
   requirements: string;
   setRequirements: (input: string) => void;
   callCreatePipeline: () => Promise<void>;
   currentNotebook: string;
   errorMessage: string;
   responseMessage: string;
 };
@@ -36,14 +43,17 @@
   saveNotebookToDisk: () => Promise<string | null>,
 ): usePipelineResponse => {
   const [loading, setLoading] = useState(false);
   const [pipelineName, setPipelineName] = useState('');
   const [pipelineProject, setPipelineProject] = useState('');
   const [imageName, setImageName] = useState('');
   const [inputSpec, setInputSpec] = useState('');
+  const [pipelinePort, setPipelinePort] = useState('');
+  const [gpuMode, setGpuMode] = useState(GpuMode.None);
+  const [resourceSpec, setResourceSpec] = useState('');
   const [requirements, setRequirements] = useState('');
   const [errorMessage, setErrorMessage] = useState('');
   const [responseMessage, setResponseMessage] = useState('');
   const [currentNotebook, setCurrentNotebook] = useState('None');
 
   useEffect(() => {
     setImageName(
@@ -57,20 +67,32 @@
     setResponseMessage('');
     if (ppsContext?.metadata?.config.input_spec) {
       setInputSpec(ppsContext.metadata.config.input_spec);
     } else {
       setInputSpec('');
     }
     setCurrentNotebook(ppsContext?.notebookModel?.name ?? 'None');
+    setPipelinePort(ppsContext?.metadata?.config.port ?? '');
+    setGpuMode(ppsContext?.metadata?.config.gpu_mode ?? GpuMode.None);
+    setResourceSpec(ppsContext?.metadata?.config.resource_spec ?? '');
   }, [ppsContext]);
 
   useEffect(() => {
     const ppsMetadata: PpsMetadata = buildMetadata();
     saveNotebookMetaData(ppsMetadata);
-  }, [pipelineName, pipelineProject, imageName, requirements, inputSpec]);
+  }, [
+    pipelineName,
+    pipelineProject,
+    imageName,
+    requirements,
+    inputSpec,
+    pipelinePort,
+    gpuMode,
+    resourceSpec,
+  ]);
 
   let callCreatePipeline: () => Promise<void>;
   if (ppsContext?.notebookModel) {
     const notebook = ppsContext.notebookModel;
     callCreatePipeline = async () => {
       setLoading(true);
       setErrorMessage('');
@@ -112,28 +134,37 @@
     return {
       version: PPS_VERSION,
       config: {
         pipeline: {name: pipelineName, project: {name: pipelineProject}},
         image: imageName,
         requirements: requirements,
         input_spec: inputSpec,
+        port: pipelinePort,
+        gpu_mode: gpuMode,
+        resource_spec: resourceSpec,
       },
     };
   };
 
   return {
     loading,
     pipelineName,
     setPipelineName,
     pipelineProject,
     setPipelineProject,
     imageName,
     setImageName,
     inputSpec,
     setInputSpec,
+    pipelinePort,
+    setPipelinePort,
+    gpuMode,
+    setGpuMode,
+    resourceSpec,
+    setResourceSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
     currentNotebook,
     errorMessage,
     responseMessage,
   };
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/types.ts`

 * *Files 3% similar despite different names*

```diff
@@ -120,22 +120,31 @@
 };
 
 export type PpsMetadata = {
   version: string;
   config: PpsConfig;
 };
 
+export enum GpuMode {
+  None = 'None',
+  Simple = 'Simple',
+  Advanced = 'Advanced',
+}
+
 // If this is updated, make sure to also update the corresponding `useEffect`
 // call in ./components/Pipeline/hooks/usePipeline.tsx that writes this type to
 // the notebook metadata.
 export type PpsConfig = {
   pipeline: Pipeline;
   image: string;
   requirements: string | null;
   input_spec: string;
+  port: string;
+  gpu_mode: GpuMode;
+  resource_spec: string | null;
 };
 
 export type PpsContext = {
   metadata: PpsMetadata | null;
   notebookModel: Contents.IModel | null;
 };
```

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/src/utils/icons.ts` & `jupyterlab_pachyderm-2.7.0rc1/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/base.css` & `jupyterlab_pachyderm-2.7.0rc1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/components/button.css` & `jupyterlab_pachyderm-2.7.0rc1/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/icons/file.svg` & `jupyterlab_pachyderm-2.7.0rc1/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/icons/info.svg` & `jupyterlab_pachyderm-2.7.0rc1/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.7.0rc1/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a5/style/icons/repo.svg` & `jupyterlab_pachyderm-2.7.0rc1/style/icons/repo.svg`

 * *Files identical despite different names*

