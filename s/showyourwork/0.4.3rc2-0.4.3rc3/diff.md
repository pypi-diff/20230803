# Comparing `tmp/showyourwork-0.4.3rc2.tar.gz` & `tmp/showyourwork-0.4.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showyourwork-0.4.3rc2.tar", last modified: Wed May  3 12:48:03 2023, max compression
+gzip compressed data, was "showyourwork-0.4.3rc3.tar", last modified: Thu Aug  3 11:58:30 2023, max compression
```

## Comparing `showyourwork-0.4.3rc2.tar` & `showyourwork-0.4.3rc3.tar`

### file list

```diff
@@ -1,196 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/actions_tab.png
--rw-r--r--   0 runner    (1001) docker     (123)   204092 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/article-abstract.png
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/badges.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   425530 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/default_ms.png
--rw-r--r--   0 runner    (1001) docker     (123)   540973 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/default_ms_with_figure.png
--rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   427880 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)   147093 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/workflow_permissions.png
--rw-r--r--   0 runner    (1001) docker     (123)    57574 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/zenodo_dois.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/attribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    24716 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/contributorguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/hacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/integration_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/overleaf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/projects.json
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/projects.rst.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/quickbuild.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/reproducibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/snakefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/zenodo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork/_showyourwork_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/run_snakemake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/tarball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.563947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/process-pull-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.563947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    37916 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst
--rw-r--r--   0 runner    (1001) docker     (123)   238984 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex
--rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/showyourwork.sty
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/zenodo.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/gitapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/userrules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/build.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/envs/render_dag.yml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/envs/tectonic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/prep.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/report/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/report/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/report/workflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.567947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/article-thumb.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/build.tex
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/preprocess.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/
--rw-r--r--   0 runner    (1001) docker     (123)   149938 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/lineno.sty
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/listofitems.tex
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   689534 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork.otf
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.sty
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/arxiv.smk
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/common.smk
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/compile.smk
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/dag.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/figure.smk
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/preprocess.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/render_dag.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/zenodo.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/compile_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/render_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    38229 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.567947 showyourwork-0.4.3rc2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/helpers/temp_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/sandbox/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_cache_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_duplicate_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_letter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_missing_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_space_in_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/unit/test_overleaf_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.087131 showyourwork-0.4.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-03 11:58:30.087131 showyourwork-0.4.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.067131 showyourwork-0.4.3rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/actions_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204092 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/article-abstract.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/badges.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   425530 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/default_ms.png
+-rw-r--r--   0 runner    (1001) docker     (123)   540973 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/default_ms_with_figure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   406519 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   147093 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/workflow_permissions.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57574 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/_static/zenodo_dois.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/attribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25996 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/contributorguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/hacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/integration_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/overleaf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/projects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/projects.rst.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/quickbuild.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/reproducibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/snakefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/docs/zenodo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:58:30.087131 showyourwork-0.4.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/showyourwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork/_showyourwork_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/showyourwork/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/run_snakemake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/commands/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.059131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/process-pull-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.059131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    37916 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst
+-rw-r--r--   0 runner    (1001) docker     (123)   238984 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.075131 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/showyourwork.sty
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/zenodo.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/exceptions/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/gitapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/userrules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/build.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/envs/render_dag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/envs/tectonic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/prep.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/report/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/report/workflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.059131 showyourwork-0.4.3rc3/showyourwork/workflow/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/resources/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/img/article-thumb.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/styles/build.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/styles/preprocess.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.079131 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/
+-rw-r--r--   0 runner    (1001) docker     (123)   149938 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/lineno.sty
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/listofitems.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork-logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   689534 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/xstring.sty
+-rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/xstring.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/showyourwork/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/arxiv.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/common.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/compile.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/dag.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/figure.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/preprocess.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/render_dag.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/rules/zenodo.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/compile_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/copy_and_fix_synctex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/workflow/scripts/render_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38229 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/showyourwork/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.071131 showyourwork-0.4.3rc3/showyourwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-08-03 11:58:30.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 11:58:29.000000 showyourwork-0.4.3rc3/showyourwork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.063131 showyourwork-0.4.3rc3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/tests/integration/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/helpers/temp_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/tests/integration/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/sandbox/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_cache_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_duplicate_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_letter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_missing_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_space_in_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_synctex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/integration/test_zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:58:30.083131 showyourwork-0.4.3rc3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 11:58:16.000000 showyourwork-0.4.3rc3/tests/unit/test_overleaf_regex.py
```

### Comparing `showyourwork-0.4.3rc2/CITATION.cff` & `showyourwork-0.4.3rc3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/HISTORY.rst` & `showyourwork-0.4.3rc3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/LICENSE` & `showyourwork-0.4.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/PKG-INFO` & `showyourwork-0.4.3rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showyourwork
-Version: 0.4.3rc2
+Version: 0.4.3rc3
 Summary: A workflow for open-source scientific articles
 Home-page: https://github.com/showyourwork/showyourwork
 Author: Rodrigo Luger
 Author-email: rodluger@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc2 Summary: A workflow
+Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc3 Summary: A workflow
 for open-source scientific articles Home-page: https://github.com/showyourwork/
 showyourwork Author: Rodrigo Luger Author-email: rodluger@gmail.com License:
 MIT Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests License-File: LICENSE
                                 [showyourwork]
   [unit_tests] [local_integration_tests] [remote_integration_tests] [tests]
                            [sample_projects] [pypi]
```

### Comparing `showyourwork-0.4.3rc2/README.md` & `showyourwork-0.4.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/.gitignore` & `showyourwork-0.4.3rc3/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/Makefile` & `showyourwork-0.4.3rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/actions_tab.png` & `showyourwork-0.4.3rc3/docs/_static/actions_tab.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/article-abstract.png` & `showyourwork-0.4.3rc3/docs/_static/article-abstract.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/badges.png` & `showyourwork-0.4.3rc3/docs/_static/badges.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/css/custom.css` & `showyourwork-0.4.3rc3/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/default_ms.png` & `showyourwork-0.4.3rc3/docs/_static/default_ms.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/default_ms_with_figure.png` & `showyourwork-0.4.3rc3/docs/_static/default_ms_with_figure.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/logo.png` & `showyourwork-0.4.3rc3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/workflow_permissions.png` & `showyourwork-0.4.3rc3/docs/_static/workflow_permissions.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/_static/zenodo_dois.png` & `showyourwork-0.4.3rc3/docs/_static/zenodo_dois.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/api.rst` & `showyourwork-0.4.3rc3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/attribution.rst` & `showyourwork-0.4.3rc3/docs/attribution.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/cli.rst` & `showyourwork-0.4.3rc3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/conf.py` & `showyourwork-0.4.3rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/config.rst` & `showyourwork-0.4.3rc3/docs/config.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1053,20 +1053,56 @@
 
 **Required:** no
 
 **Example:**
 
 .. code-block:: yaml
 
-  tectonic_args: ["-Z", "shell-escape"]
+  tectonic_args: ["-Z", "shell-escape", "-Z", "shell-escape-cwd=."]
 
 to enable TeX shell escape functionality (allows the script to run
 arbitrary commands within TeX; be careful as this could be a security hazard).
 This is required to use the ``minted`` package for syntax highlighting of code
