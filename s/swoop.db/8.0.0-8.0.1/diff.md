# Comparing `tmp/swoop.db-8.0.0.tar.gz` & `tmp/swoop.db-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-8.0.0.tar", last modified: Tue Aug  1 19:06:15 2023, max compression
+gzip compressed data, was "swoop.db-8.0.1.tar", last modified: Thu Aug  3 16:49:58 2023, max compression
```

## Comparing `swoop.db-8.0.0.tar` & `swoop.db-8.0.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-01 19:05:59.000000 swoop.db-8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-01 19:05:59.000000 swoop.db-8.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-01 19:05:59.000000 swoop.db-8.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-01 19:05:59.000000 swoop.db-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-01 19:06:15.509295 swoop.db-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-08-01 19:05:59.000000 swoop.db-8.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-01 19:05:59.000000 swoop.db-8.0.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3622 2023-08-01 19:05:59.000000 swoop.db-8.0.0/bin/db-initialization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-08-01 19:05:59.000000 swoop.db-8.0.0/bin/get-max-migration-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 19:05:59.000000 swoop.db-8.0.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 19:05:59.000000 swoop.db-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 19:05:59.000000 swoop.db-8.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:06:15.509295 swoop.db-8.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/migrations/00008_new_base.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/fixtures/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/fixtures/migrations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_uuid_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.013973 swoop.db-8.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.021973 swoop.db-8.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 16:49:35.000000 swoop.db-8.0.1/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-03 16:49:35.000000 swoop.db-8.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-03 16:49:35.000000 swoop.db-8.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-03 16:49:35.000000 swoop.db-8.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-03 16:49:35.000000 swoop.db-8.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 16:49:58.025973 swoop.db-8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-08-03 16:49:35.000000 swoop.db-8.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 16:49:35.000000 swoop.db-8.0.1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.021973 swoop.db-8.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3558 2023-08-03 16:49:35.000000 swoop.db-8.0.1/bin/db-initialization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-08-03 16:49:35.000000 swoop.db-8.0.1/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-03 16:49:35.000000 swoop.db-8.0.1/bin/run-migration-job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-03 16:49:35.000000 swoop.db-8.0.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 16:49:35.000000 swoop.db-8.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 16:49:35.000000 swoop.db-8.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:49:58.025973 swoop.db-8.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.013973 swoop.db-8.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.013973 swoop.db-8.0.1/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/migrations/00008_new_base.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-08-03 16:49:35.000000 swoop.db-8.0.1/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.021973 swoop.db-8.0.1/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 16:49:57.000000 swoop.db-8.0.1/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-03 16:49:58.000000 swoop.db-8.0.1/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:49:57.000000 swoop.db-8.0.1/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 16:49:57.000000 swoop.db-8.0.1/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-03 16:49:57.000000 swoop.db-8.0.1/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 16:49:57.000000 swoop.db-8.0.1/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.017973 swoop.db-8.0.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/tests/fixtures/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/fixtures/migrations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:49:58.025973 swoop.db-8.0.1/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/pgtap/test_uuid_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-03 16:49:35.000000 swoop.db-8.0.1/tests/test_migrations.py
```

### Comparing `swoop.db-8.0.0/.env` & `swoop.db-8.0.1/.env`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.github/workflows/publish-image.yml` & `swoop.db-8.0.1/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.github/workflows/python-publish.yml` & `swoop.db-8.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.github/workflows/python-test.yml` & `swoop.db-8.0.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.github/workflows/snyk-scan.yml` & `swoop.db-8.0.1/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.gitignore` & `swoop.db-8.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.pre-commit-config.yaml` & `swoop.db-8.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/.snyk` & `swoop.db-8.0.1/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/CHANGELOG.md` & `swoop.db-8.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/CONTRIBUTING.md` & `swoop.db-8.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/Dockerfile` & `swoop.db-8.0.1/Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 
 # copy the python venv into this output image and add it's bin to the path
 COPY --from=APP /opt/swoop/db/swoop-db-venv /opt/swoop/db/swoop-db-venv
 ENV PATH=/opt/swoop/db/swoop-db-venv/bin:$PATH
 
 RUN mkdir -p /opt/swoop/db/scripts
 COPY bin/db-initialization.py /opt/swoop/db/scripts/db-initialization.py
+COPY bin/run-migration-job.py /opt/swoop/db/scripts/run-migration-job.py
 ENV PATH=/opt/swoop/db/scripts:$PATH
```

