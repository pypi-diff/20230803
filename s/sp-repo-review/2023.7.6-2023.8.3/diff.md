# Comparing `tmp/sp_repo_review-2023.7.6.tar.gz` & `tmp/sp_repo_review-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jul  6 19:13:47 2023, max compression
+gzip compressed data, last modified: Thu Aug  3 21:15:25 2023, max compression
```

## Comparing `sp_repo_review-2023.7.6.tar` & `sp_repo_review-2023.8.3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.git_archival.txt
--rw-r--r--   0        0        0       45 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitattributes
--rw-r--r--   0        0        0     2547 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      179 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      702 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.readthedocs.yaml
--rw-r--r--   0        0        0        6 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.ruby-version
--rw-r--r--   0        0        0     1042 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile
--rw-r--r--   0        0        0     2737 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile.lock
--rw-r--r--   0        0        0    18677 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/README.md
--rw-r--r--   0        0        0     1057 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/_config.yml
--rw-r--r--   0        0        0      763 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/action.yml
--rw-r--r--   0        0        0      877 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/cookiecutter.json
--rw-r--r--   0        0        0     2120 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/copier.yml
--rw-r--r--   0        0        0    11663 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/noxfile.py
--rw-r--r--   0        0        0      640 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/dependabot.yml
--rw-r--r--   0        0        0      825 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/bump.yml
--rw-r--r--   0        0        0      726 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2109 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5295 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0     1262 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/LICENSE
--rw-r--r--   0        0        0      829 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/README.md
--rw-r--r--   0        0        0     2180 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      545 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0     2753 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/pyproject.md
--rw-r--r--   0        0        0      145 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/toc.html
--rw-r--r--   0        0        0      435 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/details.rb
--rw-r--r--   0        0        0      512 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/repo_review.rb
--rw-r--r--   0        0        0     1541 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/tabs.rb
--rw-r--r--   0        0        0       22 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2611 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    10211 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     3322 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/index.md
--rw-r--r--   0        0        0     5085 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0     9872 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/docs.md
--rw-r--r--   0        0        0    22870 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     7836 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8067 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2956 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/index.md
--rw-r--r--   0        0        0    10386 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    18232 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9364 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_compiled.md
--rw-r--r--   0        0        0     6194 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14312 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      947 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28349 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/style.md
--rw-r--r--   0        0        0     9121 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     4260 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/backports.md
--rw-r--r--   0        0        0     7171 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0     3119 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/exports.md
--rw-r--r--   0        0        0      738 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11217 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4526 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0     4795 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md
--rw-r--r--   0        0        0      998 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2578 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3300 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4645 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0      615 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/cog_helpers.py
--rw-r--r--   0        0        0      699 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/extensions.py
--rw-r--r--   0        0        0      246 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      166 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0      822 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      152 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2849 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5018 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3154 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2565 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/readthedocs.py
--rw-r--r--   0        0        0     3002 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_package.py
--rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2901 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0     1689 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0     2928 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8661 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     3987 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.__ci == 'gitlab' %}.gitlab-ci.yml{% endif %}
--rw-r--r--   0        0        0      169 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
--rw-r--r--   0        0        0     2197 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
--rw-r--r--   0        0        0      691 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
--rw-r--r--   0        0        0      915 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
--rw-r--r--   0        0        0      727 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
--rw-r--r--   0        0        0      376 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
--rw-r--r--   0        0        0      266 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
--rw-r--r--   0        0        0    11380 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1559 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1089 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}
--rw-r--r--   0        0        0      102 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
--rw-r--r--   0        0        0     2528 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/dependabot.yml
--rwxr-xr-x   0        0        0      978 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
--rw-r--r--   0        0        0      668 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3424 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}
--rw-r--r--   0        0        0      934 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0      632 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
--rw-r--r--   0        0        0      562 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
--rw-r--r--   0        0        0      422 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
--rw-r--r--   0        0        0      117 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
--rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
--rw-r--r--   0        0        0      215 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      378 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0      190 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
--rw-r--r--   0        0        0     2249 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitignore
--rw-r--r--   0        0        0     1525 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/LICENSE
--rw-r--r--   0        0        0     5530 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/pyproject.toml
--rw-r--r--   0        0        0    10037 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.git_archival.txt
+-rw-r--r--   0        0        0       45 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.gitattributes
+-rw-r--r--   0        0        0     2600 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      702 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.readthedocs.yaml
+-rw-r--r--   0        0        0        6 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.ruby-version
+-rw-r--r--   0        0        0     1182 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/Gemfile
+-rw-r--r--   0        0        0     3683 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/Gemfile.lock
+-rw-r--r--   0        0        0    18540 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/README.md
+-rw-r--r--   0        0        0     1020 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/_config.yml
+-rw-r--r--   0        0        0      763 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/action.yml
+-rw-r--r--   0        0        0     1998 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/cookiecutter.json
+-rw-r--r--   0        0        0     2634 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/copier.yml
+-rw-r--r--   0        0        0    11702 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/noxfile.py
+-rw-r--r--   0        0        0      527 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      825 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      726 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2109 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5010 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0     1262 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/LICENSE
+-rw-r--r--   0        0        0      829 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      547 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0     2753 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_includes/pyproject.md
+-rw-r--r--   0        0        0      145 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_includes/toc.html
+-rw-r--r--   0        0        0      435 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_plugins/details.rb
+-rw-r--r--   0        0        0      512 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_plugins/repo_review.rb
+-rw-r--r--   0        0        0     1541 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_plugins/tabs.rb
+-rw-r--r--   0        0        0       22 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2627 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    11110 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     4123 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/index.md
+-rw-r--r--   0        0        0     5085 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0    11700 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/docs.md
+-rw-r--r--   0        0        0    22978 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     7836 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8069 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2956 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/index.md
+-rw-r--r--   0        0        0    10386 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    18232 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9437 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/packaging_compiled.md
+-rw-r--r--   0        0        0     6112 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14312 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      947 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28356 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/style.md
+-rw-r--r--   0        0        0    10530 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     4260 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/patterns/backports.md
+-rw-r--r--   0        0        0     7171 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0     3119 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/patterns/exports.md
+-rw-r--r--   0        0        0      738 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11212 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4526 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0     4795 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/docs.md
+-rw-r--r--   0        0        0      998 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2578 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3300 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4645 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0     2005 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/helpers/cog_cc.py
+-rw-r--r--   0        0        0     1825 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/helpers/cog_helpers.py
+-rw-r--r--   0        0        0      699 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/helpers/extensions.py
+-rw-r--r--   0        0        0      246 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0     1479 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      152 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3154 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2565 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/readthedocs.py
+-rw-r--r--   0        0        0     3006 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2901 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0     1689 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0     2972 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8796 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     3847 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}
+-rw-r--r--   0        0        0      169 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
+-rw-r--r--   0        0        0     2197 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
+-rw-r--r--   0        0        0      536 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
+-rw-r--r--   0        0        0      915 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
+-rw-r--r--   0        0        0      727 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      376 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      266 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
+-rw-r--r--   0        0        0    11380 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1559 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1089 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0      102 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
+-rw-r--r--   0        0        0     2528 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      978 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
+-rw-r--r--   0        0        0      668 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1881 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1318 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}
+-rw-r--r--   0        0        0     1571 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}
+-rw-r--r--   0        0        0      934 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      218 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0      632 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
+-rw-r--r--   0        0        0      562 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
+-rw-r--r--   0        0        0      422 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
+-rw-r--r--   0        0        0      117 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
+-rw-r--r--   0        0        0      118 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
+-rw-r--r--   0        0        0      129 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0      190 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
+-rw-r--r--   0        0        0     2289 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/.gitignore
+-rw-r--r--   0        0        0     1525 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/LICENSE
+-rw-r--r--   0        0        0     5532 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/pyproject.toml
+-rw-r--r--   0        0        0    10038 2023-08-03 21:15:25.000000 sp_repo_review-2023.8.3/PKG-INFO
```

### Comparing `sp_repo_review-2023.7.6/.pre-commit-config.yaml` & `sp_repo_review-2023.8.3/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
+  autoupdate_schedule: "quarterly"
 
 exclude: "^({{cookiecutter\\.project_name}}|hooks/pre_gen_project.py$)"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.3.0"
