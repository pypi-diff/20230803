# Comparing `tmp/quartodoc-0.4.1.tar.gz` & `tmp/quartodoc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.4.1.tar", last modified: Fri Jul 14 17:58:19 2023, max compression
+gzip compressed data, was "quartodoc-0.4.2.tar", last modified: Thu Aug  3 20:34:43 2023, max compression
```

## Comparing `quartodoc-0.4.1.tar` & `quartodoc-0.4.2.tar`

### file list

```diff
@@ -1,142 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.858332 quartodoc-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.830331 quartodoc-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 17:58:06.000000 quartodoc-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-14 17:58:06.000000 quartodoc-0.4.1/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-14 17:58:06.000000 quartodoc-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-14 17:58:19.858332 quartodoc-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-14 17:58:06.000000 quartodoc-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-14 17:58:06.000000 quartodoc-0.4.1/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.818331 quartodoc-0.4.1/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/interlinks.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.838332 quartodoc-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.838332 quartodoc-0.4.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/auto-package/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/auto-package/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 17:58:06.000000 quartodoc-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/__snapshots__/test_renderers.ambr
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.md
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-14 17:58:06.000000 quartodoc-0.4.1/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.826331 quartodoc-0.4.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.858332 quartodoc-0.4.1/scripts/filter-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-14 17:58:06.000000 quartodoc-0.4.1/scripts/filter-spec/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 17:58:06.000000 quartodoc-0.4.1/scripts/filter-spec/generate_test_qmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-14 17:58:19.858332 quartodoc-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.629956 quartodoc-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-08-03 20:34:29.000000 quartodoc-0.4.2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-08-03 20:34:29.000000 quartodoc-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-03 20:34:29.000000 quartodoc-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-03 20:34:29.000000 quartodoc-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 20:34:29.000000 quartodoc-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 20:34:29.000000 quartodoc-0.4.2/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-03 20:34:29.000000 quartodoc-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-03 20:34:43.629956 quartodoc-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-03 20:34:29.000000 quartodoc-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-03 20:34:29.000000 quartodoc-0.4.2/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.601956 quartodoc-0.4.2/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 20:34:29.000000 quartodoc-0.4.2/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 20:34:29.000000 quartodoc-0.4.2/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 20:34:29.000000 quartodoc-0.4.2/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-08-03 20:34:29.000000 quartodoc-0.4.2/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-03 20:34:29.000000 quartodoc-0.4.2/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-03 20:34:29.000000 quartodoc-0.4.2/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 20:34:29.000000 quartodoc-0.4.2/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 20:34:29.000000 quartodoc-0.4.2/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.609956 quartodoc-0.4.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.613956 quartodoc-0.4.2/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-03 20:34:29.000000 quartodoc-0.4.2/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.613956 quartodoc-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.613956 quartodoc-0.4.2/examples/auto-package/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/auto-package/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.617956 quartodoc-0.4.2/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 20:34:29.000000 quartodoc-0.4.2/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-03 20:34:29.000000 quartodoc-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.621956 quartodoc-0.4.2/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.621956 quartodoc-0.4.2/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.625956 quartodoc-0.4.2/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.625956 quartodoc-0.4.2/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.625956 quartodoc-0.4.2/quartodoc/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/__snapshots__/test_builder.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/__snapshots__/test_renderers.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.629956 quartodoc-0.4.2/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.629956 quartodoc-0.4.2/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-03 20:34:29.000000 quartodoc-0.4.2/quartodoc/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.621956 quartodoc-0.4.2/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 20:34:43.000000 quartodoc-0.4.2/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-03 20:34:29.000000 quartodoc-0.4.2/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.605956 quartodoc-0.4.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:34:43.629956 quartodoc-0.4.2/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 20:34:29.000000 quartodoc-0.4.2/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 20:34:29.000000 quartodoc-0.4.2/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-03 20:34:43.629956 quartodoc-0.4.2/setup.cfg
```

### Comparing `quartodoc-0.4.1/.github/CODE_OF_CONDUCT.md` & `quartodoc-0.4.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/.github/workflows/ci.yml` & `quartodoc-0.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/.gitignore` & `quartodoc-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/LICENSE` & `quartodoc-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/Makefile` & `quartodoc-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/PKG-INFO` & `quartodoc-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.4.1/README.md` & `quartodoc-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/README.qmd` & `quartodoc-0.4.2/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/_extensions/interlinks/interlinks.lua` & `quartodoc-0.4.2/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/case_studies/objects_sqla.inv` & `quartodoc-0.4.2/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/case_studies/parsing.qmd` & `quartodoc-0.4.2/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/case_studies/some_package.py` & `quartodoc-0.4.2/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/case_studies/sphinx-inventory.md` & `quartodoc-0.4.2/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/case_studies/sphinx-inventory.qmd` & `quartodoc-0.4.2/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/_quarto.yml` & `quartodoc-0.4.2/docs/_quarto.yml`

 * *Files 15% similar despite different names*

```diff
@@ -89,27 +89,24 @@
         - collect
         - get_object
         - preview
 
     - title: Docstring Renderers
       desc: |
         Renderers convert parsed docstrings into a target format, like markdown.
+      options:
+        dynamic: true
       contents:
         - name: MdRenderer
           children: linked
