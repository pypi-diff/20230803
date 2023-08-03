# Comparing `tmp/deker-local-adapters-1.0.0.tar.gz` & `tmp/deker-local-adapters-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker-local-adapters-1.0.0.tar", last modified: Tue Aug  1 18:34:19 2023, max compression
+gzip compressed data, was "deker-local-adapters-1.0.1b0.tar", last modified: Thu Aug  3 16:19:26 2023, max compression
```

## Comparing `deker-local-adapters-1.0.0.tar` & `deker-local-adapters-1.0.1b0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.205078 deker-local-adapters-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/deker_local_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/array_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/collection_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/deker_local_adapters/varray_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-01 18:34:19.000000 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 18:34:19.000000 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:34:19.000000 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 18:34:19.000000 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 18:34:19.000000 deker-local-adapters-1.0.0/deker_local_adapters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.205078 deker-local-adapters-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/array_adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/collection_adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/hdf5_options.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/hdf5_storage_adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/docs/source/api/varray_adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.209078 deker-local-adapters-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/tests/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/array_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/collection_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/index_exp_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/schemas_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/parameters/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/plugins/subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:19.213078 deker-local-adapters-1.0.0/tests/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/test_array_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/test_collection_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/test_collection_options_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-08-01 18:34:11.000000 deker-local-adapters-1.0.0/tests/test_cases/test_varray_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.988825 deker-local-adapters-1.0.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.976824 deker-local-adapters-1.0.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.980825 deker-local-adapters-1.0.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 16:19:26.988825 deker-local-adapters-1.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.980825 deker-local-adapters-1.0.1b0/deker_local_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/array_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/collection_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.980825 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/deker_local_adapters/varray_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.980825 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 16:19:26.000000 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-03 16:19:26.000000 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:19:26.000000 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 16:19:26.000000 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 16:19:26.000000 deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.976824 deker-local-adapters-1.0.1b0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/array_adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/collection_adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/hdf5_options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/hdf5_storage_adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/docs/source/api/varray_adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 16:19:26.988825 deker-local-adapters-1.0.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/tests/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/array_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/collection_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/index_exp_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/schemas_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/parameters/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.984825 deker-local-adapters-1.0.1b0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/plugins/subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:26.988825 deker-local-adapters-1.0.1b0/tests/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/test_array_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/test_collection_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/test_collection_options_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-08-03 16:19:17.000000 deker-local-adapters-1.0.1b0/tests/test_cases/test_varray_adapter.py
```

### Comparing `deker-local-adapters-1.0.0/.dockerignore` & `deker-local-adapters-1.0.1b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/.gitignore` & `deker-local-adapters-1.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/.gitlab-ci.yml` & `deker-local-adapters-1.0.1b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/.pre-commit-config.yaml` & `deker-local-adapters-1.0.1b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/LICENSE` & `deker-local-adapters-1.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/PKG-INFO` & `deker-local-adapters-1.0.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deker-local-adapters
-Version: 1.0.0
-Summary: Interactive shell for Deker
+Version: 1.0.1b0
+Summary: Plugin with local adapters for deker
 Author-email: OpenWeather <info@openweathermap.org>
 Maintainer-email: OpenWeather <info@openweathermap.org>
 License: GPL-3.0-only
 Project-URL: Homepage, https://deker.io/
 Project-URL: Documentation, https://docs.deker.io/
 Project-URL: Repository, https://github.com/openweathermap/deker-local-adapters
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/__init__.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # nopycln: file
 from .array_adapter import LocalArrayAdapter
 from .collection_adapter import LocalCollectionAdapter
 from .factory import AdaptersFactory, storage_adapter_factory
 from .storage_adapters import (
+    HDF5BuiltinCompressionStringOptions,
+    HDF5ChunksOptions,
     HDF5CompressionOpts,
     HDF5Options,
     HDF5StorageAdapter,
-    HDF5BuiltinCompressionStringOptions,
-    HDF5ChunksOptions
 )
 from .varray_adapter import LocalVArrayAdapter
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/array_adapter.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/array_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,34 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 import os
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Generator, Optional, Tuple, Union, Type
+from typing import TYPE_CHECKING, Any, Generator, Optional, Tuple, Type, Union
 
 from deker.ABC.base_adapters import BaseArrayAdapter
 from deker.arrays import Array
 from deker.ctx import CTX
 from deker.errors import DekerArrayError
 from deker.locks import CreateArrayLock, ReadArrayLock, WriteArrayLock
 from deker.log import SelfLoggerMixin
 from deker.schemas import AttributeSchema
-from deker.tools import create_array_from_meta, get_main_path, get_symlink_path
+from deker.tools import get_main_path, get_symlink_path
 from deker.tools.decorators import check_ctx_state
 from deker.types import ArrayMeta, Numeric, Slice
 from numpy import ndarray
 
 from deker_local_adapters.mixin import LocalAdapterMixin
 
 
 if TYPE_CHECKING:
     from concurrent.futures import ThreadPoolExecutor
+
     from deker.ABC import BaseStorageAdapter
     from deker.ABC.base_collection import BaseCollectionOptions
     from deker.collection import Collection
 
 
 class LocalArrayAdapter(SelfLoggerMixin, LocalAdapterMixin, BaseArrayAdapter):
     """Default adapter for managing Array instances."""
@@ -69,19 +70,15 @@
     ) -> Optional[Path]:
         sympath_to_dir = get_symlink_path(
             self.collection_path / self.symlinks_dir,
             array_primary_attributes_schema,
             {"vid": vid, "v_position": vpos},
         )
         try:
-            files = [
-                file
-                for file in sympath_to_dir.iterdir()
-                if file.is_file() and file.name.endswith(self.file_ext)
-            ]
+            files = [file for file in sympath_to_dir.iterdir() if file.is_file() and file.name.endswith(self.file_ext)]
             if files:
                 # just one file is expected inside the list
                 return files[0]
         except FileNotFoundError:
             return None
 
     @check_ctx_state
@@ -122,17 +119,15 @@
         """Read data from the existing array.
 
         :param array: Array instance
         :param bounds: array bounds to read
         """
         filename = self._get_main_path_to_file(array)
 