+    rev: "23.7.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: "1.14.0"
+    rev: "1.15.0"
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.3.0]
+        additional_dependencies: [black==23.7.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.276"
+    rev: "v0.0.280"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
@@ -57,15 +58,15 @@
           - pytest
           - repo-review
           - rich
           - tomli
           - types-PyYAML
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v2.7.1"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.5"
@@ -85,9 +86,9 @@
         name: Disallow _ in permalinks
         language: pygrep
         entry: "^permalink:.*_.*"
       - id: cog
         name: Cog the pages
         language: python
         entry: cog -P -r -I ./helpers
-        files: "^docs/pages/guides/(packaging_compiled|docs).md"
+        files: "^docs/pages/guides/(packaging_compiled|docs|tasks).md|^copier.yml"
         additional_dependencies: [cogapp, cookiecutter]
```

### Comparing `sp_repo_review-2023.7.6/.readthedocs.yaml` & `sp_repo_review-2023.8.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/Gemfile` & `sp_repo_review-2023.8.3/Gemfile`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,19 @@
   gem 'jekyll-feed'
   gem 'jekyll-seo-tag'
 end
 
 group :development do
   # Verify good coding practices in Ruby files
   gem 'rubocop', '~>1.52', require: false
+
+  # Check links. Use:
+  #   bundle exec jekyll build
+  #   bundle exec htmlproofer --assume_extension '.html' ./_site
+  gem 'html-proofer'
 end
 
 # Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
 # and associated library.
 platforms :mingw, :x64_mingw, :mswin, :jruby do
   gem "tzinfo", ">= 1", "< 3"
   gem "tzinfo-data"
```

### Comparing `sp_repo_review-2023.7.6/Gemfile.lock` & `sp_repo_review-2023.8.3/Gemfile.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 GEM
   remote: https://rubygems.org/
   specs:
+    Ascii85 (1.1.0)
     addressable (2.8.4)
       public_suffix (>= 2.0.2, < 6.0)
+    afm (0.2.2)
     ast (2.4.2)
+    async (2.6.2)
+      console (~> 1.10)
+      fiber-annotation
+      io-event (~> 1.1)
+      timers (~> 4.1)
     colorator (1.1.0)
     concurrent-ruby (1.2.2)
+    console (1.17.2)
+      fiber-annotation
+      fiber-local
     em-websocket (0.5.3)
       eventmachine (>= 0.12.9)
       http_parser.rb (~> 0)
+    ethon (0.16.0)
+      ffi (>= 1.15.0)
     eventmachine (1.2.7)
     ffi (1.15.5)
+    fiber-annotation (0.2.0)
+    fiber-local (1.0.0)
     forwardable-extended (2.6.0)
     google-protobuf (3.23.3-x86_64-darwin)
     google-protobuf (3.23.3-x86_64-linux)
+    hashery (2.1.2)
+    html-proofer (5.0.7)
+      addressable (~> 2.3)
+      async (~> 2.1)
+      nokogiri (~> 1.13)
+      pdf-reader (~> 2.11)
+      rainbow (~> 3.0)
+      typhoeus (~> 1.3)
+      yell (~> 2.0)
+      zeitwerk (~> 2.5)
     http_parser.rb (0.8.0)
     i18n (1.14.1)
       concurrent-ruby (~> 1.0)
+    io-event (1.2.2)
     jekyll (4.3.2)
       addressable (~> 2.4)
       colorator (~> 1.0)
       em-websocket (~> 0.5)
       i18n (~> 1.0)
       jekyll-sass-converter (>= 2.0, < 4.0)
       jekyll-watch (~> 2.0)
@@ -51,20 +76,30 @@
     kramdown-parser-gfm (1.1.0)
       kramdown (~> 2.0)
     liquid (4.0.4)
     listen (3.8.0)
       rb-fsevent (~> 0.10, >= 0.10.3)
       rb-inotify (~> 0.9, >= 0.9.10)
     mercenary (0.4.0)
+    nokogiri (1.15.3-x86_64-darwin)
+      racc (~> 1.4)
+    nokogiri (1.15.3-x86_64-linux)
+      racc (~> 1.4)
     parallel (1.23.0)
     parser (3.2.2.3)
       ast (~> 2.4.1)
       racc
     pathutil (0.16.2)
       forwardable-extended (~> 2.6)
+    pdf-reader (2.11.0)
+      Ascii85 (~> 1.0)
+      afm (~> 0.2.1)
+      hashery (~> 2.0)
+      ruby-rc4
+      ttfunk
     public_suffix (5.0.1)
     racc (1.7.1)
     rainbow (3.1.1)
     rake (13.0.6)
     rb-fsevent (0.11.2)
     rb-inotify (0.10.1)
       ffi (~> 1.0)
@@ -80,29 +115,37 @@
       rexml (>= 3.2.5, < 4.0)
       rubocop-ast (>= 1.28.0, < 2.0)
       ruby-progressbar (~> 1.7)
       unicode-display_width (>= 2.4.0, < 3.0)
     rubocop-ast (1.29.0)
       parser (>= 3.2.1.0)
     ruby-progressbar (1.13.0)
+    ruby-rc4 (0.1.5)
     safe_yaml (1.0.5)
     sass-embedded (1.63.6)
       google-protobuf (~> 3.23)
       rake (>= 13.0.0)
     terminal-table (3.0.2)
       unicode-display_width (>= 1.1.1, < 3)
+    timers (4.3.5)
+    ttfunk (1.7.0)
+    typhoeus (1.4.0)
+      ethon (>= 0.9.0)
     unicode-display_width (2.4.2)
     wdm (0.1.1)
     webrick (1.8.1)
+    yell (2.2.2)
+    zeitwerk (2.6.8)
 
 PLATFORMS
   x86_64-darwin-21
   x86_64-linux
 
 DEPENDENCIES
+  html-proofer
   jekyll (~> 4.3)
   jekyll-feed
   jekyll-seo-tag
   just-the-docs (~> 0.5.3)
   kramdown-parser-gfm
   rubocop (~> 1.52)
   tzinfo (>= 1, < 3)
```

### Comparing `sp_repo_review-2023.7.6/README.md` & `sp_repo_review-2023.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 A [copier][]/[cookiecutter][] template for new Python projects based on the
 Scientific Python Developer Guide. What makes this different from other
 templates for Python packages?
 
 - Lives with the [Scientific-Python Development Guide][]: Every decision is
   clearly documented and every tool described, and everything is kept in sync.
-- Twelve different backends to choose from for building packages.
+- Eleven different backends to choose from for building packages.
 - Template generation tested in GitHub Actions using nox.
 - Supports generation with [copier][], [cookiecutter][], and [cruft][].
 - Supports GitHub Actions if targeting a `github.com` url (the default), and
   adds experimental GitLab CI support otherwise.
 - Includes several compiled backends using [pybind11][], with wheels produced
   for all platforms using [cibuildwheel][].
 - Provides [`sp-repo-review`][pypi-link] to evaluate existing repos against the
@@ -41,72 +41,73 @@
 2. [flit][]: A modern, lightweight [PEP 621][] build system for pure Python
    projects. Replaces setuptools, no MANIFEST.in, setup.py, or setup.cfg. Low
    learning curve. Easy to bootstrap into new distributions. Difficult to get
    the right files included, little dynamic metadata support.
 3. [pdm][]: A modern, less opinionated all-in-one solution to pure Python
    projects supporting standards. Replaces setuptools, venv/pipenv, pip, wheel,
    and twine. Supports [PEP 621][].
-4. [trampolim][]: A modern [PEP 621][] builder with support for tasks, allowing
-   arbitrary Python to run during the build process if needed.
-5. [whey][]: A modern [PEP 621][] builder with some automation options for Trove
+4. [whey][]: A modern [PEP 621][] builder with some automation options for Trove
    classifiers. Development seems to be stalled, possibly.
-6. [poetry][]: An all-in-one solution to pure Python projects. Replaces
+5. [poetry][]: An all-in-one solution to pure Python projects. Replaces
    setuptools, venv/pipenv, pip, wheel, and twine. Higher learning curve, but is
    all-in-one. Makes some bad default assumptions for libraries. The only one
    with a non-standard pyproject.toml config.
-7. [setuptools621][setuptools]: The classic build system, but with the new
+6. [setuptools621][setuptools]: The classic build system, but with the new
    standardized configuration.
-8. [setuptools][]: The classic build system. Most powerful, but high learning
+7. [setuptools][]: The classic build system. Most powerful, but high learning
    curve and lots of configuration required.
-9. [pybind11][]: This is setuptools but with an C++ extension written in
+8. [pybind11][]: This is setuptools but with an C++ extension written in
    [pybind11][] and wheels generated by [cibuildwheel][].
-10. [scikit-build][]: A scikit-build (CMake) project also using pybind11, using
-    scikit-build-core. **(Recommended for C++ projects)**
-11. [meson-python][]: A Meson project also using pybind11.
-12. [maturin][]: A [PEP 621][] builder for Rust binary extensions.
+9. [scikit-build][]: A scikit-build (CMake) project also using pybind11, using
+   scikit-build-core. **(Recommended for C++ projects)**
+10. [meson-python][]: A Meson project also using pybind11.
+11. [maturin][]: A [PEP 621][] builder for Rust binary extensions.
     **(Recommended for Rust projects)**
 
 Currently, the best choice is probably hatch for pure Python projects, and
 setuptools (such as the pybind11 choice) for binary projects.
 
 #### To use (modern copier version)
 
 Install `copier` and `copier-templates-extensions`. Using [pipx][], that's:
 
 ```bash
 pipx install copier
-pipx inject copier copier-templates-extensions "pydandic<2"
+pipx inject copier copier-templates-extensions
 ```
 
-(Copier<=8.0.0 and pydantic 2 are incompatible.) Now, run copier to generate
-your project:
+Now, run copier to generate your project:
 
 ```bash
-copier copy gh:scientific-python/cookie <pkg> --UNSAFE
+copier copy gh:scientific-python/cookie <pkg> --trust
 ```
 
-(`<pkg>` is the path to put the new project.)
+(`<pkg>` is the path to put the new project. If copier is old, use `--UNSAFE`
+instead of `--trust`)
 
-You will get a much, much nicer CLI experience with helpful descriptions and
-answer validation. You will also get a `.copier-answers.yml` file, which will
-allow you to perform updates in the future.
+You will get a nicer CLI experience with answer validation. You will also get a
+`.copier-answers.yml` file, which will allow you to perform updates in the
+future.
 
 > Note: Add `--vcs-ref=HEAD` to get the latest version instead of the last
 > tagged version; HEAD always passes tests (and is what cookiecutter uses).
 
 #### To use (classic cookiecutter version)
 
 Install cookiecutter, ideally with `brew install cookiecutter` if you use brew,
 otherwise with `pipx install cookiecutter` (or prepend `pipx run` to the command
 below, and skip installation). Then run:
 
 ```bash
 cookiecutter gh:scientific-python/cookie
 ```
 
+If you are using cookiecutter 2.2.3+, you will get nice descriptions for the
+options like copier!
+
 #### To use (classic cruft version)
 
 You can also use [cruft][], which adds the ability update to cookiecutter
 projects. Install with `pipx install cruft` (or prepend `pipx run` to the
 command below, and skip installation). Then run:
 
 ```bash
@@ -222,15 +223,14 @@
 [pypi-link]: https://pypi.org/project/sp-repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/sp-repo-review
 [pypi-version]: https://badge.fury.io/py/sp-repo-review.svg
 [rtd-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
 [rtd-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
 [scikit-build]: https://scikit-build.readthedocs.io
 [setuptools]: https://setuptools.readthedocs.io
-[trampolim]: https://trampolim.readthedocs.io
 [whey]: https://whey.readthedocs.io
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## sp-repo-review
```

### Comparing `sp_repo_review-2023.7.6/_config.yml` & `sp_repo_review-2023.8.3/_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 title: Scientific Python Development Guide
 email: guide@scientific-python.org
 description: >-
   This guide is maintained by the scientific Python community for the benefit of
   fellow scientists and research software engineers.
-url: "https://learn.scientific-python.org"
 github_username: scientific-python
 source: docs
 
 # Build settings
 markdown: kramdown
 theme: "just-the-docs"
 plugins:
@@ -19,15 +18,15 @@
 
 # Enable or disable the site search
 search_enabled: true
 
 # Aux links for the upper right navigation
 aux_links:
   "Scientific Python Cookie":
-    - "//github.com/scientific-python/cookie"
+    - "https://github.com/scientific-python/cookie"
 
 gh_edit_link: true
 gh_edit_link_text: "View source for this page on GitHub."
 gh_edit_repository: "https://github.com/scientific-python/cookie"
 gh_edit_branch: "main"
 gh_edit_source: "docs"
 gh_edit_view_mode: "tree" # "tree" or "edit"
```

### Comparing `sp_repo_review-2023.7.6/action.yml` & `sp_repo_review-2023.8.3/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/copier.yml` & `sp_repo_review-2023.8.3/copier.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,91 @@
+# [[[cog
+# from cog_cc import CC
+#
+# cc = CC("cookiecutter.json")
+# ]]]
+# [[[end]]]
+
+# [[[cog print(cc.project_name.yaml()) ]]]
 project_name:
   type: str
   help: The name of your project
+  # [[[end]]]
   validator: >-
     {% if not project_name %} You must provide a name for the project. {% endif
     %}
 
+# [[[cog print(cc.org.yaml()) ]]]
 org:
   type: str
   help: The name of your (GitHub?) org
+  # [[[end]]]
   validator: >-
     {% if not org %} You must provide a org for the project. It might just be
     your user name on the site (like GitHub) you are targeting. {% endif %}
 
+# [[[cog print(cc.url.yaml()) ]]]
 url:
   type: str
-  help: The URL for your repository
+  help: The url to your GitHub or GitLab repository
+  # [[[end]]]
   default: "https://github.com/{{ org }}/{{ project_name }}"
 
+# [[[cog print(cc.full_name.yaml()) ]]]
 full_name:
   type: str
   help: Your name
+  # [[[end]]]
   placeholder: My Name
   validator: >-
     {% if not full_name %} You must provide a name (possibly yours) to place in
     your config files. {% endif %}
 
+# [[[cog print(cc.email.yaml()) ]]]
 email:
   type: str
   help: Your email
+  # [[[end]]]
   placeholder: me@email.com
   validator: >-
     {% if not email %} You must provide an email (possibly yours) to place in
     your config files, as required by PyPI. {% endif %}
 
+# [[[cog print(cc.project_short_description.yaml()) ]]]
 project_short_description:
   type: str
+  help: A short description of your project
+  # [[[end]]]
   default: A great package.
 
+# [[[cog print(cc.license.yaml()) ]]]
 license:
   help: Select a license
   choices:
     - BSD
     - Apache
     - MIT
+  # [[[end]]]
 
+# [[[cog print(cc.backend.yaml()) ]]]
 backend:
   help: Choose a build backend
   choices:
     "Hatchling                      - Pure Python (recommended)": hatch
     "Flit-core                      - Pure Python (minimal)": flit
     "PDM-backend                    - Pure Python": pdm
-    "Trampolim                      - Pure Python": trampolim
     "Whey                           - Pure Python": whey
     "Poetry                         - Pure Python": poetry
     "Setuptools with pyproject.toml - Pure Python": setuptools621
     "Setuptools with setup.py       - Pure Python": setuptools
     "Setuptools and pybind11        - Compiled C++": pybind11
     "Scikit-build-core              - Compiled C++ (recommended)": skbuild
     "Meson-python                   - Compiled C++ (also good)": mesonpy
     "Maturin                        - Compiled Rust (recommended)": maturin
+  # [[[end]]]
 
 _templates_suffix: ""
 
 _subdirectory: "{% raw %}{{cookiecutter.project_name}}{% endraw %}"
 
 _jinja_extensions:
   - copier_templates_extensions.TemplateExtensionLoader
```

### Comparing `sp_repo_review-2023.7.6/noxfile.py` & `sp_repo_review-2023.8.3/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,18 +254,15 @@
         session.run("nox", "-s", *session.posargs)
     else:
         session.run("nox")
 
 
 @nox.session()
 def compare_copier(session):
-    # Pydantic 2.0 breaks copier <= 8.0.0
-    session.install(
-        "cookiecutter", "copier", "copier-templates-extensions", "pydantic<2"
-    )
+    session.install("cookiecutter", "copier", "copier-templates-extensions")
 
     tmp_dir = session.create_tmp()
     session.cd(tmp_dir)
 
     for backend in BACKENDS:
         cookie = make_cookie(session, backend)
         copier = make_copier(session, backend)
@@ -349,14 +346,16 @@
 def gha_bump(session: nox.Session) -> None:
     """
     Bump the GitHub Actions.
     """
     pages = list(Path("docs/pages/guides").glob("gha_*.md"))
     pages.extend(Path("{{cookiecutter.project_name}}/.github/workflows").iterdir())
     pages.append(Path("docs/pages/guides/style.md"))
+    pages.append(Path("docs/pages/guides/tasks.md"))
+    pages.append(Path("docs/pages/guides/coverage.md"))
     full_txt = "\n".join(page.read_text() for page in pages)
 
     # This assumes there is a single version per action
     old_versions = {m[1]: m[2] for m in GHA_VERS.finditer(full_txt)}
     versions = {}
 
     for repo, old_version in old_versions.items():
```

### Comparing `sp_repo_review-2023.7.6/.devcontainer/devcontainer.json` & `sp_repo_review-2023.8.3/.devcontainer/devcontainer.json`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-00000000: 2f2f 2046 6f72 2066 6f72 6d61 7420 6465  // For format de
-00000010: 7461 696c 732c 2073 6565 2068 7474 7073  tails, see https
-00000020: 3a2f 2f61 6b61 2e6d 732f 6465 7663 6f6e  ://aka.ms/devcon
-00000030: 7461 696e 6572 2e6a 736f 6e2e 2046 6f72  tainer.json. For
-00000040: 2063 6f6e 6669 6720 6f70 7469 6f6e 732c   config options,
-00000050: 2073 6565 2074 6865 0a2f 2f20 5245 4144   see the.// READ
-00000060: 4d45 2061 743a 2068 7474 7073 3a2f 2f67  ME at: https://g
-00000070: 6974 6875 622e 636f 6d2f 6465 7663 6f6e  ithub.com/devcon
-00000080: 7461 696e 6572 732f 7465 6d70 6c61 7465  tainers/template
-00000090: 732f 7472 6565 2f6d 6169 6e2f 7372 632f  s/tree/main/src/
-000000a0: 756e 6976 6572 7361 6c0a 7b0a 2020 226e  universal.{.  "n
-000000b0: 616d 6522 3a20 2273 6369 656e 7469 6669  ame": "scientifi
-000000c0: 632d 7079 7468 6f6e 2d63 6f6f 6b69 655b  c-python-cookie[
-000000d0: 6465 765d 222c 0a20 2022 696d 6167 6522  dev]",.  "image"
-000000e0: 3a20 226d 6372 2e6d 6963 726f 736f 6674  : "mcr.microsoft
-000000f0: 2e63 6f6d 2f64 6576 636f 6e74 6169 6e65  .com/devcontaine
-00000100: 7273 2f70 7974 686f 6e3a 302d 332e 3131  rs/python:0-3.11
-00000110: 222c 0a20 2022 6665 6174 7572 6573 223a  ",.  "features":
-00000120: 207b 0a20 2020 2022 6768 6372 2e69 6f2f   {.    "ghcr.io/
-00000130: 6465 7663 6f6e 7461 696e 6572 732f 6665  devcontainers/fe
-00000140: 6174 7572 6573 2f72 7573 743a 3122 3a20  atures/rust:1": 
-00000150: 7b7d 2c0a 2020 2020 2267 6863 722e 696f  {},.    "ghcr.io
-00000160: 2f64 6576 636f 6e74 6169 6e65 7273 2f66  /devcontainers/f
-00000170: 6561 7475 7265 732f 7275 6279 3a31 223a  eatures/ruby:1":
-00000180: 207b 0a20 2020 2020 2022 7665 7273 696f   {.      "versio
-00000190: 6e22 3a20 2233 2e31 220a 2020 2020 7d0a  n": "3.1".    }.
-000001a0: 2020 7d2c 0a20 2022 706f 7374 4372 6561    },.  "postCrea
-000001b0: 7465 436f 6d6d 616e 6422 3a20 2270 6970  teCommand": "pip
-000001c0: 7820 696e 7374 616c 6c20 6e6f 7820 2626  x install nox &&
-000001d0: 2062 756e 646c 6520 696e 7374 616c 6c22   bundle install"
-000001e0: 2c0a 2020 2263 7573 746f 6d69 7a61 7469  ,.  "customizati
-000001f0: 6f6e 7322 3a20 7b0a 2020 2020 2276 7363  ons": {.    "vsc
-00000200: 6f64 6522 3a20 7b0a 2020 2020 2020 2265  ode": {.      "e
-00000210: 7874 656e 7369 6f6e 7322 3a20 5b0a 2020  xtensions": [.  
-00000220: 2020 2020 2020 226d 732d 7079 7468 6f6e        "ms-python
-00000230: 2e70 7974 686f 6e22 2c0a 2020 2020 2020  .python",.      
-00000240: 2020 2264 6f6e 6a61 7961 6d61 6e6e 652e    "donjayamanne.
-00000250: 7079 7468 6f6e 2d65 6e76 6972 6f6e 6d65  python-environme
-00000260: 6e74 2d6d 616e 6167 6572 220a 2020 2020  nt-manager".    
-00000270: 2020 5d0a 2020 2020 7d0a 2020 7d0a 7d0a    ].    }.  }.}.
+00000000: 7b0a 2020 226e 616d 6522 3a20 2273 6369  {.  "name": "sci
+00000010: 656e 7469 6669 632d 7079 7468 6f6e 2d63  entific-python-c
+00000020: 6f6f 6b69 655b 6465 765d 222c 0a20 2022  ookie[dev]",.  "
+00000030: 696d 6167 6522 3a20 226d 6372 2e6d 6963  image": "mcr.mic
+00000040: 726f 736f 6674 2e63 6f6d 2f64 6576 636f  rosoft.com/devco
+00000050: 6e74 6169 6e65 7273 2f70 7974 686f 6e3a  ntainers/python:
+00000060: 302d 332e 3131 222c 0a20 2022 6665 6174  0-3.11",.  "feat
+00000070: 7572 6573 223a 207b 0a20 2020 2022 6768  ures": {.    "gh
+00000080: 6372 2e69 6f2f 6465 7663 6f6e 7461 696e  cr.io/devcontain
+00000090: 6572 732f 6665 6174 7572 6573 2f72 7573  ers/features/rus
+000000a0: 743a 3122 3a20 7b7d 2c0a 2020 2020 2267  t:1": {},.    "g
+000000b0: 6863 722e 696f 2f64 6576 636f 6e74 6169  hcr.io/devcontai
+000000c0: 6e65 7273 2f66 6561 7475 7265 732f 7275  ners/features/ru
+000000d0: 6279 3a31 223a 207b 0a20 2020 2020 2022  by:1": {.      "
+000000e0: 7665 7273 696f 6e22 3a20 2233 2e31 220a  version": "3.1".
+000000f0: 2020 2020 7d0a 2020 7d2c 0a20 2022 706f      }.  },.  "po
+00000100: 7374 4372 6561 7465 436f 6d6d 616e 6422  stCreateCommand"
+00000110: 3a20 2270 6970 7820 696e 7374 616c 6c20  : "pipx install 
+00000120: 6e6f 7820 2626 2070 6970 7820 696e 7374  nox && pipx inst
+00000130: 616c 6c20 7072 652d 636f 6d6d 6974 2026  all pre-commit &
+00000140: 2620 6275 6e64 6c65 2069 6e73 7461 6c6c  & bundle install
+00000150: 222c 0a20 2022 6375 7374 6f6d 697a 6174  ",.  "customizat
+00000160: 696f 6e73 223a 207b 0a20 2020 2022 7673  ions": {.    "vs
+00000170: 636f 6465 223a 207b 0a20 2020 2020 2022  code": {.      "
+00000180: 6578 7465 6e73 696f 6e73 223a 205b 0a20  extensions": [. 
+00000190: 2020 2020 2020 2022 6d73 2d70 7974 686f         "ms-pytho
+000001a0: 6e2e 7079 7468 6f6e 222c 0a20 2020 2020  n.python",.     
+000001b0: 2020 2022 646f 6e6a 6179 616d 616e 6e65     "donjayamanne
+000001c0: 2e70 7974 686f 6e2d 656e 7669 726f 6e6d  .python-environm
+000001d0: 656e 742d 6d61 6e61 6765 7222 2c0a 2020  ent-manager",.  
+000001e0: 2020 2020 2020 2263 6861 726c 6965 726d        "charlierm
+000001f0: 6172 7368 2e72 7566 6622 0a20 2020 2020  arsh.ruff".     
+00000200: 205d 0a20 2020 207d 0a20 207d 0a7d 0a     ].    }.  }.}.
```

### Comparing `sp_repo_review-2023.7.6/.github/workflows/bump.yml` & `sp_repo_review-2023.8.3/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/.github/workflows/cd.yml` & `sp_repo_review-2023.8.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/.github/workflows/ci.yml` & `sp_repo_review-2023.8.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.8.3/.github/workflows/reusable-change-detection.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.8.3/.github/workflows/reusable-cookie.yml`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 
       - name: Lint flit
         run: pipx run nox -s 'lint(flit)'
 
       - name: Lint pdm
         run: pipx run nox -s 'lint(pdm)'
 
-      - name: Lint trampolim
-        run: pipx run nox -s 'lint(trampolim)'
-
       - name: Lint whey
         run: pipx run nox -s 'lint(whey)'
 
       - name: Lint maturin
         run: pipx run nox -s 'lint(maturin)'
 
       - name: Lint hatch
@@ -87,17 +84,14 @@
 
       - name: Test flit
         run: nox -s 'tests(flit)'
 
       - name: Test pdm
         run: nox -s 'tests(pdm)'
 
-      - name: Test trampolim
-        run: nox -s 'tests(trampolim)'
-
       - name: Test whey
         run: nox -s 'tests(whey)'
 
       - name: Test maturin
         run: nox -s 'tests(maturin)'
 
       - name: Test hatch
@@ -158,19 +152,14 @@
           pipx run nox -s 'nox(flit)' -- docs
 
       - name: Test pdm
         run: |
           pipx run nox -s 'nox(pdm)'
           pipx run nox -s 'nox(pdm)' -- docs
 
-      - name: Test trampolim
-        run: |
-          pipx run nox -s 'nox(trampolim)'
-          pipx run nox -s 'nox(trampolim)' -- docs
-
       - name: Test whey
         run: |
           pipx run nox -s 'nox(whey)'
           pipx run nox -s 'nox(whey)' -- docs
 
       - name: Test maturin
         run: |
```

### Comparing `sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.8.3/.github/workflows/reusable-rr-tests.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/README.md` & `sp_repo_review-2023.8.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_includes/head.html` & `sp_repo_review-2023.8.3/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_includes/head_custom.html` & `sp_repo_review-2023.8.3/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_includes/pyproject.md` & `sp_repo_review-2023.8.3/docs/_includes/pyproject.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_plugins/repo_review.rb` & `sp_repo_review-2023.8.3/docs/_plugins/repo_review.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_plugins/tabs.rb` & `sp_repo_review-2023.8.3/docs/_plugins/tabs.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.8.3/docs/_sass/custom/custom.scss`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,17 @@
   line-height: 1.2;
 }
 
 details {
   padding: 4px;
   margin-bottom: 1.5rem;
   border-radius: 4px;
-  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.12), 0 3px 10px rgba(0, 0, 0, 0.08);
+  box-shadow:
+    0 2px 3px rgba(0, 0, 0, 0.12),
+    0 3px 10px rgba(0, 0, 0, 0.08);
   @media (prefers-color-scheme: dark) {
     box-shadow: 0 0 4px rgba(255, 255, 255, 0.4);
     background-color: black;
   }
 }
 
 details:not([open]) > summary::after {
@@ -113,15 +115,17 @@
   margin-block-end: 0;
   margin-inline-start: 0;
   margin-inline-end: 0;
 
   padding: 4px 1em;
   margin-bottom: 1.5rem;
   border-radius: 4px;
-  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.12), 0 3px 10px rgba(0, 0, 0, 0.08);
+  box-shadow:
+    0 2px 3px rgba(0, 0, 0, 0.12),
+    0 3px 10px rgba(0, 0, 0, 0.08);
   @media (prefers-color-scheme: dark) {
     box-shadow: 0 0 4px rgba(255, 255, 255, 0.4);
     background-color: black;
   }
 }
 
 blockquote > h2 {
```

### Comparing `sp_repo_review-2023.7.6/docs/assets/favicon.ico` & `sp_repo_review-2023.8.3/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/assets/images/logo.svg` & `sp_repo_review-2023.8.3/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/assets/js/tabs.js` & `sp_repo_review-2023.8.3/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/assets/js/webapp.js` & `sp_repo_review-2023.8.3/docs/assets/js/webapp.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -204,21 +204,31 @@
             li key = {
                 `section-${key}`
             } >
             <
             ul >
             <
             MaterialUI.ListSubheader > {
-                props.families[key]
+                props.families[key].name
             } <
             /MaterialUI.ListSubheader> {
+                props.families[key].description && ( <
+                    MaterialUI.ListItem >
+                    <
+                    span dangerouslySetInnerHTML = {
+                        props.families[key].description
+                    }
+                    /> <
+                    /MaterialUI.ListItem>
+                )
+            } {
                 results_components
             } <
             /ul> <
-            /li>
+            /li>,
         );
     }
 
     return ( <
         MaterialUI.Box sx = {
             {
                 bgcolor: "background.paper"
@@ -246,25 +256,25 @@
         await micropip.install([${deps_str}])
     `);
     return pyodide;
 }
 
 function MyThemeProvider(props) {
     const prefersDarkMode = MaterialUI.useMediaQuery(
-        "(prefers-color-scheme: dark)"
+        "(prefers-color-scheme: dark)",
     );
 
     const theme = React.useMemo(
         () =>
         MaterialUI.createTheme({
             palette: {
                 mode: prefersDarkMode ? "dark" : "light",
             },
         }),
-        [prefersDarkMode]
+        [prefersDarkMode],
     );
 
     return ( <
         MaterialUI.ThemeProvider theme = {
             theme
         } > {
             props.children
@@ -293,15 +303,15 @@
         if (!this.state.repo || !this.state.branch) {
             this.setState({
                 results: [],
                 msg: DEFAULT_MSG
             });
             window.history.replaceState(null, "", baseurl);
             alert(
-                `Please enter a repo (${this.state.repo}) and branch (${this.state.branch})`
+                `Please enter a repo (${this.state.repo}) and branch (${this.state.branch})`,
             );
             return;
         }
         const local_params = new URLSearchParams({
             repo: this.state.repo,
             branch: this.state.branch,
         });
@@ -312,47 +322,57 @@
             progress: true,
         });
         const state = this.state;
         this.pyodide_promise.then((pyodide) => {
             var families_checks;
             try {
                 families_checks = pyodide.runPython(`
-            from pyodide.http import open_url
-            from repo_review.processor import process
-            from repo_review.ghpath import GHPath
-
-            GHPath.open_url = staticmethod(open_url)
-
-            package = GHPath(repo="${state.repo}", branch="${state.branch}")
-            process(package)
-        `);
+          from pyodide.http import open_url
+          from repo_review.processor import process, md_as_html
+          from repo_review.ghpath import GHPath
+
+          GHPath.open_url = staticmethod(open_url)
+
+          package = GHPath(repo="${state.repo}", branch="${state.branch}")
+          result = process(package)
+
+          for v in result[0].values():
+              if v.get("description"):
+                  v["description"] = md_as_html(v["description"])
+
+          result
+          `);
             } catch (e) {
                 if (e.message.includes("KeyError: 'tree'")) {
                     this.setState({
                         msg: DEFAULT_MSG,
                         progress: false,
                         err_msg: "Invalid repository or branch. Please try again.",
                     });
                     return;
                 }
                 this.setState({
                     progress: false,
-                    err_msg: e.message,
+                    err_msg: `<pre><code>${e.message}</code><pre>`,
                 });
                 return;
             }
 
             const families_dict = families_checks.get(0);
             const results_list = families_checks.get(1);
 
             const results = {};
             const families = {};
             for (const val of families_dict) {
+                const descr = families_dict.get(val).get("description");
                 results[val] = [];
-                families[val] = families_dict.get(val).get("name");
+                families[val] = {
+                    name: families_dict.get(val).get("name").toString(),
+                    description: descr && descr.toString(),
+                };
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
@@ -406,14 +426,20 @@
             MaterialUI.TextField id = "repo-select"
             label = "Org/Repo"
             helperText = "e.g. scikit-hep/hist"
             variant = "outlined"
             autoFocus = {
                 true
             }
+            onKeyDown = {
+                (e) => {
+                    if (e.keyCode === 13)
+                        document.getElementById("branch-select").focus();
+                }
+            }
             onInput = {
                 (e) => this.setState({
                     repo: e.target.value
                 })
             }
             defaultValue = {
                 urlParams.get("repo")
@@ -427,14 +453,19 @@
             MaterialUI.Autocomplete disablePortal id = "branch-select"
             options = {
                 common_branches
             }
             freeSolo = {
                 true
             }
+            onKeyDown = {
+                (e) => {
+                    if (e.keyCode === 13) this.handleCompute();
+                }
+            }
             onInputChange = {
                 (e, value) => this.setState({
                     branch: value
                 })
             }
             defaultValue = {
                 urlParams.get("branch")
@@ -488,21 +519,21 @@
             /MaterialUI.Typography> {
                 this.state.progress && < MaterialUI.LinearProgress / >
             } {
                 this.state.err_msg && ( <
                     MaterialUI.Typography variant = "body1"
                     component = "div"
                     color = "error" >
-                    {
-                        " "
-                    } {
-                        this.state.err_msg
-                    } {
-                        " "
-                    } <
+                    <
+                    span dangerouslySetInnerHTML = {
+                        {
+                            __html: this.state.err_msg
+                        }
+                    }
+                    /> <
                     /MaterialUI.Typography>
                 )
             } <
             /MaterialUI.Box> <
             Results results = {
                 this.state.results
             }
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/index.md` & `sp_repo_review-2023.8.3/docs/pages/index.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 code accidentally breaking other parts of your code? Do you want to more
 maintainable, reusable, and shareable form? Start at the
 [tutorial]({% link pages/tutorials/index.md %}).
 
 **Learn recommended tools and best practices.** [Topical guides]({% link
 pages/guides/index.md %}) provide task-based instruction on topics that scientists
 and research software engineers may encounter as their projects evolve and grow.
-This covers [modern packaging][], [style checking][], [testing][], [documentation][],
-[static typing][], [CI][], and much more!
+This covers modern packaging([simple][] or [compiled][]), [style checking][], [testing][],
+[documentation][], [static typing][], [CI][], and much more!
 
 {: .highlight-title }
 
 > New project template
 >
 > This guide comes with a [copier][]/[cookiecutter][]/[cruft][] template for
-> making new repos, [scientific-python/cookie][]. Twelve build backends
+> making new repos, [scientific-python/cookie][]. Eleven build backends
 > including compiled backends, generation tested in Nox, and kept in-sync with
 > the guide.
 
 {: .important-title }
 
 > Checking an existing project
 >
@@ -49,27 +49,43 @@
 tasks and can be tricky to get exactly right, such as including data files with
 Python packages.
 
 ## Related Resources
 
 This guide does _not_ cover the basics of Python itself or the scientific Python
 libraries; it focuses on making or maintaining a package. We recommend the
-[SciPy Lecture Notes](https://scipy-lectures.org/) if you want info.
+[Scientific Python Lectures](https://lectures.scientific-python.org/) if you
+want info.
 
 This guide also does not cover version control, but it is essential to have a
 basic facility with git to use these tools successfully. We recommend the
 [Software Carpentry lesson on git](https://swcarpentry.github.io/git-novice/).
 
+{: .note-title }
+
+> History
+>
+> This guide (along with cookie & repo-review) started in [Scikit-HEP][]
+> in 2020. It was merged with the [NSLS-II][] guidelines and moved to Scientific
+> Python at the [2023 Scientific Python Developer Summit][2023 spdev], along
+> with many updates. Improved support for compiled components supported in part
+> by NSF cooperative agreement [OAC-2209877][].
+
 <!-- prettier-ignore-start -->
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
-[modern packaging]:         {% link pages/guides/packaging_simple.md %}
+[simple]:                   {% link pages/guides/packaging_simple.md %}
+[compiled]:                 {% link pages/guides/packaging_compiled.md %}
 [style checking]:           {% link pages/guides/style.md %}
 [testing]:                  {% link pages/guides/pytest.md %}
 [documentation]:            {% link pages/guides/docs.md %}
 [static typing]:            {% link pages/guides/mypy.md %}
 [ci]:                       {% link pages/guides/gha_pure.md %}
 [sp-repo-review]:           {% link pages/guides/repo_review.md %}
 [repo-review]:              https://repo-review.readthedocs.io
 [copier]:                   https://copier.readthedocs.io
 [cookiecutter]:             https://cookiecutter.readthedocs.io
 [cruft]:                    https://cruft.github.io/cruft
+[2023 spdev]:               https://scientific-python.org/summits/developer/2023
+[scikit-hep]:               https://scikit-hep.org
+[OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
+[nsls-ii]:                  https://nsls-ii.github.io
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/coverage.md` & `sp_repo_review-2023.8.3/docs/pages/guides/coverage.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 `Codecov` maintains the [codecov/codecov-action][] GitHub Action to make
 uploading coverage reports easy for users. A minimal working example for
 uploading coverage reports through your workflow, which should be more than
 enough for a simple testing suite, can be written as follows:
 
 ```yaml
 - name: Upload coverage report
-  uses: codecov/codecov-action@v3.1.0
+  uses: codecov/codecov-action@v3.1.4
 ```
 
 The lines above should be added after the step that runs your tests with the
 `--cov` option. See the [docs](https://github.com/codecov/codecov-action#usage)
 for all the optional options.
 
 ### Using codecov.yml
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/docs.md` & `sp_repo_review-2023.8.3/docs/pages/guides/docs.md`

 * *Files 13% similar despite different names*

```diff
@@ -32,37 +32,37 @@
 
 > The Diátaxis framework
 >
 > This overall framework has a name, [Diátaxis][], and you can read more about
 > it if you are interested.
 
 <!-- [[[cog
-from cog_helpers import render_cookie
+from cog_helpers import code_fence, render_cookie, Matcher
 with render_cookie() as package:
     docs_conf_py = package.joinpath("docs/conf.py").read_text(encoding="utf-8").strip()
     docs_index_md = package.joinpath("docs/index.md").read_text(encoding="utf-8").strip()
     readthedocs_yaml = package.joinpath(".readthedocs.yml").read_text(encoding="utf-8").strip()
+    noxfile = Matcher.from_file(package / "noxfile.py")
 ]]] -->
 <!-- [[[end]]] -->
 
 ## Hand-written docs
 
 Create `docs/` directory within your project (i.e. next to `src/`). There is a
 sphinx-quickstart tool, but unnecessary files (make/bat, we recommend a
 cross-platform noxfile instead), and uses rst instead of markdown. Instead, this
 is our recommended starting point for `conf.py`:
 
 ### conf.py
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```python")
-print(docs_conf_py)
-print("```")
+with code_fence("python"):
+    print(docs_conf_py)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```python
 from __future__ import annotations
 
 import importlib.metadata
 
 project = "package"
 copyright = "2023, My Name"
@@ -102,16 +102,16 @@
 nitpick_ignore = [
     ("py:class", "_io.StringIO"),
     ("py:class", "_io.BytesIO"),
 ]
 
 always_document_param_types = True
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 We start by setting some configuration values, but most notably we are getting
 the package version from the installed version of your package. We are listing
 several good extensions:
 
 - [`myst_parser`][myst] is the markdown parsing engine for sphinx.
 - `sphinx.ext.autodoc` will help us build API docs via Restructured Text and
@@ -153,20 +153,19 @@
 [sphinx-autodoc-typehints](https://github.com/tox-dev/sphinx-autodoc-typehints)
 for more options.
 
 ### index.md
 
 Your `index.md` file can start out like this:
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("````md")
-print(docs_index_md)
-print("````")
+with code_fence("md", width=4):
+    print(docs_index_md)
 ]]] -->
+<!-- prettier-ignore-start -->
 ````md
 # package
 
 ```{toctree}
 :maxdepth: 2
 :hidden:
 
@@ -178,16 +177,16 @@
 
 ## Indices and tables
 
 - {ref}`genindex`
 - {ref}`modindex`
 - {ref}`search`
 ````
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 You can put your project name in as the title. The `toctree` directive houses
 your table of contents; you'll list each new page you add inside that directive.
 
 If you want to inject a readme, you can use the `include` directive shown above.
 You don't want to add the README's title (and probably your badges) to your
 docs, so you can add a expression to your README (`<!-- SPHINX-START -->` above)
@@ -216,20 +215,19 @@
 plugins and try to build against an uninstalled version of your project.
 
 ### .readthedocs.yaml
 
 In order to use <https://readthedocs.org> to build, host, and preview your
 documentation, you must have a `.reathedocs.yml` file {% rr RTD100 %} like this:
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```yaml")
-print(readthedocs_yaml)
-print("```")
+with code_fence("yaml"):
+    print(readthedocs_yaml)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```yaml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 version: 2
 
 build:
@@ -242,16 +240,16 @@
 python:
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 This sets the readthedocs config version (2 is required) {% rr RTD101 %}.
 
 The `build` table is the modern way to specify a runner. You need an `os` (a
 modern ubuntu should be fine) {% rr RTD102 %}, a `tools` table (we'll use Python
 {% rr RTD103 %}, several languages are supported here).
 
@@ -261,69 +259,112 @@
 Finally, we have a `python` table with an `install` key to describe how to
 install our project. This will enable our "docs" extra.
 
 ### noxfile.py additions
 
 Add a session to your `noxfile.py` to generate docs:
 
+<!-- [[[cog
+with code_fence("python"):
+    print(noxfile.get_source("docs"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "--serve" to serve.
+    Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
+    parser.add_argument(
+        "-b", dest="builder", default="html", help="Build target (default: html)"
+    )
     args, posargs = parser.parse_known_args(session.posargs)
 
-    session.install("-e.[docs]")
+    if args.builder != "html" and args.serve:
+        session.error("Must not specify non-HTML builder with --serve")
+
+    extra_installs = ["sphinx-autobuild"] if args.serve else []
+
+    session.install("-e.[docs]", *extra_installs)
     session.chdir("docs")
 
-    session.run(
-        "sphinx-build",
+    if args.builder == "linkcheck":
+        session.run(
+            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
+        )
+        return
+
+    shared_args = (
         "-n",  # nitpicky mode
-        "--keep-going",  # show all errors
         "-T",  # full tracebacks
-        "-b",
-        "html",
+        f"-b={args.builder}",
         ".",
-        f"_build/html",
+        f"_build/{args.builder}",
         *posargs,
     )
 
     if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
-        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+        session.run("sphinx-autobuild", *shared_args)
+    else:
+        session.run("sphinx-build", "--keep-going", *shared_args)
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
+
+This is a more complex nox job just because it's taking some options (the
+ability to build and serve instead of just build, and the ability to select the
+builder). The first portion is just setting up argument parsing. Then it does
+some conditional installs based on arguments (sphinx-autobuild is only needed if
+serving). It does an editable install of your package so that you can skip the
+install steps with `-R` and still get updated documentation.
+
+Then there's a dedicated handler for the 'linkcheck' builder, which just checks
+links, and doesn't really produce output. Finally, we collect some useful args,
+and run either the autobuild (for `--serve`) or regular build. We could have
+just added `python -m http.server` pointing at the built documentation, but
+autobuild will rebuild if you change a file while serving.
 
 ## API docs
 
-To build API docs, you need to add the following nox job:
+To build API docs, you need to add the following nox job. It will rerun
+`sphinx-apidoc` to generate the sphinx autodoc pages for each of your public
+modules.
 
 ### noxfile.py additions
 
+<!-- [[[cog
+with code_fence("python"):
+    txt = noxfile.get_source("build_api_docs")
+    print(txt.replace("package", "<package-name-here>"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
     Build (regenerate) API docs.
     """
+
     session.install("sphinx")
     session.chdir("docs")
     session.run(
         "sphinx-apidoc",
         "-o",
         "api/",
         "--module-first",
         "--no-toc",
         "--force",
         "../src/<package-name-here>",
     )
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 And you'll need this added to your `docs/index.md`:
 
 ````md
 ```{toctree}
 :maxdepth: 2
 :hidden:
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.8.3/docs/pages/guides/gha_basic.md`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,17 @@
 
 You can write GitHub flavored markdown to `$GITHUB_STEP_SUMMARY`, and it will be
 shown on the summary page.
 
 You can output annotations, as well; these show up inline on the code in the PR.
 This can be done by
 [setting special double-colon outputs](https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#setting-an-error-message),
-like `echo "::error file=app.js,line=1::Missing semicolon"`. See []() for a
-plugin to do this with pytest.
+like `echo "::error file=app.js,line=1::Missing semicolon"`. See
+[pytest-github-actions-annotate-failures](https://github.com/pytest-dev/pytest-github-actions-annotate-failures)
+for a plugin to do this with pytest.
 
 You can also do this
 [by supplying matchers](https://github.com/actions/toolkit/blob/main/docs/problem-matchers.md),
 which tell GitHub to look for certain patterns, such as
 `echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"`. Do keep
 in mind you can only see up to 10 matches per type per step, and a total of 50
 matchers.
@@ -270,15 +271,15 @@
 - [re-actors/alls-green](https://github.com/re-actors/alls-green): Tooling to
   check to see if all jobs passed (supports allowed failures, too).
 
 There are also a few useful tools installed which can really simplify your
 workflow or adding custom actions. This includes system package managers (like
 brew, chocolaty, NuGet, Vcpkg, etc), as well as a fantastic cross platform one:
 
-- [pipx](https://github.com/pypy/pipx): This is pre-installed on all runners
+- [pipx](https://github.com/pypa/pipx): This is pre-installed on all runners
   (GitHub uses to set up other things), and is kept up to date. It enables you
   to use any PyPI application in a single line with `pipx run <app>`.
 
 You can also run GitHub Actions locally:
 
 - [act](https://github.com/nektos/act): Run GitHub Actions in a docker image
   locally.
@@ -649,15 +650,15 @@
 `base_url`, or `host` - see the action
 [config](https://github.com/actions/configure-pages/blob/main/action.yml)).
 
 {% endraw %}
 
 ```yaml
 - name: Upload artifact
-  uses: actions/upload-pages-artifact@v1
+  uses: actions/upload-pages-artifact@v2
 ```
 
 This actions defaults to uploading `_site`, but you can give any `with: path:`
 if you want, including `"."` which is the whole repository.
 
 Finally, you'll need to deploy the artifact (named `github-pages`) to Pages. You
 can make this a custom job with `needs:` pointing at your previous job (in this
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.8.3/docs/pages/guides/gha_pure.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.8.3/docs/pages/guides/gha_wheels.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,23 @@
 ```yaml
 build_wheels:
   name: Wheel on ${{ matrix.os }}
   runs-on: ${{ matrix.os }}
   strategy:
     fail-fast: false
     matrix:
-      os: [ubuntu-20.04, windows-2019, macos-10.15]
+      os: [ubuntu-latest, windows-latest, macos-latest]
 
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.13.1
+    - uses: pypa/cibuildwheel@v2.14
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 ```
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/index.md` & `sp_repo_review-2023.8.3/docs/pages/guides/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 {: .highlight-title }
 
 > New project template
 >
 > Once you have completed the guidelines, there is a
 > [copier][]/[cookiecutter][]/[cruft][] project, [scientific-python/cookie][],
 > that implements these guidelines and lets you setup a new package from a
-> template in less than 60 seconds! Twelve build backends including compiled
+> template in less than 60 seconds! Eleven build backends including compiled
 > backends, generation tested in Nox, and kept in-sync with the guide.
 
 {: .important-title }
 
 > Checking an existing project
 >
 > We provide [sp-repo-review][], a set of [repo-review][] checks for comparing
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/mypy.md` & `sp_repo_review-2023.8.3/docs/pages/guides/mypy.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.8.3/docs/pages/guides/packaging_classic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/packaging_compiled.md` & `sp_repo_review-2023.8.3/docs/pages/guides/packaging_compiled.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 ## Tool section in pyproject.toml
 
 These tools all read the project table. They also have extra configuration
 options in `tool.*` settings.
 
 <!-- [[[cog
-from cog_helpers import render_cookie
+from cog_helpers import code_fence, render_cookie
 with render_cookie(backend="skbuild") as skbuild:
     skbuild_cmakelists_txt = skbuild.joinpath("CMakeLists.txt").read_text(encoding="utf-8").strip()
     skbuild_src_main_cpp = skbuild.joinpath("src/main.cpp").read_text(encoding="utf-8").strip()
 with render_cookie(backend="mesonpy") as mesonpy:
     mesonpy_meson_build = mesonpy.joinpath("meson.build").read_text(encoding="utf-8").strip()
     mesonpy_src_main_cpp = mesonpy.joinpath("src/main.cpp").read_text(encoding="utf-8").strip()
 with render_cookie(backend="maturin") as maturin:
@@ -95,45 +95,45 @@
 ]]] -->
 <!-- [[[end]]] -->
 
 ## Backend specific files
 
 {% tabs %} {% tab skbc Scikit-build-core %}
 
-Example `CMakeLists.txt` file:
+Example `CMakeLists.txt` file (using pybind11, so include `pybind11` in
+`build-system.requires` too):
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```cmake")
-print(skbuild_cmakelists_txt)
-print("```")
+with code_fence("cmake"):
+    print(skbuild_cmakelists_txt)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```cmake
 cmake_minimum_required(VERSION 3.15...3.26)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES CXX)
 
 set(PYBIND11_FINDPYTHON ON)
 find_package(pybind11 CONFIG REQUIRED)
 
 pybind11_add_module(_core MODULE src/main.cpp)
 install(TARGETS _core DESTINATION ${SKBUILD_PROJECT_NAME})
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% tab meson Meson-python %}
 
-Example `meson.build` file:
+Example `meson.build` file (using pybind11, so include `pybind11` in
+`build-system.requires` too):
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```meson")
-print(mesonpy_meson_build)
-print("```")
+with code_fence("meson"):
+    print(mesonpy_meson_build)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```meson
 project(
   'package',
   'cpp',
   version: '0.1.0',
   license: 'BSD',
   meson_version: '>= 0.64.0',
@@ -162,67 +162,62 @@
     dependencies : [pybind11],
     link_language : 'cpp',
     override_options: [
         'cpp_rtti=true',
     ]
 )
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% tab maturin Maturin %}
 
-<!-- prettier-ignore-start -->
+Example `Cargo.toml` file:
+
 <!-- [[[cog
-print("```toml")
-print(maturin_cargo_toml)
-print("```")
+with code_fence("toml"):
+    print(maturin_cargo_toml)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```toml
 [package]
 name = "package"
 version = "0.1.0"
 edition = "2018"
 
 [lib]
 name = "_core"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
-[package.metadata.maturin]
-name = "package._core"
-python-packages = ["package"]
-python-source = "src"
-
 [dependencies]
 rand = "0.8.3"
 
 [dependencies.pyo3]
-version = "0.18.1"
+version = "0.19.1"
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 features = ["extension-module", "abi3-py38"]
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% endtabs %}
 
 ## Example compiled file
 
 {% tabs %} {% tab skbc Scikit-build-core %}
 
 Example `src/main.cpp` file:
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```cpp")
-print(skbuild_src_main_cpp)
-print("```")
+with code_fence("cpp"):
+    print(skbuild_src_main_cpp)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```cpp
 #include <pybind11/pybind11.h>
 
 int add(int i, int j) { return i + j; }
 
 namespace py = pybind11;
 
@@ -245,27 +240,26 @@
   m.def(
       "subtract", [](int i, int j) { return i - j; }, R"pbdoc(
       Subtract two numbers
       Some other explanation about the subtract function.
   )pbdoc");
 }
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% tab meson Meson-python %}
 
 Example `src/main.cpp` file:
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```cpp")
-print(mesonpy_src_main_cpp)
-print("```")
+with code_fence("cpp"):
+    print(mesonpy_src_main_cpp)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```cpp
 #include <pybind11/pybind11.h>
 
 int add(int i, int j) { return i + j; }
 
 namespace py = pybind11;
 
@@ -288,25 +282,24 @@
   m.def(
       "subtract", [](int i, int j) { return i - j; }, R"pbdoc(
       Subtract two numbers
       Some other explanation about the subtract function.
   )pbdoc");
 }
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% tab maturin Maturin %}
 
-<!-- prettier-ignore-start -->
 <!-- [[[cog
-print("```rs")
-print(maturin_src_lib_rs)
-print("```")
+with code_fence("rs"):
+    print(maturin_src_lib_rs)
 ]]] -->
+<!-- prettier-ignore-start -->
 ```rs
 use pyo3::prelude::*;
 
 #[pyfunction]
 fn add(x: i64, y: i64) -> i64 {
     x + y
 }
@@ -324,16 +317,16 @@
     m.add_function(wrap_pyfunction!(add, m)?)?;
     m.add_function(wrap_pyfunction!(subtract, m)?)?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
 
     Ok(())
 }
 ```
-<!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 {% endtab %} {% endtabs %}
 
 ## Package structure
 
 The recommendation (followed above) is to have source code in `/src`, and the
 Python package files in `/src/<package>`.
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2023.8.3/docs/pages/guides/packaging_simple.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 Python packages can now use a modern build system instead of the classic but
 verbose setuptools and `setup.py`. The one you select doesn't really matter that
 much; they all use a [standard configuration language][metadata] introduced in
 [PEP 621][]. The PyPA's Flit is a great option. [scikit-build-core][] and
 [meson-python][] are being developed to support this sort of configuration,
 enabling binary extension packages to benefit too. These [PEP 621][] tools
-currently include [Hatch][], [PDM][], [Flit][], [Trampolim][], [Whey][], and
-[Setuptools][]. [Poetry][] will eventually gain support in 2.0.
+currently include [Hatch][], [PDM][], [Flit][], [Whey][], and [Setuptools][].
+[Poetry][] will eventually gain support in 2.0.
 
 {: .note-title }
 
 > Classic files
 >
 > These systems do not use or require `setup.py`, `setup.cfg`, or `MANIFEST.in`.
 > Those are for setuptools. Unless you are using setuptools, of course, which
@@ -87,15 +87,15 @@
 have a `src` folder! However, this is a bad practice, and it causes several
 common bugs, such as running `pytest` and getting the local version instead of
 the installed version - this obviously tends to break if you build parts of the
 library or if you access package metadata.
 
 This sadly is not part of the standard metadata in `[project]`, so it depends on
 what backend you you use. Hatchling, Flit, PDM, and setuptools use automatic
-detection, while Trampolim and whey do not, requiring a `tool` setting.
+detection, while Whey does not, requiring a `tool` setting.
 
 If you don't match your package name and import name (which you should except
 for very special cases), you will likely need extra configuration here.
 
 You should have a `README` {% rr PY002 %} and a `LICENSE` {% rr PY003 %} file.
 You should have a `docs/` folder {%
 rr PY003 %}. You should have a `/tests` folder (recommended) and/or a `src/<package>/tests`
@@ -165,15 +165,15 @@
 
 - [Hatchling info here](https://hatch.pypa.io/latest/config/build/#file-selection).
   Hatchling uses your VCS ignore file by default, so make sure it is accurate
   (which is a good idea anyway).
 - [Flit info here](https://flit.readthedocs.io/en/latest/pyproject_toml.html#sdist-section).
   Flit requires manual inclusion/exclusion in many cases, like using a dirty
   working directory.
-- [PDM info here](https://pdm.fming.dev/pyproject/tool-pdm/#include-and-exclude-package-files).
+- [PDM info here](https://pdm-backend.fming.dev/build_config/#include-or-exclude-files).
 - Setuptools still uses `MANIFEST.in`.
 
 {: .warning }
 
 > Flit will not use VCS (like git) to populate the SDist if you use standard
 > tooling, even if it can do that using its own tooling. So make sure you list
 > explicit include/exclude rules, and test the contents:
@@ -186,15 +186,14 @@
 > ```
 
 <!-- prettier-ignore-start -->
 
 [flit]: https://flit.readthedocs.io
 [poetry]: https://python-poetry.org
 [pdm]: https://pdm.fming.dev
-[trampolim]: https://github.com/FFY00/trampolim
 [whey]: https://whey.readthedocs.io
 [hatch]: https://hatch.pypa.io/latest
 [setuptools]: https://setuptools.readthedocs.io
 [pep 621]: https://www.python.org/dev/peps/pep-0621
 [scikit-build-core]: https://scikit-build-core.readthedocs.io
 [meson-python]: https://meson-python.readthedocs.io
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/pytest.md` & `sp_repo_review-2023.8.3/docs/pages/guides/pytest.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.8.3/docs/pages/guides/repo_review.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/style.md` & `sp_repo_review-2023.8.3/docs/pages/guides/style.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 normalization, and to change the line length, and those go in your
 `pyproject.toml` file.
 
 Here is the snippet to add Black to your `.pre-commit-config.yml`:
 
 ```yaml
 - repo: https://github.com/psf/black
-  rev: "23.3.0"
+  rev: "23.7.0"
   hooks:
     - id: black
 ```
 
 {% details You can add a Black badge to your repo as well %}
 
 ```md
@@ -137,18 +137,18 @@
 {% rr PC111 %} If you want Black used in your documentation, you can use
 blacken-docs. This can even catch syntax errors in code snippets! It supports
 markdown and restructured text. Note that because black is in
 `additional_dependencies`, you'll have to keep it up to date manually.
 
 ```yaml
 - repo: https://github.com/asottile/blacken-docs
-  rev: "1.14.0"
+  rev: "1.15.0"
   hooks:
     - id: blacken-docs
-      additional_dependencies: [black==23.3.0]
+      additional_dependencies: [black==23.7.0]
 ```
 
 {% enddetails %}
 
 ## Ruff
 
 {% rr PC190 %} [Ruff][] [(docs)][ruff docs] is a Python code linter and
@@ -158,15 +158,15 @@
 pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
 [ruff]: https://github.com/astral-sh/ruff
 
 ```yaml
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.0.276"
+  rev: "v0.0.280"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
 {% rr PC191 %} The `--fix` argument is optional, but recommended, since you can
 inspect and undo changes in git.
@@ -293,15 +293,15 @@
 [PyCln][] will clean up your imports if you have any that are not needed. There
 is a Flake8 check for this, but it's usually nicer to automatically do the
 cleanup instead of forcing a user to manually delete unneeded imports. If you
 use the manual stage, it's opt-in instead of automatic.
 
 ```yaml
 - repo: https://github.com/hadialqattan/pycln
-  rev: "v2.1.5"
+  rev: "v2.1.7"
   hooks:
     - id: pycln
       args: [--all]
       stages: [manual]
 ```
 
 ### Flake8
@@ -333,15 +333,15 @@
 ```
 
 (Error E722 is important, but it is identical to the activated B001.) Here is
 the flake8 addition for pre-commit, with the `bugbear` plugin:
 
 ```yaml
 - repo: https://github.com/pycqa/flake8
-  rev: "6.0.0"
+  rev: "6.1.0"
   hooks:
     - id: flake8
       additional_dependencies: [flake8-bugbear]
 ```
 
 This _will_ be too much at first, so you can disable or enable any test by it's
 label. You can also disable a check or a list of checks inline with
@@ -431,21 +431,21 @@
 style syntax. Most useful to keep Python 2 outdated constructs out, it can even
 do some code updates for different versions of Python 3, like adding f-strings
 when clearly better (please always use them, they are faster) if you set
 `--py36-plus` (for example). This is a recommended addition for any project.
 
 ```yaml
 - repo: https://github.com/asottile/pyupgrade
-  rev: "v3.8.0"
+  rev: "v3.10.1"
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 ```
 
-[pyupgrade]: https://github.com/asottile/pyupgrade:
+[pyupgrade]: https://github.com/asottile/pyupgrade
 
 {: .note }
 
 > If you set this to at least `--py37-plus`, you can add the annotations import
 > by adding the following line to your isort pre-commit hook configuration:
 >
 > ```yaml
@@ -710,15 +710,15 @@
 ## Prettier
 
 {% rr PC180 %} The [prettier](https://prettier.io) tool can format a large
 number of different file types. An example of usage:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-prettier
-  rev: "v2.7.1"
+  rev: "v3.0.0"
   hooks:
     - id: prettier
       types_or: [yaml, markdown, html, css, scss, javascript, json]
 ```
 
 Since this formats a variety of very common file types (like `.html`, `.md`,
 `.yaml`, `.js`, and `.json`), you will usually want to provide a `types_or`
@@ -761,17 +761,17 @@
 ```
 
 And a noxfile entry:
 
 ```python
 @nox.session
 def pylint(session: nox.Session) -> None:
-    session.install("-e", ".")
+    session.install("-e.")
     session.install("pylint")
-    session.run("pylint", "src", *session.posargs)
+    session.run("pylint", "<your package>", *session.posargs)
 ```
 
 And you can add this to your GitHub Actions using `run: pipx run nox -s pylint`.
 You can replace `src` with the module name.
 
 ## Jupyter notebook support
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/guides/tasks.md` & `sp_repo_review-2023.8.3/docs/pages/guides/tasks.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
 # Task runners
 
+<!-- [[[cog
+from cog_helpers import  code_fence, render_cookie, Matcher
+with render_cookie() as package:
+    noxfile = Matcher.from_file(package / "noxfile.py")
+]]] -->
+<!-- [[[end]]] -->
+
 A task runner, like [make][] (fully general), [rake][] (Ruby general),
 [invoke][] (Python general), [tox][] (Python packages), or [nox][] (Python
 simi-general), is a tool that lets you specify a set of tasks via a common
 interface. These have been discouraged by some community projects in the past,
 since they can be a crutch, allowing poor packaging practices to be employed
 behind a custom script, and they can hide what is actually happening.
 
@@ -58,24 +65,24 @@
 `nox`.
 
 On GitHub Actions or Azure, pipx is available by default, so you should use
 `pipx run nox`. To give it access to all Python versions, you can use this
 action:
 
 ```yaml
-- uses: wntrblm/nox@2022.8.7
+- uses: wntrblm/nox@v0.19.1
 ```
 
 You can now access all current versions of Python from nox. At least in GitHub
 Actions, you should add `--forcecolor` to your nox runs to get color output in
 your logs, or set `env: FORCE_COLOR: 3`. If you'd like to customise the versions
 of Python prepared for you, then use this input:
 
 ```yaml
-- uses: wntrblm/nox@2022.8.7
+- uses: wntrblm/nox@v0.19.1
   with:
     python-versions: "3.8, 3.9, 3.10, 3.11, 3.12, pypy-3.9, pypy-3.10-nightly"
 ```
 
 ### Introduction
 
 Nox is a tool for running tasks, called "sessions", inside temporary virtual
@@ -165,87 +172,128 @@
 will likely look similar across different projects:
 
 #### Lint
 
 Ideally, all developers should be using pre-commit directly, but this helps new
 users.
 
+<!-- [[[cog
+with code_fence("python"):
+    print(noxfile.get_source("lint"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
     session.install("pre-commit")
     session.run(
-        "pre-commit", "run", "--show-diff-on-failure", "--all-files", *session.posargs
+        "pre-commit", "run", "--all-files", "--show-diff-on-failure", *session.posargs
     )
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 #### Tests
 
+<!-- [[[cog
+with code_fence("python"):
+    print(noxfile.get_source("tests"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
-import nox
-
-
 @nox.session
 def tests(session: nox.Session) -> None:
     """
     Run the unit and regular tests.
     """
     session.install(".[test]")
     session.run("pytest", *session.posargs)
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 #### Docs
 
+<!-- [[[cog
+with code_fence("python"):
+    print(noxfile.get_source("docs"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "--serve" to serve.
+    Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
+    parser.add_argument(
+        "-b", dest="builder", default="html", help="Build target (default: html)"
+    )
     args, posargs = parser.parse_known_args(session.posargs)
 
-    session.install("-e.[docs]")
+    if args.builder != "html" and args.serve:
+        session.error("Must not specify non-HTML builder with --serve")
+
+    extra_installs = ["sphinx-autobuild"] if args.serve else []
+
+    session.install("-e.[docs]", *extra_installs)
     session.chdir("docs")
 
-    session.run(
-        "sphinx-build",
+    if args.builder == "linkcheck":
+        session.run(
+            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
+        )
+        return
+
+    shared_args = (
         "-n",  # nitpicky mode
-        "--keep-going",  # show all errors
         "-T",  # full tracebacks
-        "-b",
-        "html",
+        f"-b={args.builder}",
         ".",
-        f"_build/html",
+        f"_build/{args.builder}",
         *posargs,
     )
 
     if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
-        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+        session.run("sphinx-autobuild", *shared_args)
+    else:
+        session.run("sphinx-build", "--keep-going", *shared_args)
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 This supports setting up a quick server as well, run like this:
 
 ```console
 $ nox -s docs -- --serve
 ```
 
 #### Build (pure Python)
 
 For pure Python packages, this could be useful:
 
+<!-- [[[cog
+with code_fence("python"):
+    print("import shutil")
+    print("from pathlib import Path")
+    print()
+    print("DIR = Path(__file__).parent.resolve()")
+    print()
+    print()
+    print(noxfile.get_source("build"))
+]]] -->
+<!-- prettier-ignore-start -->
 ```python
-from pathlib import Path
 import shutil
+from pathlib import Path
 
 DIR = Path(__file__).parent.resolve()
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
@@ -255,14 +303,16 @@
     build_path = DIR.joinpath("build")
     if build_path.exists():
         shutil.rmtree(build_path)
 
     session.install("build")
     session.run("python", "-m", "build")
 ```
+<!-- prettier-ignore-end -->
+<!-- [[[end]]] -->
 
 ### Examples
 
 A standard
 [powered by nox](https://github.com/scikit-hep/hist/blob/main/noxfile.py)
 package in Pure Python can be found in the Hist project of Scikit-HEP.
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/patterns/backports.md` & `sp_repo_review-2023.8.3/docs/pages/patterns/backports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.8.3/docs/pages/patterns/data_files.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/patterns/exports.md` & `sp_repo_review-2023.8.3/docs/pages/patterns/exports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/patterns/index.md` & `sp_repo_review-2023.8.3/docs/pages/patterns/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/principles/design.md` & `sp_repo_review-2023.8.3/docs/pages/principles/design.md`

 * *Files 1% similar despite different names*

```diff
@@ -265,10 +265,10 @@
 exercising some restraint and consistency with the scientific Python ecosystem,
 Python can be used to build scientific tools that last and grow well over time.
 
 <!-- prettier-ignore-start -->
 
 [the UNIX philosophy]: https://en.wikipedia.org/wiki/Unix_philosophy
 [Duck typing]: https://en.wikipedia.org/wiki/Duck_typing
-["Stop Writing Classes"]: https:k//www.youtube.com/watch?v=o9pEzgHorH0&t=193s
+["Stop Writing Classes"]: https://youtube.com/watch?v=o9pEzgHorH0&t=193s
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/principles/index.md` & `sp_repo_review-2023.8.3/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/principles/process.md` & `sp_repo_review-2023.8.3/docs/pages/principles/process.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/dev-environment.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/index.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/module.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/module.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/packaging.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 Place `refraction.py`, our code from the previous section, next to it, at
 `src/refraction.py`.
 
 The last element your package needs is a `pyproject.toml` file, placed in the
 root directory.
 
 ```bash
-touch pyproject.yaml
+touch pyproject.toml
 ```
 
 Fill in the minimally required metadata, which includes the package name,
 version, and some options related to how to install it, which you can copy as
 is.
 
 ```bash
```

### Comparing `sp_repo_review-2023.7.6/docs/pages/tutorials/test.md` & `sp_repo_review-2023.8.3/docs/pages/tutorials/test.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/helpers/extensions.py` & `sp_repo_review-2023.8.3/helpers/extensions.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/readthedocs.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/readthedocs.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.8.3/src/sp_repo_review/checks/ruff.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 class RF1xx(Ruff):
     family = "ruff"
     requires = {"RF001"}
 
     @classmethod
     def check(cls: type[RuffMixin], pyproject: dict[str, Any]) -> bool:
         """
-        Must select the {cls.name} `{cls.code}` checks. Recommended:
+        Must select the {self.name} `{self.code}` checks. Recommended:
         ```toml
-        select = ["{cls.code}"]  # {cls.name}
+        select = ["{self.code}"]  # {self.name}
         ```
         """
 
         match pyproject:
             case {"tool": {"ruff": {"select": list(x)}}} | {
                 "tool": {"ruff": {"extend-select": list(x)}}
             }:
```

### Comparing `sp_repo_review-2023.7.6/tests/test_package.py` & `sp_repo_review-2023.8.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.3.0"
+    rev: "23.7.0"
     hooks:
       - id: black-jupyter
 
+  - repo: https://github.com/asottile/blacken-docs
+    rev: "1.15.0"
+    hooks:
+      - id: blacken-docs
+        additional_dependencies: [black==23.7.0]
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
@@ -28,28 +34,22 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v2.7.1"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
-  - repo: https://github.com/asottile/blacken-docs
-    rev: "1.14.0"
-    hooks:
-      - id: blacken-docs
-        additional_dependencies: [black==23.3.0]
-
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.276"
+    rev: "v0.0.280"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
 {%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
 
   - repo: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,78 +18,79 @@
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
     session.install("pre-commit")
-    session.run("pre-commit", "run", "--all-files", *session.posargs)
+    session.run(
+        "pre-commit", "run", "--all-files", "--show-diff-on-failure", *session.posargs
+    )
 
 
 @nox.session
 def pylint(session: nox.Session) -> None:
     """
     Run PyLint.
     """
     # This needs to be installed into the package environment, and is slower
     # than a pre-commit check
     session.install(".", "pylint")
-    session.run("pylint", "src", *session.posargs)
+    session.run("pylint", "{{ cookiecutter.__project_slug }}", *session.posargs)
 
 
 @nox.session
 def tests(session: nox.Session) -> None:
     """
-    Run the unit and regular tests. Use --cov to activate coverage.
+    Run the unit and regular tests.
     """
     session.install(".[test]")
     session.run("pytest", *session.posargs)
 
 
-@nox.session
+@nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "--serve" to serve.
+    Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
     parser.add_argument(
         "-b", dest="builder", default="html", help="Build target (default: html)"
     )
     args, posargs = parser.parse_known_args(session.posargs)
 
     if args.builder != "html" and args.serve:
         session.error("Must not specify non-HTML builder with --serve")
 
-    session.install(".[docs]")
+    extra_installs = ["sphinx-autobuild"] if args.serve else []
+
+    session.install("-e.[docs]", *extra_installs)
     session.chdir("docs")
 
     if args.builder == "linkcheck":
         session.run(
             "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
         )
         return
 
-    session.run(
-        "sphinx-build",
+    shared_args = (
         "-n",  # nitpicky mode
         "-T",  # full tracebacks
-        "-W",  # Warnings as errors
-        "--keep-going",  # See all errors
-        "-b",
-        args.builder,
+        f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
     if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
-        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+        session.run("sphinx-autobuild", *shared_args)
+    else:
+        session.run("sphinx-build", "--keep-going", *shared_args)
 
 
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
     Build (regenerate) API docs.
     """
@@ -112,15 +113,15 @@
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
 
-    build_p = DIR.joinpath("build")
-    if build_p.exists():
-        shutil.rmtree(build_p)
+    build_path = DIR.joinpath("build")
+    if build_path.exists():
+        shutil.rmtree(build_path)
 
     session.install("build")
     session.run("python", "-m", "build")
 
 {%- endif %}
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 [build-system]
-{%- if cookiecutter.backend == "trampolim" %}
-requires = ["trampolim>=0.1.0"]
-build-backend = "trampolim"
-{%- elif cookiecutter.backend == "whey" %}
+{%- if cookiecutter.backend == "whey" %}
 requires = ["whey>=0.0.17"]
 build-backend = "whey"
 {%- elif cookiecutter.backend == "pdm" %}
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
 {%- elif cookiecutter.backend == "maturin" %}
-requires = ["maturin>=0.12,<0.15"]
+requires = ["maturin>=0.15,<2"]
 build-backend = "maturin"
 {%- elif cookiecutter.backend == "hatch" %}
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 {%- elif cookiecutter.backend == "setuptools621" %}
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 {%- elif cookiecutter.backend == "flit" %}
-requires = ["flit_core >=3.4"]
+requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 {%- elif cookiecutter.backend == "setuptools" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
 {%- elif cookiecutter.backend == "pybind11" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4", "pybind11"]
 build-backend = "setuptools.build_meta"
 {%- elif cookiecutter.backend == "skbuild"  %}
 requires = ["pybind11", "scikit-build-core"]
 build-backend = "scikit_build_core.build"
 {%- elif cookiecutter.backend == "mesonpy"  %}
-requires = ["pybind11", "meson-python"]
+requires = ["meson-python", "pybind11"]
 build-backend = "mesonpy"
 {%- elif cookiecutter.backend == "poetry" %}
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 {%- endif %}
 
 {%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
@@ -87,15 +84,14 @@
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-typing_extensions = { version = ">=4.6", python = "<3.11" }
 
 furo = { version = ">=22", optional = true }
 myst_parser = { version = ">=0.13", optional = true }
 pytest = { version = ">=6", optional = true }
 pytest-cov = { version = ">=3", optional = true }
 sphinx = { version = ">=4.0", optional = true }
 sphinx_copybutton = { version = ">=0.3.0", optional = true }
@@ -118,15 +114,15 @@
 
 
 {%- else %}
 
 
 [project]
 name = "{{ cookiecutter.project_name }}"
-{%- if cookiecutter.backend not in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.backend not in ["flit", "hatch"] %}
 version = "0.1.0"
 {%- endif %}
 authors = [
   { name = "{{ cookiecutter.full_name }}", email = "{{ cookiecutter.email }}" },
 ]
 {%- if cookiecutter.org | lower == "scikit-hep" %}
 maintainers = [
@@ -155,20 +151,18 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
-{%- if cookiecutter.backend in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.backend in ["flit", "hatch"] %}
 dynamic = ["version"]
 {%- endif %}
-dependencies = [
-  "typing_extensions >=4.6; python_version<'3.11'",
-]
+dependencies = []
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
@@ -189,43 +183,70 @@
 "Bug Tracker" = "{{ cookiecutter.url }}/issues"
 Discussions = "{{ cookiecutter.url }}/discussions"
 Changelog = "{{ cookiecutter.url }}/releases"
 {%- endif %}
 
 
 {%- if cookiecutter.backend == "skbuild" %}
+
+
 [tool.scikit-build]
-minimum-version = "0.2"
-build-dir = "build/{cache_tag}"
+minimum-version = "0.4"
+build-dir = "build/{wheel_tag}"
+
 {%- elif cookiecutter.backend == "whey" %}
+
+
 [tool.whey]
 source-dir = "src"
-{%- elif cookiecutter.backend == "trampolim" %}
-[tool.trampolim]
-module-location = "src"
+
+{%- elif cookiecutter.backend == "maturin" %}
+
+
+[tool.maturin]
+module-name = "{{ cookiecutter.__project_slug }}._core"
+python-packages = ["{{ cookiecutter.__project_slug }}"]
+python-source = "src"
+sdist-generator = "git"  # default is cargo
+
 {%- elif cookiecutter.backend == "hatch" %}
+
+
 [tool.hatch]
 version.path = "src/{{ cookiecutter.__project_slug  }}/__init__.py"
 envs.default.dependencies = [
   "pytest",
   "pytest-cov",
 ]
+
 {%- elif cookiecutter.backend == "pdm" %}
+
+
 [tool.pdm.dev-dependencies]
 devtest = ["pytest", "pytest-cov"]
+
+{%- endif %}
+
+
+{%- if cookiecutter.__type == "compiled" %}
+
+
+[tool.cibuildwheel]
+test-command = "pytest {project}/tests"
+test-extras = ["test"]
+test-skip = ["*universal2:arm64"]
 {%- endif %}
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
   "error",
-  "ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest",
 ]
 log_cli_level = "INFO"
 testpaths = [
   "tests",
 ]
 
 
@@ -283,32 +304,36 @@
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
 ]
 {%- if cookiecutter.backend in ["setuptools", "pybind11", "poetry"] %}
 target-version = "py38"
 {%- endif %}
-typing-modules = ["{{ cookiecutter.__project_slug }}._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
 isort.required-imports = ["from __future__ import annotations"]
+# Uncomment if using a _compat.typing backport
+# typing-modules = ["{{ cookiecutter.__project_slug }}._compat.typing"]
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
 
 
 [tool.pylint]
 py-version = "3.8"
-ignore-paths= ["src/{{ cookiecutter.__project_slug }}/_version.py"]
+ignore-paths = [".*/_version.py"]
+{%- if cookiecutter.__type == "compiled" %}
+extension-pkg-allow-list = ["{{ cookiecutter.__project_slug }}._core"]
+{%- endif %}
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.__ci == 'gitlab' %}.gitlab-ci.yml{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}`

 * *Files 11% similar despite different names*

```diff
@@ -77,39 +77,35 @@
     - python -V
     - python -m pip install .[test]
     - python -m pytest -ra --cov={{ cookiecutter.project_name }}
   parallel:
     matrix:
       - IMAGE: ['python:3.8-buster', 'python:3.11-buster']
 
-{%- if not cookiecutter.__compiled %}
+{%- if cookiecutter.__type == "pure" %}
 package:
   stage: build
   rules:
     - if: $CI_PIPELINE_SOURCE == "push"
   script:
     - pipx run build
-    {%- if cookiecutter.project_type != "trampolim" %}
     - pipx run twine check dist/*
-    {%- endif %}
   artifacts:
     paths:
       - dist/
     expire_in: 1 day
 
 {%- else %}
 make_sdist:
   stage: build
   rules:
     - if: $CI_PIPELINE_SOURCE == "push"
   script:
     - pipx run build --sdist
-    {%- if cookiecutter.project_type != "trampolim" %}
     - pipx run twine check dist/*
-    {%- endif %}
   artifacts:
     paths:
       - dist/*.tar.gz
     expire_in: 1 day
 
 make_wheels:
   stage: build
@@ -141,15 +137,15 @@
     paths:
       - dist/*.whl
     expire_in: 1 day
 
 .deploy:
   stage: deploy
   dependencies:
-    {%- if not cookiecutter.__compiled %}
+    {%- if cookiecutter.__type == "pure" %}
     - package
     {%- else %}
     - make_sdist
     - make_wheels
     {%- endif %}
   script:
     - pipx run twine upload --verbose dist/*whl dist/*gz
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,70 @@
-{%- set compiled = cookiecutter.backend in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
-name: CI
+name: wheels
 
 on:
   workflow_dispatch:
-  pull_request:
-  push:
-    branches:
-      - master
-      - main
-      - develop
-  {%- if not compiled %}
   release:
     types:
       - published
-  {%- endif %}
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 3
 
 jobs:
-  pre-commit:
-    name: Format
+  make_sdist:
+    name: Make SDist
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - uses: pre-commit/action@v3.0.0
-        with:
-          extra_args: --hook-stage manual --all-files
-      - name: Run PyLint
-        run: |
-          echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
-          pipx run nox -s pylint
-
-  checks:
-    name: {% raw %}Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}{% endraw %}
-    runs-on: {% raw %}${{ matrix.runs-on }}{% endraw %}
-    needs: [pre-commit]
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.8", "3.11", "3.12"]
-        runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
-        include:
-          - python-version: pypy-3.9
-            runs-on: ubuntu-latest
+      - name: Build SDist
+        run: pipx run build --sdist
 
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-
-      - uses: actions/setup-python@v4
+      - uses: actions/upload-artifact@v3
         with:
-          python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
-          allow-prereleases: true
-
-      {%- if cookiecutter.backend == "mesonpy" %}
-      - name: Activate MSVC for Meson
-        if: runner.os == 'Windows'
-        uses: ilammy/msvc-dev-cmd@v1
-      {%- endif %}
-
-      - name: Install package
-        run: python -m pip install .[test]
+          path: dist/*.tar.gz
 
-      - name: Test package
-        run: >-
-          python -m pytest -ra --cov --cov-report=xml --cov-report=term
-          --durations=20
-
-      - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
-
-  {%- if not compiled %}
-
-  dist:
-    needs: [pre-commit]
-    name: Distribution build
-    runs-on: ubuntu-latest
+  build_wheels:
+    name: {% raw %}Wheel on ${{ matrix.os }}{% endraw %}
+    runs-on: {% raw %}${{ matrix.os }}{% endraw %}
+    strategy:
+      fail-fast: false
+      matrix:
+        os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - name: Build sdist and wheel
-        run: pipx run build
+      - uses: pypa/cibuildwheel@v2.14
 
-      - uses: actions/upload-artifact@v3
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
         with:
-          path: dist
-
-      {%- if cookiecutter.backend != "trampolim" %}
+          path: wheelhouse/*.whl
 
-      - name: Check products
-        run: pipx run twine check dist/*
-
-      {%- endif %}
-
-  publish:
-    needs: [dist]
-    name: Publish to PyPI
+  upload_all:
+    needs: [build_wheels, make_sdist]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
-        if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
-          {%- if cookiecutter.backend == "trampolim" %}
-          # Check not supported currently by twine + trampolim
-          verify-metadata: false
-          {%- endif %}
-
-  {%- endif %}
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,61 @@
-name: wheels
+name: CD
 
 on:
   workflow_dispatch:
+  pull_request:
+  push:
+    branches:
+      - main
   release:
     types:
       - published
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 3
 
 jobs:
-  make_sdist:
-    name: Make SDist
+  dist:
+    needs: [pre-commit]
+    name: Distribution build
     runs-on: ubuntu-latest
+
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - name: Build SDist
-        run: pipx run build --sdist
+      - name: Build sdist and wheel
+        run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
-          path: dist/*.tar.gz
-
-  build_wheels:
-    name: {% raw %}Wheel on ${{ matrix.os }}{% endraw %}
-    runs-on: {% raw %}${{ matrix.os }}{% endraw %}
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
-
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-
-      - uses: pypa/cibuildwheel@v2.13.1
+          path: dist
 
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          path: wheelhouse/*.whl
+      - name: Check products
+        run: pipx run twine check dist/*
 
-  upload_all:
-    needs: [build_wheels, make_sdist]
+  publish:
+    needs: [dist]
+    name: Publish to PyPI
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
+        if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
```

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/conf.py` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}` & `sp_repo_review-2023.8.3/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/.gitignore` & `sp_repo_review-2023.8.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -148,7 +148,10 @@
 # NodeJS stuff, just in case (developer tooling)
 node_modules/
 package-lock.json
 package.json
 
 # readthedocs
 _readthedocs
+
+# Default cookiecutter output
+/package
```

### Comparing `sp_repo_review-2023.7.6/LICENSE` & `sp_repo_review-2023.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.6/pyproject.toml` & `sp_repo_review-2023.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed",
 ]
 dynamic = ["version", "readme"]
 dependencies = [
   "pyyaml",
-  "repo-review>=0.7,<0.9",
+  "repo-review>=0.7,<0.10",
 ]
 
 [project.optional-dependencies]
 cli = [
   "repo-review[cli]",
 ]
 test = [
@@ -67,15 +67,15 @@
 [project.entry-points."repo_review.fixtures"]
 workflows = "sp_repo_review.checks.github:workflows"
 dependabot = "sp_repo_review.checks.github:dependabot"
 precommit = "sp_repo_review.checks.precommit:precommit"
 readthedocs = "sp_repo_review.checks.readthedocs:readthedocs"
 
 [project.entry-points."repo_review.families"]
-scikit-hep = "sp_repo_review.families:get_familes"
+scikit-hep = "sp_repo_review.families:get_families"
 
 
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/sp_repo_review/_version.py"
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
```

### Comparing `sp_repo_review-2023.7.6/PKG-INFO` & `sp_repo_review-2023.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sp_repo_review
-Version: 2023.7.6
+Version: 2023.8.3
 Summary: Review repos for compliance to the Scientific-Python development guidelines
 Project-URL: Guide, https://learn.scientific-python.org/development
 Project-URL: Homepage, https://scientific-python.github.io/cookie
 Project-URL: Preview, https://scientific-python-cookie.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/cookie
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: pyyaml
-Requires-Dist: repo-review<0.9,>=0.7
+Requires-Dist: repo-review<0.10,>=0.7
 Provides-Extra: cli
 Requires-Dist: repo-review[cli]; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: pytest>=7; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
```