-        - name: MdRenderer.render
-          dynamic: true
-        - name: MdRenderer.render_annotation
-          dynamic: true
-        - name: MdRenderer.render_header
-          dynamic: true
-        - name: MdRenderer.signature
-          dynamic: true
-        - name: MdRenderer.summarize
-          dynamic: true
+        - MdRenderer.render
+        - MdRenderer.render_annotation
+        - MdRenderer.render_header
+        - MdRenderer.signature
+        - MdRenderer.summarize
 
     - title: API Builders
       desc: |
         Builders are responsible for building documentation. They tie all the pieces
         of quartodoc together, and can be defined in your _quarto.yml config.
       contents:
         - kind: auto
@@ -127,46 +124,41 @@
       desc: |
         Inventory files map a functions name to its corresponding url in your docs.
         These functions allow you to create and transform inventory files.
       contents:
         - create_inventory
         - convert_inventory
 
-    - title: "Data models: structural"
+    - title: "Data models"
+
+    - subtitle: "Structural"
       desc: |
         Classes for specifying the broad structure your docs.
       contents:
-        - kind: "page"
-          path: "layouts-structure"
-          flatten: true
-          contents:
-            - layout.Layout
-            - layout.Section
-            - layout.Page
-            - layout.SectionElement
-            - layout.ContentElement
+        - layout.Layout
+        - layout.Section
+        - layout.Page
+        - layout.SectionElement
+        - layout.ContentElement
 
-    - title: "Data models: docable"
+    - subtitle: "Docable"
       desc: |
         Classes representing python objects to be rendered.
       contents:
-        - kind: "page"
-          path: "layouts-docable"
-          flatten: true
-          contents:
-            - name: layout.Doc
-              members: []
-            - layout.DocFunction
-            - layout.DocAttribute
-            - layout.DocModule
-            - layout.DocClass
-            - layout.Link
-            - layout.Item
-            - layout.ChoicesChildren
-    - title: "Data models: docstring patches"
+        - name: layout.Doc
+          members: []
+        - layout.DocFunction
+        - layout.DocAttribute
+        - layout.DocModule
+        - layout.DocClass
+        - layout.Link
+        - layout.Item
+        - layout.ChoicesChildren
+
+    - subtitle: "Docstring patches"
       desc: |
         Most of the classes for representing python objects live
         in [](`griffe.dataclasses`) or [](`griffe.docstrings.dataclasses`).
         However, the `quartodoc.ast` module has a number of custom classes to fill
         in support for some important docstring sections.
       contents:
          - ast.DocstringSectionSeeAlso
```

### Comparing `quartodoc-0.4.1/docs/examples/index.qmd` & `quartodoc-0.4.2/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/architecture.qmd` & `quartodoc-0.4.2/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/basic-building.qmd` & `quartodoc-0.4.2/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/basic-content.qmd` & `quartodoc-0.4.2/docs/get-started/basic-content.qmd`

 * *Files 16% similar despite different names*

```diff
@@ -91,105 +91,95 @@
     - title: Some section
       desc: ""
       contents:
 
         # set the children option, so that methods get documented
         # on separate pages. MdRenderer's docs will include a summary
         # table that links to each page.
-        - name: quartodoc.MdRenderer
-          children: separate
-```
-
-## Grouping on a page
-
-By default, content in each section gets included in the same index table,
-with each piece of content documented on its own page.
-
-For example, consider the config below.
-
-```yaml
-quartodoc:
-  package: quartodoc
-  sections:
-    - title: Cool functions
-      desc: ""
-      contents:
-        - get_object
         - name: MdRenderer
-          members: ["render"]
+          children: separate
 ```
 
-Both `get_object` and `MdRenderer` will be:
 
-* summarized and linked to in the "Cool functions" section of the index.
-* documented on their own, separate pages.
+## Setting default options
 
-### Page layout element
+The section above showed how you can set options like `members:` and `children:` on content.
+When specifying API documentation, you may need to specify the same options across multiple pieces of content.
 
-Use a custom page element to group object documentation on the same page.
+Use the `options:` field in a section to specify options to apply across all content in that section.
 
-Custom page elements are specified by including a `kind: <element name>` field.
+For example, the config blocks below show how to document multiple classes without their members.
 
 :::::: {.columns}
-
-
 ::: {.column}
 
-**Separate**
+**Manual**
 
 ```yaml
 quartodoc:
   package: quartodoc
   sections:
-    - title: Cool functions
-      desc: ""
+    - title: "Some section"
 
-      # normal contents setup ----
+      # options set manually ---
       contents:
-        - get_object
         - name: MdRenderer
-          members: ["render"]
+          members: []
+        - name: Builder
+          members: []
 ```
 
 :::
 ::: {.column}
 
-**Grouped on same page**
+**With options**
 
 ```yaml
 quartodoc:
   package: quartodoc
   sections:
-    - title: Cool functions
-      desc: ""
+    - title: "Some section"
 
-      # contents with a page grouping ----
+      # default options ---
+      options:
+        members: []
+      
       contents:
-        - kind: page
-          path: some_funcs
-          contents:
-            - get_object
-            - name: MdRenderer
-              members: ["render"]
+        - MdRenderer
+        - Builder
 ```
 
 :::
 ::::::
 
-Note these three important pieces of the page entry:
+Note that the **with options** block sets `members: []` inside `options`.
+This sets `members: []` as the default for each piece of content.
 
-* `kind: page` - indicates that we are creating a page
-* `path:` - specifies what the name of the page will be in the generated docs.
-  For example, `path: some_funcs` in the config above produces a file called
-  `some_funcs.qmd` in the API reference folder.
-* `contents:` - lists out the contents of the page.
+::: {.callout-tip}
+Options can be given a name, and re-used in multiple sections:
 
+```yaml
+- title: Some section
+  options: &no-members
+    members: []
+  content:
+    - ThingA
+    - ThingB
+- title: Another section
+  options: *no-members
+  content:
+    - ThingC
+```
 
+The code above uses `&no-members` to name the options in the first section "no-members",
+then `*no-members` to reference it in the second section.
+The `&` and `*` are called an anchor and alias, respectively, in YAML.
+:::
 
-## Setting default package path
+## Specifying package path
 
 Different levels of configuration let you set the `package` option.
 This controls the package path that quartodoc will try to import control content from.
 
 The example below shows three different places it can be set:
 top-level site config, section config, or in a page element.
 
@@ -230,21 +220,135 @@
     - title: ""
       desc: ""
       package: null
       contents:
         - quartodoc.get_object
 ```
 