-        return self.storage_adapter.read_data(
-            filename, array.shape, bounds, array.fill_value, array.dtype
-        )
+        return self.storage_adapter.read_data(filename, array.shape, bounds, array.fill_value, array.dtype)
 
     @check_ctx_state
     @ReadArrayLock()
     def read_meta(self, array: Union[Array, Path]) -> ArrayMeta:
         """Read array metadata.
 
         :param array: Array instance
@@ -227,12 +222,12 @@
 
         def _delete(array: Array) -> None:
             array.delete()
 
         try:
             metas = self.executor.map(self.read_meta, self._adapter_iter(vid))
             if metas:
-                arrays = [create_array_from_meta(collection, meta, self) for meta in metas]
+                arrays = [Array._create_from_meta(collection, meta, self) for meta in metas]
                 list(self.executor.map(_delete, arrays))
         except Exception as e:
             self.logger.exception(e)
             raise e
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/collection_adapter.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/collection_adapter.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/errors.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/errors.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/factory.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Type
 
 from deker.ABC import BaseCollectionAdapter
 from deker.ABC.base_factory import BaseAdaptersFactory
 from deker.tools.decorators import check_ctx_state
 
-from deker_local_adapters.errors import DekerStorageError
 from deker_local_adapters.array_adapter import LocalArrayAdapter
 from deker_local_adapters.collection_adapter import LocalCollectionAdapter
+from deker_local_adapters.errors import DekerStorageError
 from deker_local_adapters.storage_adapters import HDF5StorageAdapter
-from deker_local_adapters.varray_adapter import LocalVArrayAdapter
 from deker_local_adapters.storage_adapters.enums import StorageAdapterTypes
+from deker_local_adapters.varray_adapter import LocalVArrayAdapter
+
 
 if TYPE_CHECKING:
-    from deker.ABC.base_adapters import BaseArrayAdapter, BaseVArrayAdapter, BaseStorageAdapter
+    from deker.ABC.base_adapters import BaseArrayAdapter, BaseStorageAdapter, BaseVArrayAdapter
     from deker.ABC.base_collection import BaseCollectionOptions
 
 
 class AdaptersFactory(BaseAdaptersFactory):
     """Adapters factory for Collections, Arrays and VArrays."""
 
     uri_schemes = ("file",)
@@ -51,17 +52,15 @@
     ) -> "BaseArrayAdapter":
         """Create ArrayAdapter instance.
 
         :param collection_path: path to collection
         :param storage_adapter: storage adapter implementation
         :param collection_options: chunking and compression options
         """
-        return LocalArrayAdapter(
-            collection_path, self.ctx, storage_adapter, self.executor, collection_options
-        )
+        return LocalArrayAdapter(collection_path, self.ctx, storage_adapter, self.executor, collection_options)
 
     @check_ctx_state
     def get_varray_adapter(
         self, collection_path: Path, storage_adapter: Type["BaseStorageAdapter"]
     ) -> "BaseVArrayAdapter":
         """Create VArrayAdapter instance.
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/mixin.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 
 from concurrent.futures import ThreadPoolExecutor
 from logging import Logger
 from pathlib import Path
-from typing import TYPE_CHECKING, Generator, Optional, Tuple
+from typing import TYPE_CHECKING, Generator, Optional, Tuple, Union
 
+from deker.arrays import Array, VArray
 from deker.errors import DekerArrayError, DekerValidationError
-from deker.tools import create_array_from_meta, get_main_path, get_paths, get_symlink_path
+from deker.tools import get_main_path, get_paths, get_symlink_path
 from deker.tools.decorators import check_ctx_state
 from deker.types import ArrayMeta
 from deker_tools.path import is_empty
 
 
 if TYPE_CHECKING:
     from deker.ABC import BaseArray, BaseArraysSchema
@@ -134,25 +135,28 @@
 
     def _init_array(
         self,
         path: Path,
         collection: "Collection",
         array_adapter: "BaseArrayAdapter",
         varray_adapter: "BaseVArrayAdapter",
-    ) -> "BaseArray":
+    ) -> Union[Array, VArray]:
         """Read meta and make an array/varray object from it.
 
         :param path: Path to meta
         :param collection: Collection instance
         :param array_adapter: Arrays' adapter
         :param varray_adapter: VArrays' adapter
         """
         meta = self.read_meta(path)  # type: ignore[attr-defined]
 