-snippets.
+snippets. The `shell-escape-cwd=.` option lets `showyourwork` save outputs
+of shell calls, whereas without this option they would be deleted (for example,
+the `minted` cache).
+
+.. _config.preprocess_arxiv_script:
+
+``preprocess_arxiv_script``
+^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``str``
+
+**Description:** A script controlling the preprocessing of the manuscript
+for submission to the arXiv. This is the path to a custom preprocessing script to use.
+The script should be executable and accept a single
+argument; this argument will be the path to the contents of the arXiv
+tarball. This script can modify the contents of the tarball in place,
+before the contents are put into a `.tar.gz` archive for submission.
+
+**Required:** no
+
+**Example:**
+
+The following example script preprocesses the manuscript to set up
+`minted` in a way that is compatible with the arXiv,
+by freezing the `minted` cache after the build is complete.
+It also switches `xcolor` to require the `table` option for
+compatibility with the LaTeX used on arXiv.
+
+.. code-block:: bash
+
+  #!/bin/bash
+  pushd $1
+  sed -i ms.tex -e 's/finalizecache/frozencache/g'
+  sed -i ms.tex -e '/PassOptionsToPackage/d'
+  sed -i showyourwork.tex -e 's/RequirePackage{xcolor}/RequirePackage[table]{xcolor}/g'
+  popd
+
 
 .. _config.verbose:
 
 ``verbose``
 ^^^^^^^^^^^
 
 **Type:** ``bool``
```

#### html2text {}

```diff
@@ -283,24 +283,41 @@
 `*.synctex.gz` file that allows certain editors (like VSCode) to automatically
 sync locations in your manuscript with locations in the compiled PDF.
 **Default:** ``true`` **Required:** no **Example:** .. code-block:: yaml
 synctex: true .. _config.tectonic_args: ``tectonic_args`` ^^^^^^^^^^^^^^^^^
 **Type:** ``list`` **Description:** A list of additional command-line options
 to be passed directly to ``tectonic`` when building the manuscript. **Default:
 ** ``[]`` **Required:** no **Example:** .. code-block:: yaml tectonic_args: ["-
-Z", "shell-escape"] to enable TeX shell escape functionality (allows the script
-to run arbitrary commands within TeX; be careful as this could be a security
-hazard). This is required to use the ``minted`` package for syntax highlighting
-of code snippets. .. _config.verbose: ``verbose`` ^^^^^^^^^^^ **Type:**
-``bool`` **Description:** Enable verbose output? Useful for debugging runs. By
-default, |showyourwork| suppresses nearly all Snakemake output, sending it
-directly to the log file (see :doc:`logging`). Setting ``verbose:Â true``
-results in all Snakemake output being printed to the screen as well. Note that
-you can crank up the verbosity even more by passing the ``--verbose`` argument
-to ``snakemakeÂ build``, which makes Snakemake itself more talkative.
-**Required:** no **Default:** ``false`` **Example:** .. code-block:: yaml
-verbose: true .. _config.version: ``version`` ^^^^^^^^^^^ **Type:** ``str``
-**Description:** The version of the |showyourwork| package used to create the
-workflow. As of ``0.4.0`` this setting no longer has any effect on the build
-process, as articles are now always compiled using the installed version of
+Z", "shell-escape", "-Z", "shell-escape-cwd=."] to enable TeX shell escape
+functionality (allows the script to run arbitrary commands within TeX; be
+careful as this could be a security hazard). This is required to use the
+``minted`` package for syntax highlighting of code snippets. The `shell-escape-
+cwd=.` option lets `showyourwork` save outputs of shell calls, whereas without
+this option they would be deleted (for example, the `minted` cache). ..
+_config.preprocess_arxiv_script: ``preprocess_arxiv_script``
+^^^^^^^^^^^^^^^^^^^^ **Type:** ``str`` **Description:** A script controlling
+the preprocessing of the manuscript for submission to the arXiv. This is the
+path to a custom preprocessing script to use. The script should be executable
+and accept a single argument; this argument will be the path to the contents of
+the arXiv tarball. This script can modify the contents of the tarball in place,
+before the contents are put into a `.tar.gz` archive for submission.
+**Required:** no **Example:** The following example script preprocesses the
+manuscript to set up `minted` in a way that is compatible with the arXiv, by
+freezing the `minted` cache after the build is complete. It also switches
+`xcolor` to require the `table` option for compatibility with the LaTeX used on
+arXiv. .. code-block:: bash #!/bin/bash pushd $1 sed -i ms.tex -e 's/
+finalizecache/frozencache/g' sed -i ms.tex -e '/PassOptionsToPackage/d' sed -
+i showyourwork.tex -e 's/RequirePackage{xcolor}/RequirePackage[table]{xcolor}/
+g' popd .. _config.verbose: ``verbose`` ^^^^^^^^^^^ **Type:** ``bool``
+**Description:** Enable verbose output? Useful for debugging runs. By default,
+|showyourwork| suppresses nearly all Snakemake output, sending it directly to
+the log file (see :doc:`logging`). Setting ``verbose:Â true`` results in all
+Snakemake output being printed to the screen as well. Note that you can crank
+up the verbosity even more by passing the ``--verbose`` argument to
+``snakemakeÂ build``, which makes Snakemake itself more talkative. **Required:
+** no **Default:** ``false`` **Example:** .. code-block:: yaml verbose: true ..
+_config.version: ``version`` ^^^^^^^^^^^ **Type:** ``str`` **Description:** The
+version of the |showyourwork| package used to create the workflow. As of
+``0.4.0`` this setting no longer has any effect on the build process, as
+articles are now always compiled using the installed version of
 ``showyourwork``. However, to improve compatibility with previous versions of
 the code, we recommend keeping this setting in your config file.