+
 ## Dynamic lookup
 
 By default, quartodoc uses static analysis to look up objects.
 This means it gets information about your docstring without actually running your package's code.
 
 This usually works well, but may get the docstring wrong for those created in an extremely dynamic way (e.g. you manually set the `__doc__` attribute on an object).
 
 In this case, you can set the dynamic option on a piece of content.
 
 ```yaml
 contents:
   - name: get_object
     dynamic: true
 ```
+
+
+## Reference page sub-sections
+
+quartodoc supports two levels of grouping on the reference page.
+Use the `subtitle:` option to add an additional level of grouping.
+
+For example, the code below creates an API reference page with one top-level section ("Some section"),
+with two sub-sections inside it.
+
+
+```yaml
+quartodoc:
+  package: quartodoc
+  sections:
+    - title: Some section
+
+    - subtitle: Stuff A
+      desc: This is subsection A
+      contents:
+        - MdRenderer
+
+    - subtitle: Stuff B
+      desc: This is subsection B
+      contents:
+        - get_object
+```
+
+## Grouping on a page
+
+By default, content in each section gets included in the same index table,
+with each piece of content documented on its own page.
+
+For example, consider the config below.
+
+```yaml
+quartodoc:
+  package: quartodoc
+  sections:
+    - title: Cool functions
+      desc: ""
+      contents:
+        - get_object
+        - name: MdRenderer
+          members: ["render"]
+```
+
+Both `get_object` and `MdRenderer` will be:
+
+* summarized and linked to in the "Cool functions" section of the index.
+* documented on their own, separate pages.
+
+### Page layout element
+
+Use a custom page element to group object documentation on the same page.
+
+Custom page elements are specified by including a `kind: <element name>` field.
+
+:::::: {.columns}
+
+
+::: {.column}
+
+**Separate**
+
+```yaml
+quartodoc:
+  package: quartodoc
+  sections:
+    - title: Cool functions
+      desc: ""
+
+      # normal contents setup ----
+      contents:
+        - get_object
+        - name: MdRenderer
+          members: ["render"]
+```
+
+:::
+::: {.column}
+
+**Grouped on same page**
+
+```yaml
+quartodoc:
+  package: quartodoc
+  sections:
+    - title: Cool functions
+      desc: ""
+
+      # contents with a page grouping ----
+      contents:
+        - kind: page
+          path: some_funcs
+          contents:
+            - get_object
+            - name: MdRenderer
+              members: ["render"]
+```
+
+:::
+::::::
+
+Note these three important pieces of the page entry:
+
+* `kind: page` - indicates that we are creating a page
+* `path:` - specifies what the name of the page will be in the generated docs.
+  For example, `path: some_funcs` in the config above produces a file called
+  `some_funcs.qmd` in the API reference folder.
+* `contents:` - lists out the contents of the page.
+
+
```

### Comparing `quartodoc-0.4.1/docs/get-started/basic-docs.qmd` & `quartodoc-0.4.2/docs/get-started/basic-docs.qmd`

 * *Files 9% similar despite different names*

```diff
@@ -42,13 +42,14 @@
 print(renderer.render(doc_params))
 ```
 
 ### Section options
 
 The `sections` field defines which functions to document.
 
-It requires three pieces of configuration:
+It commonly requires three pieces of configuration:
 
 * `title`: a title for the section
 * `desc`: a description for the section
 * `contents`: a list of functions to document
 
+You can also replace `title` with `subtitle` to create a sub-section.
```

### Comparing `quartodoc-0.4.1/docs/get-started/crossrefs.qmd` & `quartodoc-0.4.2/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.4.2/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.4.2/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/dev-prepare.qmd` & `quartodoc-0.4.2/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/dev-renderers.qmd` & `quartodoc-0.4.2/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/docstring-examples.qmd` & `quartodoc-0.4.2/docs/get-started/docstring-examples.qmd`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,21 @@
     quarto syntax:
     
     ```{{python}}
     1 + 1
     ```
 ```
 
+Note that different syntaxes are handled differently:
+
+* doctest and markdown syntax: rendered without executing.
+* quarto syntax: executed by quarto when you run commands like `quarto render`.
+
+See the quarto documentation on [code blocks](https://quarto.org/docs/computations/python.html#code-blocks) for more detail.
+
 
 ## Examples, etc..: the "s" matters
 
 The numpydoc spec pluralizes section most names.
 If you leave off the "s", then they may be misparsed.
 
 For example, the docstring below erroneously has a "Return" section:
```

### Comparing `quartodoc-0.4.1/docs/get-started/extending.qmd` & `quartodoc-0.4.2/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.4.2/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/interlinks.qmd` & `quartodoc-0.4.2/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/overview.qmd` & `quartodoc-0.4.2/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/get-started/sidebar.qmd` & `quartodoc-0.4.2/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/docs/styles.css` & `quartodoc-0.4.2/docs/styles.css`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,33 @@
 .sidebar-item-text {
   /*color: rgba(60, 60, 60, 0.7);*/
   font-weight: 500;
   font-size: 14px;
   line-height: 22px;
 }
 
