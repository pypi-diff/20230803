# Comparing `tmp/pip-tools-7.1.0.tar.gz` & `tmp/pip-tools-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tools-7.1.0.tar", last modified: Wed Jul 19 05:17:55 2023, max compression
+gzip compressed data, was "pip-tools-7.2.0.tar", last modified: Wed Aug  2 23:42:33 2023, max compression
```

## Comparing `pip-tools-7.1.0.tar` & `pip-tools-7.2.0.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/reusable-qa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    43302 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-19 05:17:37.000000 pip-tools-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-19 05:17:55.726570 pip-tools-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-19 05:17:37.000000 pip-tools-7.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 05:17:37.000000 pip-tools-7.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/django.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/flask.in
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/hypothesis.in
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/protection.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/sentry.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-19 05:17:37.000000 pip-tools-7.1.0/img/pip-tools-overview.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.710570 pip-tools-7.1.0/pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.710570 pip-tools-7.1.0/piptools/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/_compat/pip_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22000 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    23984 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-19 05:17:37.000000 pip-tools-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:17:55.726570 pip-tools-7.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.718571 pip-tools-7.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13145 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    93693 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cli_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cli_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.722571 pip-tools-7.1.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/fake-editables.json
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/fake-index.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/minimal_wheels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.694570 pip-tools-7.1.0/tests/test_data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_a/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_a/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.694570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_unpinned_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_fake_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_minimal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_repository_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_repository_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_top_level_editable.py
--rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/reusable-qa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    43984 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 23:42:09.000000 pip-tools-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-08-02 23:42:33.262357 pip-tools-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-08-02 23:42:09.000000 pip-tools-7.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 23:42:09.000000 pip-tools-7.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/pip-compile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/pip-sync.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/django.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/flask.in
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/hypothesis.in
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/protection.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/sentry.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-02 23:42:09.000000 pip-tools-7.2.0/img/pip-tools-overview.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/_compat/pip_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22721 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-02 23:42:09.000000 pip-tools-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:42:33.262357 pip-tools-7.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.258357 pip-tools-7.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95931 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cli_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cli_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.258357 pip-tools-7.2.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/fake-editables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/fake-index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/minimal_wheels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.238356 pip-tools-7.2.0/tests/test_data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_a/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.238356 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_unpinned_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_fake_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_minimal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_repository_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_repository_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_top_level_editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tox.ini
```

### Comparing `pip-tools-7.1.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pip-tools-7.2.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `pip-tools-7.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/release-drafter.yml` & `pip-tools-7.2.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/workflows/ci.yml` & `pip-tools-7.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/workflows/release-drafter.yml` & `pip-tools-7.2.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/workflows/release.yml` & `pip-tools-7.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.github/workflows/reusable-qa.yml` & `pip-tools-7.2.0/.github/workflows/reusable-qa.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/.pre-commit-config.yaml` & `pip-tools-7.2.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         args: [--target-version=py38]
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.9.0
+    rev: v3.10.1
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-pytest-style
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
```

