# Comparing `tmp/lamindb_setup-0.49.2.tar.gz` & `tmp/lamindb_setup-0.49.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.49.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.49.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.49.2.tar` & `lamindb_setup-0.49.3.tar`

### file list

```diff
@@ -1,76 +1,105 @@
--rw-r--r--   0        0        0     4107 2023-07-26 11:10:58.438067 lamindb_setup-0.49.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-07-26 11:10:58.438169 lamindb_setup-0.49.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-07-26 11:10:58.438248 lamindb_setup-0.49.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-07-26 11:10:58.438319 lamindb_setup-0.49.2/.gitignore
--rw-r--r--   0        0        0      100 2023-07-26 11:10:58.438385 lamindb_setup-0.49.2/.gitmodules
--rw-r--r--   0        0        0     1798 2023-07-26 11:10:58.438458 lamindb_setup-0.49.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-07-26 11:10:58.438557 lamindb_setup-0.49.2/LICENSE
--rw-r--r--   0        0        0      318 2023-07-26 11:10:58.438617 lamindb_setup-0.49.2/README.md
--rw-r--r--   0        0        0    58824 2023-07-31 15:00:32.632568 lamindb_setup-0.49.2/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-07-26 11:10:58.439028 lamindb_setup-0.49.2/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-26 11:10:58.439089 lamindb_setup-0.49.2/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-26 11:10:58.439190 lamindb_setup-0.49.2/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-07-26 11:10:58.439259 lamindb_setup-0.49.2/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6645 2023-07-26 11:10:58.439322 lamindb_setup-0.49.2/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7739 2023-07-26 11:10:58.439470 lamindb_setup-0.49.2/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4349 2023-07-26 11:10:58.439547 lamindb_setup-0.49.2/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-07-26 11:10:58.439625 lamindb_setup-0.49.2/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-26 11:10:58.439683 lamindb_setup-0.49.2/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-07-26 11:10:58.439738 lamindb_setup-0.49.2/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-07-26 11:10:58.439790 lamindb_setup-0.49.2/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-07-26 11:10:58.439846 lamindb_setup-0.49.2/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-07-26 11:10:58.439902 lamindb_setup-0.49.2/docs/index.md
--rw-r--r--   0        0        0       61 2023-07-26 11:10:58.439954 lamindb_setup-0.49.2/docs/reference.md
--rw-r--r--   0        0        0      365 2023-07-26 11:10:58.440014 lamindb_setup-0.49.2/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-07-26 11:10:58.440073 lamindb_setup-0.49.2/lamin-project.yaml
--rw-r--r--   0        0        0     2758 2023-07-31 15:00:41.484606 lamindb_setup-0.49.2/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5704 2023-07-31 14:59:30.046977 lamindb_setup-0.49.2/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2073 2023-07-26 11:10:58.440346 lamindb_setup-0.49.2/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      825 2023-07-26 11:10:58.440404 lamindb_setup-0.49.2/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-07-26 11:10:58.440476 lamindb_setup-0.49.2/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-07-26 11:10:58.440534 lamindb_setup-0.49.2/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-07-26 11:10:58.440590 lamindb_setup-0.49.2/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7485 2023-07-26 11:10:58.440688 lamindb_setup-0.49.2/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6602 2023-07-26 11:10:58.440806 lamindb_setup-0.49.2/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1413 2023-07-26 11:10:58.440875 lamindb_setup-0.49.2/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-26 11:10:58.440935 lamindb_setup-0.49.2/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-07-26 11:10:58.440993 lamindb_setup-0.49.2/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-07-26 11:10:58.441057 lamindb_setup-0.49.2/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-07-26 11:10:58.441126 lamindb_setup-0.49.2/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-07-26 11:10:58.441187 lamindb_setup-0.49.2/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-07-26 11:10:58.441247 lamindb_setup-0.49.2/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-07-26 11:10:58.441305 lamindb_setup-0.49.2/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-07-26 11:10:58.441378 lamindb_setup-0.49.2/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-26 11:10:58.441434 lamindb_setup-0.49.2/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-07-26 11:10:58.441522 lamindb_setup-0.49.2/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5999 2023-07-26 11:10:58.441598 lamindb_setup-0.49.2/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-07-26 11:10:58.441661 lamindb_setup-0.49.2/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10929 2023-07-26 11:10:58.441746 lamindb_setup-0.49.2/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-07-26 11:10:58.441805 lamindb_setup-0.49.2/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3652 2023-07-26 11:10:58.441873 lamindb_setup-0.49.2/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0    11225 2023-07-31 14:59:30.047346 lamindb_setup-0.49.2/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     4686 2023-07-26 11:10:58.442040 lamindb_setup-0.49.2/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4854 2023-07-26 11:10:58.442124 lamindb_setup-0.49.2/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9341 2023-07-26 11:10:58.442210 lamindb_setup-0.49.2/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-07-26 11:10:58.442270 lamindb_setup-0.49.2/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-07-26 11:10:58.442329 lamindb_setup-0.49.2/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-07-26 11:10:58.442386 lamindb_setup-0.49.2/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-07-26 11:10:58.442440 lamindb_setup-0.49.2/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-07-26 11:10:58.442505 lamindb_setup-0.49.2/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-07-26 11:10:58.442574 lamindb_setup-0.49.2/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4603 2023-07-31 14:59:30.047620 lamindb_setup-0.49.2/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2734 2023-07-31 14:59:30.047891 lamindb_setup-0.49.2/lamindb_setup/dev/upath.py
-drwxr-xr-x   0        0        0        0 2023-07-26 11:10:58.442738 lamindb_setup-0.49.2/lnschema-core/
--rw-r--r--   0        0        0     2055 2023-07-26 11:10:58.442824 lamindb_setup-0.49.2/noxfile.py
--rw-r--r--   0        0        0     1101 2023-07-26 11:10:58.442894 lamindb_setup-0.49.2/pyproject.toml
--rw-r--r--   0        0        0     2481 2023-07-26 11:10:58.443017 lamindb_setup-0.49.2/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-07-26 11:10:58.443073 lamindb_setup-0.49.2/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-07-26 11:10:58.443127 lamindb_setup-0.49.2/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-07-26 11:10:58.443186 lamindb_setup-0.49.2/tests/test_bionty.py
--rw-r--r--   0        0        0     4049 2023-07-26 11:10:58.443250 lamindb_setup-0.49.2/tests/test_init_instance.py
--rw-r--r--   0        0        0     2207 2023-07-26 11:10:58.443308 lamindb_setup-0.49.2/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-07-26 11:10:58.443366 lamindb_setup-0.49.2/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-26 11:10:58.443428 lamindb_setup-0.49.2/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-07-26 11:10:58.443485 lamindb_setup-0.49.2/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-07-26 11:10:58.443538 lamindb_setup-0.49.2/tests/test_signup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.49.2/PKG-INFO
+-rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.3/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.3/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.3/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.3/README.md
+-rw-r--r--   0        0        0    59336 2023-08-03 12:06:57.634491 lamindb_setup-0.49.3/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.3/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.3/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.3/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.3/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.3/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.3/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.3/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.3/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.3/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.3/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.3/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.3/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.3/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.3/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.49.3/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.3/lamin-project.yaml
+-rw-r--r--   0        0        0     2758 2023-08-03 16:00:08.225891 lamindb_setup-0.49.3/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5704 2023-07-31 17:31:23.899228 lamindb_setup-0.49.3/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.49.3/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.49.3/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.49.3/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.3/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.3/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.49.3/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6602 2023-07-25 01:43:24.440143 lamindb_setup-0.49.3/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1413 2023-07-24 10:02:47.316262 lamindb_setup-0.49.3/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.49.3/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.49.3/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.3/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.49.3/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.3/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.3/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.3/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.49.3/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.3/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.3/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.49.3/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.3/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.49.3/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.3/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.3/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0    11249 2023-08-02 03:33:18.382713 lamindb_setup-0.49.3/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.3/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.3/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.49.3/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.3/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.3/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-07-18 04:17:11.571437 lamindb_setup-0.49.3/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.3/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.3/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.49.3/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4862 2023-08-03 12:06:57.634858 lamindb_setup-0.49.3/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2734 2023-07-31 17:31:23.900624 lamindb_setup-0.49.3/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.3/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.3/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.3/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.3/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.3/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    33450 2023-07-25 01:43:38.325656 lamindb_setup-0.49.3/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.3/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.3/lnschema-core/README.md
+-rw-r--r--   0        0        0      447 2023-07-25 01:43:38.325792 lamindb_setup-0.49.3/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.3/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
+-rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
+-rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
+-rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
+-rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
+-rw-r--r--   0        0        0     3585 2023-07-25 01:43:38.326104 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.3/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.3/lnschema-core/lnschema_core/mocks.py
+-rw-r--r--   0        0        0    64949 2023-07-31 11:23:10.578935 lamindb_setup-0.49.3/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.3/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.3/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.3/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.3/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.3/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.3/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.49.3/pyproject.toml
+-rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.3/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.3/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.3/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.3/tests/test_bionty.py
+-rw-r--r--   0        0        0     4936 2023-08-03 09:23:05.337238 lamindb_setup-0.49.3/tests/test_init_instance.py
+-rw-r--r--   0        0        0     2207 2023-07-25 01:43:24.442039 lamindb_setup-0.49.3/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.3/tests/test_login.py
+-rw-r--r--   0        0        0      457 2023-07-24 10:02:47.316450 lamindb_setup-0.49.3/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.3/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.3/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.49.3/PKG-INFO
```