+.sidebar-item {
+  margin-top: 0px;
+}
+
 .sidebar-item-section {
   padding-top: 16px;
 }
 
 .sidebar-section {
   padding-left: 0px !important;
 }
+
+.sidebar-item-section .sidebar-item-section {
+  padding-top: 0px;
+  padding-left: 10px;
+}
+
+
+td:first-child {
+  text-wrap: nowrap;
+  text-size-adjust: 100%;
+}
+
+td:first-child a {
+  word-break: normal;
+}
```

### Comparing `quartodoc-0.4.1/examples/dascore/_quarto.yml` & `quartodoc-0.4.2/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/dascore/generate_api.py` & `quartodoc-0.4.2/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/pkgdown/_quarto.yml` & `quartodoc-0.4.2/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/pkgdown/objects.json` & `quartodoc-0.4.2/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.4.2/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.4.2/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/single-page/_quarto.yml` & `quartodoc-0.4.2/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/single-page/objects.json` & `quartodoc-0.4.2/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/examples/single-page/reference/index.qmd` & `quartodoc-0.4.2/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/__init__.py` & `quartodoc-0.4.2/quartodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/ast.py` & `quartodoc-0.4.2/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/autosummary.py` & `quartodoc-0.4.2/quartodoc/autosummary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import inspect
 import logging
 import warnings
 import yaml
 
 from fnmatch import fnmatchcase
 from griffe.loader import GriffeLoader
 from griffe.collections import ModulesCollection, LinesCollection
@@ -272,26 +273,32 @@
         canonical_path = mod.__name__
 
     # Case 2: path is to a member of a module
     else:
         splits = object_path.split(".")
 
         canonical_path = None
-        parts = []
         crnt_part = mod
         for ii, attr_name in enumerate(splits):
             try:
                 crnt_part = getattr(crnt_part, attr_name)
                 if not isinstance(crnt_part, ModuleType) and not canonical_path:
-                    canonical_path = crnt_part.__module__ + ":" + ".".join(splits[ii:])
+                    if inspect.isclass(crnt_part) or inspect.isfunction(crnt_part):
+                        _mod = getattr(crnt_part, "__module__", None)
+
+                        if _mod is None:
+                            canonical_path = path
+                        else:
+                            canonical_path = _mod + ":" + ".".join(splits[ii:])
+                    else:
+                        canonical_path = path
                 elif isinstance(crnt_part, ModuleType) and ii == (len(splits) - 1):
                     # final object is module
                     canonical_path = crnt_part.__name__
 
-                parts.append(crnt_part)
             except AttributeError:
                 # Fetching the attribute can fail if it is purely a type hint,
                 # and has no value. This can be an issue if you have added a
                 # docstring below the annotation
                 if canonical_path:
                     # See if we can return the static object for a value-less attr
                     try:
@@ -568,20 +575,38 @@
 
         return inventory
 
     # sidebar ----
 
     def _generate_sidebar(self, blueprint: layout.Layout):
         contents = [f"{self.dir}/index{self.out_page_suffix}"]
+        in_subsection = False
+        crnt_entry = {}
         for section in blueprint.sections:
+            if section.title:
+                if crnt_entry:
+                    contents.append(crnt_entry)
+
+                in_subsection = False
+                crnt_entry = {"section": section.title, "contents": []}
+            elif section.subtitle:
+                in_subsection = True
+
             links = []
             for entry in section.contents:
                 links.extend(self._page_to_links(entry))
 
-            contents.append({"section": section.title, "contents": links})
+            if in_subsection:
+                sub_entry = {"section": section.subtitle, "contents": links}
+                crnt_entry["contents"].append(sub_entry)
+            else:
+                crnt_entry["contents"].extend(links)
+
+        if crnt_entry:
+            contents.append(crnt_entry)
 
         entries = [{"id": self.dir, "contents": contents}, {"id": "dummy-sidebar"}]
         return {"website": {"sidebar": entries}}
 
     def write_sidebar(self, blueprint: layout.Layout):
         """Write a yaml config file for API sidebar."""
```

### Comparing `quartodoc-0.4.1/quartodoc/builder/blueprint.py` & `quartodoc-0.4.2/quartodoc/builder/blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,22 @@
     Page,
     Section,
 )
 from quartodoc import get_object as _get_object
 
 from .utils import PydanticTransformer, ctx_node, WorkaroundKeyError
 
-from typing import overload
+from typing import overload, TYPE_CHECKING
+
 
 _log = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    from pydantic import BaseModel
+
 
 def _auto_package(mod: dc.Module) -> list[Section]:
     """Create default sections for the given package."""
 
     import griffe.docstrings.dataclasses as ds
 
     # get module members for content ----
@@ -82,36 +86,48 @@
             # assumes everything from module was loaded, so target must
             # be outside module
             return True
 
     return False
 
 
-def _to_simple_dict(el):
+def _to_simple_dict(el: "BaseModel"):
     # round-trip to json, so we can take advantage of pydantic
     # dumping Enums, etc.. There may be a simple way to do
     # this in pydantic v2.
     return json.loads(el.json(exclude_unset=True))
 
 