-        array = create_array_from_meta(collection, meta, array_adapter, varray_adapter)
+        if varray_adapter:
+            array = VArray._create_from_meta(collection, meta, array_adapter, varray_adapter)
+        else:
+            array = Array._create_from_meta(collection, meta, array_adapter, varray_adapter)
         return array
 
     def get_by_primary_attributes(
         self,
         primary_attributes: dict,
         schema: "BaseArraysSchema",
         collection: "Collection",
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/__init__.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .hdf5 import (
-    HDF5StorageAdapter,
-    HDF5Options,
-    HDF5CompressionOpts,
+    HDF5BuiltinCompressionStringOptions,
     HDF5ChunksOptions,
-    HDF5BuiltinCompressionStringOptions
+    HDF5CompressionOpts,
+    HDF5Options,
+    HDF5StorageAdapter,
 )
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/enums.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/enums.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/__init__.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,9 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # nopycln: file
-from .hdf5_options import (
-    HDF5CompressionOpts,
-    HDF5Options,
-    HDF5ChunksOptions,
-    HDF5BuiltinCompressionStringOptions
-)
+from .hdf5_options import HDF5BuiltinCompressionStringOptions, HDF5ChunksOptions, HDF5CompressionOpts, HDF5Options
 from .hdf5_storage_adapter import HDF5StorageAdapter
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dataclasses import asdict, dataclass
 from typing import List, Optional, Tuple, Union
 
 from deker.ABC.base_collection import BaseCollectionOptions
 from deker.errors import DekerValidationError
 from deker.types import Serializer
+
 from deker_local_adapters.storage_adapters.enums import HDF5BuiltinCompressionStringOptions, HDF5ChunksOptions
 
 
 @dataclass()
 class HDF5CompressionOpts(Serializer):
     """HDF5 compression options.
 
@@ -48,46 +49,40 @@
         """Convert compression options to tuple."""
         if self.compression is not None:
             if not isinstance(self.compression, (str, int)) or isinstance(self.compression, bool):
                 raise DekerValidationError(
                     f"Invalid compression type: {type(self.compression)}; str, int or None expected"
                 )
 
-            if isinstance(self.compression, str) and (
-                self.compression.isspace() or not self.compression
-            ):
+            if isinstance(self.compression, str) and (self.compression.isspace() or not self.compression):
                 raise DekerValidationError(f"Invalid compression value: {self.compression}")
 
             if isinstance(self.compression, int) and self.compression < 0:
                 raise DekerValidationError(f"Invalid compression value: {self.compression}")
 
         if self.compression_opts is not None:
             if self.compression is None:
                 raise DekerValidationError(
                     "HDF5CompressionOpts `compression_opts` is not None and `compression` is None. "
                     "Perhaps you forgot to indicate filter name?"
                 )
 
-            if not isinstance(self.compression_opts, (list, tuple, int)) or isinstance(
-                self.compression_opts, bool
-            ):
+            if not isinstance(self.compression_opts, (list, tuple, int)) or isinstance(self.compression_opts, bool):
                 raise DekerValidationError(
                     f"Invalid compression_opts type: {type(self.compression)}; list, tuple, int or None expected"
                 )
 
             if isinstance(self.compression_opts, list):
                 self.compression_opts = tuple(self.compression_opts)
 
             if not self.compression_opts:
                 self.compression_opts = None
 
             if isinstance(self.compression_opts, int) and self.compression_opts < 0:
-                raise DekerValidationError(
-                    f"Invalid compression level value: {self.compression_opts}"
-                )
+                raise DekerValidationError(f"Invalid compression level value: {self.compression_opts}")
 
     @property
     def as_dict(self) -> dict:
         """Serialize self into a dictionary."""
         return {"compression": self.compression, "compression_opts": self.compression_opts}
 
     def __repr__(self) -> str:
@@ -191,18 +186,18 @@
                             compression_options = None
 
                         if compression_type == HDF5BuiltinCompressionStringOptions.none.value:
                             compression_type = None
                             compression_options = None
                         elif compression_type == HDF5BuiltinCompressionStringOptions.gzip.value:
                             if compression_options:
-                                compression_options = compression_options[0]
+                                compression_options = compression_options[0]  # type: ignore[assignment]
                         elif compression_type == HDF5BuiltinCompressionStringOptions.szip.value:
                             if compression_options:
-                                compression_options = tuple(compression_options)
+                                compression_options = tuple(compression_options)  # type: ignore[assignment]
                         elif compression_type == HDF5BuiltinCompressionStringOptions.lzf.value:
                             if compression_options:
                                 raise ValueError("LZF filter does not accept any options")
                         else:
                             compression_type = int(compression_type)
 
                     else:
@@ -219,47 +214,47 @@
                         chunks = "none"
                     else:
                         chunks = dic["chunks"]["mode"]
 
                     if chunks == HDF5ChunksOptions.manual.value:
                         chunks = dic["chunks"]["size"]
                     elif chunks == HDF5ChunksOptions.true.value:
-                        chunks = True
+                        chunks = True  # type: ignore[assignment]
                     else:
-                        chunks = None
+                        chunks = None  # type: ignore[assignment]
                     coll_params.update({"chunks": chunks})
         if compression:
             coll_params.update({"compression_opts": HDF5CompressionOpts(**compression)})  # type: ignore[dict-item]
 
         return coll_params
 
     @property
     def as_dict(self) -> dict:
         """Serialize object as dict."""
         compression_dict = asdict(self.compression_opts)  # type: ignore[arg-type]
         options: Optional[Tuple[Optional[str], ...]] = None
 
-        if self.compression_opts.compression is None:
+        if self.compression_opts.compression is None:  # type: ignore[union-attr]
             compression_dict["compression"] = "none"
             options = tuple()
         else:
             opts = compression_dict["compression_opts"]
             if opts is not None:
                 if not isinstance(opts, (list, tuple)):
                     opts = [opts]
                 options = tuple(str(opt) for opt in opts)
             compression_dict["compression"] = str(compression_dict["compression"])
 
         chunks = self.chunks
         if isinstance(self.chunks, (list, tuple)):
-            chunks = {"mode": "manual", "size": self.chunks}
+            chunks = {"mode": "manual", "size": self.chunks}  # type: ignore[assignment]
         elif chunks:
-            chunks = {"mode": "true"}
+            chunks = {"mode": "true"}  # type: ignore[assignment]
         else:
-            chunks = {"mode": "none"}
+            chunks = {"mode": "none"}  # type: ignore[assignment]
         return {
             "chunks": chunks,
             "compression": {"compression": compression_dict["compression"], "options": options},
         }
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(chunks={self.chunks}, compression_opts={self.compression_opts})"
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,31 +46,29 @@
 
     Wraps `h5py` files managing logic.
     """
 
     file_ext: str = ".hdf5"
     storage_options = HDF5Options
 
-    def create(
-        self, path: Path, array_shape: Tuple[int, ...], metadata: Union[str, bytes, dict]
-    ) -> None:
+    def create(self, path: Path, array_shape: Tuple[int, ...], metadata: Union[str, bytes, dict]) -> None:
         """Create new hdf5 file with metadata.
 
         :param path: path to hdf5 file
         :param array_shape: shape of the array
         :param metadata: array metadata
         """
         try:
             self.logger.debug(f"trying to create {path}")
             with h5py.File(path, "w", locking=False) as f:
                 self.logger.debug(f"{path} opened in 'w'-mode")
                 if not isinstance(metadata, (str, bytes)):
                     value = json.dumps(metadata, default=str)
                 else:
-                    value = metadata
+                    value = metadata  # type: ignore[assignment]
                 dtype = f"S{sys.getsizeof(value.encode('utf-8'))}"
                 shape = ()
                 meta_ds = f.create_dataset(
                     "meta",
                     data=value,
                     dtype=dtype,
                     shape=shape,
@@ -120,17 +118,15 @@
         :param path: path to hdf5 file
         """
         self.logger.debug(f"trying to read meta from {path}")
         with h5py.File(path, mode="r", locking=False) as f:
             self.logger.debug(f"{path} opened in 'r'-mode")
             ds: Dataset = f.get("meta")
             if not ds:
-                raise DekerArrayError(
-                    "No metadata in the array. Try to delete and recreate the array."
-                )
+                raise DekerArrayError("No metadata in the array. Try to delete and recreate the array.")
             data = ds[()]
         decoded = data.decode("utf-8")
         meta = json.loads(decoded)
         self.logger.debug(f"{path} meta read OK and closed")
         return meta
 
     def update_data(
@@ -192,16 +188,16 @@
                         to_storage: ndarray = ndarray(shape=shape, dtype=dtype)
                         to_storage.fill(fill_value)
                         to_storage[bounds] = data
 
                         ds_kwargs = {"data": to_storage, "dtype": dtype, "shape": shape}
 
                         if collection_options:
-                            compression = collection_options.compression_opts.compression
-                            options = collection_options.compression_opts.compression_opts
+                            compression = collection_options.compression_opts.compression  # type: ignore[union-attr]
+                            options = collection_options.compression_opts.compression_opts  # type: ignore[union-attr]
                             ds_kwargs.update(
                                 {
                                     "chunks": collection_options.chunks,  # type: ignore[dict-item]
                                     "compression": compression,  # type: ignore[dict-item]
                                     "compression_opts": options,  # type: ignore[dict-item]
                                 }
                             )
@@ -227,17 +223,15 @@
         """
         try:
             self.logger.debug(f"trying to update meta in {path}")
             with h5py.File(path, "r+", locking=False) as f:
                 self.logger.debug(f"{path} opened in 'r+'-mode")
                 ds = f.get("meta")
                 if not ds:
-                    raise DekerArrayError(
-                        "No metadata in the array. Try to delete and recreate the array."
-                    )
+                    raise DekerArrayError("No metadata in the array. Try to delete and recreate the array.")
                 meta = json.loads(ds[()])
                 del f["meta"]
                 f.flush()
 
                 meta["custom_attributes"] = attributes
                 json_meta = json.dumps(meta, default=str)
                 ds = f.create_dataset(
@@ -250,17 +244,15 @@
                 f.flush()
             self.logger.debug(f"{path} meta updated OK and closed")
             return attributes
         except Exception as e:
             self.logger.exception(e)
             raise e
 
-    def clear_data(
-        self, path: Path, array_shape: Tuple[int, ...], bounds: Slice, fill_value: Numeric
-    ) -> None:
+    def clear_data(self, path: Path, array_shape: Tuple[int, ...], bounds: Slice, fill_value: Numeric) -> None:
         """Clear array data in hdf5 file.
 
         :param path: path to hdf5 file
         :param array_shape: array shape
         :param bounds: array bounds to update
         :param fill_value: array fill_value
         """
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters/varray_adapter.py` & `deker-local-adapters-1.0.1b0/deker_local_adapters/varray_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,17 +100,15 @@
             filename = array
         try:
             with open(filename, encoding="utf-8") as f:
                 data = f.read()
                 meta = json.loads(data)
                 return meta
         except Exception:
-            raise DekerArrayError(
-                "No metadata in the varray. Try to delete and recreate the varray."
-            )
+            raise DekerArrayError("No metadata in the varray. Try to delete and recreate the varray.")
 
     @check_ctx_state
     @UpdateMetaAttributeLock()
     def update_meta_custom_attributes(self, array: VArray, attributes: dict) -> None:
         """Update meta data in VArray.
 
         :param array: VArray instance
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters.egg-info/PKG-INFO` & `deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deker-local-adapters
-Version: 1.0.0
-Summary: Interactive shell for Deker
+Version: 1.0.1b0
+Summary: Plugin with local adapters for deker
 Author-email: OpenWeather <info@openweathermap.org>
 Maintainer-email: OpenWeather <info@openweathermap.org>
 License: GPL-3.0-only
 Project-URL: Homepage, https://deker.io/
 Project-URL: Documentation, https://docs.deker.io/
 Project-URL: Repository, https://github.com/openweathermap/deker-local-adapters
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deker-local-adapters-1.0.0/deker_local_adapters.egg-info/SOURCES.txt` & `deker-local-adapters-1.0.1b0/deker_local_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/docs/Makefile` & `deker-local-adapters-1.0.1b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/docs/conf.py` & `deker-local-adapters-1.0.1b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/docs/index.rst` & `deker-local-adapters-1.0.1b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/docs/make.bat` & `deker-local-adapters-1.0.1b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/pyproject.toml` & `deker-local-adapters-1.0.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 dynamic = ["version", "readme", "dependencies"]
 authors = [
     {name = "OpenWeather", email = "info@openweathermap.org"},
 ]
 maintainers = [
         {name = "OpenWeather", email = "info@openweathermap.org"},
 ]
-description = "Interactive shell for Deker"
+description = "Plugin with local adapters for deker" 
 license = {text = "GPL-3.0-only"}
 
 classifiers = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
```

### Comparing `deker-local-adapters-1.0.0/setup.cfg` & `deker-local-adapters-1.0.1b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/tests/conftest.py` & `deker-local-adapters-1.0.1b0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,17 +91,15 @@
 @pytest.fixture()
 def ctx(uri: Uri, config, storage_adapter, workers) -> CTX:
     """Creates Client context."""
     return CTX(uri, config, storage_adapter, ThreadPoolExecutor(workers))
 
 
 @pytest.fixture()
-def client(
-    root_path: Path, storage_adapter: Type[BaseStorageAdapter], workers: int, executor
-) -> Client:
+def client(root_path: Path, storage_adapter: Type[BaseStorageAdapter], workers: int, executor) -> Client:
     """Creates Client object and init all connections.
 
     :param root_path: path to directory with collections fixture
     :param storage_adapter: BaseStorageAdapter fixture
     :param workers: Number of workers for pool
     """
     with Client(
```

### Comparing `deker-local-adapters-1.0.0/tests/parameters/array_params.py` & `deker-local-adapters-1.0.1b0/tests/parameters/array_params.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/tests/parameters/collection_params.py` & `deker-local-adapters-1.0.1b0/tests/parameters/collection_params.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/tests/parameters/common.py` & `deker-local-adapters-1.0.1b0/tests/parameters/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
     numpy.compat.long,
     numpy.longlong,
 ]
 
 
 def random_string() -> str:
     """Get random string with length from 1 to 20."""
-    strings = (
-        (digits + ascii_letters + punctuation).replace("/", "").replace("\\", "").replace("$", "")
-    )
+    strings = (digits + ascii_letters + punctuation).replace("/", "").replace("\\", "").replace("$", "")
     return "".join((random.choice(strings) for _ in range(random.randint(5, 20))))
 
 
 def _random_positive_int() -> int:
     """Get random positive integer from 1 to 6."""
     return random.randint(1, 6)
```

### Comparing `deker-local-adapters-1.0.0/tests/parameters/index_exp_params.py` & `deker-local-adapters-1.0.1b0/tests/parameters/index_exp_params.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/tests/parameters/schemas_params.py` & `deker-local-adapters-1.0.1b0/tests/parameters/schemas_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 import random
 
 from datetime import datetime, timedelta
 from types import NoneType
 from typing import Any, List, Tuple, Type, Union
-from zoneinfo import ZoneInfo
 
 from deker.ABC.base_schemas import BaseDimensionSchema
-from deker.schemas import (
-    ArraySchema,
-    AttributeSchema,
-    DimensionSchema,
-    TimeDimensionSchema,
-    VArraySchema,
-)
-from deker.types import Scale
-from deker.types import Numeric
-
-from tests.parameters.common import (
-    INTEG,
-    NumericDtypes,
-    _random_positive_int,
-    random_step,
-    random_string,
-)
+from deker.schemas import ArraySchema, AttributeSchema, DimensionSchema, TimeDimensionSchema, VArraySchema
+from deker.types import Numeric, Scale
+from zoneinfo import ZoneInfo
+
+from tests.parameters.common import INTEG, NumericDtypes, _random_positive_int, random_step, random_string
 
 
 def get_vgrids(dimensions: List[BaseDimensionSchema]):
     def make_variations(vgrid, index) -> List[list]:
         vgrds = []
         d = dimensions[index]
         if len(vgrid) == 1:
@@ -79,68 +66,55 @@
         "start_value": datetime.now(ZoneInfo(random.choice(tz))),
     }
 
 
 class SchemaParams:
     @classmethod
     def _get_dims_dtype(cls) -> Tuple[List[DimensionSchema], Type[Numeric]]:
-        dims = [
-            DimensionSchema(**dimension_schema_random_params())
-            for _ in range(_random_positive_int())
-        ]
+        dims = [DimensionSchema(**dimension_schema_random_params()) for _ in range(_random_positive_int())]
         dtype = random.choice(NumericDtypes)
         return dims, dtype
 
     @classmethod
     def _get_attrs(cls, primary: bool) -> List[AttributeSchema]:
-        attrs = [
-            AttributeSchema(**attributes_schema_params(primary))
-            for _ in range(random.randint(1, 3))
-        ]
+        attrs = [AttributeSchema(**attributes_schema_params(primary)) for _ in range(random.randint(1, 3))]
         return attrs
 
 
 class ArraySchemaParamsNoTime(SchemaParams):
     @classmethod
     def OK_params_no_vgrid_no_attrs(cls):
         dimensions, dtype = cls._get_dims_dtype()
         return ArraySchema(dimensions=dimensions, dtype=dtype)
 
     @classmethod
     def OK_params_no_vgrid_primary_attributes(cls):
         dimensions, dtype = cls._get_dims_dtype()
-        attrs = [
-            AttributeSchema(**attributes_schema_params(True)) for _ in range(random.randint(1, 3))
-        ]
+        attrs = [AttributeSchema(**attributes_schema_params(True)) for _ in range(random.randint(1, 3))]
         return ArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs)
 
     @classmethod
     def OK_params_no_vgrid_custom_attributes(cls):
         dimensions, dtype = cls._get_dims_dtype()
-        attrs = [
-            AttributeSchema(**attributes_schema_params(False)) for _ in range(random.randint(1, 3))
-        ]
+        attrs = [AttributeSchema(**attributes_schema_params(False)) for _ in range(random.randint(1, 3))]
         return ArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs)
 
     @classmethod
     def OK_params_no_vgrid_all_attrs(cls):
         dimensions, dtype = cls._get_dims_dtype()
         attrs = [*cls._get_attrs(True), *cls._get_attrs(False)]
         return ArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs)
 
     @classmethod
     def OK_params_vgrid_primary_attributes(cls):
         dimensions, dtype = cls._get_dims_dtype()
         attrs = [
             AttributeSchema(dtype=str, name="vid", primary=True),
             AttributeSchema(dtype=str, name="v_position", primary=True),
-            *[
-                AttributeSchema(**attributes_schema_params(True))
-                for _ in range(random.randint(1, 3))
-            ],
+            *[AttributeSchema(**attributes_schema_params(True)) for _ in range(random.randint(1, 3))],
         ]
         return ArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs)
 
     @classmethod
     def OK_params_vgrid_all_attrs(cls):
         dimensions, dtype = cls._get_dims_dtype()
         attrs = [
@@ -183,92 +157,69 @@
         def no_attrs(cls):
             dimensions, dtype = cls._get_dims_dtype()
             return VArraySchema(dimensions=dimensions, dtype=dtype, vgrid=[1] * len(dimensions))
 
         @classmethod
         def primary_attributes(cls):
             dimensions, dtype = cls._get_dims_dtype()
-            attrs = [
-                AttributeSchema(**attributes_schema_params(True))
-                for _ in range(random.randint(1, 3))
-            ]
-            return VArraySchema(
-                dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions)
-            )
+            attrs = [AttributeSchema(**attributes_schema_params(True)) for _ in range(random.randint(1, 3))]
+            return VArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions))
 
         @classmethod
         def custom_attributes(cls):
             dimensions, dtype = cls._get_dims_dtype()
-            attrs = [
-                AttributeSchema(**attributes_schema_params(False))
-                for _ in range(random.randint(1, 3))
-            ]
-            return VArraySchema(
-                dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions)
-            )
+            attrs = [AttributeSchema(**attributes_schema_params(False)) for _ in range(random.randint(1, 3))]
+            return VArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions))
 
         @classmethod
         def no_vgrid_all_attrs(cls):
             dimensions, dtype = cls._get_dims_dtype()
             attrs = [*cls._get_attrs(True), *cls._get_attrs(False)]
-            return VArraySchema(
-                dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions)
-            )
+            return VArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions))
 
         @classmethod
         def vgrid_primary_attributes(cls):
             dimensions, dtype = cls._get_dims_dtype()
             attrs = [
                 AttributeSchema(dtype=str, name="vid", primary=True),
                 AttributeSchema(dtype=str, name="v_position", primary=True),
-                *[
-                    AttributeSchema(**attributes_schema_params(True))
-                    for _ in range(random.randint(1, 3))
-                ],
+                *[AttributeSchema(**attributes_schema_params(True)) for _ in range(random.randint(1, 3))],
             ]
-            return VArraySchema(
-                dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions)
-            )
+            return VArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions))
 
         @classmethod
         def vgrid_all_attrs(cls):
             dimensions, dtype = cls._get_dims_dtype()
             attrs = [
                 AttributeSchema(dtype=str, name="vid", primary=True),
                 AttributeSchema(dtype=str, name="v_position", primary=True),
                 *cls._get_attrs(False),
                 *cls._get_attrs(True),
             ]
-            return VArraySchema(
-                dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions)
-            )
+            return VArraySchema(dimensions=dimensions, dtype=dtype, attributes=attrs, vgrid=[1] * len(dimensions))
 
 
 class TimedSchemaParams:
     """Parameters for any schema that contains time dimension"""
 
     class OK(ArraySchemaParamsNoTime):
         @classmethod
         def _get_dims_dtype(cls) -> tuple:
             dims, dtype = super()._get_dims_dtype()
             time = TimeDimensionSchema(**time_dimension_schema_datetime_random_params())
             dims.insert(random.randint(0, len(dims)), time)  # type: ignore
             return dims, dtype
 
         @classmethod
-        def _insert_time_attribute(
-            cls, attrs: List[AttributeSchema], dimensions: List[DimensionSchema]
-        ) -> None:
+        def _insert_time_attribute(cls, attrs: List[AttributeSchema], dimensions: List[DimensionSchema]) -> None:
             for d in dimensions:
                 if isinstance(d, TimeDimensionSchema):
                     if isinstance(d.start_value, str):
                         primary = random.choice([True, False])
-                        time_attr = AttributeSchema(
-                            **attributes_schema_params(primary=primary, name=d.name)
-                        )
+                        time_attr = AttributeSchema(**attributes_schema_params(primary=primary, name=d.name))
                         attrs.insert(random.randint(0, len(attrs)), time_attr)
                         break
 
         @classmethod
         def _with_attributes(
             cls, make_primary: bool
         ) -> Tuple[List[DimensionSchema], Type[Numeric], List[AttributeSchema]]:
@@ -411,17 +362,15 @@
             cls,
             start_value: Union[str, datetime],
             primary: bool = None,
             vgrid=None,
             create_as_list=False,
         ):
             dims, dtype = ArraySchemaParamsNoTime._get_dims_dtype()
-            time_dimension = TimeDimensionSchema(
-                name="dt", size=3, start_value=start_value, step=timedelta(days=10)
-            )
+            time_dimension = TimeDimensionSchema(name="dt", size=3, start_value=start_value, step=timedelta(days=10))
             dims.append(time_dimension)  # type: ignore[arg-type]
             attrs = []
             if primary is not None:
                 attrs += cls._get_attrs(primary)
             vgrd = vgrid or [1] * len(dims)
             cls._insert_time_attribute(attrs, dims)
             if create_as_list:
@@ -445,65 +394,55 @@
         @classmethod
         def start_value_string_primary_attrs(cls, create_as_list: bool = False) -> VArraySchema:
             """VArray schema with start  value as string, and without any extra arguments
             (Only vid, vpos and step label attribute)
 
             :return:
             """
-            return cls.__make_schema_with_attributes(
-                start_value="$dt", primary=True, create_as_list=create_as_list
-            )
+            return cls.__make_schema_with_attributes(start_value="$dt", primary=True, create_as_list=create_as_list)
 
         @classmethod
         def start_value_string_custom_attrs(cls, create_as_list: bool = False) -> VArraySchema:
             """VArray schema with string start value, and without any extra arguments
             (Only vid, vpos and step label attribute)
 
             :return:
             """
-            return cls.__make_schema_with_attributes(
-                start_value="$dt", primary=False, create_as_list=create_as_list
-            )
+            return cls.__make_schema_with_attributes(start_value="$dt", primary=False, create_as_list=create_as_list)
 
         @classmethod
         def start_value_datetime_no_extra_attrs(cls, create_as_list: bool = False) -> VArraySchema:
             return cls.__make_schema_with_attributes(
                 start_value=datetime.now(ZoneInfo("UTC")),
                 primary=None,  # type: ignore[arg-type]
                 create_as_list=create_as_list,
             )
 
         @classmethod
-        def start_value_datetime_primary_attributes(
-            cls, create_as_list: bool = False
-        ) -> VArraySchema:
+        def start_value_datetime_primary_attributes(cls, create_as_list: bool = False) -> VArraySchema:
             return cls.__make_schema_with_attributes(
                 start_value=datetime.now(ZoneInfo("UTC")),
                 primary=True,
                 create_as_list=create_as_list,
             )
 
         @classmethod
-        def start_value_datetime_custom_attributes(
-            cls, create_as_list: bool = False
-        ) -> VArraySchema:
+        def start_value_datetime_custom_attributes(cls, create_as_list: bool = False) -> VArraySchema:
             return cls.__make_schema_with_attributes(
                 start_value=datetime.now(ZoneInfo("UTC")),
                 primary=False,
                 create_as_list=create_as_list,
             )
 
 
 class TypedSchemaParams:
     """Provides functionality to generate list with different types"""
 
     @classmethod
-    def _generate_types(
-        cls, base_dict: dict, key: str, *, exception_types: List[type] = None
-    ) -> List[dict]:
+    def _generate_types(cls, base_dict: dict, key: str, *, exception_types: List[type] = None) -> List[dict]:
         """Generates different types.
 
         :param base_dict: Dict with fixed values
         :param key: key for different types
         :param exception_types: if we need to skip some type
         """
         result = []
```

### Comparing `deker-local-adapters-1.0.0/tests/plugins/adapter.py` & `deker-local-adapters-1.0.1b0/tests/plugins/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 
 import pytest
 
 from deker.ABC import BaseStorageAdapter
 from deker.collection import Collection
 from deker.ctx import CTX
 
-from deker_local_adapters import (
-    HDF5StorageAdapter,
-    LocalArrayAdapter,
-    LocalCollectionAdapter,
-    LocalVArrayAdapter,
-)
+from deker_local_adapters import HDF5StorageAdapter, LocalArrayAdapter, LocalCollectionAdapter, LocalVArrayAdapter
 
 
 @pytest.fixture()
 def collection_adapter(ctx) -> LocalCollectionAdapter:
     """Creates a PathCollection adapter.
 
     :param ctx: client context
@@ -33,16 +28,23 @@
 @pytest.fixture()
 def local_array_adapter(array_collection: Collection, ctx: CTX) -> LocalArrayAdapter:
     """Instance of LocalArrayAdapter.
 
     Instance would be different from the one that appears in Array.
     """
     return LocalArrayAdapter(
-        collection_path=array_collection.path, collection_options=array_collection.options, ctx=ctx, storage_adapter=HDF5StorageAdapter, executor=ThreadPoolExecutor(workers=1)
+        collection_path=array_collection.path,
+        collection_options=array_collection.options,
+        ctx=ctx,
+        storage_adapter=HDF5StorageAdapter,
+        executor=ThreadPoolExecutor(workers=1),
     )
 
 
 @pytest.fixture()
 def local_varray_adapter(varray_collection: Collection, ctx: CTX) -> LocalVArrayAdapter:
     return LocalVArrayAdapter(
-        collection_path=varray_collection.path, ctx=ctx, executor=ThreadPoolExecutor(max_workers=1), storage_adapter=HDF5StorageAdapter
+        collection_path=varray_collection.path,
+        ctx=ctx,
+        executor=ThreadPoolExecutor(max_workers=1),
+        storage_adapter=HDF5StorageAdapter,
     )
```

### Comparing `deker-local-adapters-1.0.0/tests/plugins/arrays.py` & `deker-local-adapters-1.0.1b0/tests/plugins/arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     try:
         array.delete()
     except (BlockingIOError, DekerLockError):
         pass
 
 
 @pytest.fixture()
-def inserted_array_with_attributes(
-    array_collection_with_attributes: Collection, array_data: np.ndarray
-) -> Array:
+def inserted_array_with_attributes(array_collection_with_attributes: Collection, array_data: np.ndarray) -> Array:
     """Returns an instance of Array with data initialized in file and attributes.
 
     :param array_collection_with_attributes: Collection object
     :param array_data: array real data
     """
     array = array_collection_with_attributes.create(
         **{
@@ -132,17 +130,15 @@
     varray = varray_collection.create()
     varray[:].update(array_data)
     yield varray
     varray.delete()
 
 
 @pytest.fixture()
-def inserted_varray_with_attributes(
-    varray_collection_with_attributes: Collection, array_data: np.ndarray
-) -> VArray:
+def inserted_varray_with_attributes(varray_collection_with_attributes: Collection, array_data: np.ndarray) -> VArray:
     """Returns an instance of VArray with data initialized in file and attributes.
 
     :param varray_collection_with_attributes: Collection object
     :param array_data: array real data
     """
     array: VArray = varray_collection_with_attributes.create(
         **{
```

### Comparing `deker-local-adapters-1.0.0/tests/plugins/collection.py` & `deker-local-adapters-1.0.1b0/tests/plugins/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 from random import choices
 from string import ascii_letters
 
 import pytest
 
 from deker.client import Client
 from deker.collection import Collection
-from deker.schemas import (
-    ArraySchema,
-    AttributeSchema,
-    DimensionSchema,
-    TimeDimensionSchema,
-    VArraySchema,
-)
+from deker.schemas import ArraySchema, AttributeSchema, DimensionSchema, TimeDimensionSchema, VArraySchema
 from deker.types import Scale
 
 from deker_local_adapters import HDF5Options
 
 
 @pytest.fixture()
 def array_collection(
@@ -58,29 +52,25 @@
 
 
 @pytest.fixture()
 def varray_collection(
     client: "Client",
     varray_schema: "VArraySchema",
 ) -> Collection:
-    coll = client.create_collection(
-        name="".join(choices(ascii_letters, k=10)), schema=varray_schema
-    )
+    coll = client.create_collection(name="".join(choices(ascii_letters, k=10)), schema=varray_schema)
     yield coll
     coll.delete()
 
 
 @pytest.fixture()
 def varray_collection_with_attributes(
     client: "Client",
     varray_schema_with_attributes: "VArraySchema",
 ) -> Collection:
-    coll = client.create_collection(
-        name="".join(choices(ascii_letters, k=10)), schema=varray_schema_with_attributes
-    )
+    coll = client.create_collection(name="".join(choices(ascii_letters, k=10)), schema=varray_schema_with_attributes)
     yield coll
     coll.delete()
 
 
 @pytest.fixture()
 def collection_options() -> HDF5Options:
     """Creates an empty collection options object."""
@@ -121,40 +111,32 @@
 
 
 @pytest.fixture()
 def timed_collection(client) -> Collection:
     """Creates collection with regular scale description."""
     schema = ArraySchema(
         dimensions=[
-            TimeDimensionSchema(
-                name="days", size=31, start_value=datetime(2023, 1, 1), step=timedelta(days=1)
-            ),
-            TimeDimensionSchema(
-                name="hours", size=24, start_value="$time", step=timedelta(hours=1)
-            ),
+            TimeDimensionSchema(name="days", size=31, start_value=datetime(2023, 1, 1), step=timedelta(days=1)),
+            TimeDimensionSchema(name="hours", size=24, start_value="$time", step=timedelta(hours=1)),
         ],
         attributes=[AttributeSchema(name="time", dtype=datetime, primary=True)],
         dtype=float,
     )
     collection = client.create_collection("timed_collection", schema)
     yield collection
     collection.delete()
 
 
 @pytest.fixture()
 def timed_varray_collection(client) -> Collection:
     """Creates collection with regular scale description."""
     schema = VArraySchema(
         dimensions=[
-            TimeDimensionSchema(
-                name="days", size=31, start_value=datetime(2023, 1, 1), step=timedelta(days=1)
-            ),
-            TimeDimensionSchema(
-                name="hours", size=24, start_value="$time", step=timedelta(hours=1)
-            ),
+            TimeDimensionSchema(name="days", size=31, start_value=datetime(2023, 1, 1), step=timedelta(days=1)),
+            TimeDimensionSchema(name="hours", size=24, start_value="$time", step=timedelta(hours=1)),
         ],
         attributes=[AttributeSchema(name="time", dtype=datetime, primary=True)],
         dtype=float,
         vgrid=(1, 6),
     )
     collection = client.create_collection("timed_v_collection", schema)
     yield collection
```

### Comparing `deker-local-adapters-1.0.0/tests/plugins/schema.py` & `deker-local-adapters-1.0.1b0/tests/plugins/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 
 from datetime import datetime, timedelta, timezone
 from typing import List
 
 import pytest
 
 from deker.ABC.base_schemas import BaseDimensionSchema
-from deker.schemas import (
-    ArraySchema,
-    AttributeSchema,
-    DimensionSchema,
-    TimeDimensionSchema,
-    VArraySchema,
-)
+from deker.schemas import ArraySchema, AttributeSchema, DimensionSchema, TimeDimensionSchema, VArraySchema
 
 
 @pytest.fixture()
 def dimensions() -> List[BaseDimensionSchema]:
     """Dimensions for array schema."""
     return [
         DimensionSchema(name="x", size=10),
```

### Comparing `deker-local-adapters-1.0.0/tests/test_cases/test_array_adapter.py` & `deker-local-adapters-1.0.1b0/tests/test_cases/test_array_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import pytest
 
 from deker.arrays import Array
 from deker.client import Client
 from deker.collection import Collection
 from deker.errors import DekerArrayError, DekerArrayTypeError, DekerValidationError
 from deker.schemas import ArraySchema, DimensionSchema
-from deker.tools import create_array_from_meta, get_paths
+from deker.tools import get_paths
 
-from deker_local_adapters import LocalArrayAdapter, AdaptersFactory
+from deker_local_adapters import AdaptersFactory, LocalArrayAdapter
 from deker_local_adapters.storage_adapters.hdf5.hdf5_storage_adapter import HDF5StorageAdapter
 
 
 class TestArrayAdapter:
     """Class for testing local array adapter."""
 
     @pytest.mark.parametrize(
@@ -326,44 +326,39 @@
         """Tests getting array path from attributes.
 
         :param array_with_attributes: Array which contains some primary attributes
         """
         main_tree, rest = array_with_attributes.id.split("-", 1)
         main_tree = os.path.sep.join((s for s in main_tree))
         main_path = (
-            array_with_attributes._adapter.collection_path
-            / array_with_attributes._adapter.data_dir
-            / main_tree
-            / rest
+            array_with_attributes._adapter.collection_path / array_with_attributes._adapter.data_dir / main_tree / rest
         )
 
         sym_path = (
             array_with_attributes._adapter.collection_path
             / array_with_attributes._adapter.symlinks_dir
             / str(array_with_attributes.primary_attributes.get("primary_attribute"))
         )
 
-        adapter_paths = get_paths(
-            array_with_attributes, array_with_attributes._adapter.collection_path
-        )
+        adapter_paths = get_paths(array_with_attributes, array_with_attributes._adapter.collection_path)
 
         assert adapter_paths.main == main_path
         assert adapter_paths.symlink == sym_path
 
     def test_array_adapter_update_custom_attributes(self, array_with_attributes: Array):
         new_custom_attributes = {
             "custom_attribute": 0.6,
             "time_attr_name": datetime.now(timezone.utc),
         }
         adapter = array_with_attributes._adapter
         adapter.create(array_with_attributes)
         adapter.update_meta_custom_attributes(array_with_attributes, new_custom_attributes)
         assert array_with_attributes.custom_attributes == new_custom_attributes
         meta = array_with_attributes.read_meta()
-        ar = create_array_from_meta(
+        ar = Array._create_from_meta(
             array_with_attributes._Array__collection,  # type: ignore[attr-defined]
             meta,  # type: ignore[arg-type]
             array_with_attributes._adapter,
         )
         assert ar.custom_attributes == new_custom_attributes
 
     def test_array_adapter_iter(self, array_collection: Collection):
```

### Comparing `deker-local-adapters-1.0.0/tests/test_cases/test_collection_adapter.py` & `deker-local-adapters-1.0.1b0/tests/test_cases/test_collection_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import pytest
 
 from deker.client import Client
 from deker.collection import Collection
 from deker.errors import DekerMemoryError
 from deker.schemas import ArraySchema, DimensionSchema
-from deker_local_adapters.storage_adapters.hdf5.hdf5_storage_adapter import HDF5StorageAdapter
 
 from tests.parameters.common import random_string
 
-from deker_local_adapters import LocalCollectionAdapter, AdaptersFactory
+from deker_local_adapters import AdaptersFactory, LocalCollectionAdapter
+from deker_local_adapters.storage_adapters.hdf5.hdf5_storage_adapter import HDF5StorageAdapter
 
 
 @pytest.mark.asyncio()
 class TestCollectionAdapter:
     """Class for testing local collection adapter."""
 
     def test_collection_adapter_create_collection(
@@ -30,15 +30,23 @@
         """Tests if adapter creates array_collection in DB.
 
         :param collection_adapter: CollectionAdapter
         :param root_path: Path to collections directory
         :param array_schema: ArraySchema instance
         """
         name = random_string()
-        collection_adapter.create(Collection(name=name, schema=array_schema, adapter=collection_adapter, factory=factory, storage_adapter=HDF5StorageAdapter ))
+        collection_adapter.create(
+            Collection(
+                name=name,
+                schema=array_schema,
+                adapter=collection_adapter,
+                factory=factory,
+                storage_adapter=HDF5StorageAdapter,
+            )
+        )
         assert root_path.joinpath(factory.ctx.config.collections_directory).joinpath(name).exists()
 
     def test_collection_adapter_create_collection_memory_error(
         self,
         collection_adapter: LocalCollectionAdapter,
         factory: AdaptersFactory,
     ):
@@ -53,15 +61,23 @@
                 DimensionSchema(name="x", size=10000),
                 DimensionSchema(name="y", size=10000),
             ],
             dtype=float,
         )
         col_name = "memory_excess_adapter"
         with pytest.raises(DekerMemoryError):
-            collection_adapter.create(Collection(name=col_name, schema=schema, adapter=collection_adapter, factory=factory, storage_adapter=HDF5StorageAdapter))
+            collection_adapter.create(
+                Collection(
+                    name=col_name,
+                    schema=schema,
+                    adapter=collection_adapter,
+                    factory=factory,
+                    storage_adapter=HDF5StorageAdapter,
+                )
+            )
 
     def test_collection_adapter_deletes_collection(
         self,
         collection_adapter: LocalCollectionAdapter,
         array_collection: Collection,
         root_path: Path,
     ):
@@ -99,27 +115,23 @@
         :param array_collection: Pre created collection
         :param collection_adapter: collection adapter
         :param root_path: Path to collections directory
         """
         collection_adapter.clear(array_collection)
 
         collection_dir = None
-        for child in root_path.joinpath(
-            collection_adapter.ctx.config.collections_directory
-        ).iterdir():
+        for child in root_path.joinpath(collection_adapter.ctx.config.collections_directory).iterdir():
             if child.name == array_collection.name:
                 collection_dir = child
 
         assert collection_dir is not None
         collection_dir = os.listdir(collection_dir)
         assert f"{array_collection.name}.json" in collection_dir
 
-    def test_collection_adapter_iter(
-        self, client: Client, array_schema: ArraySchema, root_path: Path, ctx
-    ):
+    def test_collection_adapter_iter(self, client: Client, array_schema: ArraySchema, root_path: Path, ctx):
         for root, dirs, files in os.walk(root_path / ctx.config.collections_directory):
             for f in files:
                 os.remove(os.path.join(root, f))
             for d in dirs:
                 shutil.rmtree(os.path.join(root, d))
 
         names = {random_string() for _ in range(10)}
```

### Comparing `deker-local-adapters-1.0.0/tests/test_cases/test_collection_options_validation.py` & `deker-local-adapters-1.0.1b0/tests/test_cases/test_collection_options_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,15 @@
         options = HDF5Options(
             chunks=None,
             compression_opts=HDF5CompressionOpts(compression="gzip", compression_opts=9),
         )
 
         schema = ArraySchema(dtype=float, dimensions=dims)
         collection = client.create_collection("simple", schema=schema)
-        compressed = client.create_collection(
-            "compressed", schema=schema, collection_options=options
-        )
+        compressed = client.create_collection("compressed", schema=schema, collection_options=options)
         collection_path = collection.path
         compressed_path = compressed.path
         data = np.random.random((1024, 1024))
 
         array = collection.create()
         array_id = array.id
         array_path = collection_path / "array_symlinks" / (array_id + ".hdf5")
@@ -202,17 +200,15 @@
         name: str,
         array_schema: ArraySchema,
         array_data: np.ndarray,
         chunks,
         compression,
         level,
     ):
-        params = HDF5Options(
-            chunks, HDF5CompressionOpts(compression=compression, compression_opts=level)
-        )
+        params = HDF5Options(chunks, HDF5CompressionOpts(compression=compression, compression_opts=level))
         collection = client.create_collection(name, array_schema, params)
         try:
             assert collection.options.as_dict == params.as_dict
             coll_from_meta = client.get_collection(name)
             assert collection.options == coll_from_meta.options
             array = collection.create()
             subset = array[:]
```

### Comparing `deker-local-adapters-1.0.0/tests/test_cases/test_factory.py` & `deker-local-adapters-1.0.1b0/tests/test_cases/test_factory.py`

 * *Files identical despite different names*

### Comparing `deker-local-adapters-1.0.0/tests/test_cases/test_varray_adapter.py` & `deker-local-adapters-1.0.1b0/tests/test_cases/test_varray_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import numpy as np
 import pytest
 
 from deker.arrays import VArray
 from deker.collection import Collection
 from deker.errors import DekerArrayError, DekerValidationError
-from deker.tools import create_array_from_meta, get_paths
-from deker_local_adapters.storage_adapters.hdf5.hdf5_storage_adapter import HDF5StorageAdapter
+from deker.tools import get_paths
 from deker_tools.path import is_empty
 
 from deker_local_adapters import LocalVArrayAdapter
+from deker_local_adapters.storage_adapters.hdf5.hdf5_storage_adapter import HDF5StorageAdapter
 
 
 class TestVArrayAdapterMethods:
     def test_varray_adapter_init(self, array_collection, ctx, executor):
         adapter = LocalVArrayAdapter(array_collection.path, ctx, HDF5StorageAdapter, executor)
         assert adapter
 
@@ -68,17 +68,15 @@
 
         paths = get_paths(varray, varray._VArray__collection.path)  # type: ignore[attr-defined]
         adapter.delete(varray)
         assert find.first() is None
         assert not (paths.symlink / array.id).exists()
         assert not (paths.main / array.id).exists()
         assert not paths.main.exists()
-        assert not (
-            varray._VArray__collection.path / ctx.config.array_data_directory / array.id
-        ).exists()
+        assert not (varray._VArray__collection.path / ctx.config.array_data_directory / array.id).exists()
 
         assert not is_empty(
             varray._VArray__collection.path / ctx.config.array_symlinks_directory  # type: ignore[attr-defined]
         )
 
     def test_varray_adapter_delete_varray_and_arrays(self, varray: VArray, ctx):
         """Test delete varray with all its contents."""
@@ -97,17 +95,15 @@
 
         paths = get_paths(varray, varray._VArray__collection.path)  # type: ignore[attr-defined]
         array.delete()
         assert find.first() is None
         assert not (paths.symlink / array.id).exists()
         assert not (paths.main / array.id).exists()
         assert not paths.main.exists()
-        assert not (
-            varray._VArray__collection.path / ctx.config.array_data_directory / array.id
-        ).exists()
+        assert not (varray._VArray__collection.path / ctx.config.array_data_directory / array.id).exists()
 
         assert is_empty(
             varray._VArray__collection.path / ctx.config.array_symlinks_directory  # type: ignore[attr-defined]
         )
 
     def test_varray_adapter_read_meta_from_varray(self, varray: VArray):
         """Test read meta."""
@@ -132,15 +128,15 @@
             "time_attr_name": datetime.now(timezone.utc),
         }
         adapter: LocalVArrayAdapter = varray_with_attributes._adapter
         adapter.create(varray_with_attributes)
         adapter.update_meta_custom_attributes(varray_with_attributes, new_custom_attributes)
         assert varray_with_attributes.custom_attributes == new_custom_attributes
         meta = varray_with_attributes.read_meta()
-        ar = create_array_from_meta(
+        ar = VArray._create_from_meta(
             varray_with_attributes._VArray__collection,  # type: ignore[attr-defined]
             meta,  # type: ignore[arg-type]
             varray_adapter=adapter,
             array_adapter=varray_with_attributes._VArray__array_adapter,  # type: ignore[attr-defined]
         )
         assert ar.custom_attributes == new_custom_attributes
```