### Comparing `lamindb_setup-0.49.2/.github/workflows/build.yml` & `lamindb_setup-0.49.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/.gitignore` & `lamindb_setup-0.49.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/.pre-commit-config.yaml` & `lamindb_setup-0.49.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/LICENSE` & `lamindb_setup-0.49.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/changelog.md` & `lamindb_setup-0.49.3/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Add `.record` property to `StorageSettings` | [451](https://github.com/laminlabs/lamindb-setup/pull/451) | [falexwolf](https://github.com/falexwolf) | 2023-08-03 |
+✅ Fix init-instance test for sqlite instance | [450](https://github.com/laminlabs/lamindb-setup/pull/450) | [bpenteado](https://github.com/bpenteado) | 2023-08-02 |
+🎨 Fix `init-instance` anti-patterns and expand tests | [449](https://github.com/laminlabs/lamindb-setup/pull/449) | [bpenteado](https://github.com/bpenteado) | 2023-08-01 |
 ✨ Propagate kwargs through synchronization functions | [448](https://github.com/laminlabs/lamindb-setup/pull/448) | [Koncopd](https://github.com/Koncopd) | 2023-07-31 | 0.49.2
 🐛 Fix local variable 'db_dsn' referenced before assignment | [447](https://github.com/laminlabs/lamindb-setup/pull/447) | [fredericenard](https://github.com/fredericenard) | 2023-07-30 |
 🚸 Show help by default and add --version | [446](https://github.com/laminlabs/lamindb-setup/pull/446) | [Zethson](https://github.com/Zethson) | 2023-07-30 |
 🐛 Fix flawed DBUser logic in `init_instance` | [442](https://github.com/laminlabs/lamindb-setup/pull/442) | [bpenteado](https://github.com/bpenteado) | 2023-07-24 | 0.49.1
 🗃️ Enable multiple DB access roles in instances (decompose connection string) | [431](https://github.com/laminlabs/lamindb-setup/pull/431) | [bpenteado](https://github.com/bpenteado) | 2023-07-19 | 0.49.0
 💚 Fix instability | [441](https://github.com/laminlabs/lamindb-setup/pull/441) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
 👷 Run CI against the staging environment | [440](https://github.com/laminlabs/lamindb-setup/pull/440) | [bpenteado](https://github.com/bpenteado) | 2023-07-18 |
```

### Comparing `lamindb_setup-0.49.2/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.49.3/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/faq/multi-session.ipynb` & `lamindb_setup-0.49.3/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.49.3/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.49.3/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.49.3/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.49.3/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.49.3/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.49.3/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/docs/guide/setup-user.md` & `lamindb_setup-0.49.3/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/__init__.py` & `lamindb_setup-0.49.3/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.49.2"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.49.3"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.49.2/lamindb_setup/__main__.py` & `lamindb_setup-0.49.3/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.49.3/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_close.py` & `lamindb_setup-0.49.3/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_delete.py` & `lamindb_setup-0.49.3/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_docstrings.py` & `lamindb_setup-0.49.3/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_init_instance.py` & `lamindb_setup-0.49.3/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_load_instance.py` & `lamindb_setup-0.49.3/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_migrate.py` & `lamindb_setup-0.49.3/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_notebook.py` & `lamindb_setup-0.49.3/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_register_instance.py` & `lamindb_setup-0.49.3/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_schema.py` & `lamindb_setup-0.49.3/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_set.py` & `lamindb_setup-0.49.3/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_settings.py` & `lamindb_setup-0.49.3/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_setup_user.py` & `lamindb_setup-0.49.3/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.49.3/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_django.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_hub_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     )
     try:
         # validate input arguments
         schema_str = validate_schema_arg(schema)
         # storage is validated in add_storage
         validate_db_arg(db)
 
-        if db:
+        if db is not None:
             db_dsn = LaminDsnModel(db=db)
         else:
             db_dsn = None
 
         # get account
         account = sb_select_account_by_handle(owner, hub)
         if account is None:
@@ -129,15 +129,15 @@
         validate_unique_sqlite(
             hub=hub, db=db, storage_id=storage_id, name=name, account=account
         )
 
         instance_id = uuid4().hex
         db_user_id = None
 
-        if db_dsn:
+        if db_dsn is not None:
             db_user_id = uuid4().hex
             instance = sb_insert_instance(  # noqa
                 {
                     "id": instance_id,
                     "account_id": account["id"],
                     "name": name,
                     "storage_id": storage_id,
```

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import Literal, Optional, Union
+from typing import Any, Literal, Optional, Union
 
 from appdirs import AppDirs
 
 from .upath import UPath
 
 DIRS = AppDirs("lamindb", "laminlabs")
 
@@ -24,15 +24,16 @@
             root_path = root.resolve()
         elif isinstance(root, str):
             root_path = Storage._str_to_path(root)
         else:
             raise ValueError("root should be of type Union[str, Path, UPath].")
         self._root = root_path
         self._region = region
-        self._id: Optional[str] = None
+        # would prefer to type below as ORM, but need to think through import order
+        self._record: Optional[Any] = None
 
     @staticmethod
     def _str_to_path(storage: str) -> Union[Path, UPath]:
         if storage.startswith("s3://"):
             # for new buckets there could be problems if the region is not specified
             storage_root = UPath(storage, cache_regions=True)
         elif storage.startswith("gs://"):
@@ -41,19 +42,25 @@
             os.makedirs(storage, exist_ok=True)  # resolve fails for nonexisting dir
             storage_root = Path(storage).resolve()
         return storage_root
 
     @property
     def id(self) -> str:
         """Storage id."""
-        if self._id is None:
+        return self.record.id
+
+    @property
+    def record(self) -> Any:
+        """Storage record."""
+        if self._record is None:
+            # dynamic import because of import order
             from lnschema_core.models import Storage
 
-            self._id = Storage.objects.get(root=self.root_as_str).id
-        return self._id
+            self._record = Storage.objects.get(root=self.root_as_str)
+        return self._record
 
     @property
     def root(self) -> Union[Path, UPath]:
         """Root storage location."""
         return self._root
 
     def _set_fs_kwargs(self, **kwargs):
```

### Comparing `lamindb_setup-0.49.2/lamindb_setup/dev/upath.py` & `lamindb_setup-0.49.3/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/noxfile.py` & `lamindb_setup-0.49.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/pyproject.toml` & `lamindb_setup-0.49.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/tests/hub/test_instance.py` & `lamindb_setup-0.49.3/tests/hub/test_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/tests/hub/test_storage.py` & `lamindb_setup-0.49.3/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/tests/test_init_instance.py` & `lamindb_setup-0.49.3/tests/test_init_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,38 @@
     assert ln_setup.settings.instance.name == "lndb-setup-ci-europe"
     assert (
         str(ln_setup.settings.instance._sqlite_file)
         == "s3://lndb-setup-ci-eu-central-1/lndb-setup-ci-europe.lndb"
     )
 
 
+def test_init_instance_sqlite():
+    ln_setup.init(
+        storage="./mydatasqlite",
+        name="local-sqlite-instance",
+        _test=True,
+    )
+    ln_setup.register()
+    hub = connect_hub_with_auth(access_token=ln_setup.settings.user.access_token)
+    account = sb_select_account_by_handle(
+        handle=ln_setup.settings.instance.owner, supabase_client=hub
+    )
+    instance = sb_select_instance_by_name(
+        account_id=account["id"],
+        name=ln_setup.settings.instance.name,
+        supabase_client=hub,
+    )
+    assert ln_setup.settings.instance.name == "local-sqlite-instance"
+    assert not ln_setup.settings.instance.storage.is_cloud
+    assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
+    assert ln_setup.settings.instance.dialect == "sqlite"
+    ln_setup.delete("local-sqlite-instance")
+    sb_delete_instance(instance["id"], hub)
+
+
 # def test_db_unique_error():
 #     ln_setup.login("testuser2")
 
 #     # postgres
 
 
 # #     with pytest.raises(RuntimeError):
```

### Comparing `lamindb_setup-0.49.2/tests/test_load_instance.py` & `lamindb_setup-0.49.3/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.2/PKG-INFO` & `lamindb_setup-0.49.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.49.2
+Version: 0.49.3
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
```