+def _non_default_entries(el: "BaseModel"):
+    field_defaults = {mf.name: mf.default for mf in el.__fields__.values()}
+    set_fields = [
+        k for k, v in el if field_defaults[k] is not v if not isinstance(v, MISSING)
+    ]
+
+    d = el.dict()
+
+    return {k: d[k] for k in set_fields}
+
+
 class BlueprintTransformer(PydanticTransformer):
     def __init__(self, get_object=None, parser="numpy"):
 
         if get_object is None:
             loader = GriffeLoader(
                 docstring_parser=Parser(parser),
                 modules_collection=ModulesCollection(),
                 lines_collection=LinesCollection(),
             )
             self.get_object = partial(_get_object, loader=loader)
         else:
             self.get_object = get_object
 
         self.crnt_package = None
-        self.dynamic = None
+        self.options = None
+        self.dynamic = False
 
     @staticmethod
     def _append_member_path(path: str, new: str):
         if ":" in path:
             return f"{path}.{new}"
 
         return f"{path}:{new}"
@@ -134,24 +150,34 @@
         return new
 
     @dispatch
     def visit(self, el):
         # TODO: use a context handler
         self._log("VISITING", el)
 
+        # set package ----
         package = getattr(el, "package", MISSING())
         old = self.crnt_package
 
         if not isinstance(package, MISSING):
             self.crnt_package = package
 
+        # set options ----
+        # TODO: check for Section instead?
+        options = getattr(el, "options", None)
+        old_options = self.options
+
+        if options is not None:
+            self.options = options
+
         try:
             return super().visit(el)
         finally:
             self.crnt_package = old
+            self.options = old_options
 
     @dispatch
     def enter(self, el: Layout):
         if not el.sections:
             # TODO: should be shown all the time, not just logged,
             # but also want to be able to disable (similar to pins)
             print("Autogenerating contents (since no contents specified in config)")
@@ -204,23 +230,32 @@
 
         return new
 
     @dispatch
     def enter(self, el: Auto):
         self._log("Entering", el)
 
+        # settings based on parent context options (package, options) ----
         # TODO: make this less brittle
         pkg = self.crnt_package
         if pkg is None:
             path = el.name
         elif ":" in pkg or ":" in el.name:
             path = f"{pkg}.{el.name}"
         else:
             path = f"{pkg}:{el.name}"
 
+        # auto default overrides
+        if self.options is not None:
+            # TODO: is this round-tripping guaranteed by pydantic?
+            _option_dict = _non_default_entries(self.options)
+            _el_dict = _non_default_entries(el)
+            el = el.__class__(**{**_option_dict, **_el_dict})
+
+        # fetching object ----
         _log.info(f"Getting object for {path}")
 
         dynamic = el.dynamic if el.dynamic is not None else self.dynamic
 
         obj = self.get_object_fixed(path, dynamic=dynamic)
         raw_members = self._fetch_members(el, obj)
```

### Comparing `quartodoc-0.4.1/quartodoc/builder/collect.py` & `quartodoc-0.4.2/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/builder/utils.py` & `quartodoc-0.4.2/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/interlinks.py` & `quartodoc-0.4.2/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/inventory.py` & `quartodoc-0.4.2/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/layout.py` & `quartodoc-0.4.2/quartodoc/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,43 @@
     """A section of content on the reference index page.
 
     Attributes
     ----------
     kind:
     title:
         Title of the section on the index.
+    subtitle:
+        Subtitle of the section on the index. Note that either title or subtitle,
+        but not both, may be set.
     desc:
         Description of the section on the index.
     package:
         If specified, all object lookups will be relative to this path.
     contents:
         Individual objects (e.g. functions, classes, methods) being documented.
     """
 
     kind: Literal["section"] = "section"
-    title: str
-    desc: str
+    title: Optional[str] = None
+    subtitle: Optional[str] = None
+    desc: Optional[str] = None
     package: Union[str, None, MISSING] = MISSING()
-    contents: ContentList
+    contents: ContentList = []
+    options: Optional["AutoOptions"] = None
+
+    def __init__(self, **data):
+        super().__init__(**data)
+
+        # TODO: should these be a custom type? Or can we use pydantic's ValidationError?
+        if self.title is None and self.subtitle is None and not self.contents:
+            raise ValueError(
+                "Section must specify a title, subtitle, or contents field"
+            )
+        elif self.title is not None and self.subtitle is not None:
+            raise ValueError("Section cannot specify both title and subtitle fields.")
 
 
 class SummaryDetails(_Base):
     """Details that can be used in a summary table (e.g. on the index page)."""
 
     name: str
     desc: str = ""
@@ -180,15 +196,29 @@
 
     embedded = "embedded"
     flat = "flat"
     separate = "separate"
     linked = "linked"
 
 
-class Auto(_Base):
+class AutoOptions(_Base):
+    """Options available for Auto content layout element."""
+
+    members: Optional[list[str]] = None
+    include_private: bool = False
+    include_imports: bool = False
+    include_empty: bool = False
+    include: Optional[str] = None
+    exclude: Optional[str] = None
+    dynamic: Union[None, bool, str] = None
+    children: ChoicesChildren = ChoicesChildren.embedded
+    package: Union[str, None, MISSING] = MISSING()
+
+
+class Auto(AutoOptions):
     """Configure a python object to document (e.g. module, class, function, attribute).
 
     Attributes
     ----------
     kind:
     name:
         Name of the object. This should be the path needed to import it.
@@ -214,23 +244,14 @@
         If specified, object lookup will be relative to this path.
 
 
     """
 
     kind: Literal["auto"] = "auto"
     name: str