```

### Comparing `showyourwork-0.4.3rc2/docs/contributorguide.rst` & `showyourwork-0.4.3rc3/docs/contributorguide.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/faqs.rst` & `showyourwork-0.4.3rc3/docs/faqs.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/hacks.py` & `showyourwork-0.4.3rc3/docs/hacks.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/index.rst` & `showyourwork-0.4.3rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/install.rst` & `showyourwork-0.4.3rc3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/integration_tests.rst` & `showyourwork-0.4.3rc3/docs/integration_tests.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/intro.rst` & `showyourwork-0.4.3rc3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/latex.rst` & `showyourwork-0.4.3rc3/docs/latex.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/layout.rst` & `showyourwork-0.4.3rc3/docs/layout.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/logging.rst` & `showyourwork-0.4.3rc3/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/migrating.rst` & `showyourwork-0.4.3rc3/docs/migrating.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/overleaf.rst` & `showyourwork-0.4.3rc3/docs/overleaf.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/projects.json` & `showyourwork-0.4.3rc3/docs/projects.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'arm61/linearization-issues'": "OrderedDict([('title', 'Is there still a place for linearization "*

 * *                                 "in the chemistry curriculum?'), ('authors', ['Andrew R. "*

 * *                                 "McCluskey']), ('doi', '10.26434/chemrxiv-2023-44b29'), ('url', "*

 * *                                 "'https://doi.org/10.26434/chemrxiv-2023-44b29'), ('field', "*

 * *                                 "'Chemistry')])",*

 * * "'arm61/msd-errors'": "OrderedDict([('title', 'Accurate Estimation of Dif […]*

```diff
@@ -6,14 +6,34 @@
             "Selma E. de Mink"
         ],
         "doi": "arXiv:2111.08717",
         "field": "Astronomy",
         "title": "LEGWORK: A python package for computing the evolution and detectability of stellar-origin gravitational-wave sources with space-based detectors",
         "url": "https://ui.adsabs.harvard.edu/abs/2021arXiv211108717W"
     },
+    "arm61/linearization-issues": {
+        "authors": [
+            "Andrew R. McCluskey"
+        ],
+        "doi": "10.26434/chemrxiv-2023-44b29",
+        "field": "Chemistry",
+        "title": "Is there still a place for linearization in the chemistry curriculum?",
+        "url": "https://doi.org/10.26434/chemrxiv-2023-44b29"
+    },
+    "arm61/msd-errors": {
+        "authors": [
+            "Andrew R. McCluskey",
+            "Samuel W. Coles",
+            "Benjamin J. Morgan"
+        ],
+        "doi": "arXiv:2305.18244",
+        "field": "Materials Science",
+        "title": "Accurate Estimation of Diffusion Coefficients and their Uncertainties from Computer Simulation",
+        "url": "https://arxiv.org/abs/arXiv:2305.18244"
+    },
     "arm61/reporting_sampling": {
         "authors": [
             "Andrew R. McCluskey",
             "Andrew J. Caruana",
             "Christy J. Kinane",
             "Alexander J. Armstrong",
             "Thomas Arnold",
```

### Comparing `showyourwork-0.4.3rc2/docs/projects.rst.jinja` & `showyourwork-0.4.3rc3/docs/projects.rst.jinja`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/quickbuild.rst` & `showyourwork-0.4.3rc3/docs/quickbuild.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/quickstart.rst` & `showyourwork-0.4.3rc3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/snakefile.rst` & `showyourwork-0.4.3rc3/docs/snakefile.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/docs/zenodo.rst` & `showyourwork-0.4.3rc3/docs/zenodo.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/pyproject.toml` & `showyourwork-0.4.3rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/setup.py` & `showyourwork-0.4.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/build.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/cache.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/clean.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/preprocess.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/preprocess.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/run_snakemake.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/run_snakemake.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/setup.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/setup.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/tarball.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/tarball.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/commands/zenodo.py` & `showyourwork-0.4.3rc3/showyourwork/cli/commands/zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cli/main.py` & `showyourwork-0.4.3rc3/showyourwork/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,18 @@
 
 
 @contextmanager
 def cwd_as(path):
     """Temporarily change the current working directory to `path`."""
     old_dir = os.getcwd()
     os.chdir(path)
-    yield
-    os.chdir(old_dir)
+    try:
+        yield
+    finally:
+        os.chdir(old_dir)
 
 
 def echo(text="", **kwargs):
     """Print a message to the terminal with some custom formatting.
 
     Breaks long lines using ``TextWrapper`` and adds custom colors and
     indentation to code snippets and environment variables.
```

### Comparing `showyourwork-0.4.3rc2/showyourwork/config.py` & `showyourwork-0.4.3rc3/showyourwork/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,20 @@
         config["margin_icons"]["colors"]["dataset"] = config["margin_icons"][
             "colors"
         ].get("dataset", "0.12,0.47,0.71")
         offset = int(config["margin_icons"].get("horizontal_offset", 0))
         if offset < 0:
             config["margin_icons"]["horizontal_offset"] = r"\!" * abs(offset)
         else:
-            config["margin_icons"]["horizontal_offset"] = "\," * offset
+            config["margin_icons"]["horizontal_offset"] = r"\," * offset
+
+        # Preprocessing arXiv tarball settings:
+        config["preprocess_arxiv_script"] = config.get(
+            "preprocess_arxiv_script", None
+        )
 
         #
         # -- Internal settings --
         #
 
         # Cache settings
         config["cache"] = config.get("cache", {})
```

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml`

 * *Files 9% similar despite different names*

```diff
@@ -88,12 +88,18 @@
 
 # Enable SyncTeX?
 synctex: True
 
 # Command-line options to be passed to tectonic when building the manuscript
 tectonic_args: []
 
+# Preprocessing script for arXiv tarball
+# (such as to switch `minted` from `finalizecache` to `frozencache`)
+# The script will be passed a directory containing the manuscript source
+# as input, and should modify the contents of that directory in-place.
+# preprocess_arxiv_script: my_preprocess_script.sh
+
 # Enable verbose output?
 verbose: false
 
 # Version of `showyourwork` used to create this workflow
 version: {{ cookiecutter.showyourwork_version }}
```

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png` & `showyourwork-0.4.3rc3/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/exceptions/base.py` & `showyourwork-0.4.3rc3/showyourwork/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/exceptions/latex.py` & `showyourwork-0.4.3rc3/showyourwork/exceptions/latex.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/exceptions/other.py` & `showyourwork-0.4.3rc3/showyourwork/exceptions/other.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/exceptions/overleaf.py` & `showyourwork-0.4.3rc3/showyourwork/exceptions/overleaf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/exceptions/zenodo.py` & `showyourwork-0.4.3rc3/showyourwork/exceptions/zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/git.py` & `showyourwork-0.4.3rc3/showyourwork/git.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/gitapi.py` & `showyourwork-0.4.3rc3/showyourwork/gitapi.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/logging.py` & `showyourwork-0.4.3rc3/showyourwork/logging.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/overleaf.py` & `showyourwork-0.4.3rc3/showyourwork/overleaf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/patches.py` & `showyourwork-0.4.3rc3/showyourwork/patches.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/paths.py` & `showyourwork-0.4.3rc3/showyourwork/paths.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/subproc.py` & `showyourwork-0.4.3rc3/showyourwork/subproc.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/userrules.py` & `showyourwork-0.4.3rc3/showyourwork/userrules.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/build.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/build.smk`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     # Parse the config file
     parse_config()
 
 
     # Hack to make the pdf generation the default rule
     rule syw__main:
         input:
-            config["ms_pdf"]
-
+            config["ms_pdf"],
+            (config["ms_name"] + ".synctex.gz" if config["synctex"] else [])
 
     # Wrap other top-level rules to ensure tempfiles are properly
     # deleted; these are the rules we actually call from the Makefile
     rule syw__arxiv_entrypoint:
         input:
             "arxiv.tar.gz"
```

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/prep.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/prep.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/article-thumb.png` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/img/article-thumb.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/build.tex` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/styles/build.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/preprocess.tex` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/styles/preprocess.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/lineno.sty` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/lineno.sty`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/listofitems.tex` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/listofitems.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork-logo.pdf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork.otf` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/showyourwork.otf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.tex` & `showyourwork-0.4.3rc3/showyourwork/workflow/resources/tex/xstring.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/arxiv.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/arxiv.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/compile.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/compile.smk`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         "dag.pdf" if config["dag"]["render"] else [],
         WORKFLOW_GRAPH,
         "showyourwork.yml",
         "zenodo.yml" if (paths.user().repo / "zenodo.yml").exists() else [],
         compile_dir=paths.user().compile.as_posix()
     output:
         (paths.user().compile / f'{config["ms_name"]}.pdf').as_posix(),
-        (paths.user().compile / f'{config["ms_name"]}.synctex.gz').as_posix(),
+        (paths.user().compile / f'{config["ms_name"]}.synctex.gz').as_posix() if config["synctex"] else [],
     conda:
         tectonic_yml.as_posix()
     params:
         maybe_synctex="--synctex" if config["synctex"] else "",
         user_args=" ".join(config["user_args"])
     shell:
         """
@@ -97,18 +97,16 @@
         "syw__compile_copy_synctex"
     message:
         "Copying the article synctex..."
     input:
         (paths.user().compile / f'{config["ms_name"]}.synctex.gz').as_posix()
     output:
         config["ms_name"] + ".synctex.gz"
-    shell:
-        """
-        cp "{input}" "{output}"
-        """
+    script:
+        "../scripts/copy_and_fix_synctex.py"
 
 rule:
     """
     Compile the manuscript into the article PDF.
 
     """
     name:
```

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/dag.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/dag.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/figure.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/figure.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/preprocess.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/preprocess.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/render_dag.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/render_dag.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/rules/zenodo.smk` & `showyourwork-0.4.3rc3/showyourwork/workflow/rules/zenodo.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/compile_setup.py` & `showyourwork-0.4.3rc3/showyourwork/workflow/scripts/compile_setup.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/download.py` & `showyourwork-0.4.3rc3/showyourwork/workflow/scripts/download.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/extract.py` & `showyourwork-0.4.3rc3/showyourwork/workflow/scripts/extract.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/preprocess.py` & `showyourwork-0.4.3rc3/showyourwork/workflow/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/render_dag.py` & `showyourwork-0.4.3rc3/showyourwork/workflow/scripts/render_dag.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork/zenodo.py` & `showyourwork-0.4.3rc3/showyourwork/zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/showyourwork.egg-info/PKG-INFO` & `showyourwork-0.4.3rc3/showyourwork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showyourwork
-Version: 0.4.3rc2
+Version: 0.4.3rc3
 Summary: A workflow for open-source scientific articles
 Home-page: https://github.com/showyourwork/showyourwork
 Author: Rodrigo Luger
 Author-email: rodluger@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc2 Summary: A workflow
+Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc3 Summary: A workflow
 for open-source scientific articles Home-page: https://github.com/showyourwork/
 showyourwork Author: Rodrigo Luger Author-email: rodluger@gmail.com License:
 MIT Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests License-File: LICENSE
                                 [showyourwork]
   [unit_tests] [local_integration_tests] [remote_integration_tests] [tests]
                            [sample_projects] [pypi]
```

### Comparing `showyourwork-0.4.3rc2/showyourwork.egg-info/SOURCES.txt` & `showyourwork-0.4.3rc3/showyourwork.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 showyourwork/workflow/rules/dag.smk
 showyourwork/workflow/rules/figure.smk
 showyourwork/workflow/rules/preprocess.smk
 showyourwork/workflow/rules/render_dag.smk
 showyourwork/workflow/rules/zenodo.smk
 showyourwork/workflow/scripts/arxiv.py
 showyourwork/workflow/scripts/compile_setup.py
+showyourwork/workflow/scripts/copy_and_fix_synctex.py
 showyourwork/workflow/scripts/download.py
 showyourwork/workflow/scripts/extract.py
 showyourwork/workflow/scripts/preprocess.py
 showyourwork/workflow/scripts/render_dag.py
 tests/integration/conftest.py
 tests/integration/test_cache.py
 tests/integration/test_cache_optim.py
@@ -146,13 +147,14 @@
 tests/integration/test_duplicate_graphics.py
 tests/integration/test_latex.py
 tests/integration/test_letter.py
 tests/integration/test_missing_inputs.py
 tests/integration/test_overleaf.py
 tests/integration/test_pr.py
 tests/integration/test_space_in_path.py
+tests/integration/test_synctex.py
 tests/integration/test_variable.py
 tests/integration/test_zenodo.py
 tests/integration/helpers/__init__.py
 tests/integration/helpers/temp_repo.py
 tests/integration/sandbox/.gitignore
 tests/unit/test_overleaf_regex.py
```

### Comparing `showyourwork-0.4.3rc2/tests/integration/conftest.py` & `showyourwork-0.4.3rc3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/helpers/temp_repo.py` & `showyourwork-0.4.3rc3/tests/integration/helpers/temp_repo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_cache.py` & `showyourwork-0.4.3rc3/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_cache_optim.py` & `showyourwork-0.4.3rc3/tests/integration/test_cache_optim.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_latex.py` & `showyourwork-0.4.3rc3/tests/integration/test_latex.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_letter.py` & `showyourwork-0.4.3rc3/tests/integration/test_letter.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_missing_inputs.py` & `showyourwork-0.4.3rc3/tests/integration/test_missing_inputs.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_overleaf.py` & `showyourwork-0.4.3rc3/tests/integration/test_overleaf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_pr.py` & `showyourwork-0.4.3rc3/tests/integration/test_pr.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_variable.py` & `showyourwork-0.4.3rc3/tests/integration/test_variable.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/integration/test_zenodo.py` & `showyourwork-0.4.3rc3/tests/integration/test_zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.3rc2/tests/unit/test_overleaf_regex.py` & `showyourwork-0.4.3rc3/tests/unit/test_overleaf_regex.py`

 * *Files identical despite different names*