### Comparing `pip-tools-7.1.0/CHANGELOG.md` & `pip-tools-7.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,45 @@
-## 7.1.0 (2023-07-18)
+## v7.2.0
+
+02 Aug 2023
+
+Features:
+
+- Add `-c/--constraint` option to `pip-compile`
+  ([#1936](https://github.com/jazzband/pip-tools/pull/1936)). Thanks @atugushev
+
+Bug Fixes:
+
+- Allow options in config from both `pip-compile` and `pip-sync`
+  ([#1933](https://github.com/jazzband/pip-tools/pull/1933)). Thanks @atugushev
+- Fix rejection of negating CLI boolean flags in config
+  ([#1913](https://github.com/jazzband/pip-tools/pull/1913)). Thanks @chrysle
+
+Other Changes:
+
+- Add Command Line Reference section to docs
+  ([#1934](https://github.com/jazzband/pip-tools/pull/1934)). Thanks @atugushev
+
+## v7.1.0
+
+18 Jul 2023
 
 Features:
 
 - Validate parsed config against CLI options
   ([#1910](https://github.com/jazzband/pip-tools/pull/1910)). Thanks @atugushev
 
 Bug Fixes:
 
 - Fix a bug where pip-sync would unexpectedly uninstall some packages
   ([#1919](https://github.com/jazzband/pip-tools/pull/1919)). Thanks @atugushev
 
-## 7.0.0 (2023-07-14)
+## v7.0.0
+
+14 Jul 2023
 
 Backwards Incompatible Changes:
 
 - Default to `--resolver=backtracking`
   ([#1897](https://github.com/jazzband/pip-tools/pull/1897)). Thanks @atugushev
 - Drop support for Python 3.7
   ([#1879](https://github.com/jazzband/pip-tools/pull/1879)). Thanks @chrysle
@@ -29,15 +54,17 @@
 Bug Fixes:
 
 - Sync direct references with hashes
   ([#1885](https://github.com/jazzband/pip-tools/pull/1885)). Thanks @siddharthab
 - Fix missing `via`s when more than two input files are used
   ([#1890](https://github.com/jazzband/pip-tools/pull/1890)). Thanks @lpulley
 
-## 6.14.0 (2023-06-28)
+## v6.14.0
+
+28 Jun 2023
 
 Features:
 
 - Support config defaults using `.pip-tools.toml` or `pyproject.toml`
   ([#1863](https://github.com/jazzband/pip-tools/pull/1863)). Thanks @j00bar
 - Log a warning if the user specifies `-P` and the output file is present but empty
   ([#1822](https://github.com/jazzband/pip-tools/pull/1822)). Thanks @davidmreed
@@ -47,15 +74,17 @@
 Other Changes:
 
 - Correct in README `pre-commit` hook to run off `requirements.in`
   ([#1847](https://github.com/jazzband/pip-tools/pull/1847)). Thanks @atugushev
 - Add pyprojects.toml example for using setuptools
   ([#1851](https://github.com/jazzband/pip-tools/pull/1851)). Thanks @shatakshiiii
 
-## 6.13.0 (2023-04-07)
+## v6.13.0
+
+07 Apr 2023
 
 Features:
 
 - Add support for self-referential extras
   ([#1791](https://github.com/jazzband/pip-tools/pull/1791)). Thanks @q0w
 - Add support for `pip==23.1` where removed `FormatControl` in `WheelCache`
   ([#1834](https://github.com/jazzband/pip-tools/pull/1834)). Thanks @atugushev
@@ -70,42 +99,50 @@
   ([#1827](https://github.com/jazzband/pip-tools/pull/1827)). Thanks @q0w
 
 Other Changes:
 
 - Update examples in README ([#1835](https://github.com/jazzband/pip-tools/pull/1835)).
   Thanks @lucaswerkmeister
 
-## 6.12.3 (2023-03-01)
+## v6.12.3
+
+01 Mar 2023
 
 Bug Fixes:
 
 - Remove extras from user-supplied constraints in backtracking resolver
   ([#1808](https://github.com/jazzband/pip-tools/pull/1808)). Thanks @thomdixon
 - Fix for sync error when the ireqs being merged have no names
   ([#1802](https://github.com/jazzband/pip-tools/pull/1802)). Thanks @richafrank
 
-## 6.12.2 (2022-12-25)
+## v6.12.2
+
+25 Dec 2022
 
 Bug Fixes:
 
 - Raise error if input and output filenames are matched
   ([#1787](https://github.com/jazzband/pip-tools/pull/1787)). Thanks @atugushev
 - Add `pyproject.toml` as default input file format
   ([#1780](https://github.com/jazzband/pip-tools/pull/1780)). Thanks @berislavlopac
 - Fix a regression with unsafe packages for `--allow-unsafe`
   ([#1788](https://github.com/jazzband/pip-tools/pull/1788)). Thanks @q0w
 
-## 6.12.1 (2022-12-16)
+## v6.12.1
+
+16 Dec 2022
 
 Bug Fixes:
 
 - Set explicitly packages for setuptools
   ([#1782](https://github.com/jazzband/pip-tools/pull/1782)). Thanks @q0w
 
-## 6.12.0 (2022-12-13)
+## v6.12.0
+
+13 Dec 2022
 
 Features:
 
 - Add `--no-index` flag to `pip-compile`
   ([#1745](https://github.com/jazzband/pip-tools/pull/1745)). Thanks @atugushev
 
 Bug Fixes:
@@ -113,15 +150,17 @@
 - Treat `--upgrade-packages` PKGSPECs as constraints (not just minimums), consistently
   ([#1578](https://github.com/jazzband/pip-tools/pull/1578)). Thanks @AndydeCleyre
 - Filter out the user provided unsafe packages
   ([#1766](https://github.com/jazzband/pip-tools/pull/1766)). Thanks @q0w
 - Adopt PEP-621 for packaging
   ([#1763](https://github.com/jazzband/pip-tools/pull/1763)). Thanks @ssbarnea
 
-## 6.11.0 (2022-11-30)
+## v6.11.0
+
+30 Nov 2022
 
 Features:
 
 - Add `pyproject.toml` file ([#1643](https://github.com/jazzband/pip-tools/pull/1643)).
   Thanks @otherJL0
 - Support build isolation using `setuptools/pyproject.toml` requirement files
   ([#1727](https://github.com/jazzband/pip-tools/pull/1727)). Thanks @atugushev
@@ -136,15 +175,17 @@
 Other Changes:
 
 - Bump click minimum version to `>= 8`
   ([#1733](https://github.com/jazzband/pip-tools/pull/1733)). Thanks @atugushev
 - Bump pip minimum version to `>= 22.2`
   ([#1729](https://github.com/jazzband/pip-tools/pull/1729)). Thanks @atugushev
 
-## 6.10.0 (2022-11-13)
+## v6.10.0
+
+13 Nov 2022
 
 Features:
 
 - Deprecate `pip-compile --resolver=legacy`
   ([#1724](https://github.com/jazzband/pip-tools/pull/1724)). Thanks @atugushev
 - Prompt user to use the backtracking resolver on errors
   ([#1719](https://github.com/jazzband/pip-tools/pull/1719)). Thanks @maxfenv
@@ -165,15 +206,17 @@
 - Update pip-tools version in the README's pre-commit examples
   ([#1701](https://github.com/jazzband/pip-tools/pull/1701)). Thanks @Kludex
 - Document use of the backtracking resolver
   ([#1718](https://github.com/jazzband/pip-tools/pull/1718)). Thanks @maxfenv
 - Use HTTPS in a readme link ([#1716](https://github.com/jazzband/pip-tools/pull/1716)).
   Thanks @Arhell
 
-## 6.9.0 (2022-10-05)
+## v6.9.0
+
+05 Oct 2022
 
 Features:
 
 - Add `--all-extras` flag to `pip-compile`
   ([#1630](https://github.com/jazzband/pip-tools/pull/1630)). Thanks @apljungquist
 - Support Exclude Package with custom unsafe packages
   ([#1509](https://github.com/jazzband/pip-tools/pull/1509)). Thanks @hmc-cs-mdrissi
@@ -186,23 +229,27 @@
   ([#1648](https://github.com/jazzband/pip-tools/pull/1648)). Thanks @FlorentJeannot
 
 Other Changes:
 
 - Add pyproject.toml & modern packaging to introduction.
   ([#1668](https://github.com/jazzband/pip-tools/pull/1668)). Thanks @hynek
 
-## 6.8.0 (2022-06-30)
+## v6.8.0
+
+30 Jun 2022
 
 Features:
 
 - Add support for pip's 2020 dependency resolver. Use
   `pip-compile --resolver backtracking` to enable new resolver
   ([#1539](https://github.com/jazzband/pip-tools/pull/1539)). Thanks @atugushev
 
-## 6.7.0 (2022-06-27)
+## v6.7.0
+
+27 Jun 2022
 
 Features:
 
 - Support for the `importlib.metadata` metadata implementation
   ([#1632](https://github.com/jazzband/pip-tools/pull/1632)). Thanks @richafrank
 
 Bug Fixes:
@@ -212,92 +259,108 @@
 
 Other Changes:
 
 - Replace direct usage of the `pep517` module with the `build` module, for loading
   project metadata ([#1629](https://github.com/jazzband/pip-tools/pull/1629)). Thanks
   @AndydeCleyre
 
-## 6.6.2 (2022-05-23)
+## v6.6.2
+
+23 May 2022
 
 Bug Fixes:
 
 - Update `PyPIRepository::resolve_reqs()` for pip>=22.1.1
   ([#1624](https://github.com/jazzband/pip-tools/pull/1624)). Thanks @m000
 
-## 6.6.1 (2022-05-13)
+## v6.6.1
+
+13 May 2022
 
 Bug Fixes:
 
 - Fix support for pip>=22.1 ([#1618](https://github.com/jazzband/pip-tools/pull/1618)).
   Thanks @wizpig64
 
-## 6.6.0 (2022-04-06)
+## v6.6.0
+
+06 Apr 2022
 
 Features:
 
 - Add support for pip>=22.1 ([#1607](https://github.com/jazzband/pip-tools/pull/1607)).
   Thanks @atugushev
 
 Bug Fixes:
 
 - Ensure `pip-compile --dry-run --quiet` still shows what would be done, while omitting
   the dry run message ([#1592](https://github.com/jazzband/pip-tools/pull/1592)). Thanks
   @AndydeCleyre
 - Fix `--generate-hashes` when hashes are computed from files
   ([#1540](https://github.com/jazzband/pip-tools/pull/1540)). Thanks @RazerM
 
-## 6.5.1 (2022-02-08)
+## v6.5.1
+
+08 Feb 2022
 
 Bug Fixes:
 
 - Ensure canonicalized requirement names are used as keys, to prevent unnecessary
   reinstallations during sync
   ([#1572](https://github.com/jazzband/pip-tools/pull/1572)). Thanks @AndydeCleyre
 
-## 6.5.0 (2022-02-04)
+## v6.5.0
+
+04 Feb 2022
 
 Features:
 
 - Add support for pip>=22.0, drop support for Python 3.6
   ([#1567](https://github.com/jazzband/pip-tools/pull/1567)). Thanks @di
 - Test on Python 3.11 ([#1527](https://github.com/jazzband/pip-tools/pull/1527)). Thanks
   @hugovk
 
 Other Changes:
 
 - Minor doc edits ([#1445](https://github.com/jazzband/pip-tools/pull/1445)). Thanks
   @ssiano
 
-## 6.4.0 (2021-10-12)
+## v6.4.0
+
+12 Oct 2021
 
 Features:
 
 - Add support for `pip>=21.3`
   ([#1501](https://github.com/jazzband/pip-tools/pull/1501)). Thanks @atugushev
 - Add support for Python 3.10
   ([#1497](https://github.com/jazzband/pip-tools/pull/1497)). Thanks @joshuadavidthomas
 
 Other Changes:
 
 - Bump pip minimum version to `>= 21.2`
   ([#1500](https://github.com/jazzband/pip-tools/pull/1500)). Thanks @atugushev
 
-## 6.3.1 (2021-10-08)
+## v6.3.1
+
+08 Oct 2021
 
 Bug Fixes:
 
 - Ensure `pip-tools` unions dependencies of multiple declarations of a package with
   different extras ([#1486](https://github.com/jazzband/pip-tools/pull/1486)). Thanks
   @richafrank
 - Allow comma-separated arguments for `--extra`
   ([#1493](https://github.com/jazzband/pip-tools/pull/1493)). Thanks @AndydeCleyre
 - Improve clarity of help text for options supporting multiple
   ([#1492](https://github.com/jazzband/pip-tools/pull/1492)). Thanks @AndydeCleyre
 
-## 6.3.0 (2021-09-21)
+## v6.3.0
+
+21 Sep 2021
 
 Features:
 
 - Enable single-line annotations with `pip-compile --annotation-style=line`
   ([#1477](https://github.com/jazzband/pip-tools/pull/1477)). Thanks @AndydeCleyre
 - Generate PEP 440 direct reference whenever possible
   ([#1455](https://github.com/jazzband/pip-tools/pull/1455)). Thanks @FlorentJeannot
@@ -307,15 +370,17 @@
 Bug Fixes:
 
 - Change log level of hash message
   ([#1460](https://github.com/jazzband/pip-tools/pull/1460)). Thanks @plannigan
 - Allow passing `--no-upgrade` option
   ([#1438](https://github.com/jazzband/pip-tools/pull/1438)). Thanks @ssbarnea
 
-## 6.2.0 (2021-06-22)
+## v6.2.0
+
+22 Jun 2021
 
 Features:
 
 - Add `--emit-options/--no-emit-options` flags to `pip-compile`
   ([#1123](https://github.com/jazzband/pip-tools/pull/1123)). Thanks @atugushev
 - Add `--python-executable` option for `pip-sync`
   ([#1333](https://github.com/jazzband/pip-tools/pull/1333)). Thanks @MaratFM
@@ -341,42 +406,48 @@
 - Add `setuptools` and `wheel` dependencies to the `setup.cfg`
   ([#889](https://github.com/jazzband/pip-tools/pull/889)). Thanks @jayvdb
 - Improve instructions for new contributors
   ([#1394](https://github.com/jazzband/pip-tools/pull/1394)). Thanks @FlorentJeannot
 - Better explain role of existing `requirements.txt`
   ([#1369](https://github.com/jazzband/pip-tools/pull/1369)). Thanks @mikepqr
 
-## 6.1.0 (2021-04-14)
+## v6.1.0
+
+14 Apr 2021
 
 Features:
 
 - Add support for `pyproject.toml` or `setup.cfg` as input dependency file (PEP-517) for
   `pip-compile` ([#1356](https://github.com/jazzband/pip-tools/pull/1356)). Thanks
   @orsinium
 - Add `pip-compile --extra` option to specify `extras_require` dependencies
   ([#1363](https://github.com/jazzband/pip-tools/pull/1363)). Thanks @orsinium
 
 Bug Fixes:
 
 - Restore ability to set compile cache with env var `PIP_TOOLS_CACHE_DIR`
   ([#1368](https://github.com/jazzband/pip-tools/pull/1368)). Thanks @AndydeCleyre
 
-## 6.0.1 (2021-03-15)
+## v6.0.1
+
+15 Mar 2021
 
 Bug Fixes:
 
 - Fixed a bug with undeclared dependency on `importlib-metadata` at Python 3.6
   ([#1353](https://github.com/jazzband/pip-tools/pull/1353)). Thanks @atugushev
 
 Dependencies:
 
 - Add `pep517` dependency ([#1353](https://github.com/jazzband/pip-tools/pull/1353)).
   Thanks @atugushev
 
-## 6.0.0 (2021-03-12)
+## v6.0.0
+
+12 Mar 2021
 
 Backwards Incompatible Changes:
 
 - Remove support for EOL Python 3.5 and 2.7
   ([#1243](https://github.com/jazzband/pip-tools/pull/1243)). Thanks @jdufresne
 - Remove deprecated `--index/--no-index` option from `pip-compile`
   ([#1234](https://github.com/jazzband/pip-tools/pull/1234)). Thanks @jdufresne
@@ -401,15 +472,17 @@
   ([#1325](https://github.com/jazzband/pip-tools/pull/1325)). Thanks @fahrradflucht
 
 Dependencies:
 
 - Bump `pip` minimum version to `>= 20.3`
   ([#1340](https://github.com/jazzband/pip-tools/pull/1340)). Thanks @atugushev
 
-## 5.5.0 (2020-12-31)
+## v5.5.0
+
+31 Dec 2020
 
 Features:
 
 - Add Python 3.9 support ([1222](https://github.com/jazzband/pip-tools/pull/1222)).
   Thanks @jdufresne
 - Improve formatting of long "via" annotations
   ([1237](https://github.com/jazzband/pip-tools/pull/1237)). Thanks @jdufresne
@@ -432,38 +505,44 @@
 Improved Documentation:
 
 - Add `pip-requirements.el` (for Emacs) to useful tools to `README`
   ([#1244](https://github.com/jazzband/pip-tools/pull/1244)). Thanks @jdufresne
 - Add supported Python versions to `README`
   ([#1246](https://github.com/jazzband/pip-tools/pull/1246)). Thanks @jdufresne
 
-## 5.4.0 (2020-11-21)
+## v5.4.0
+
+21 Nov 2020
 
 Features:
 
 - Add `pip>=20.3` support ([1216](https://github.com/jazzband/pip-tools/pull/1216)).
   Thanks @atugushev and @AndydeCleyre
 - Exclude `--no-reuse-hashes` option from «command to run» header
   ([1197](https://github.com/jazzband/pip-tools/pull/1197)). Thanks @graingert
 
 Dependencies:
 
 - Bump `pip` minimum version to `>= 20.1`
   ([1191](https://github.com/jazzband/pip-tools/pull/1191)). Thanks @atugushev and
   @AndydeCleyre
 
-## 5.3.1 (2020-07-31)
+## v5.3.1
+
+31 Jul 2020
 
 Bug Fixes:
 
 - Fix `pip-20.2` compatibility issue that caused `pip-tools` to sometime fail to
   stabilize in a constant number of rounds
   ([1194](https://github.com/jazzband/pip-tools/pull/1194)). Thanks @vphilippon
 
-## 5.3.0 (2020-07-26)
+## v5.3.0
+
+26 Jul 2020
 
 Features:
 
 - Add `-h` alias for `--help` option to `pip-sync` and `pip-compile`
   ([1163](https://github.com/jazzband/pip-tools/pull/1163)). Thanks @jan25
 - Add `pip>=20.2` support ([1168](https://github.com/jazzband/pip-tools/pull/1168)).
   Thanks @atugushev
@@ -471,23 +550,27 @@
   ([1172](https://github.com/jazzband/pip-tools/pull/1172)). Thanks @francisbrito
 - `pip-compile` now doesn't resolve constraints from `-c constraints.txt`that are not
   (yet) requirements ([1175](https://github.com/jazzband/pip-tools/pull/1175)). Thanks
   @clslgrnc
 - Add `--reuse-hashes/--no-reuse-hashes` options to `pip-compile`
   ([1177](https://github.com/jazzband/pip-tools/pull/1177)). Thanks @graingert
 
-## 5.2.1 (2020-06-09)
+## v5.2.1
+
+09 Jun 2020
 
 Bug Fixes:
 
 - Fix a bug where `pip-compile` would lose some dependencies on update a
   `requirements.txt` ([1159](https://github.com/jazzband/pip-tools/pull/1159)). Thanks
   @richafrank
 
-## 5.2.0 (2020-05-27)
+## v5.2.0
+
+27 May 2020
 
 Features:
 
 - Show basename of URLs when `pip-compile` generates hashes in a verbose mode
   ([1113](https://github.com/jazzband/pip-tools/pull/1113)). Thanks @atugushev
 - Add `--emit-index-url/--no-emit-index-url` options to `pip-compile`
   ([1130](https://github.com/jazzband/pip-tools/pull/1130)). Thanks @atugushev
@@ -509,39 +592,47 @@
   Thanks @atugushev
 
 Other Changes:
 
 - Switch to `setuptools` declarative syntax through `setup.cfg`
   ([1141](https://github.com/jazzband/pip-tools/pull/1141)). Thanks @jdufresne
 
-## 5.1.2 (2020-05-05)
+## v5.1.2
+
+05 May 2020
 
 Bug Fixes:
 
 - Fix grouping of editables and non-editables requirements
   ([1132](https://github.com/jazzband/pip-tools/pull/1132)). Thanks @richafrank
 
-## 5.1.1 (2020-05-01)
+## v5.1.1
+
+01 May 2020
 
 Bug Fixes:
 
 - Fix a bug where `pip-compile` would generate hashes for `*.egg` files
   ([#1122](https://github.com/jazzband/pip-tools/pull/1122)). Thanks @atugushev
 
-## 5.1.0 (2020-04-27)
+## v5.1.0
+
+27 Apr 2020
 
 Features:
 
 - Show progress bar when downloading packages in `pip-compile` verbose mode
   ([#949](https://github.com/jazzband/pip-tools/pull/949)). Thanks @atugushev
 - `pip-compile` now gets hashes from `PyPI` JSON API (if available) which significantly
   increases the speed of hashes generation
   ([#1109](https://github.com/jazzband/pip-tools/pull/1109)). Thanks @atugushev
 
-## 5.0.0 (2020-04-16)
+## v5.0.0
+
+16 Apr 2020
 
 Backwards Incompatible Changes:
 
 - `pip-tools` now requires `pip>=20.0` (previously `8.1.x` - `20.0.x`). Windows users,
   make sure to use `python -m pip install pip-tools` to avoid issues with `pip`
   self-update from now on ([#1055](https://github.com/jazzband/pip-tools/pull/1055)).
   Thanks @atugushev
@@ -575,28 +666,32 @@
 Improved Documentation:
 
 - Add cross-environment usage documentation to `README`
   ([#651](https://github.com/jazzband/pip-tools/pull/651)). Thanks @vphilippon
 - Add versions compatibility table to `README`
   ([#1106](https://github.com/jazzband/pip-tools/pull/1106)). Thanks @atugushev
 
-## 4.5.1 (2020-02-26)
+## v4.5.1
+
+26 Feb 2020
 
 Bug Fixes:
 
 - Strip line number annotations such as "(line XX)" from file requirements, to prevent
   diff noise when modifying input requirement files
   ([#1075](https://github.com/jazzband/pip-tools/pull/1075)). Thanks @adamchainz
 
 Improved Documentation:
 
 - Updated `README` example outputs for primary requirement annotations
   ([#1072](https://github.com/jazzband/pip-tools/pull/1072)). Thanks @richafrank
 
-## 4.5.0 (2020-02-20)
+## v4.5.0
+
+20 Feb 2020
 
 Features:
 
 - Primary requirements and VCS dependencies are now get annotated with any source `.in`
   files and reverse dependencies
   ([#1058](https://github.com/jazzband/pip-tools/pull/1058)). Thanks @AndydeCleyre
 
@@ -606,15 +701,17 @@
   `pip` ([#1062](https://github.com/jazzband/pip-tools/pull/1062)). Thanks @kammala
 
 Improved Documentation:
 
 - Replace outdated link in the `README` with rationale for pinning
   ([#1053](https://github.com/jazzband/pip-tools/pull/1053)). Thanks @m-aciek
 
-## 4.4.1 (2020-01-31)
+## v4.4.1
+
+31 Jan 2020
 
 Bug Fixes:
 
 - Fix a bug where `pip-compile` would keep outdated options from `requirements.txt`
   ([#1029](https://github.com/jazzband/pip-tools/pull/1029)). Thanks @atugushev
 - Fix the `No handlers could be found for logger "pip.*"` error by configuring the
   builtin logging module ([#1035](https://github.com/jazzband/pip-tools/pull/1035)).
@@ -632,30 +729,34 @@
 - Make the `README` more imperative about installing into a project's virtual
   environment to avoid confusion
   ([#1023](https://github.com/jazzband/pip-tools/pull/1023)). Thanks @tekumara
 - Add a note to the `README` about how to install requirements on different stages to
   [Workflow for layered requirements](https://pip-tools.rtfd.io/en/latest/#workflow-for-layered-requirements)
   section ([#1044](https://github.com/jazzband/pip-tools/pull/1044)). Thanks @hramezani
 
-## 4.4.0 (2020-01-21)
+## v4.4.0
+
+21 Jan 2020
 
 Features:
 
 - Add `--cache-dir` option to `pip-compile`
   ([#1022](https://github.com/jazzband/pip-tools/pull/1022)). Thanks @richafrank
 - Add `pip>=20.0` support ([#1024](https://github.com/jazzband/pip-tools/pull/1024)).
   Thanks @atugushev
 
 Bug Fixes:
 
 - Fix a bug where `pip-compile --upgrade-package` would upgrade those passed packages
   not already required according to the `*.in` and `*.txt` files
   ([#1031](https://github.com/jazzband/pip-tools/pull/1031)). Thanks @AndydeCleyre
 
-## 4.3.0 (2019-11-25)
+## v4.3.0
+
+25 Nov 2019
 
 Features:
 
 - Add Python 3.8 support ([#956](https://github.com/jazzband/pip-tools/pull/956)).
   Thanks @hramezani
 - Unpin commented out unsafe packages in `requirements.txt`
   ([#975](https://github.com/jazzband/pip-tools/pull/975)). Thanks @atugushev
@@ -673,15 +774,17 @@
 
 Improved Documentation:
 
 - Add a note to `README` about `requirements.txt` file, which would possibly interfere
   if you're compiling from scratch
   ([#959](https://github.com/jazzband/pip-tools/pull/959)). Thanks @hramezani
 
-## 4.2.0 (2019-10-12)
+## v4.2.0
+
+12 Oct 2019
 
 Features:
 
 - Add `--ask` option to `pip-sync`
   ([#913](https://github.com/jazzband/pip-tools/pull/913)). Thanks @georgek
 
 Bug Fixes:
@@ -699,57 +802,65 @@
   ([#931](https://github.com/jazzband/pip-tools/pull/931)). Thanks @hramezani
 
 Improved Documentation:
 
 - Add info to `README` about layered requirements files and `-c` flag
   ([#905](https://github.com/jazzband/pip-tools/pull/905)). Thanks @jamescooke
 
-## 4.1.0 (2019-08-26)
+## v4.1.0
+
+26 Aug 2019
 
 Features:
 
 - Add `--no-emit-find-links` option to `pip-compile`
   ([#873](https://github.com/jazzband/pip-tools/pull/873)). Thanks @jacobtolar
 
 Bug Fixes:
 
 - Prevent `--dry-run` log message from being printed with `--quiet` option in
   `pip-compile` ([#861](https://github.com/jazzband/pip-tools/pull/861)). Thanks
   @ddormer
 - Fix resolution of requirements from Git URLs without `-e`
   ([#879](https://github.com/jazzband/pip-tools/pull/879)). Thanks @andersk
 
-## 4.0.0 (2019-07-25)
+## v4.0.0
+
+25 Jul 2019
 
 Backwards Incompatible Changes:
 
 - Drop support for EOL Python 3.4
   ([#803](https://github.com/jazzband/pip-tools/pull/803)). Thanks @auvipy
 
 Bug Fixes:
 
 - Fix `pip>=19.2` compatibility
   ([#857](https://github.com/jazzband/pip-tools/pull/857)). Thanks @atugushev
 
-## 3.9.0 (2019-07-17)
+## v3.9.0
+
+17 Jul 2019
 
 Features:
 
 - Print provenance information when `pip-compile` fails
   ([#837](https://github.com/jazzband/pip-tools/pull/837)). Thanks @jakevdp
 
 Bug Fixes:
 
 - Output all logging to stderr instead of stdout
   ([#834](https://github.com/jazzband/pip-tools/pull/834)). Thanks @georgek
 - Fix output file update with `--dry-run` option in `pip-compile`
   ([#842](https://github.com/jazzband/pip-tools/pull/842)). Thanks @shipmints and
   @atugushev
 
-## 3.8.0 (2019-06-06)
+## v3.8.0
+
+06 Jun 2019
 
 Features:
 
 - Options `--upgrade` and `--upgrade-package` are no longer mutually exclusive
   ([#831](https://github.com/jazzband/pip-tools/pull/831)). Thanks @adamchainz
 
 Bug Fixes:
@@ -759,15 +870,17 @@
 - Fix issues with `UnicodeError` when installing `pip-tools` from source in some systems
   ([#816](https://github.com/jazzband/pip-tools/pull/816)). Thanks @AbdealiJK
 - Respect `--pre` option in the input file
   ([#822](https://github.com/jazzband/pip-tools/pull/822)). Thanks @atugushev
 - Option `--upgrade-package` now works even if the output file does not exist
   ([#831](https://github.com/jazzband/pip-tools/pull/831)). Thanks @adamchainz
 
-## 3.7.0 (2019-05-09)
+## v3.7.0
+
+09 May 2019
 
 Features:
 
 - Show progressbar on generation hashes in `pip-compile` verbose mode
   ([#743](https://github.com/jazzband/pip-tools/pull/743)). Thanks @atugushev
 - Add options `--cert` and `--client-cert` to `pip-sync`
   ([#798](https://github.com/jazzband/pip-tools/pull/798)). Thanks @atugushev
@@ -779,31 +892,37 @@
   Thanks @jcushman, @nim65s and @toejough
 
 Bug Fixes:
 
 - Fix replacing password to asterisks in `pip-compile`
   ([#808](https://github.com/jazzband/pip-tools/pull/808)). Thanks @atugushev
 
-## 3.6.1 (2019-04-24)
+## v3.6.1
+
+24 Apr 2019
 
 Bug Fixes:
 
 - Fix `pip>=19.1` compatibility
   ([#795](https://github.com/jazzband/pip-tools/pull/795)). Thanks @atugushev
 
-## 3.6.0 (2019-04-03)
+## v3.6.0
+
+03 Apr 2019
 
 Features:
 
 - Show less output on `pip-sync` with `--quiet` option
   ([#765](https://github.com/jazzband/pip-tools/pull/765)). Thanks @atugushev
 - Support the flag `--trusted-host` in `pip-sync`
   ([#777](https://github.com/jazzband/pip-tools/pull/777)). Thanks @firebirdberlin
 
-## 3.5.0 (2019-03-13)
+## v3.5.0
+
+13 Mar 2019
 
 Features:
 
 - Show default index url provided by `pip`
   ([#735](https://github.com/jazzband/pip-tools/pull/735)). Thanks @atugushev
 - Add an option to allow enabling/disabling build isolation
   ([#758](https://github.com/jazzband/pip-tools/pull/758)). Thanks @atugushev
@@ -811,43 +930,51 @@
 Bug Fixes:
 
 - Fix the output file for `pip-compile` with an explicit `setup.py` as source file
   ([#731](https://github.com/jazzband/pip-tools/pull/731)). Thanks @atugushev
 - Fix order issue with generated lock file when `hashes` and `markers` are used together
   ([#763](https://github.com/jazzband/pip-tools/pull/763)). Thanks @milind-shakya-sp
 
-## 3.4.0 (2019-02-19)
+## v3.4.0
+
+19 Feb 2019
 
 Features:
 
 - Add option `--quiet` to `pip-compile`
   ([#720](https://github.com/jazzband/pip-tools/pull/720)). Thanks @bendikro
 - Emit the original command to the `pip-compile`'s header
   ([#733](https://github.com/jazzband/pip-tools/pull/733)). Thanks @atugushev
 
 Bug Fixes:
 
 - Fix `pip-sync` to use pip script depending on a python version
   ([#737](https://github.com/jazzband/pip-tools/pull/737)). Thanks @atugushev
 
-## 3.3.2 (2019-01-26)
+## v3.3.2
+
+26 Jan 2019
 
 Bug Fixes:
 
 - Fix `pip-sync` with a temporary requirement file on Windows
   ([#723](https://github.com/jazzband/pip-tools/pull/723)). Thanks @atugushev
 - Fix `pip-sync` to prevent uninstall of stdlib and dev packages
   ([#718](https://github.com/jazzband/pip-tools/pull/718)). Thanks @atugushev
 
-## 3.3.1 (2019-01-24)
+## v3.3.1
+
+24 Jan 2019
 
 - Re-release of 3.3.0 after fixing the deployment pipeline
   ([#716](https://github.com/jazzband/pip-tools/issues/716)). Thanks @atugushev
 
-## 3.3.0 (2019-01-23)
+## v3.3.0
+
+23 Jan 2019
 
 (Unreleased - Deployment pipeline issue, see 3.3.1)
 
 Features:
 
 - Added support of `pip` 19.0 ([#715](https://github.com/jazzband/pip-tools/pull/715)).
   Thanks @atugushev
@@ -855,59 +982,71 @@
   ([#708](https://github.com/jazzband/pip-tools/pull/708)). Thanks @richafrank
 
 Bug Fixes:
 
 - Fix `pip-sync` to check hashes
   ([#706](https://github.com/jazzband/pip-tools/pull/706)). Thanks @atugushev
 
-## 3.2.0 (2018-12-18)
+## v3.2.0
+
+18 Dec 2018
 
 Features:
 
 - Apply version constraints specified with package upgrade option
   (`-P, --upgrade-package`) ([#694](https://github.com/jazzband/pip-tools/pull/694)).
   Thanks @richafrank
 
-## 3.1.0 (2018-10-05)
+## v3.1.0
+
+05 Oct 2018
 
 Features:
 
 - Added support of `pip` 18.1 ([#689](https://github.com/jazzband/pip-tools/pull/689)).
   Thanks @vphilippon
 
-## 3.0.0 (2018-09-24)
+## v3.0.0
+
+24 Sep 2018
 
 Major changes:
 
 - Update `pip-tools` for native `pip` 8, 9, 10 and 18 compatibility, un-vendoring `pip`
   to use the user-installed `pip`
   ([#657](https://github.com/jazzband/pip-tools/pull/657) and
   [#672](https://github.com/jazzband/pip-tools/pull/672)). Thanks to @techalchemy,
   @suutari, @tysonclugg and @vphilippon for contributing on this.
 
 Features:
 
 - Removed the dependency on the external library `first`
   ([#676](https://github.com/jazzband/pip-tools/pull/676)). Thanks @jdufresne
 
-## 2.0.2 (2018-04-28)
+## v2.0.2
+
+28 Apr 2018
 
 Bug Fixes:
 
 - Added clearer error reporting when skipping pre-releases
   ([#655](https://github.com/jazzband/pip-tools/pull/655)). Thanks @WoLpH
 
-## 2.0.1 (2018-04-15)
+## v2.0.1
+
+15 Apr 2018
 
 Bug Fixes:
 
 - Added missing package data from vendored pip, such as missing cacert.pem file. Thanks
   @vphilippon
 
-## 2.0.0 (2018-04-15)
+## v2.0.0
+
+15 Apr 2018
 
 Major changes:
 
 - Vendored `pip` 9.0.3 to keep compatibility for users with `pip` 10.0.0
   ([#644](https://github.com/jazzband/pip-tools/pull/644)). Thanks @vphilippon
 
 Features:
@@ -923,15 +1062,17 @@
 Bug fixes:
 
 - The pip environment markers on top-level requirements in the source file
   (requirements.in) are now properly handled and will only be processed in the right
   environment ([#647](https://github.com/jazzband/pip-tools/pull/647)). Thanks
   @JoergRittinger
 
-## 1.11.0 (2017-11-30)
+## v1.11.0
+
+30 Nov 2017
 
 Features:
 
 - Allow editable packages in requirements.in with `pip-compile --generate-hashes`
   ([#524](https://github.com/jazzband/pip-tools/pull/524)). Thanks @jdufresne
 - Allow for CA bundles with `pip-compile --cert`
   ([#612](https://github.com/jazzband/pip-tools/pull/612)). Thanks @khwilson
@@ -942,33 +1083,39 @@
   ([#614](https://github.com/jazzband/pip-tools/pull/614)). Thanks @vphilippon
 
 Bug Fixes:
 
 - Add `-markerlib` to the list of `PACKAGES_TO_IGNORE` of `pip-sync`
   ([#613](https://github.com/jazzband/pip-tools/pull/613)).
 
-## 1.10.2 (2017-11-22)
+## v1.10.2
+
+22 Nov 2017
 
 Bug Fixes:
 
 - Fixed bug causing dependencies from invalid wheels for the current platform to be
   included ([#571](https://github.com/jazzband/pip-tools/pull/571)).
 - `pip-sync` will respect environment markers in the requirements.txt
   ([600](https://github.com/jazzband/pip-tools/pull/600)). Thanks @hazmat345
 - Converted the ReadMe to have a nice description rendering on PyPI. Thanks @bittner
 
-## 1.10.1 (2017-09-27)
+## v1.10.1
+
+27 Sep 2017
 
 Bug Fixes:
 
 - Fixed bug breaking `pip-sync` on Python 3, raising
   `TypeError: '<' not supported between instances of 'InstallRequirement' and 'InstallRequirement'`
   ([#570](https://github.com/jazzband/pip-tools/pull/570)).
 
-## 1.10.0 (2017-09-27)
+## v1.10.0
+
+27 Sep 2017
 
 Features:
 
 - `--generate-hashes` now generates hashes for all wheels, not only wheels for the
   currently running platform ([#520](https://github.com/jazzband/pip-tools/pull/520)).
   Thanks @jdufresne
 - Added a `-q`/`--quiet` argument to the pip-sync command to reduce log output.
@@ -990,15 +1137,17 @@
 - Fixed bug where the resolver would sometime not stabilize on requirements specifying
   extras. ([#566](https://github.com/jazzband/pip-tools/pull/566)). Thanks @vphilippon
 - Fixed an unicode encoding error when distribution package contains non-ASCII file
   names ([#567](https://github.com/jazzband/pip-tools/pull/567)). Thanks @suutari
 - Fixed package hashing doing unnecessary unpacking
   ([#557](https://github.com/jazzband/pip-tools/pull/557)). Thanks @suutari-ai
 
-## 1.9.0 (2017-04-12)
+## v1.9.0
+
+12 Apr 2017
 
 Features:
 
 - Added ability to read requirements from `setup.py` instead of just `requirements.in`
   ([#418](https://github.com/jazzband/pip-tools/pull/418)). Thanks to @tysonclugg and
   @majuscule.
 - Added a `--max-rounds` argument to the pip-compile command to allow for solving large
@@ -1021,147 +1170,187 @@
   ([#491](https://github.com/jazzband/pip-tools/pull/491)).
 - Fixed the default output file name when the source file has no extension
   ([#488](https://github.com/jazzband/pip-tools/pull/488)). Thanks @vphilippon
 - Fixed crash on editable requirements introduced in 1.8.2.
 - Fixed duplicated --trusted-host, --extra-index-url and --index-url in the generated
   requirements.
 
-## 1.8.2 (2017-03-28)
+## v1.8.2
+
+28 Mar 2017
 
 - Regression fix: editable reqs were losing their dependencies after first round
   ([#476](https://github.com/jazzband/pip-tools/pull/476)) Thanks @mattlong
 - Remove duplicate index urls in generated requirements.txt
   ([#468](https://github.com/jazzband/pip-tools/pull/468)) Thanks @majuscule
 
-## 1.8.1 (2017-03-22)
+## v1.8.1
+
+22 Mar 2017
 
 - Recalculate secondary dependencies between rounds (#378)
 - Calculated dependencies could be left with wrong candidates when toplevel requirements
   happen to be also pinned in sub-dependencies (#450)
 - Fix duplicate entries that could happen in generated requirements.txt (#427)
 - Gracefully report invalid pip version (#457)
 - Fix capitalization in the generated requirements.txt, packages will always be
   lowercased (#452)
 
-## 1.8.0 (2016-11-17)
+## v1.8.0
+
+17 Nov 2016
 
 - Adds support for upgrading individual packages with a new option `--upgrade-package`.
   To upgrade a _specific_ package to the latest or a specific version use
   `--upgrade-package <pkg>`. To upgrade all packages, you can still use
   `pip-compile --upgrade`. (#409)
 - Adds support for pinning dependencies even further by including the hashes found on
   PyPI at compilation time, which will be re-checked when dependencies are installed at
   installation time. This adds protection against packages that are tampered with.
   (#383)
 - Improve support for extras, like `hypothesis[django]`
 - Drop support for pip < 8
 
-## 1.7.1 (2016-10-20)
+## v1.7.1
+
+20 Oct 2016
 
 - Add `--allow-unsafe` option (#377)
 
-## 1.7.0 (2016-07-06)
+## v1.7.0
+
+06 Jul 2016
 
 - Add compatibility with pip >= 8.1.2 (#374) Thanks so much, @jmbowman!
 
-## 1.6.5 (2016-05-11)
+## v1.6.5
+
+11 May 2016
 
 - Add warning that pip >= 8.1.2 is not supported until 1.7.x is out
 
-## 1.6.4 (2016-05-03)
+## v1.6.4
+
+03 May 2016
 
 - Incorporate fix for atomic file saving behaviour on the Windows platform (see #351)
 
-## 1.6.3 (2016-05-02)
+## v1.6.3
+
+02 May 2016
 
 - PyPI won't let me upload 1.6.2
 
-## 1.6.2 (2016-05-02)
+## v1.6.2
+
+02 May 2016
 
 - Respect pip configuration from pip.{ini,conf}
 - Fixes for atomic-saving of output files on Windows (see #351)
 
-## 1.6.1 (2016-04-06)
+## v1.6.1
+
+06 Apr 2016
 
 Minor changes:
 
 - pip-sync now supports being invoked from within and outside an activated virtualenv
   (see #317)
 - pip-compile: support -U as a shorthand for --upgrade
 - pip-compile: support pip's --no-binary and --binary-only flags
 
 Fixes:
 
 - Change header format of output files to mention all input files
 
-## 1.6 (2016-02-05)
+## v1.6
+
+05 Feb 2016
 
 Major change:
 
 - pip-compile will by default try to fulfill package specs by looking at a previously
   compiled output file first, before checking PyPI. This means pip-compile will only
   update the requirements.txt when it absolutely has to. To get the old behaviour
   (picking the latest version of all packages from PyPI), use the new `--upgrade`
   option.
 
 Minor changes:
 
 - Bugfix where pip-compile would lose "via" info when on pip 8 (see #313)
 - Ensure cache dir exists (see #315)
 
-## 1.5 (2016-01-23)
+## v1.5
+
+23 Jan 2016
 
 - Add support for pip >= 8
 - Drop support for pip < 7
 - Fix bug where `pip-sync` fails to uninstall packages if you're using the `--no-index`
   (or other) flags
 
-## 1.4.5 (2016-01-20)
+## v1.4.5
+
+20 Jan 2016
 
 - Add `--no-index` flag to `pip-compile` to avoid emitting `--index-url` into the output
   (useful if you have configured a different index in your global ~/.pip/pip.conf, for
   example)
 - Fix: ignore stdlib backport packages, like `argparse`, when listing which packages
   will be installed/uninstalled (#286)
 - Fix pip-sync failed uninstalling packages when using `--find-links` (#298)
 - Explicitly error when pip-tools is used with pip 8.0+ (for now)
 
-## 1.4.4 (2016-01-11)
+## v1.4.4
+
+11 Jan 2016
 
 - Fix: unintended change in behaviour where packages installed by `pip-sync` could
   accidentally get upgraded under certain conditions, even though the requirements.txt
   would dictate otherwise (see #290)
 
-## 1.4.3 (2016-01-06)
+## v1.4.3
+
+06 Jan 2016
 
 - Fix: add `--index-url` and `--extra-index-url` options to `pip-sync`
 - Fix: always install using `--upgrade` flag when running `pip-sync`
 
-## 1.4.2 (2015-12-13)
+## v1.4.2
+
+13 Dec 2015
 
 - Fix bug where umask was ignored when writing requirement files (#268)
 
-## 1.4.1 (2015-12-13)
+## v1.4.1
+
+13 Dec 2015
 
 - Fix bug where successive invocations of pip-sync with editables kept
   uninstalling/installing them (fixes #270)
 
-## 1.4.0 (2015-12-13)
+## v1.4.0
+
+13 Dec 2015
 
 - Add command line option -f / --find-links
 - Add command line option --no-index
 - Add command line alias -n (for --dry-run)
 - Fix a unicode issue
 
-## 1.3.0 (2015-12-08)
+## v1.3.0
+
+08 Dec 2015
 
 - Support multiple requirement files to pip-compile
 - Support requirements from stdin for pip-compile
 - Support --output-file option on pip-compile, to redirect output to a file (or stdout)
 
-## 1.2.0 (2015-11-30)
+## v1.2.0
+
+30 Nov 2015
 
 - Add CHANGELOG :)
 - Support pip-sync'ing editable requirements
 - Support extras properly (i.e. package[foo] syntax)
 
 (Anything before 1.2.0 was not recorded.)
```

### Comparing `pip-tools-7.1.0/CODE_OF_CONDUCT.md` & `pip-tools-7.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/CONTRIBUTING.md` & `pip-tools-7.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/LICENSE` & `pip-tools-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/PKG-INFO` & `pip-tools-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.1.0
+Version: 7.2.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -131,15 +131,14 @@
 [project]
 name = "my-cool-django-app"
 version = "42"
 dependencies = ["django"]
 
 [project.optional-dependencies]
 dev = ["pytest"]
-
 ```
 
 You can produce your pin files as easily as:
 
 ```console
 $ pip-compile -o requirements.txt pyproject.toml
 #
@@ -323,26 +322,34 @@
 writing them to a configuration file in the same directory as your requirements
 input files (or the current working directory if piping input from stdin).
 By default, both `pip-compile` and `pip-sync` will look first
 for a `.pip-tools.toml` file and then in your `pyproject.toml`. You can
 also specify an alternate TOML configuration file with the `--config` option.
 
 For example, to by default generate `pip` hashes in the resulting
-requirements file output, you can specify in a configuration file
+requirements file output, you can specify in a configuration file:
 
 ```toml
 [tool.pip-tools]
 generate-hashes = true
-
 ```
 
 Options to `pip-compile` and `pip-sync` that may be used more than once
 must be defined as lists in a configuration file, even if they only have one
 value.
 
+`pip-tools` supports default values for [all valid command-line flags](/cli/index.md)
+of its subcommands. Configuration keys may contain underscores instead of dashes,
+so the above could also be specified in this format:
+
+```toml
+[tool.pip-tools]
+generate_hashes = true
+```
+
 You might be wrapping the `pip-compile` command in another script. To avoid
 confusing consumers of your custom script you can override the update command
 generated at the top of requirements files by setting the
 `CUSTOM_COMPILE_COMMAND` environment variable.
 
 ```console
 $ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
@@ -448,37 +455,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.1.0/README.md` & `pip-tools-7.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 [project]
 name = "my-cool-django-app"
 version = "42"
 dependencies = ["django"]
 
 [project.optional-dependencies]
 dev = ["pytest"]
-
 ```
 
 You can produce your pin files as easily as:
 
 ```console
 $ pip-compile -o requirements.txt pyproject.toml
 #
@@ -286,26 +285,34 @@
 writing them to a configuration file in the same directory as your requirements
 input files (or the current working directory if piping input from stdin).
 By default, both `pip-compile` and `pip-sync` will look first
 for a `.pip-tools.toml` file and then in your `pyproject.toml`. You can
 also specify an alternate TOML configuration file with the `--config` option.
 
 For example, to by default generate `pip` hashes in the resulting
-requirements file output, you can specify in a configuration file
+requirements file output, you can specify in a configuration file:
 
 ```toml
 [tool.pip-tools]
 generate-hashes = true
-
 ```
 
 Options to `pip-compile` and `pip-sync` that may be used more than once
 must be defined as lists in a configuration file, even if they only have one
 value.
 
+`pip-tools` supports default values for [all valid command-line flags](/cli/index.md)
+of its subcommands. Configuration keys may contain underscores instead of dashes,
+so the above could also be specified in this format:
+
+```toml
+[tool.pip-tools]
+generate_hashes = true
+```
+
 You might be wrapping the `pip-compile` command in another script. To avoid
 confusing consumers of your custom script you can override the update command
 generated at the top of requirements files by setting the
 `CUSTOM_COMPILE_COMMAND` environment variable.
 
 ```console
 $ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
@@ -411,37 +418,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.1.0/docs/conf.py` & `pip-tools-7.2.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 logger.info(bold("%s release: %s"), project, release)
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["myst_parser"]
+extensions = ["myst_parser", "sphinxcontrib.programoutput"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `pip-tools-7.1.0/img/pip-tools-overview.svg` & `pip-tools-7.2.0/img/pip-tools-overview.svg`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/pip_tools.egg-info/PKG-INFO` & `pip-tools-7.2.0/pip_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.1.0
+Version: 7.2.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -131,15 +131,14 @@
 [project]
 name = "my-cool-django-app"
 version = "42"
 dependencies = ["django"]
 
 [project.optional-dependencies]
 dev = ["pytest"]
-
 ```
 
 You can produce your pin files as easily as:
 
 ```console
 $ pip-compile -o requirements.txt pyproject.toml
 #
@@ -323,26 +322,34 @@
 writing them to a configuration file in the same directory as your requirements
 input files (or the current working directory if piping input from stdin).
 By default, both `pip-compile` and `pip-sync` will look first
 for a `.pip-tools.toml` file and then in your `pyproject.toml`. You can
 also specify an alternate TOML configuration file with the `--config` option.
 
 For example, to by default generate `pip` hashes in the resulting
-requirements file output, you can specify in a configuration file
+requirements file output, you can specify in a configuration file:
 
 ```toml
 [tool.pip-tools]
 generate-hashes = true
-
 ```
 
 Options to `pip-compile` and `pip-sync` that may be used more than once
 must be defined as lists in a configuration file, even if they only have one
 value.
 
+`pip-tools` supports default values for [all valid command-line flags](/cli/index.md)
+of its subcommands. Configuration keys may contain underscores instead of dashes,
+so the above could also be specified in this format:
+
+```toml
+[tool.pip-tools]
+generate_hashes = true
+```
+
 You might be wrapping the `pip-compile` command in another script. To avoid
 confusing consumers of your custom script you can override the update command
 generated at the top of requirements files by setting the
 `CUSTOM_COMPILE_COMMAND` environment variable.
 
 ```console
 $ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
@@ -448,37 +455,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.1.0
+    rev: 7.2.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.1.0/pip_tools.egg-info/SOURCES.txt` & `pip-tools-7.2.0/pip_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 .github/workflows/reusable-qa.yml
 docs/.gitignore
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/requirements.txt
+docs/cli/index.md
+docs/cli/pip-compile.md
+docs/cli/pip-sync.md
 examples/django.in
 examples/flask.in
 examples/hypothesis.in
 examples/protection.in
 examples/sentry.in
 img/pip-tools-overview.svg
 pip_tools.egg-info/PKG-INFO
```

### Comparing `pip-tools-7.1.0/piptools/_compat/pip_compat.py` & `pip-tools-7.2.0/piptools/_compat/pip_compat.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/cache.py` & `pip-tools-7.2.0/piptools/cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/exceptions.py` & `pip-tools-7.2.0/piptools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/logging.py` & `pip-tools-7.2.0/piptools/logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/repositories/base.py` & `pip-tools-7.2.0/piptools/repositories/base.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/repositories/local.py` & `pip-tools-7.2.0/piptools/repositories/local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/repositories/pypi.py` & `pip-tools-7.2.0/piptools/repositories/pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/resolver.py` & `pip-tools-7.2.0/piptools/resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/scripts/compile.py` & `pip-tools-7.2.0/piptools/scripts/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,28 @@
 @click.option(
     "--no-config",
     is_flag=True,
     default=False,
     help="Do not read any config file.",
     is_eager=True,
 )
+@click.option(
+    "-c",
+    "--constraint",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        allow_dash=False,
+        path_type=str,
+    ),
+    multiple=True,
+    help="Constrain versions using the given constraints file; may be used more than once.",
+)
 def cli(
     ctx: click.Context,
     verbose: int,
     quiet: int,
     dry_run: bool,
     pre: bool,
     rebuild: bool,
@@ -362,14 +376,15 @@
     pip_args_str: str | None,
     resolver_name: str,
     emit_index_url: bool,
     emit_options: bool,
     unsafe_package: tuple[str, ...],
     config: Path | None,
     no_config: bool,
+    constraint: tuple[str, ...],
 ) -> None:
     """
     Compiles requirements.txt from requirements.in, pyproject.toml, setup.cfg,
     or setup.py specs.
     """
     log.verbosity = verbose - quiet
 
@@ -557,14 +572,26 @@
                     src_file,
                     finder=repository.finder,
                     session=repository.session,
                     options=repository.options,
                 )
             )
 
+    # Parse all constraints from `--constraint` files
+    for filename in constraint:
+        constraints.extend(
+            parse_requirements(
+                filename,
+                constraint=True,
+                finder=repository.finder,
+                options=repository.options,
+                session=repository.session,
+            )
+        )
+
     if upgrade_packages:
         constraints_file = tempfile.NamedTemporaryFile(mode="wt", delete=False)
         constraints_file.write("\n".join(upgrade_packages))
         constraints_file.flush()
         try:
             reqs = list(
                 parse_requirements(
```

### Comparing `pip-tools-7.1.0/piptools/scripts/sync.py` & `pip-tools-7.2.0/piptools/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/subprocess_utils.py` & `pip-tools-7.2.0/piptools/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/sync.py` & `pip-tools-7.2.0/piptools/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/piptools/utils.py` & `pip-tools-7.2.0/piptools/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     "--upgrade-package",
     "--verbose",
     "--cache-dir",
     "--no-reuse-hashes",
     "--no-config",
 }
 
+# Set of option that are only negative, i.e. --no-<option>
+ONLY_NEGATIVE_OPTIONS = {"--no-index"}
+
 
 def key_from_ireq(ireq: InstallRequirement) -> str:
     """Get a standardized key for an InstallRequirement."""
     if ireq.req is None and ireq.link is not None:
         return str(ireq.link)
     else:
         return key_from_req(ireq.req)
@@ -556,15 +559,15 @@
     if value is None:
         config_file = select_config_file(ctx.params.get("src_files", ()))
         if config_file is None:
             return None
     else:
         config_file = Path(value)
 
-    config = parse_config_file(config_file)
+    config = parse_config_file(ctx, config_file)
     if config:
         _validate_config(ctx, config)
         _assign_config_to_cli_context(ctx, config)
 
     return config_file
 
 
@@ -584,41 +587,58 @@
 ) -> None:
     """
     Validate parsed config against click command params.
 
     :raises click.NoSuchOption: if config contains unknown keys.
     :raises click.BadOptionUsage: if config contains invalid values.
     """
-    cli_params = {
-        param.name: param
-        for param in click_context.command.params
-        if param.name is not None
+    from piptools.scripts.compile import cli as compile_cli
+    from piptools.scripts.sync import cli as sync_cli
+
+    compile_cli_params = {
+        param.name: param for param in compile_cli.params if param.name is not None
+    }
+
+    sync_cli_params = {
+        param.name: param for param in sync_cli.params if param.name is not None
     }
 
+    all_keys = set(compile_cli_params) | set(sync_cli_params)
+
     for key, value in config.items():
-        # Validate unknown keys
-        if key not in cli_params:
-            possibilities = difflib.get_close_matches(key, cli_params.keys())
+        # Validate unknown keys in both compile and sync
+        if key not in all_keys:
+            possibilities = difflib.get_close_matches(key, all_keys)
             raise click.NoSuchOption(
                 option_name=key,
                 message=f"No such config key {key!r}.",
                 possibilities=possibilities,
                 ctx=click_context,
             )
 
-        # Validate invalid values
-        param = cli_params[key]
-        try:
-            param.type.convert(value=value, param=param, ctx=click_context)
-        except Exception as e:
-            raise click.BadOptionUsage(
-                option_name=key,
-                message=f"Invalid value for config key {key!r}: {value!r}.",
-                ctx=click_context,
-            ) from e
+        # Get all params associated with this key in both compile and sync
+        associated_params = (
+            cli_params[key]
+            for cli_params in (compile_cli_params, sync_cli_params)
+            if key in cli_params
+        )
+
+        # Validate value against types of all associated params
+        for param in associated_params:
+            try:
+                param.type_cast_value(value=value, ctx=click_context)
+            except Exception as e:
+                raise click.BadOptionUsage(
+                    option_name=key,
+                    message=(
+                        f"Invalid value for config key {key!r}: {value!r}.{os.linesep}"
+                        f"Details: {e}"
+                    ),
+                    ctx=click_context,
+                ) from e
 
 
 def select_config_file(src_files: tuple[str, ...]) -> Path | None:
     """
     Returns the config file to use for defaults given ``src_files`` provided.
     """
     # NOTE: If no src_files were specified, consider the current directory the
@@ -645,47 +665,27 @@
     return (
         config_file_path.relative_to(working_directory)
         if is_path_relative_to(config_file_path, working_directory)
         else config_file_path
     )
 
 
-# Some of the defined click options have different `dest` values than the defaults
-NON_STANDARD_OPTION_DEST_MAP: dict[str, str] = {
-    "extra": "extras",
-    "upgrade_package": "upgrade_packages",
-    "resolver": "resolver_name",
-    "user": "user_only",
-    "pip_args": "pip_args_str",
-}
-
-
-def get_click_dest_for_option(option_name: str) -> str:
-    """
-    Returns the click ``dest`` value for the given option name.
-    """
-    # Format the keys properly
-    option_name = option_name.lstrip("-").replace("-", "_").lower()
-    # Some options have dest values that are overrides from the click generated default
-    option_name = NON_STANDARD_OPTION_DEST_MAP.get(option_name, option_name)
-    return option_name
-
-
-# Ensure that any default overrides for these click options are lists, supporting multiple values
-MULTIPLE_VALUE_OPTIONS = [
-    "extras",
-    "upgrade_packages",
-    "unsafe_package",
-    "find_links",
-    "extra_index_url",
-    "trusted_host",
-]
+def get_cli_options(ctx: click.Context) -> dict[str, click.Parameter]:
+    cli_opts = {
+        opt: option
+        for option in ctx.command.params
+        for opt in itertools.chain(option.opts, option.secondary_opts)
+        if opt.startswith("--") and option.name is not None
+    }
+    return cli_opts
 
 
-def parse_config_file(config_file: Path) -> dict[str, Any]:
+def parse_config_file(
+    click_context: click.Context, config_file: Path
+) -> dict[str, Any]:
     try:
         config = tomllib.loads(config_file.read_text(encoding="utf-8"))
     except OSError as os_err:
         raise click.FileError(
             filename=str(config_file),
             hint=f"Could not read '{config_file !s}': {os_err !s}",
         )
@@ -693,27 +693,61 @@
         raise click.FileError(
             filename=str(config_file),
             hint=f"Could not parse '{config_file !s}': {value_err !s}",
         )
 
     # In a TOML file, we expect the config to be under `[tool.pip-tools]`
     piptools_config: dict[str, Any] = config.get("tool", {}).get("pip-tools", {})
-    piptools_config = {
-        get_click_dest_for_option(k): v for k, v in piptools_config.items()
-    }
-    # Any option with multiple values needs to be a list in the pyproject.toml
-    for mv_option in MULTIPLE_VALUE_OPTIONS:
-        if not isinstance(piptools_config.get(mv_option), (list, type(None))):
-            original_option = mv_option.replace("_", "-")
-            raise click.BadOptionUsage(
-                original_option, f"Config key '{original_option}' must be a list"
-            )
+    piptools_config = _normalize_keys_in_config(piptools_config)
+    piptools_config = _invert_negative_bool_options_in_config(
+        ctx=click_context,
+        config=piptools_config,
+    )
     return piptools_config
 
 
+def _normalize_keys_in_config(config: dict[str, Any]) -> dict[str, Any]:
+    return {_normalize_config_key(key): value for key, value in config.items()}
+
+
+def _invert_negative_bool_options_in_config(
+    ctx: click.Context, config: dict[str, Any]
+) -> dict[str, Any]:
+    new_config = {}
+    cli_opts = get_cli_options(ctx)
+
+    for key, value in config.items():
+        # Transform config key to its equivalent in the CLI
+        long_option = _convert_to_long_option(key)
+        new_key = cli_opts[long_option].name if long_option in cli_opts else key
+        assert new_key is not None
+
+        # Invert negative boolean according to the CLI
+        new_value = (
+            not value
+            if long_option.startswith("--no-")
+            and long_option not in ONLY_NEGATIVE_OPTIONS
+            and isinstance(value, bool)
+            else value
+        )
+        new_config[new_key] = new_value
+
+    return new_config
+
+
+def _normalize_config_key(key: str) -> str:
+    """Transform given ``some-key`` into ``some_key``."""
+    return key.lstrip("-").replace("-", "_").lower()
+
+
+def _convert_to_long_option(key: str) -> str:
+    """Transform given ``some-key`` into ``--some-key``."""
+    return "--" + key.lstrip("-").replace("_", "-").lower()
+
+
 def is_path_relative_to(path1: Path, path2: Path) -> bool:
     """Return True if ``path1`` is relative to ``path2``."""
     # TODO: remove this function in favor of Path.is_relative_to()
     #       when we drop support for Python 3.8
     try:
         path1.relative_to(path2)
     except ValueError:
```

### Comparing `pip-tools-7.1.0/piptools/writer.py` & `pip-tools-7.2.0/piptools/writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/pyproject.toml` & `pip-tools-7.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/conftest.py` & `pip-tools-7.2.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import sys
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
 from textwrap import dedent
-from typing import Any
+from typing import Any, cast
 
 import pytest
 import tomli_w
 from click.testing import CliRunner
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
@@ -230,15 +230,15 @@
     with cli_runner.isolated_filesystem():
         yield cli_runner
 
 
 @pytest.fixture
 def tmpdir_cwd(tmpdir):
     with tmpdir.as_cwd():
-        yield tmpdir
+        yield Path(tmpdir)
 
 
 @pytest.fixture
 def make_pip_conf(tmpdir, monkeypatch):
     created_paths = []
 
     def _make_pip_conf(content):
@@ -451,16 +451,16 @@
     value, returning a ``pathlib.Path`` to the config file.
     """
 
     def _maker(
         pyproject_param: str, new_default: Any, config_file_name: str = CONFIG_FILE_NAME
     ) -> Path:
         # Make a config file with this one config default override
-        config_path = Path(tmpdir_cwd) / pyproject_param
+        config_path = tmpdir_cwd / pyproject_param
         config_file = config_path / config_file_name
         config_path.mkdir(exist_ok=True)
 
         config_to_dump = {"tool": {"pip-tools": {pyproject_param: new_default}}}
         config_file.write_text(tomli_w.dumps(config_to_dump))
-        return config_file.relative_to(tmpdir_cwd)
+        return cast(Path, config_file.relative_to(tmpdir_cwd))
 
     return _maker
```

### Comparing `pip-tools-7.1.0/tests/test_cache.py` & `pip-tools-7.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_cli_compile.py` & `pip-tools-7.2.0/tests/test_cli_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -3013,7 +3013,90 @@
     req_in = tmp_path / "requirements.in"
     req_in.touch()
 
     out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
 
     assert out.exit_code == 2
     assert "Invalid value for config key 'dry_run': ['invalid', 'value']" in out.stderr
+
+
+@pytest.mark.parametrize("option", ("-c", "--constraint"))
+def test_constraint_option(pip_conf, runner, tmpdir_cwd, make_config_file, option):
+    req_in = tmpdir_cwd / "requirements.in"
+    req_in.write_text("small-fake-a")
+
+    constraints_txt = tmpdir_cwd / "constraints.txt"
+    constraints_txt.write_text("small-fake-a==0.1")
+
+    out = runner.invoke(
+        cli,
+        [
+            req_in.name,
+            option,
+            constraints_txt.name,
+            "--output-file",
+            "-",
+            "--no-header",
+            "--no-emit-options",
+        ],
+    )
+
+    assert out.exit_code == 0
+    assert out.stdout == dedent(
+        """\
+        small-fake-a==0.1
+            # via
+            #   -c constraints.txt
+            #   -r requirements.in
+        """
+    )
+
+
+def test_allow_in_config_pip_sync_option(pip_conf, runner, tmp_path, make_config_file):
+    config_file = make_config_file("--ask", True)  # pip-sync's option
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(
+        cli, [req_in.as_posix(), "--verbose", "--config", config_file.as_posix()]
+    )
+
+    assert out.exit_code == 0
+    assert "Using pip-tools configuration defaults found" in out.stderr
+
+
+def test_cli_boolean_flag_config_option_has_valid_context(
+    pip_conf, runner, tmp_path, make_config_file
+):
+    config_file = make_config_file("no-annotate", True)
+
+    req_in = tmp_path / "requirements.in"
+    req_in.write_text("small-fake-a==0.1")
+    out = runner.invoke(
+        cli,
+        [
+            req_in.as_posix(),
+            "--config",
+            config_file.as_posix(),
+            "--no-emit-options",
+            "--no-header",
+            "--output-file",
+            "-",
+        ],
+    )
+    assert out.exit_code == 0
+    assert out.stdout == "small-fake-a==0.1\n"
+
+
+def test_invalid_cli_boolean_flag_config_option_captured(
+    pip_conf, runner, tmp_path, make_config_file
+):
+    config_file = make_config_file("no-annnotate", True)
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
+
+    assert out.exit_code == 2
+    assert "No such config key 'no_annnotate'." in out.stderr
```

### Comparing `pip-tools-7.1.0/tests/test_cli_sync.py` & `pip-tools-7.2.0/tests/test_cli_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,7 +420,20 @@
     with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
         reqs_txt.write("six==1.10.0")
 
     out = runner.invoke(cli, ["--config", config_file.as_posix()])
 
     assert out.exit_code == 2
     assert "Invalid value for config key 'dry_run': ['invalid', 'value']" in out.stderr
+
+
+@mock.patch("piptools.sync.run")
+def test_allow_in_config_pip_compile_option(run, runner, tmp_path, make_config_file):
+    config_file = make_config_file("generate-hashes", True)  # pip-compile's option
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli, ["--verbose", "--config", config_file.as_posix()])
+
+    assert out.exit_code == 0
+    assert "Using pip-tools configuration defaults found" in out.stderr
```

### Comparing `pip-tools-7.1.0/tests/test_data/fake-index.json` & `pip-tools-7.2.0/tests/test_data/fake-index.json`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/setup.py` & `pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/setup.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_fake_index.py` & `pip-tools-7.2.0/tests/test_fake_index.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_logging.py` & `pip-tools-7.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_minimal_upgrade.py` & `pip-tools-7.2.0/tests/test_minimal_upgrade.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_repository_local.py` & `pip-tools-7.2.0/tests/test_repository_local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_repository_pypi.py` & `pip-tools-7.2.0/tests/test_repository_pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_resolver.py` & `pip-tools-7.2.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_sync.py` & `pip-tools-7.2.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tests/test_utils.py` & `pip-tools-7.2.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from piptools.utils import (
     as_tuple,
     dedup,
     drop_extras,
     flat_map,
     format_requirement,
     format_specifier,
-    get_click_dest_for_option,
+    get_cli_options,
     get_compile_command,
     get_hashes_from_ireq,
     get_pip_version_for_python_executable,
     get_sys_path_for_python_executable,
     is_pinned_requirement,
     is_url_requirement,
     key_from_ireq,
@@ -581,15 +581,15 @@
         ("verbose", True),
         ("quiet", True),
         ("cert", "changed"),
         ("client-cert", "changed"),
         ("pip-args", "changed"),
         ("pre", True),
         ("rebuild", True),
-        ("extras", ["changed"]),
+        ("extra", ["changed"]),
         ("all-extras", True),
         ("index-url", "changed"),
         ("header", False),
         ("emit-trusted-host", False),
         ("annotate", False),
         ("annotation-style", "line"),
         ("upgrade", True),
@@ -611,37 +611,43 @@
     ),
 )
 def test_callback_config_file_defaults(pyproject_param, new_default, make_config_file):
     config_file = make_config_file(pyproject_param, new_default)
     # Create a "compile" run example pointing to the config file
     ctx = Context(compile_cli)
     ctx.params["src_files"] = (str(config_file),)
+    cli_opts = get_cli_options(ctx)
     found_config_file = override_defaults_from_config_file(ctx, "config", None)
     assert found_config_file == config_file
     # Make sure the default has been updated
-    lookup_param = get_click_dest_for_option(pyproject_param)
+    lookup_param = cli_opts["--" + pyproject_param].name
     assert ctx.default_map[lookup_param] == new_default
 
 
 @pytest.mark.parametrize(
-    "mv_option",
+    ("param", "value"),
     (
-        "extra",
-        "upgrade-package",
-        "unsafe-package",
-        "find-links",
-        "extra-index-url",
-        "trusted-host",
+        ("extra", "not-a-list"),
+        ("upgrade_package", "not-a-list"),
+        ("unsafe_package", "not-a-list"),
+        ("find_links", "not-a-list"),
+        ("extra_index_url", "not-a-list"),
+        ("trusted_host", "not-a-list"),
+        ("annotate", "not-a-bool"),
+        ("max_rounds", "not-an-int"),
+        ("constraint", "not-an-list"),
     ),
 )
-def test_callback_config_file_defaults_multi_value_options(mv_option, make_config_file):
-    config_file = make_config_file(mv_option, "not-a-list")
+def test_callback_config_file_defaults_multi_validate_value(
+    param, value, make_config_file
+):
+    config_file = make_config_file(param, value)
     ctx = Context(compile_cli)
     ctx.params["src_files"] = (str(config_file),)
-    with pytest.raises(BadOptionUsage, match="must be a list"):
+    with pytest.raises(BadOptionUsage, match="Invalid value for config key"):
         override_defaults_from_config_file(ctx, "config", None)
 
 
 def test_callback_config_file_defaults_bad_toml(make_config_file):
     config_file = make_config_file("verbose", True)
     # Simple means of making invalid TOML: have duplicate keys
     with Path(config_file).open("r+") as fs:
@@ -657,16 +663,15 @@
     piptools_config_file = make_config_file("newline", "LF")
     project_config_file = make_config_file("newline", "CRLF", "pyproject.toml")
     ctx = Context(compile_cli)
     ctx.params["src_files"] = (str(project_config_file),)
     found_config_file = override_defaults_from_config_file(ctx, "config", None)
     # The pip-tools specific config file should take precedence over pyproject.toml
     assert found_config_file == piptools_config_file
-    lookup_param = get_click_dest_for_option("newline")
-    assert ctx.default_map[lookup_param] == "LF"
+    assert ctx.default_map["newline"] == "LF"
 
 
 def test_callback_config_file_defaults_unreadable_toml(make_config_file):
     ctx = Context(compile_cli)
     with pytest.raises(FileError, match="Could not read "):
         override_defaults_from_config_file(
             ctx,
```

### Comparing `pip-tools-7.1.0/tests/test_writer.py` & `pip-tools-7.2.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.1.0/tox.ini` & `pip-tools-7.2.0/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
   {envpython} -m sphinx_autobuild \
     -j auto \
     -b html \
     -n \
     -W \
     -d "{temp_dir}/.doctrees" \
     . \
-    --watch ../README.rst \
+    --watch ../README.md \
     --watch ../CHANGELOG.md \
     "{envdir}/docs_out"
 
 changedir = {[testenv:build-docs]changedir}
 isolated_build = {[testenv:build-docs]isolated_build}
 passenv = {[testenv:build-docs]passenv}
 skip_install = {[testenv:build-docs]skip_install}
```