-    members: Optional[list[str]] = None
-    include_private: bool = False
-    include_imports: bool = False
-    include_empty: bool = False
-    include: Optional[str] = None
-    exclude: Optional[str] = None
-    dynamic: Union[None, bool, str] = None
-    children: ChoicesChildren = ChoicesChildren.embedded
-    package: Union[str, None, MISSING] = MISSING()
 
 
 # TODO: rename to Default or something
 class _AutoDefault(_Base):
     """This hacky class allows creating Auto as a default option in Pages and Sections."""
 
     __root__: Union[str, dict]
```

### Comparing `quartodoc-0.4.1/quartodoc/renderers/base.py` & `quartodoc-0.4.2/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/renderers/md_renderer.py` & `quartodoc-0.4.2/quartodoc/renderers/md_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,24 +543,33 @@
     @dispatch
     def summarize(self, el: layout.Layout):
         rendered_sections = list(map(self.summarize, el.sections))
         return "\n\n".join(rendered_sections)
 
     @dispatch
     def summarize(self, el: layout.Section):
-        header = f"## {el.title}\n\n{el.desc}"
-
-        thead = "| | |\n| --- | --- |"
-
-        rendered = []
-        for child in el.contents:
-            rendered.append(self.summarize(child))
-
-        str_func_table = "\n".join([thead, *rendered])
-        return f"{header}\n\n{str_func_table}"
+        desc = f"\n\n{el.desc}" if el.desc is not None else ""
+        if el.title is not None:
+            header = f"## {el.title}{desc}"
+        elif el.subtitle is not None:
+            header = f"### {el.subtitle}{desc}"
+        else:
+            header = ""
+
+        if el.contents:
+            thead = "| | |\n| --- | --- |"
+
+            rendered = []
+            for child in el.contents:
+                rendered.append(self.summarize(child))
+
+            str_func_table = "\n".join([thead, *rendered])
+            return f"{header}\n\n{str_func_table}"
+        
+        return header
 
     @dispatch
     def summarize(self, el: layout.Page):
         if el.summary is not None:
             # TODO: assumes that files end with .qmd
             return self._summary_row(f"[{el.summary.name}]({el.path}.qmd)", el.summary.desc)
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/__snapshots__/test_renderers.ambr` & `quartodoc-0.4.2/quartodoc/tests/__snapshots__/test_renderers.ambr`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_class.py` & `quartodoc-0.4.2/quartodoc/tests/example_class.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_dynamic.py` & `quartodoc-0.4.2/quartodoc/tests/example_dynamic.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     # note that we could use the partialmethod, but I am not sure how to
     # correctly set its __doc__ attribute in that case.
     dynamic_create = partial(dynamic_doc, x=1)
     dynamic_create.__doc__ = dynamic_doc.__doc__
 
 
 class InstanceAttrs:
+    """Some InstanceAttrs class"""
+
     z: int
     """The z attribute"""
 
     def __init__(self, a: int, b: str):
         self.a = a
         self.b = b
         """The b attribute"""
+
+
+some_instance = InstanceAttrs(1, 1)
+some_instance.__doc__ = "Dynamic instance doc"
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_interlinks/interlinks.lua` & `quartodoc-0.4.2/quartodoc/tests/example_interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.4.2/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.4.2/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.md` & `quartodoc-0.4.2/quartodoc/tests/example_interlinks/test.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.qmd` & `quartodoc-0.4.2/quartodoc/tests/example_interlinks/test.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_ast.py` & `quartodoc-0.4.2/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_basic.py` & `quartodoc-0.4.2/quartodoc/tests/test_basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -75,24 +75,45 @@
 def test_get_object_dynamic_class_method_doc():
     obj = get_object("quartodoc.tests.example_dynamic:AClass", dynamic=True)
 
     meth = obj.members["dynamic_doc"]
     assert meth.docstring.value == "A dynamic method"
 
 
-def test_get_object_dynamic_class_method_doc():
+def test_get_object_dynamic_class_method_doc_partial():
     obj = get_object("quartodoc.tests.example_dynamic:AClass", dynamic=True)
 
     meth = obj.members["dynamic_create"]
     assert meth.docstring.value == "A dynamic method"
 
 
 def test_get_object_dynamic_class_instance_attr_doc():
     obj = get_object("quartodoc.tests.example_dynamic:InstanceAttrs", dynamic=True)
 
     assert obj.members["b"].docstring.value == "The b attribute"
 
 
-def test_get_object_dynamic_class_instance_attr_doc():
+def test_get_object_dynamic_class_instance_attr_doc_class_attr_valueless():
     obj = get_object("quartodoc.tests.example_dynamic:InstanceAttrs", dynamic=True)
 
     assert obj.members["z"].docstring.value == "The z attribute"
+
+
+def test_get_object_dynamic_module_attr_str():
+    # a key behavior here is that it does not error attempting to look up
+    # str.__module__, which does not exist
+    obj = get_object("quartodoc.tests.example_dynamic:NOTE", dynamic=True)
+
+    assert obj.name == "NOTE"
+
+    # this case is weird, but we are dynamically looking up a string
+    # so our __doc__ is technically str.__doc__
+    assert obj.docstring.value == str.__doc__
+
+
+def test_get_object_dynamic_module_attr_class_instance():
+    # a key behavior here is that it does not error attempting to look up
+    # str.__module__, which does not exist
+    obj = get_object("quartodoc.tests.example_dynamic:some_instance", dynamic=True)
+
+    assert obj.path == "quartodoc.tests.example_dynamic.some_instance"
+    assert obj.docstring.value == "Dynamic instance doc"
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_builder.py` & `quartodoc-0.4.2/quartodoc/tests/test_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
+import yaml
 
 from pathlib import Path
 from quartodoc import layout as lo
-from quartodoc import Builder
+from quartodoc import Builder, blueprint
 
 
 @pytest.fixture
 def builder(tmp_path):
     section = lo.Section(
         title="abc",
         desc="xyz",
@@ -36,7 +37,32 @@
     len(list(Path(builder.dir).glob("Mdrenderer*"))) == 3
 
 
 def test_builder_build_filter_wildcard_methods(builder):
     builder.build(filter="MdRenderer.*")
 
     len(list(Path(builder.dir).glob("Mdrenderer.*"))) == 2
+
+
+def test_builder_generate_sidebar(tmp_path, snapshot):
+    cfg = yaml.safe_load(
+        """
+    quartodoc:
+      package: quartodoc.tests.example
+      sections:
+        - title: first section
+          desc: some description
+          contents: [a_func]
+        - title: second section
+          desc: title description
+        - subtitle: a subsection
+          desc: subtitle description
+          contents:
+            - a_attr
+    """
+    )
+
+    builder = Builder.from_quarto_config(cfg)
+    bp = blueprint(builder.layout)
+    d_sidebar = builder._generate_sidebar(bp)
+
+    assert yaml.dump(d_sidebar) == snapshot
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.4.2/quartodoc/tests/test_builder_blueprint.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,7 +113,25 @@
     sections = layout.sections
     assert len(sections) == 1
     assert sections[0].title == "quartodoc.tests.example"
     assert sections[0].desc == "A module"
 
     # 4 objects documented
     assert len(sections[0].contents) == 4
+
+
+def test_blueprint_section_options():
+    layout = lo.Layout(
+        sections=[
+            lo.Section(
+                contents=[lo.Auto(name="AClass")],
+                package="quartodoc.tests.example",
+                options={"members": []},
+            )
+        ]
+    )
+
+    res = blueprint(layout)
+    page = res.sections[0].contents[0]
+    doc = page.contents[0]
+
+    assert doc.members == []
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_interlinks.py` & `quartodoc-0.4.2/quartodoc/tests/test_interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_layout.py` & `quartodoc-0.4.2/quartodoc/tests/test_layout.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,12 +26,26 @@
     page = Page(**cfg)
     assert page == res
 
     layout = Layout(sections=[cfg])
     assert layout.sections[0] == res
 
 
+@pytest.mark.parametrize(
+    "kwargs, msg_part",
+    [
+        ({}, "must specify a title, subtitle, or contents field"),
+        ({"title": "x", "subtitle": "y"}, "cannot specify both"),
+    ],
+)
+def test_section_validation_fails(kwargs, msg_part):
+    with pytest.raises(ValueError) as exc_info:
+        Section(**kwargs)
+
+    assert msg_part in exc_info.value.args[0]
+
+
 def test_layout_extra_forbidden():
     with pytest.raises(ValidationError) as exc_info:
         Section(title="abc", desc="xyz", contents=[], zzzzz=1)
 
     assert "extra fields not permitted" in str(exc_info.value)
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_renderers.py` & `quartodoc-0.4.2/quartodoc/tests/test_renderers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import griffe.docstrings.dataclasses as ds
 import griffe.expressions as exp
 
 from quartodoc.renderers import MdRenderer
-from quartodoc import Auto, blueprint, get_object
+from quartodoc import layout, get_object, blueprint, Auto
 
 
 @pytest.fixture
 def renderer():
     return MdRenderer()
 
 
@@ -59,14 +59,41 @@
     cls_section, cls_par = pair
     pars = cls_section([cls_par(name="x", description=interlink)])
 
     res = renderer.render(pars)
     assert interlink in res
 
 
+@pytest.mark.parametrize(
+    "section, dst",
+    [
+        (layout.Section(title="abc"), "## abc"),
+        (layout.Section(subtitle="abc"), "### abc"),
+        (layout.Section(title="abc", desc="zzz"), "## abc\n\nzzz"),
+        (layout.Section(subtitle="abc", desc="zzz"), "### abc\n\nzzz"),
+    ],
+)
+def test_render_summarize_section_title(renderer, section, dst):
+    res = renderer.summarize(section)
+
+    assert res == dst
+
+
+def test_render_summarize_section_contents(renderer):
+    obj = blueprint(layout.Auto(name="a_func", package="quartodoc.tests.example"))
+    section = layout.Section(title="abc", desc="zzz", contents=[obj])
+    res = renderer.summarize(section)
+
+    table = (
+        "| | |\n| --- | --- |\n"
+        "| [a_func](#quartodoc.tests.example.a_func) | A function |"
+    )
+    assert res == f"## abc\n\nzzz\n\n{table}"
+
+
 def test_render_doc_attribute(renderer):
     attr = ds.DocstringAttribute(
         name="abc",
         description="xyz",
         annotation=exp.Expression(exp.Name("Optional", full="Optional"), "[", "]"),
         value=1,
     )
```

