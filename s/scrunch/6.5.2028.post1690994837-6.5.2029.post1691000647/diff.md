# Comparing `tmp/scrunch-6.5.2028.post1690994837.tar.gz` & `tmp/scrunch-6.5.2029.post1691000647.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrunch-6.5.2028.post1690994837.tar", last modified: Wed Aug  2 16:48:37 2023, max compression
+gzip compressed data, was "dist/scrunch-6.5.2029.post1691000647.tar", last modified: Wed Aug  2 18:25:07 2023, max compression
```

## Comparing `scrunch-6.5.2028.post1690994837.tar` & `scrunch-6.5.2029.post1691000647.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/.github/workflows/test-and-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/crunchboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)   126327 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/mutable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/streaming_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/subentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/crunch_test.ini
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/crunch_test_api_key.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38590 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/integration/scrunch_workflow_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/mock_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)   283761 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   100713 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/scrunch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/scrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 16:48:37.000000 scrunch-6.5.2028.post1690994837/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 16:48:25.000000 scrunch-6.5.2028.post1690994837/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/.github/workflows/test-and-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/crunchboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126327 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/mutable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/streaming_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/subentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/crunch_test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/crunch_test_api_key.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38590 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/integration/scrunch_workflow_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/mock_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283761 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100713 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/scrunch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/scrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 18:25:07.000000 scrunch-6.5.2029.post1691000647/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 18:25:00.000000 scrunch-6.5.2029.post1691000647/tox.ini
```

### Comparing `scrunch-6.5.2028.post1690994837/.github/workflows/test-and-deploy.yaml` & `scrunch-6.5.2029.post1691000647/.github/workflows/test-and-deploy.yaml`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/.gitignore` & `scrunch-6.5.2029.post1691000647/.gitignore`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/COPYING` & `scrunch-6.5.2029.post1691000647/COPYING`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/COPYING.LESSER` & `scrunch-6.5.2029.post1691000647/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/LICENSE` & `scrunch-6.5.2029.post1691000647/LICENSE`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/PKG-INFO` & `scrunch-6.5.2029.post1691000647/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 6.5.2028.post1690994837
+Version: 6.5.2029.post1691000647
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-6.5.2028.post1690994837/README.rst` & `scrunch-6.5.2029.post1691000647/README.rst`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/docs/conf.py` & `scrunch-6.5.2029.post1691000647/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/fixtures.py` & `scrunch-6.5.2029.post1691000647/integration/fixtures.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_accounts.py` & `scrunch-6.5.2029.post1691000647/integration/test_accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_backfill.py` & `scrunch-6.5.2029.post1691000647/integration/test_backfill.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_dataset.py` & `scrunch-6.5.2029.post1691000647/integration/test_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_folders.py` & `scrunch-6.5.2029.post1691000647/integration/test_folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_projects.py` & `scrunch-6.5.2029.post1691000647/integration/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_recodes.py` & `scrunch-6.5.2029.post1691000647/integration/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_scripts.py` & `scrunch-6.5.2029.post1691000647/integration/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/integration/test_views.py` & `scrunch-6.5.2029.post1691000647/integration/test_views.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/accounts.py` & `scrunch-6.5.2029.post1691000647/scrunch/accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/categories.py` & `scrunch-6.5.2029.post1691000647/scrunch/categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/connections.py` & `scrunch-6.5.2029.post1691000647/scrunch/connections.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/crunchboxes.py` & `scrunch-6.5.2029.post1691000647/scrunch/crunchboxes.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/cubes.py` & `scrunch-6.5.2029.post1691000647/scrunch/cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/datasets.py` & `scrunch-6.5.2029.post1691000647/scrunch/datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/expressions.py` & `scrunch-6.5.2029.post1691000647/scrunch/expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/folders.py` & `scrunch-6.5.2029.post1691000647/scrunch/folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/helpers.py` & `scrunch-6.5.2029.post1691000647/scrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/mutable_dataset.py` & `scrunch-6.5.2029.post1691000647/scrunch/mutable_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/order.py` & `scrunch-6.5.2029.post1691000647/scrunch/order.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/scripts.py` & `scrunch-6.5.2029.post1691000647/scrunch/scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/session.py` & `scrunch-6.5.2029.post1691000647/scrunch/session.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/streaming_dataset.py` & `scrunch-6.5.2029.post1691000647/scrunch/streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/subentity.py` & `scrunch-6.5.2029.post1691000647/scrunch/subentity.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/integration/scrunch_workflow_integration_test.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/integration/scrunch_workflow_integration_test.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/mock_session.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/mock_session.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_accounts.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_categories.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_cubes.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_datasets.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_expressions.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_folders.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_projects.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_recodes.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_scripts.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_teams.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_utilities.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/tests/test_views.py` & `scrunch-6.5.2029.post1691000647/scrunch/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/variables.py` & `scrunch-6.5.2029.post1691000647/scrunch/variables.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch/views.py` & `scrunch-6.5.2029.post1691000647/scrunch/views.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/scrunch.egg-info/PKG-INFO` & `scrunch-6.5.2029.post1691000647/scrunch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 6.5.2028.post1690994837
+Version: 6.5.2029.post1691000647
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-6.5.2028.post1690994837/scrunch.egg-info/SOURCES.txt` & `scrunch-6.5.2029.post1691000647/scrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/setup.py` & `scrunch-6.5.2029.post1691000647/setup.py`

 * *Files identical despite different names*

### Comparing `scrunch-6.5.2028.post1690994837/tox.ini` & `scrunch-6.5.2029.post1691000647/tox.ini`

 * *Files identical despite different names*