### Comparing `swoop.db-8.0.0/LICENSE` & `swoop.db-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/PKG-INFO` & `swoop.db-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 8.0.0
+Version: 8.0.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-8.0.0/README.md` & `swoop.db-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/RELEASE.md` & `swoop.db-8.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/bin/db-initialization.py` & `swoop.db-8.0.1/bin/db-initialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,28 @@
     - PGDATABASE: name of the database to be created
     - API_ROLE_USER and API_ROLE_PASS:
           swoop-api role username and password
     - CABOOSE_ROLE_USER and CABOOSE_ROLE_PASS:
           swoop-caboose role username and password
     - CONDUCTOR_ROLE_USER and CONDUCTOR_ROLE_PASS:
           swoop-conductor role username and password
-    - MIGRATION_ROLE_USER and MIGRATION_ROLE_PASS:
-          username and password for migration role
+    - OWNER_ROLE_USER and OWNER_ROLE_PASS:
+          username and password for owner role
     - Any additional libpq-supported connection parameters
           (https://www.postgresql.org/docs/current/libpq-envars.html)
 """
 import asyncio
 import os
 import sys
 
 import asyncpg
 from buildpg import V, render
 
 from swoop.db import SwoopDB
 
-OWNER_ROLE_NAME = "swoop"
-OWNER_ROLE = "OWNER_ROLE"
 APPLICATION_ROLES: list[str] = [
     "API_ROLE",
     "CABOOSE_ROLE",
     "CONDUCTOR_ROLE",
 ]
```

### Comparing `swoop.db-8.0.0/docker-compose.yml` & `swoop.db-8.0.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/pyproject.toml` & `swoop.db-8.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/src/swoop/db/cli.py` & `swoop.db-8.0.1/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/src/swoop/db/fixtures/base_01.sql` & `swoop.db-8.0.1/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/src/swoop/db/migrations/00008_new_base.up.sql` & `swoop.db-8.0.1/src/swoop/db/migrations/00008_new_base.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/src/swoop/db/schema.sql` & `swoop.db-8.0.1/src/swoop/db/schema.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-8.0.1/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 8.0.0
+Version: 8.0.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-8.0.0/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-8.0.1/src/swoop.db.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 requirements.txt
 .github/workflows/publish-image.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 .github/workflows/snyk-scan.yml
 bin/db-initialization.py
 bin/get-max-migration-version.py
+bin/run-migration-job.py
 src/swoop.db.egg-info/PKG-INFO
 src/swoop.db.egg-info/SOURCES.txt
 src/swoop.db.egg-info/dependency_links.txt
 src/swoop.db.egg-info/entry_points.txt
 src/swoop.db.egg-info/requires.txt
 src/swoop.db.egg-info/top_level.txt
 src/swoop/db/__init__.py
```

### Comparing `swoop.db-8.0.0/tests/conftest.py` & `swoop.db-8.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/fixtures/migrations/README.md` & `swoop.db-8.0.1/tests/fixtures/migrations/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/pgtap/test_action.sql` & `swoop.db-8.0.1/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/pgtap/test_find_cached_action_for_payload.sql` & `swoop.db-8.0.1/tests/pgtap/test_find_cached_action_for_payload.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/pgtap/test_limit-locking.sql` & `swoop.db-8.0.1/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/pgtap/test_uuid_v7.sql` & `swoop.db-8.0.1/tests/pgtap/test_uuid_v7.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/test_database.py` & `swoop.db-8.0.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `swoop.db-8.0.0/tests/test_migrations.py` & `swoop.db-8.0.1/tests/test_migrations.py`

 * *Files identical despite different names*