### Comparing `quartodoc-0.4.1/quartodoc/tests/test_validation.py` & `quartodoc-0.4.2/quartodoc/tests/test_validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,79 @@
-import pytest, copy
+import copy
+import pytest
+
 from quartodoc.autosummary import Builder
 
 EXAMPLE_SECTIONS = [
-                  {'title':  'Preperation Functions',
-                   'desc': 'Functions that fetch objects.\nThey prepare a representation of the site.\n', 
-                   'contents': ['Auto', 'blueprint', 'collect', 'get_object', 'preview']}, 
-                  {'title': 'Docstring Renderers', 
-                   'desc': 'Renderers convert parsed docstrings into a target format, like markdown.\n', 
-                   'contents': [{'name': 'MdRenderer', 'children': 'linked'}, 
-                                {'name': 'MdRenderer.render', 'dynamic': True}, 
-                                {'name': 'MdRenderer.render_annotation', 'dynamic': True}, 
-                                {'name': 'MdRenderer.render_header', 'dynamic': True}]
-                    }, 
-                    {'title': 'API Builders', 
-                     'desc': 'Builders build documentation. They tie all the pieces\nof quartodoc together.\n', 
-                     'contents': [{'kind': 'auto', 'name': 'Builder', 'members': []}, 
-                                   'Builder.from_quarto_config', 'Builder.build', 'Builder.write_index']
-                    },
-                ]
+    {
+        "title": "Preperation Functions",
+        "desc": "Functions that fetch objects.\nThey prepare a representation of the site.\n",
+        "contents": ["Auto", "blueprint", "collect", "get_object", "preview"],
+    },
+    {
+        "title": "Docstring Renderers",
+        "desc": "Renderers convert parsed docstrings into a target format, like markdown.\n",
+        "contents": [
+            {"name": "MdRenderer", "children": "linked"},
+            {"name": "MdRenderer.render", "dynamic": True},
+            {"name": "MdRenderer.render_annotation", "dynamic": True},
+            {"name": "MdRenderer.render_header", "dynamic": True},
+        ],
+    },
+    {
+        "title": "API Builders",
+        "desc": "Builders build documentation. They tie all the pieces\nof quartodoc together.\n",
+        "contents": [
+            {"kind": "auto", "name": "Builder", "members": []},
+            "Builder.from_quarto_config",
+            "Builder.build",
+            "Builder.write_index",
+        ],
+    },
+]
+
 
 @pytest.fixture
 def sections():
     return copy.deepcopy(EXAMPLE_SECTIONS)
 
+
 def check_ValueError(sections):
     "Check that a ValueError is raised when creating a `Builder` instance. Return the error message as a string."
     with pytest.raises(ValueError) as e:
-        Builder(sections=sections, package='quartodoc')
+        Builder(sections=sections, package="quartodoc")
     return str(e.value)
 
+
 def test_valid_yaml(sections):
     "Test that valid YAML passes validation"
-    Builder(sections=sections, package='quartodoc')
+    Builder(sections=sections, package="quartodoc")
 
-def test_missing_title(sections):
-    "Test that missing title raises an error"
-    del sections[0]['title']
-    msg = check_ValueError(sections)
-    assert '- Missing field `title` for element 0 in the list for `sections`' in msg
-
-def test_missing_desc(sections):
-    "Test that a missing description raises an error"
-    sections = copy.deepcopy(EXAMPLE_SECTIONS)
-    del sections[2]['desc']
-    msg = check_ValueError(sections)
-    assert '- Missing field `desc` for element 2 in the list for `sections`' in msg
 
 def test_missing_name_contents_1(sections):
     "Test that a missing name in contents raises an error"
-    del sections[2]['contents'][0]['name']
+    del sections[2]["contents"][0]["name"]
     msg = check_ValueError(sections)
-    assert '- Missing field `name` for element 0 in the list for `contents` located in element 2 in the list for `sections`' in msg
+    assert (
+        "- Missing field `name` for element 0 in the list for `contents` located in element 2 in the list for `sections`"
+        in msg
+    )
+
 
 def test_missing_name_contents_2(sections):
     "Test that a missing name in contents raises an error in a different section."
-    del sections[1]['contents'][0]['name']
+    del sections[1]["contents"][0]["name"]
     msg = check_ValueError(sections)
-    assert '- Missing field `name` for element 0 in the list for `contents` located in element 1 in the list for `sections`' in msg
+    assert (
+        "- Missing field `name` for element 0 in the list for `contents` located in element 1 in the list for `sections`"
+        in msg
+    )
+
 
 def test_misplaced_kindpage(sections):
     "Test that a misplaced kind: page raises an error"
-    sections[0]['kind'] = 'page'
+    sections[0]["kind"] = "page"
     msg = check_ValueError(sections)
-    assert ' - Missing field `path` for element 0 in the list for `sections`, which you need when setting `kind: page`.' in msg
+    assert (
+        " - Missing field `path` for element 0 in the list for `sections`, which you need when setting `kind: page`."
+        in msg
+    )
```

### Comparing `quartodoc-0.4.1/quartodoc/validation.py` & `quartodoc-0.4.2/quartodoc/validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.4.2/quartodoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.4.1/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.4.2/quartodoc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 quartodoc/tests/test_basic.py
 quartodoc/tests/test_builder.py
 quartodoc/tests/test_builder_blueprint.py
 quartodoc/tests/test_interlinks.py
 quartodoc/tests/test_layout.py
 quartodoc/tests/test_renderers.py
 quartodoc/tests/test_validation.py
+quartodoc/tests/__snapshots__/test_builder.ambr
 quartodoc/tests/__snapshots__/test_renderers.ambr
 quartodoc/tests/example_interlinks/.gitignore
 quartodoc/tests/example_interlinks/README.md
 quartodoc/tests/example_interlinks/_quarto.yml
 quartodoc/tests/example_interlinks/interlinks.lua
 quartodoc/tests/example_interlinks/objects.json
 quartodoc/tests/example_interlinks/spec.yml
```

### Comparing `quartodoc-0.4.1/requirements-dev.txt` & `quartodoc-0.4.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/scripts/filter-spec/generate_files.py` & `quartodoc-0.4.2/scripts/filter-spec/generate_files.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.1/setup.cfg` & `quartodoc-0.4.2/setup.cfg`

 * *Files identical despite different names*

