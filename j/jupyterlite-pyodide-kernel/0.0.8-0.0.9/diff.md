# Comparing `tmp/jupyterlite_pyodide_kernel-0.0.8.tar.gz` & `tmp/jupyterlite_pyodide_kernel-0.0.9.tar.gz`

## Comparing `jupyterlite_pyodide_kernel-0.0.8.tar` & `jupyterlite_pyodide_kernel-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/install.json
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/package.json
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/tsconfigbase.json
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/_version.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/app.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/__init__.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/_base.py
--rw-r--r--   0        0        0    12607 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/piplite.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/pyodide.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/package.json
--rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-r--r--   0        0        0    32006 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/518.a3c6a3ae7ee95e5158aa.js.map
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-r--r--   0        0        0    32534 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.map
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/652.07cda501733578161e13.js
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/652.07cda501733578161e13.js.map
--rw-r--r--   0        0        0   165727 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
--rw-r--r--   0        0        0   385878 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.map
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
--rw-r--r--   0        0        0    38817 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.b340cae4b3c1bda6a7fd.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/style.js
--rw-r--r--   0        0        0    14685 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/all.json
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/schema/kernel.v0.schema.json
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/schema/piplite.v0.schema.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/__init__.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/conftest.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_metadata.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_piplite.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_pyodide.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_repo.py
--rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/fixtures/the_smallest_extension-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/.gitignore
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/LICENSE
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/README.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/install.json
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/package.json
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/tsconfigbase.json
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/_version.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/app.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/__init__.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/_base.py
+-rw-r--r--   0        0        0    12607 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/piplite.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/pyodide.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/package.json
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/324.2759063405b36360da9d.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/324.2759063405b36360da9d.js.LICENSE.txt
+-rw-r--r--   0        0        0    32006 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/324.2759063405b36360da9d.js.map
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-r--r--   0        0        0    32534 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.map
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/652.ecdf94afc2748b3fc2e0.js
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/652.ecdf94afc2748b3fc2e0.js.map
+-rw-r--r--   0        0        0   165727 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+-rw-r--r--   0        0        0   385878 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.map
+-rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.703f03086e9738104706.js
+-rw-r--r--   0        0        0    38828 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.703f03086e9738104706.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/style.js
+-rw-r--r--   0        0        0    14685 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/all.json
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/piplite-0.0.9-py3-none-any.whl
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/pyodide_kernel-0.0.9-py3-none-any.whl
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/schema/kernel.v0.schema.json
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/schema/piplite.v0.schema.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/__init__.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/conftest.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_metadata.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_piplite.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_pyodide.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_repo.py
+-rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/fixtures/the_smallest_extension-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/README.md
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 jupyterlite_pyodide_kernel-0.0.9/PKG-INFO
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/CHANGELOG.md` & `jupyterlite_pyodide_kernel-0.0.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.0.9
+
+([Full Changelog](https://github.com/jupyterlite/pyodide-kernel/compare/@jupyterlite/pyodide-kernel-extension@0.0.8...80dde027d0f1e9f2c4f4cd4f2679675ebd8da499))
+
+### Enhancements made
+
+- Update to Pyodide 0.23.4 [#50](https://github.com/jupyterlite/pyodide-kernel/pull/50) ([@jtpio](https://github.com/jtpio))
+
+### Maintenance and upkeep improvements
+
+- Add `before-bump-version` hook [#51](https://github.com/jupyterlite/pyodide-kernel/pull/51) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlite/pyodide-kernel/graphs/contributors?from=2023-05-04&to=2023-08-02&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlite%2Fpyodide-kernel+involves%3Agithub-actions+updated%3A2023-05-04..2023-08-02&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyterlite%2Fpyodide-kernel+involves%3Ajtpio+updated%3A2023-05-04..2023-08-02&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.0.8
 
 ([Full Changelog](https://github.com/jupyterlite/pyodide-kernel/compare/@jupyterlite/pyodide-kernel-extension@0.0.7...55f8602a1ff83cc199ec6a45c440d0566ff727a4))
 
 ### Enhancements made
 
 - pyodide 0.23.2 [#46](https://github.com/jupyterlite/pyodide-kernel/pull/46) ([@bollwyvl](https://github.com/bollwyvl))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlite/pyodide-kernel/graphs/contributors?from=2023-04-24&to=2023-05-04&type=c))
 
 [@bollwyvl](https://github.com/search?q=repo%3Ajupyterlite%2Fpyodide-kernel+involves%3Abollwyvl+updated%3A2023-04-24..2023-05-04&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.0.7
 
 ([Full Changelog](https://github.com/jupyterlite/pyodide-kernel/compare/@jupyterlite/pyodide-kernel-extension@0.0.6...6af9a12b844dae5d5ac1b7ad703bc0d20b2c8e19))
 
 ### Enhancements made
 
 - Update to Pyodide `0.23.1` [#45](https://github.com/jupyterlite/pyodide-kernel/pull/45) ([@jtpio](https://github.com/jtpio))
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/CONTRIBUTING.md` & `jupyterlite_pyodide_kernel-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/RELEASE.md` & `jupyterlite_pyodide_kernel-0.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/package.json` & `jupyterlite_pyodide_kernel-0.0.9/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/tsconfigbase.json` & `jupyterlite_pyodide_kernel-0.0.9/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/app.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/app.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/constants.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #: where we put pyodide, for now
 PYODIDE = "pyodide"
 PYODIDE_JS = "pyodide.js"
 PYODIDE_REPODATA = "repodata.json"
 PYODIDE_URL_ENV_VAR = "JUPYTERLITE_PYODIDE_URL"
 
 #: probably only compatible with this version of pyodide
-PYODIDE_VERSION = "0.23.2"
+PYODIDE_VERSION = "0.23.4"
 
 #: the only kind of noarch wheel piplite understands
 NOARCH_WHL = "py3-none-any.whl"
 
 #: the only kind of binary wheel piplite understands
 WASM_WHL = "emscripten_*_wasm32.whl"
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/_base.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/_base.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/piplite.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/piplite.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/addons/pyodide.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/addons/pyodide.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/package.json` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/pyodide-kernel': '^0.0.9'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.703f03086e9738104706.js'}}",*

 * * "'version'": "'0.0.9'"}*

```diff
@@ -3,15 +3,15 @@
     "bugs": {
         "url": "https://github.com/jupyterlite/pyodide-kernel/issues"
     },
     "dependencies": {
         "@jupyterlab/coreutils": "^5.5.2",
         "@jupyterlite/contents": "^0.1.0-beta.18",
         "@jupyterlite/kernel": "^0.1.0-beta.18",
-        "@jupyterlite/pyodide-kernel": "^0.0.8",
+        "@jupyterlite/pyodide-kernel": "^0.0.9",
         "@jupyterlite/server": "^0.1.0-beta.18"
     },
     "description": "JupyterLite - Pyodide Kernel Extension",
     "devDependencies": {
         "@jupyterlab/builder": "^3.5.0",
         "rimraf": "~3.0.0",
         "typescript": "~4.9.4"
@@ -28,15 +28,15 @@
         "style/index.js",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jupyterlite/pyodide-kernel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b340cae4b3c1bda6a7fd.js"
+            "load": "static/remoteEntry.703f03086e9738104706.js"
         },
         "extension": true,
         "outputDir": "../../jupyterlite_pyodide_kernel/labextension",
         "sharedPackages": {
             "@jupyterlite/contents": {
                 "bundled": false,
                 "singleton": true
@@ -85,9 +85,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "types": "lib/index.d.ts",
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/518.a3c6a3ae7ee95e5158aa.js` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/324.2759063405b36360da9d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
-/*! For license information please see 518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt */
+/*! For license information please see 324.2759063405b36360da9d.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_jupyterlite_pyodide_kernel_extension = self.webpackChunk_jupyterlite_pyodide_kernel_extension || []).push([
-    [518], {
-        2: (e, t, n) => {
+    [324], {
+        742: (e, t, n) => {
             n.r(t), n.d(t, {
                 PIPLITE_INDEX_SCHEMA: () => D,
                 PyodideKernel: () => H,
                 PyodideRemoteKernel: () => N.O,
                 allJSONUrl: () => a,
                 ipykernelWheelUrl: () => i,
                 pipliteWheelUrl: () => l,
@@ -14,17 +14,17 @@
                 widgetsnbextensionWheelUrl: () => d,
                 widgetsnbextensionWheelUrl1: () => h
             });
             const r = n.p + "pypi/all.json";
             var a = n.t(r);
             const s = n.p + "pypi/ipykernel-6.9.2-py3-none-any.whl";
             var i = n.t(s);
-            const o = n.p + "pypi/piplite-0.0.8-py3-none-any.whl";
+            const o = n.p + "pypi/piplite-0.0.9-py3-none-any.whl";
             var l = n.t(o);
-            const c = n.p + "pypi/pyodide_kernel-0.0.8-py3-none-any.whl";
+            const c = n.p + "pypi/pyodide_kernel-0.0.9-py3-none-any.whl";
             var p = n.t(c);
             const u = n.p + "pypi/widgetsnbextension-3.6.4-py3-none-any.whl";
             var d = n.t(u);
             const m = n.p + "pypi/widgetsnbextension-4.0.7-py3-none-any.whl";
             var h = n.t(m),
                 y = n(526),
                 g = n(671),
@@ -439,8 +439,8 @@
             }
             const I = n.p + "schema/piplite.v0.schema.json";
             var D = n.t(I),
                 N = n(951)
         }
     }
 ]);
-//# sourceMappingURL=518.a3c6a3ae7ee95e5158aa.js.map?v=a3c6a3ae7ee95e5158aa
+//# sourceMappingURL=324.2759063405b36360da9d.js.map?v=2759063405b36360da9d
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/518.a3c6a3ae7ee95e5158aa.js.map` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/324.2759063405b36360da9d.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'324.2759063405b36360da9d.js?v=2759063405b36360da9d'",*

 * * "'mappings'": "';ozBAKA,MAAMA,EAAcC,OAAO,iBACrBC,EAAiBD,OAAO,oBACxBE,EAAeF,OAAO,wBACtBG,EAAYH,OAAO,qBACnBI,EAAcJ,OAAO,kBACrBK,EAAYC,GAAwB,iBAARA,GAA4B,OAARA,GAAgC,mBAARA,EAgDxEC,EAAmB,IAAIC,IAAI,CAC7B,CAAC,QA7CwB,CACzBC,UAAYH,GAAQD,EAASC,IAAQA,EAAIP,GACzCW,UAAUC,GACN,MAAM,MAAEC,EAAK,MAAEC,GAAU,IAAIC,eAE7B,OADAC,EAAOJ,EAAKC,GACL,CAACC,EAAO,CAACA,GACpB,EACAG,YAAYC,IACRA,EAAKC,QACEC,EAAKF,MAqChB,CAAC,QA/BwB,CACzBR,UAAYW,GAAUf,EAASe,IAAUhB,KAAe […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "518.a3c6a3ae7ee95e5158aa.js?v=a3c6a3ae7ee95e5158aa",
-    "mappings": "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",
+    "file": "324.2759063405b36360da9d.js?v=2759063405b36360da9d",
+    "mappings": "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",
     "names": [
         "proxyMarker",
         "Symbol",
         "createEndpoint",
         "releaseProxy",
         "finalizer",
         "throwMarker",
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.map` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/568.371c75f0cd43fa31532d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/652.07cda501733578161e13.js` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/652.ecdf94afc2748b3fc2e0.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
                 p = [{
                     id: d,
                     autoStart: !0,
                     requires: [s.IKernelSpecs],
                     optional: [i.IServiceWorkerManager, r.IBroadcastChannelWrapper],
                     activate: (e, l, i, s) => {
                         const r = JSON.parse(t.PageConfig.getOption("litePluginSettings") || "{}")[d] || {},
-                            a = r.pyodideUrl || "https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js",
+                            a = r.pyodideUrl || "https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js",
                             o = t.URLExt.parse(a).href,
                             p = r.pipliteWheelUrl ? t.URLExt.parse(r.pipliteWheelUrl).href : void 0,
                             c = (r.pipliteUrls || []).map((e => t.URLExt.parse(e).href)),
                             v = !!r.disablePyPIFallback;
                         l.register({
                             spec: {
                                 name: "python",
@@ -36,15 +36,15 @@
                                     "logo-32x32": h,
                                     "logo-64x64": h
                                 }
                             },
                             create: async e => {
                                 const {
                                     PyodideKernel: l
-                                } = await n.e(52).then(n.t.bind(n, 52, 23)), t = !(!(null == i ? void 0 : i.enabled) || !(null == s ? void 0 : s.enabled));
+                                } = await n.e(828).then(n.t.bind(n, 828, 23)), t = !(!(null == i ? void 0 : i.enabled) || !(null == s ? void 0 : s.enabled));
                                 return t ? console.info("Pyodide contents will be synced with Jupyter Contents") : console.warn("Pyodide contents will NOT be synced with Jupyter Contents"), new l({
                                     ...e,
                                     pyodideUrl: o,
                                     pipliteWheelUrl: p,
                                     pipliteUrls: c,
                                     disablePyPIFallback: v,
                                     mountDrive: t
@@ -52,8 +52,8 @@
                             }
                         })
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=652.07cda501733578161e13.js.map?v=07cda501733578161e13
+//# sourceMappingURL=652.ecdf94afc2748b3fc2e0.js.map?v=ecdf94afc2748b3fc2e0
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/652.07cda501733578161e13.js.map` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/652.ecdf94afc2748b3fc2e0.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238094%*

 * *Differences: {"'file'": "'652.ecdf94afc2748b3fc2e0.js?v=ecdf94afc2748b3fc2e0'",*

 * * "'mappings'": "'uTAAA,MCQMA,EAAkB,6BAA6BC,KDRrD,4iCCgBMC,EAAY,+CAoDlB,EADgB,CA/CD,CACXC,GAAID,EACJE,WAAW,EACXC,SAAU,CAAC,EAAAC,cACXC,SAAU,CAAC,EAAAC,sBAAuB,EAAAC,0BAClCC,SAAU,CAACC,EAAKC,EAAaC,EAAeC,KACxC,MAAMC,EAASC,KAAKC,MAAM,EAAAC,WAAA,UAAqB,uBAAyB,MAAMhB,IAAc,CAAC,EACvFiB,EAAMJ,EAAOK,YAfH,2DAgBVA,EAAa,EAAAC,OAAA,MAAaF,GAAKG,KAC/BC,EAAkBR,EAAOQ,gBACzB,EAAAF,OAAA,MAAaN,EAAOQ,iBAAiBD,UACrCE,EAEAC,GADaV,EAAOU,aAAe,IACVC,KAAKC,GAAW,EAAAN,OAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "652.07cda501733578161e13.js?v=07cda501733578161e13",
-    "mappings": "uTAAA,MCQMA,EAAkB,6BAA6BC,KDRrD,4iCCgBMC,EAAY,+CAoDlB,EADgB,CA/CD,CACXC,GAAID,EACJE,WAAW,EACXC,SAAU,CAAC,EAAAC,cACXC,SAAU,CAAC,EAAAC,sBAAuB,EAAAC,0BAClCC,SAAU,CAACC,EAAKC,EAAaC,EAAeC,KACxC,MAAMC,EAASC,KAAKC,MAAM,EAAAC,WAAA,UAAqB,uBAAyB,MAAMhB,IAAc,CAAC,EACvFiB,EAAMJ,EAAOK,YAfH,2DAgBVA,EAAa,EAAAC,OAAA,MAAaF,GAAKG,KAC/BC,EAAkBR,EAAOQ,gBACzB,EAAAF,OAAA,MAAaN,EAAOQ,iBAAiBD,UACrCE,EAEAC,GADaV,EAAOU,aAAe,IACVC,KAAKC,GAAW,EAAAN,OAAA,MAAaM,GAAQL,OAC9DM,IAAwBb,EAAOa,oBACrChB,EAAYiB,SAAS,CACjBC,KAAM,CACFC,KAAM,SACNC,aAAc,mBACdC,SAAU,SACVC,KAAM,GACNC,UAAW,CACP,aAAcnC,EACd,aAAcA,IAGtBoC,OAAQC,MAAOC,IACX,MAAM,cAAEC,SAAwB,gCAC1BC,MAAiB3B,aAAqD,EAASA,EAAc4B,YAAa3B,aAA2D,EAASA,EAAiB2B,UAOrM,OANID,EACAE,QAAQC,KAAK,yDAGbD,QAAQE,KAAK,6DAEV,IAAIL,EAAc,IAClBD,EACHlB,aACAG,kBACAE,cACAG,sBACAY,cACF,GAER,G",
+    "file": "652.ecdf94afc2748b3fc2e0.js?v=ecdf94afc2748b3fc2e0",
+    "mappings": "uTAAA,MCQMA,EAAkB,6BAA6BC,KDRrD,4iCCgBMC,EAAY,+CAoDlB,EADgB,CA/CD,CACXC,GAAID,EACJE,WAAW,EACXC,SAAU,CAAC,EAAAC,cACXC,SAAU,CAAC,EAAAC,sBAAuB,EAAAC,0BAClCC,SAAU,CAACC,EAAKC,EAAaC,EAAeC,KACxC,MAAMC,EAASC,KAAKC,MAAM,EAAAC,WAAA,UAAqB,uBAAyB,MAAMhB,IAAc,CAAC,EACvFiB,EAAMJ,EAAOK,YAfH,2DAgBVA,EAAa,EAAAC,OAAA,MAAaF,GAAKG,KAC/BC,EAAkBR,EAAOQ,gBACzB,EAAAF,OAAA,MAAaN,EAAOQ,iBAAiBD,UACrCE,EAEAC,GADaV,EAAOU,aAAe,IACVC,KAAKC,GAAW,EAAAN,OAAA,MAAaM,GAAQL,OAC9DM,IAAwBb,EAAOa,oBACrChB,EAAYiB,SAAS,CACjBC,KAAM,CACFC,KAAM,SACNC,aAAc,mBACdC,SAAU,SACVC,KAAM,GACNC,UAAW,CACP,aAAcnC,EACd,aAAcA,IAGtBoC,OAAQC,MAAOC,IACX,MAAM,cAAEC,SAAwB,kCAC1BC,MAAiB3B,aAAqD,EAASA,EAAc4B,YAAa3B,aAA2D,EAASA,EAAiB2B,UAOrM,OANID,EACAE,QAAQC,KAAK,yDAGbD,QAAQE,KAAK,6DAEV,IAAIL,EAAc,IAClBD,EACHlB,aACAG,kBACAE,cACAG,sBACAY,cACF,GAER,G",
     "names": [
         "KERNEL_ICON_URL",
         "btoa",
         "PLUGIN_ID",
         "id",
         "autoStart",
         "requires",
@@ -51,11 +51,11 @@
     "sourceRoot": "",
     "sources": [
         "webpack://@jupyterlite/pyodide-kernel-extension/./style/img/pyodide.svg",
         "webpack://@jupyterlite/pyodide-kernel-extension/./lib/index.js"
     ],
     "sourcesContent": [
         "export default \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\"?>\\n<svg width=\\\"182\\\" height=\\\"182\\\" data-name=\\\"Layer 1\\\" version=\\\"1.1\\\" viewBox=\\\"0 0 182 182\\\" xmlns=\\\"http://www.w3.org/2000/svg\\\">\\n <defs>\\n  <style>.cls-1 {\\n        fill: #fff;\\n      }\\n\\n      .cls-2 {\\n        fill: #654ff0;\\n      }</style>\\n </defs>\\n <rect width=\\\"182\\\" height=\\\"182\\\" fill=\\\"#fff\\\" stop-color=\\\"#000000\\\" style=\\\"paint-order:stroke fill markers\\\"/>\\n <rect class=\\\"cls-1\\\" x=\\\"107\\\" y=\\\"125\\\" width=\\\"50\\\" height=\\\"32\\\"/>\\n <path class=\\\"cls-2\\\" d=\\\"m135.18 97c0-0.13-0.01-7.24-0.02-7.37h27.51v71.33h-71.34v-71.33h27.51c0 0.13-0.02 7.24-0.02 7.37m32.59 56.33h4.9l-7.43-25.25h-7.45l-6.12 25.25h4.75l1.24-5.62h8.49l1.61 5.62zm-26.03 0h4.69l6.02-25.25h-4.63l-3.69 17.4h-0.06l-3.5-17.4h-4.42l-3.9 17.19h-0.06l-3.23-17.19h-4.72l5.44 25.25h4.78l3.75-17.19h0.06zm18.89-19.03h1.99l2.37 9.27h-6.42z\\\"/>\\n <path d=\\\"m89 49.66c0 10.6-8.8 20-20 20h-40v20h-10v-70h50c10.7 0 19.7 8.9 20 20zm-10-10c0-5.5-4.5-10-10-10h-40v30h40c5.5 0 10-4.5 10-10z\\\"/>\\n <path d=\\\"m132 67.66v22h-10v-22l-30-33v-15h10v10.9l25 27.5 25-27.5v-10.9h10v15z\\\"/>\\n</svg>\\n\";",
-        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\nimport { PageConfig, URLExt } from '@jupyterlab/coreutils';\nimport { IServiceWorkerManager, } from '@jupyterlite/server';\nimport { IKernelSpecs } from '@jupyterlite/kernel';\nimport { IBroadcastChannelWrapper } from '@jupyterlite/contents';\nexport * as KERNEL_SETTINGS_SCHEMA from '../schema/kernel.v0.schema.json';\nimport KERNEL_ICON_SVG_STR from '../style/img/pyodide.svg';\nconst KERNEL_ICON_URL = `data:image/svg+xml;base64,${btoa(KERNEL_ICON_SVG_STR)}`;\n/**\n * The default CDN fallback for Pyodide\n */\nconst PYODIDE_CDN_URL = 'https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js';\n/**\n * The id for the extension, and key in the litePlugins.\n */\nconst PLUGIN_ID = '@jupyterlite/pyodide-kernel-extension:kernel';\n/**\n * A plugin to register the Pyodide kernel.\n */\nconst kernel = {\n    id: PLUGIN_ID,\n    autoStart: true,\n    requires: [IKernelSpecs],\n    optional: [IServiceWorkerManager, IBroadcastChannelWrapper],\n    activate: (app, kernelspecs, serviceWorker, broadcastChannel) => {\n        const config = JSON.parse(PageConfig.getOption('litePluginSettings') || '{}')[PLUGIN_ID] || {};\n        const url = config.pyodideUrl || PYODIDE_CDN_URL;\n        const pyodideUrl = URLExt.parse(url).href;\n        const pipliteWheelUrl = config.pipliteWheelUrl\n            ? URLExt.parse(config.pipliteWheelUrl).href\n            : undefined;\n        const rawPipUrls = config.pipliteUrls || [];\n        const pipliteUrls = rawPipUrls.map((pipUrl) => URLExt.parse(pipUrl).href);\n        const disablePyPIFallback = !!config.disablePyPIFallback;\n        kernelspecs.register({\n            spec: {\n                name: 'python',\n                display_name: 'Python (Pyodide)',\n                language: 'python',\n                argv: [],\n                resources: {\n                    'logo-32x32': KERNEL_ICON_URL,\n                    'logo-64x64': KERNEL_ICON_URL,\n                },\n            },\n            create: async (options) => {\n                const { PyodideKernel } = await import('@jupyterlite/pyodide-kernel');\n                const mountDrive = !!((serviceWorker === null || serviceWorker === void 0 ? void 0 : serviceWorker.enabled) && (broadcastChannel === null || broadcastChannel === void 0 ? void 0 : broadcastChannel.enabled));\n                if (mountDrive) {\n                    console.info('Pyodide contents will be synced with Jupyter Contents');\n                }\n                else {\n                    console.warn('Pyodide contents will NOT be synced with Jupyter Contents');\n                }\n                return new PyodideKernel({\n                    ...options,\n                    pyodideUrl,\n                    pipliteWheelUrl,\n                    pipliteUrls,\n                    disablePyPIFallback,\n                    mountDrive,\n                });\n            },\n        });\n    },\n};\nconst plugins = [kernel];\nexport default plugins;\n"
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\nimport { PageConfig, URLExt } from '@jupyterlab/coreutils';\nimport { IServiceWorkerManager, } from '@jupyterlite/server';\nimport { IKernelSpecs } from '@jupyterlite/kernel';\nimport { IBroadcastChannelWrapper } from '@jupyterlite/contents';\nexport * as KERNEL_SETTINGS_SCHEMA from '../schema/kernel.v0.schema.json';\nimport KERNEL_ICON_SVG_STR from '../style/img/pyodide.svg';\nconst KERNEL_ICON_URL = `data:image/svg+xml;base64,${btoa(KERNEL_ICON_SVG_STR)}`;\n/**\n * The default CDN fallback for Pyodide\n */\nconst PYODIDE_CDN_URL = 'https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js';\n/**\n * The id for the extension, and key in the litePlugins.\n */\nconst PLUGIN_ID = '@jupyterlite/pyodide-kernel-extension:kernel';\n/**\n * A plugin to register the Pyodide kernel.\n */\nconst kernel = {\n    id: PLUGIN_ID,\n    autoStart: true,\n    requires: [IKernelSpecs],\n    optional: [IServiceWorkerManager, IBroadcastChannelWrapper],\n    activate: (app, kernelspecs, serviceWorker, broadcastChannel) => {\n        const config = JSON.parse(PageConfig.getOption('litePluginSettings') || '{}')[PLUGIN_ID] || {};\n        const url = config.pyodideUrl || PYODIDE_CDN_URL;\n        const pyodideUrl = URLExt.parse(url).href;\n        const pipliteWheelUrl = config.pipliteWheelUrl\n            ? URLExt.parse(config.pipliteWheelUrl).href\n            : undefined;\n        const rawPipUrls = config.pipliteUrls || [];\n        const pipliteUrls = rawPipUrls.map((pipUrl) => URLExt.parse(pipUrl).href);\n        const disablePyPIFallback = !!config.disablePyPIFallback;\n        kernelspecs.register({\n            spec: {\n                name: 'python',\n                display_name: 'Python (Pyodide)',\n                language: 'python',\n                argv: [],\n                resources: {\n                    'logo-32x32': KERNEL_ICON_URL,\n                    'logo-64x64': KERNEL_ICON_URL,\n                },\n            },\n            create: async (options) => {\n                const { PyodideKernel } = await import('@jupyterlite/pyodide-kernel');\n                const mountDrive = !!((serviceWorker === null || serviceWorker === void 0 ? void 0 : serviceWorker.enabled) && (broadcastChannel === null || broadcastChannel === void 0 ? void 0 : broadcastChannel.enabled));\n                if (mountDrive) {\n                    console.info('Pyodide contents will be synced with Jupyter Contents');\n                }\n                else {\n                    console.warn('Pyodide contents will NOT be synced with Jupyter Contents');\n                }\n                return new PyodideKernel({\n                    ...options,\n                    pyodideUrl,\n                    pipliteWheelUrl,\n                    pipliteUrls,\n                    disablePyPIFallback,\n                    mountDrive,\n                });\n            },\n        });\n    },\n};\nconst plugins = [kernel];\nexport default plugins;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.map` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/951.b9fa6250974e699a3731.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.703f03086e9738104706.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, d, f, s, p, c, h, b, v, y, m, g, j = {
+    var e, r, t, n, o, i, a, l, u, d, f, s, c, p, h, b, v, y, m, g, j = {
             405: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(694), t.e(652)]).then((() => () => t(763))),
                         "./extension": () => Promise.all([t.e(694), t.e(652)]).then((() => () => t(763)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -49,26 +49,26 @@
         return i.default = () => t, k.d(o, i), o
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        52: "354648418987bd848171",
-        518: "a3c6a3ae7ee95e5158aa",
+        324: "2759063405b36360da9d",
         568: "371c75f0cd43fa31532d",
-        652: "07cda501733578161e13",
+        652: "ecdf94afc2748b3fc2e0",
         694: "e063d498fa9e311b3f30",
+        828: "18cd1cea0272a9fd42b1",
         951: "b9fa6250974e699a3731"
     } [e] + ".js?v=" + {
-        52: "354648418987bd848171",
-        518: "a3c6a3ae7ee95e5158aa",
+        324: "2759063405b36360da9d",
         568: "371c75f0cd43fa31532d",
-        652: "07cda501733578161e13",
+        652: "ecdf94afc2748b3fc2e0",
         694: "e063d498fa9e311b3f30",
+        828: "18cd1cea0272a9fd42b1",
         951: "b9fa6250974e699a3731"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -83,19 +83,19 @@
                     if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == n + o) {
                         a = f;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, k.nc && a.setAttribute("nonce", k.nc), a.setAttribute("data-webpack", n + o), a.src = e), t[e] = [r];
             var s = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = t[e];
                     if (delete t[e], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -121,15 +121,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlite/pyodide-kernel-extension", "0.0.8", (() => Promise.all([k.e(694), k.e(652)]).then((() => () => k(763))))), l("@jupyterlite/pyodide-kernel", "0.0.8", (() => Promise.all([k.e(951), k.e(518), k.e(694)]).then((() => () => k(2)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlite/pyodide-kernel-extension", "0.0.9", (() => Promise.all([k.e(694), k.e(652)]).then((() => () => k(763))))), l("@jupyterlite/pyodide-kernel", "0.0.9", (() => Promise.all([k.e(951), k.e(324), k.e(694)]).then((() => () => k(742)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -199,52 +199,52 @@
                     u = !1, a--
                 } else {
                     if (a <= t || f < s != n) return !1;
                     u = !1
                 } else "s" != s && "n" != s && (u = !1, a--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? l(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, u = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && i(e, r) ? r : e), 0)
     }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var o = d(e, t);
-        return l(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), c(e[t][o])
-    }, p = (e, r, t) => {
+        return l(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), p(e[t][o])
+    }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !l(t, r) || e && !i(e, r) ? e : r), 0)) && n[r]
-    }, c = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, n, o) {
         var i = k.I(r);
         return i && i.then ? i.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
     })(((e, r, t, n) => (u(e, t), s(r, 0, t, n)))), v = h(((e, r, t, n, o) => {
-        var i = r && k.o(r, t) && p(r, t, n);
-        return i ? c(i) : o()
+        var i = r && k.o(r, t) && c(r, t, n);
+        return i ? p(i) : o()
     })), y = {}, m = {
         289: () => b("default", "@jupyterlite/kernel", [2, 0, 1, 0, , "beta", 18]),
         671: () => b("default", "@jupyterlab/coreutils", [1, 5, 5, 3]),
         174: () => b("default", "@jupyterlite/server", [2, 0, 1, 0, , "beta", 18]),
         685: () => b("default", "@jupyterlite/contents", [2, 0, 1, 0, , "beta", 18]),
         526: () => b("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        52: () => v("default", "@jupyterlite/pyodide-kernel", [3, 0, 0, 8], (() => Promise.all([k.e(951), k.e(518)]).then((() => () => k(2)))))
+        828: () => v("default", "@jupyterlite/pyodide-kernel", [3, 0, 0, 9], (() => Promise.all([k.e(951), k.e(324)]).then((() => () => k(742)))))
     }, g = {
-        52: [52],
-        518: [526],
+        324: [526],
         652: [174, 685],
-        694: [289, 671]
+        694: [289, 671],
+        828: [828]
     }, k.f.consumes = (e, r) => {
         k.o(g, e) && g[e].forEach((e => {
             if (k.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
@@ -266,15 +266,15 @@
         var e = {
             335: 0
         };
         k.f.j = (r, t) => {
             var n = k.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(52|694)$/.test(r)) e[r] = 0;
+                else if (/^(694|828)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
                 var i = k.p + k.u(r),
                     a = new Error;
                 k.l(i, (t => {
                     if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
@@ -296,8 +296,8 @@
             },
             t = self.webpackChunk_jupyterlite_pyodide_kernel_extension = self.webpackChunk_jupyterlite_pyodide_kernel_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var P = k(405);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlite/pyodide-kernel-extension"] = P
 })();
-//# sourceMappingURL=remoteEntry.b340cae4b3c1bda6a7fd.js.map
+//# sourceMappingURL=remoteEntry.703f03086e9738104706.js.map
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.b340cae4b3c1bda6a7fd.js.map` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/remoteEntry.703f03086e9738104706.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'remoteEntry.703f03086e9738104706.js'",*

 * * "'mappings'": "'uCACIA,EADAC,ECAAC,EACAC,ECDAC,EAIAC,EAIAC,EAIAC,EAIAC,EAYAC,EAMAC,EAOAC,EAUAC,EAuBAC,EAIAC,EAqBAC,EAwBAC,EAQAC,EACAC,EASAC,E,iBC7IJ,IAAIC,EAAY,CACf,UAAW,IACHC,QAAQC,IAAI,CAACC,EAAoBC,EAAE,KAAMD,EAAoBC,EAAE,OAAOC,MAAK,IAAM,IAASF,EAAoB,OAEtH,cAAe,IACPF,QAAQC,IAAI,CAACC,EAAoBC,EAAE,KAAMD,EAAoBC,EAAE,OAAOC,MAAK,IAAM,IAASF,EAAoB,QAGnHV,EAAM,CAACa,EAAQC,KAClBJ,EAAoBK,EAAID,EACxBA,EACCJ,EAAoBM,EAAET,EAAWM,GAC9BN,EAAUM,KACVL,QAAQS,UAAUL,MAAK,KACx […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.b340cae4b3c1bda6a7fd.js",
-    "mappings": "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",
+    "file": "remoteEntry.703f03086e9738104706.js",
+    "mappings": "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",
     "names": [
         "leafPrototypes",
         "getProto",
         "inProgress",
         "dataWebpackPrefix",
         "parseVersion",
         "versionLt",
@@ -202,24 +202,24 @@
         "webpack://@jupyterlite/pyodide-kernel-extension/webpack/runtime/publicPath",
         "webpack://@jupyterlite/pyodide-kernel-extension/webpack/runtime/jsonp chunk loading",
         "webpack://@jupyterlite/pyodide-kernel-extension/webpack/startup"
     ],
     "sourcesContent": [
         "var getProto = Object.getPrototypeOf ? (obj) => (Object.getPrototypeOf(obj)) : (obj) => (obj.__proto__);\nvar leafPrototypes;\n// create a fake namespace object\n// mode & 1: value is a module id, require it\n// mode & 2: merge all properties of value into the ns\n// mode & 4: return value when already ns object\n// mode & 16: return value when it's Promise-like\n// mode & 8|1: behave like require\n__webpack_require__.t = function(value, mode) {\n\tif(mode & 1) value = this(value);\n\tif(mode & 8) return value;\n\tif(typeof value === 'object' && value) {\n\t\tif((mode & 4) && value.__esModule) return value;\n\t\tif((mode & 16) && typeof value.then === 'function') return value;\n\t}\n\tvar ns = Object.create(null);\n\t__webpack_require__.r(ns);\n\tvar def = {};\n\tleafPrototypes = leafPrototypes || [null, getProto({}), getProto([]), getProto(getProto)];\n\tfor(var current = mode & 2 && value; typeof current == 'object' && !~leafPrototypes.indexOf(current); current = getProto(current)) {\n\t\tObject.getOwnPropertyNames(current).forEach((key) => (def[key] = () => (value[key])));\n\t}\n\tdef['default'] = () => (value);\n\t__webpack_require__.d(ns, def);\n\treturn ns;\n};",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@jupyterlite/pyodide-kernel-extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t289: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/kernel\", [2,0,1,0,,\"beta\",18])),\n\t671: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t174: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/server\", [2,0,1,0,,\"beta\",18])),\n\t685: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/contents\", [2,0,1,0,,\"beta\",18])),\n\t526: () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t52: () => (loadStrictVersionCheckFallback(\"default\", \"@jupyterlite/pyodide-kernel\", [3,0,0,8], () => (Promise.all([__webpack_require__.e(951), __webpack_require__.e(518)]).then(() => (() => (__webpack_require__(2)))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"52\": [\n\t\t52\n\t],\n\t\"518\": [\n\t\t526\n\t],\n\t\"652\": [\n\t\t174,\n\t\t685\n\t],\n\t\"694\": [\n\t\t289,\n\t\t671\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t289: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/kernel\", [2,0,1,0,,\"beta\",18])),\n\t671: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t174: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/server\", [2,0,1,0,,\"beta\",18])),\n\t685: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlite/contents\", [2,0,1,0,,\"beta\",18])),\n\t526: () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t828: () => (loadStrictVersionCheckFallback(\"default\", \"@jupyterlite/pyodide-kernel\", [3,0,0,9], () => (Promise.all([__webpack_require__.e(951), __webpack_require__.e(324)]).then(() => (() => (__webpack_require__(742)))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"324\": [\n\t\t526\n\t],\n\t\"652\": [\n\t\t174,\n\t\t685\n\t],\n\t\"694\": [\n\t\t289,\n\t\t671\n\t],\n\t\"828\": [\n\t\t828\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(694), __webpack_require__.e(652)]).then(() => (() => ((__webpack_require__(763)))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(694), __webpack_require__.e(652)]).then(() => (() => ((__webpack_require__(763)))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "__webpack_require__.amdO = {};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"52\":\"354648418987bd848171\",\"518\":\"a3c6a3ae7ee95e5158aa\",\"568\":\"371c75f0cd43fa31532d\",\"652\":\"07cda501733578161e13\",\"694\":\"e063d498fa9e311b3f30\",\"951\":\"b9fa6250974e699a3731\"}[chunkId] + \".js?v=\" + {\"52\":\"354648418987bd848171\",\"518\":\"a3c6a3ae7ee95e5158aa\",\"568\":\"371c75f0cd43fa31532d\",\"652\":\"07cda501733578161e13\",\"694\":\"e063d498fa9e311b3f30\",\"951\":\"b9fa6250974e699a3731\"}[chunkId] + \"\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"324\":\"2759063405b36360da9d\",\"568\":\"371c75f0cd43fa31532d\",\"652\":\"ecdf94afc2748b3fc2e0\",\"694\":\"e063d498fa9e311b3f30\",\"828\":\"18cd1cea0272a9fd42b1\",\"951\":\"b9fa6250974e699a3731\"}[chunkId] + \".js?v=\" + {\"324\":\"2759063405b36360da9d\",\"568\":\"371c75f0cd43fa31532d\",\"652\":\"ecdf94afc2748b3fc2e0\",\"694\":\"e063d498fa9e311b3f30\",\"828\":\"18cd1cea0272a9fd42b1\",\"951\":\"b9fa6250974e699a3731\"}[chunkId] + \"\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@jupyterlite/pyodide-kernel-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@jupyterlite/pyodide-kernel-extension\", \"0.0.8\", () => (Promise.all([__webpack_require__.e(694), __webpack_require__.e(652)]).then(() => (() => (__webpack_require__(763))))));\n\t\t\tregister(\"@jupyterlite/pyodide-kernel\", \"0.0.8\", () => (Promise.all([__webpack_require__.e(951), __webpack_require__.e(518), __webpack_require__.e(694)]).then(() => (() => (__webpack_require__(2))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@jupyterlite/pyodide-kernel-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@jupyterlite/pyodide-kernel-extension\", \"0.0.9\", () => (Promise.all([__webpack_require__.e(694), __webpack_require__.e(652)]).then(() => (() => (__webpack_require__(763))))));\n\t\t\tregister(\"@jupyterlite/pyodide-kernel\", \"0.0.9\", () => (Promise.all([__webpack_require__.e(951), __webpack_require__.e(324), __webpack_require__.e(694)]).then(() => (() => (__webpack_require__(742))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t335: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^(52|694)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_jupyterlite_pyodide_kernel_extension\"] = self[\"webpackChunk_jupyterlite_pyodide_kernel_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t335: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^(694|828)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_jupyterlite_pyodide_kernel_extension\"] = self[\"webpackChunk_jupyterlite_pyodide_kernel_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(405);\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/third-party-licenses.json` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '0.0.9'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "BSD 3-Clause License\n\nCopyright (c) 2022, JupyterLite Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/pyodide-kernel",
-            "versionInfo": "0.0.8"
+            "versionInfo": "0.0.9"
         },
         {
             "extractedText": "\n                                 Apache License\n                           Version 2.0, January 2004\n                        http://www.apache.org/licenses/\n\n   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION\n\n   1. Definitions.\n\n      \"License\" shall mean the terms and conditions for use, reproduction,\n      and distribution as defined by Sections 1 through 9 of this document.\n\n      \"Licensor\" shall mean the copyright owner or entity authorized by\n      the copyright owner that is granting the License.\n\n      \"Legal Entity\" shall mean the union of the acting entity and all\n      other entities that control, are controlled by, or are under common\n      control with that entity. For the purposes of this definition,\n      \"control\" means (i) the power, direct or indirect, to cause the\n      direction or management of such entity, whether by contract or\n      otherwise, or (ii) ownership of fifty percent (50%) or more of the\n      outstanding shares, or (iii) beneficial ownership of such entity.\n\n      \"You\" (or \"Your\") shall mean an individual or Legal Entity\n      exercising permissions granted by this License.\n\n      \"Source\" form shall mean the preferred form for making modifications,\n      including but not limited to software source code, documentation\n      source, and configuration files.\n\n      \"Object\" form shall mean any form resulting from mechanical\n      transformation or translation of a Source form, including but\n      not limited to compiled object code, generated documentation,\n      and conversions to other media types.\n\n      \"Work\" shall mean the work of authorship, whether in Source or\n      Object form, made available under the License, as indicated by a\n      copyright notice that is included in or attached to the work\n      (an example is provided in the Appendix below).\n\n      \"Derivative Works\" shall mean any work, whether in Source or Object\n      form, that is based on (or derived from) the Work and for which the\n      editorial revisions, annotations, elaborations, or other modifications\n      represent, as a whole, an original work of authorship. For the purposes\n      of this License, Derivative Works shall not include works that remain\n      separable from, or merely link (or bind by name) to the interfaces of,\n      the Work and Derivative Works thereof.\n\n      \"Contribution\" shall mean any work of authorship, including\n      the original version of the Work and any modifications or additions\n      to that Work or Derivative Works thereof, that is intentionally\n      submitted to Licensor for inclusion in the Work by the copyright owner\n      or by an individual or Legal Entity authorized to submit on behalf of\n      the copyright owner. For the purposes of this definition, \"submitted\"\n      means any form of electronic, verbal, or written communication sent\n      to the Licensor or its representatives, including but not limited to\n      communication on electronic mailing lists, source code control systems,\n      and issue tracking systems that are managed by, or on behalf of, the\n      Licensor for the purpose of discussing and improving the Work, but\n      excluding communication that is conspicuously marked or otherwise\n      designated in writing by the copyright owner as \"Not a Contribution.\"\n\n      \"Contributor\" shall mean Licensor and any individual or Legal Entity\n      on behalf of whom a Contribution has been received by Licensor and\n      subsequently incorporated within the Work.\n\n   2. Grant of Copyright License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      copyright license to reproduce, prepare Derivative Works of,\n      publicly display, publicly perform, sublicense, and distribute the\n      Work and such Derivative Works in Source or Object form.\n\n   3. Grant of Patent License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      (except as stated in this section) patent license to make, have made,\n      use, offer to sell, sell, import, and otherwise transfer the Work,\n      where such license applies only to those patent claims licensable\n      by such Contributor that are necessarily infringed by their\n      Contribution(s) alone or by combination of their Contribution(s)\n      with the Work to which such Contribution(s) was submitted. If You\n      institute patent litigation against any entity (including a\n      cross-claim or counterclaim in a lawsuit) alleging that the Work\n      or a Contribution incorporated within the Work constitutes direct\n      or contributory patent infringement, then any patent licenses\n      granted to You under this License for that Work shall terminate\n      as of the date such litigation is filed.\n\n   4. Redistribution. You may reproduce and distribute copies of the\n      Work or Derivative Works thereof in any medium, with or without\n      modifications, and in Source or Object form, provided that You\n      meet the following conditions:\n\n      (a) You must give any other recipients of the Work or\n          Derivative Works a copy of this License; and\n\n      (b) You must cause any modified files to carry prominent notices\n          stating that You changed the files; and\n\n      (c) You must retain, in the Source form of any Derivative Works\n          that You distribute, all copyright, patent, trademark, and\n          attribution notices from the Source form of the Work,\n          excluding those notices that do not pertain to any part of\n          the Derivative Works; and\n\n      (d) If the Work includes a \"NOTICE\" text file as part of its\n          distribution, then any Derivative Works that You distribute must\n          include a readable copy of the attribution notices contained\n          within such NOTICE file, excluding those notices that do not\n          pertain to any part of the Derivative Works, in at least one\n          of the following places: within a NOTICE text file distributed\n          as part of the Derivative Works; within the Source form or\n          documentation, if provided along with the Derivative Works; or,\n          within a display generated by the Derivative Works, if and\n          wherever such third-party notices normally appear. The contents\n          of the NOTICE file are for informational purposes only and\n          do not modify the License. You may add Your own attribution\n          notices within Derivative Works that You distribute, alongside\n          or as an addendum to the NOTICE text from the Work, provided\n          that such additional attribution notices cannot be construed\n          as modifying the License.\n\n      You may add Your own copyright statement to Your modifications and\n      may provide additional or different license terms and conditions\n      for use, reproduction, or distribution of Your modifications, or\n      for any such Derivative Works as a whole, provided Your use,\n      reproduction, and distribution of the Work otherwise complies with\n      the conditions stated in this License.\n\n   5. Submission of Contributions. Unless You explicitly state otherwise,\n      any Contribution intentionally submitted for inclusion in the Work\n      by You to the Licensor shall be under the terms and conditions of\n      this License, without any additional terms or conditions.\n      Notwithstanding the above, nothing herein shall supersede or modify\n      the terms of any separate license agreement you may have executed\n      with Licensor regarding such Contributions.\n\n   6. Trademarks. This License does not grant permission to use the trade\n      names, trademarks, service marks, or product names of the Licensor,\n      except as required for reasonable and customary use in describing the\n      origin of the Work and reproducing the content of the NOTICE file.\n\n   7. Disclaimer of Warranty. Unless required by applicable law or\n      agreed to in writing, Licensor provides the Work (and each\n      Contributor provides its Contributions) on an \"AS IS\" BASIS,\n      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\n      implied, including, without limitation, any warranties or conditions\n      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A\n      PARTICULAR PURPOSE. You are solely responsible for determining the\n      appropriateness of using or redistributing the Work and assume any\n      risks associated with Your exercise of permissions under this License.\n\n   8. Limitation of Liability. In no event and under no legal theory,\n      whether in tort (including negligence), contract, or otherwise,\n      unless required by applicable law (such as deliberate and grossly\n      negligent acts) or agreed to in writing, shall any Contributor be\n      liable to You for damages, including any direct, indirect, special,\n      incidental, or consequential damages of any character arising as a\n      result of this License or out of the use or inability to use the\n      Work (including but not limited to damages for loss of goodwill,\n      work stoppage, computer failure or malfunction, or any and all\n      other commercial damages or losses), even if such Contributor\n      has been advised of the possibility of such damages.\n\n   9. Accepting Warranty or Additional Liability. While redistributing\n      the Work or Derivative Works thereof, You may choose to offer,\n      and charge a fee for, acceptance of support, warranty, indemnity,\n      or other liability obligations and/or rights consistent with this\n      License. However, in accepting such obligations, You may act only\n      on Your own behalf and on Your sole responsibility, not on behalf\n      of any other Contributor, and only if You agree to indemnify,\n      defend, and hold each Contributor harmless for any liability\n      incurred by, or claims asserted against, such Contributor by reason\n      of your accepting any such warranty or additional liability.\n\n   END OF TERMS AND CONDITIONS\n\n   APPENDIX: How to apply the Apache License to your work.\n\n      To apply the Apache License to your work, attach the following\n      boilerplate notice, with the fields enclosed by brackets \"[]\"\n      replaced with your own identifying information. (Don't include\n      the brackets!)  The text should be enclosed in the appropriate\n      comment syntax for the file format. We also recommend that a\n      file or class name and description of purpose be included on the\n      same \"printed page\" as the copyright notice for easier\n      identification within third-party archives.\n\n   Copyright 2017 Google Inc.\n\n   Licensed under the Apache License, Version 2.0 (the \"License\");\n   you may not use this file except in compliance with the License.\n   You may obtain a copy of the License at\n\n       http://www.apache.org/licenses/LICENSE-2.0\n\n   Unless required by applicable law or agreed to in writing, software\n   distributed under the License is distributed on an \"AS IS\" BASIS,\n   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n   See the License for the specific language governing permissions and\n   limitations under the License.",
             "licenseId": "Apache-2.0",
             "name": "comlink",
             "versionInfo": "4.4.1"
         },
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/all.json` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/all.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8656250000000001%*

 * *Differences: {"'ipykernel'": "{'releases': {'6.9.2': {0: {'digests': {'md5': "*

 * *                "'79e6908c1898dab331c487c46ca355bc', 'sha256': "*

 * *                "'e5bf6bf7c38ffbb71085a95f7eb55d55e89c82fab61fd9361e317fcb90360130'}, "*

 * *                "'md5_digest': '79e6908c1898dab331c487c46ca355bc', 'size': 6513, 'upload_time': "*

 * *                "'2023-08-02T12:44:14.557813Z', 'upload_time_iso_8601': "*

 * *                "'2023-08-02T12:44:14.557813Z'}}}}",*

 * * "'piplite'": "{'releases': {replace: OrderedDict([('0.0.9', [Ordere […]*

```diff
@@ -1,127 +1,127 @@
 {
     "ipykernel": {
         "releases": {
             "6.9.2": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "50b0ac28df1e02972a7ba285a5498af8",
-                        "sha256": "cc0462b5e9eb7fcbe412f1c2f716c3d13a4ad567c418afa253d974e631341f26"
+                        "md5": "79e6908c1898dab331c487c46ca355bc",
+                        "sha256": "e5bf6bf7c38ffbb71085a95f7eb55d55e89c82fab61fd9361e317fcb90360130"
                     },
                     "downloads": -1,
                     "filename": "ipykernel-6.9.2-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "50b0ac28df1e02972a7ba285a5498af8",
+                    "md5_digest": "79e6908c1898dab331c487c46ca355bc",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": ">=3.10",
-                    "size": 6512,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 6513,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./ipykernel-6.9.2-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "piplite": {
         "releases": {
-            "0.0.8": [
+            "0.0.9": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "653e410da79aef82d7b7dcc25500033e",
-                        "sha256": "94fb854bc4a72fd9dcdbae39d719294166dda95cdec3dadcd2468dfd5962c444"
+                        "md5": "d37090e6a13ea988333a51ab1fa865fa",
+                        "sha256": "1797f065c1e845e29960333955d0b9222d97ed0dbcae422872ac0c0713201031"
                     },
                     "downloads": -1,
-                    "filename": "piplite-0.0.8-py3-none-any.whl",
+                    "filename": "piplite-0.0.9-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "653e410da79aef82d7b7dcc25500033e",
+                    "md5_digest": "d37090e6a13ea988333a51ab1fa865fa",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 6720,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
-                    "url": "./piplite-0.0.8-py3-none-any.whl",
+                    "size": 6718,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
+                    "url": "./piplite-0.0.9-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "pyodide-kernel": {
         "releases": {
-            "0.0.8": [
+            "0.0.9": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "e7a145dc94d6973a2e5c302a354d5768",
-                        "sha256": "66d2829fb698aa2a6360871960eb8df4e661cf637ad1ba94b3e003eaefe4fcf7"
+                        "md5": "0df4ba9b821f1fa6f176ca7e4d6e382a",
+                        "sha256": "d2224fe7066ce8b372e20d7aa1f8d69e5ed1b2547340331d8ea5b01402279403"
                     },
                     "downloads": -1,
-                    "filename": "pyodide_kernel-0.0.8-py3-none-any.whl",
+                    "filename": "pyodide_kernel-0.0.9-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "e7a145dc94d6973a2e5c302a354d5768",
+                    "md5_digest": "0df4ba9b821f1fa6f176ca7e4d6e382a",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 8221,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
-                    "url": "./pyodide_kernel-0.0.8-py3-none-any.whl",
+                    "size": 8222,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
+                    "url": "./pyodide_kernel-0.0.9-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "widgetsnbextension": {
         "releases": {
             "3.6.4": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "0c562267b54decbba3df65748e8a50c1",
-                        "sha256": "508cf73575b9efb7fe405f50a52c5fbb0a4d5f7ebe3b8e5098c13f74bc58a366"
+                        "md5": "cacd42516decc405948cc366d99deeef",
+                        "sha256": "8e2dc2570bf54e61aedd2c52ebae4e048a7d860bad3f6a5eec0b2c7529807bcc"
                     },
                     "downloads": -1,
                     "filename": "widgetsnbextension-3.6.4-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "0c562267b54decbba3df65748e8a50c1",
+                    "md5_digest": "cacd42516decc405948cc366d99deeef",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 2337,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 2338,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./widgetsnbextension-3.6.4-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ],
             "4.0.7": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "522d33a007aa29a012295f9505f093d5",
-                        "sha256": "d0fb5501925193f011d56ea7df530cff64ed90fdce2c5aa8d7cb755953694a10"
+                        "md5": "6c1bf4b38ec6a57b885322f085902e88",
+                        "sha256": "8933202971deb5120a9ebb518a640b51acbb37ae54e8623ad7883c348e6646ad"
                     },
                     "downloads": -1,
                     "filename": "widgetsnbextension-4.0.7-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "522d33a007aa29a012295f9505f093d5",
+                    "md5_digest": "6c1bf4b38ec6a57b885322f085902e88",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 2337,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 2338,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./widgetsnbextension-4.0.7-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     }
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6512 bytes, number of entries: 7
--rw-r--r--  2.0 unx      133 b- defN 23-May-04 13:01 ipykernel/__init__.py
--rw-r--r--  2.0 unx     7026 b- defN 23-May-04 13:01 ipykernel/comm.py
--rw-r--r--  2.0 unx     5102 b- defN 23-May-04 13:01 ipykernel/jsonutil.py
-?rw-r--r--  2.0 unx      424 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      539 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/RECORD
-7 files, 14835 bytes uncompressed, 5562 bytes compressed:  62.5%
+Zip file size: 6513 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      133 b- defN 23-Aug-02 07:20 ipykernel/__init__.py
+-rw-r--r--  2.0 unx     7026 b- defN 23-Aug-02 07:20 ipykernel/comm.py
+-rw-r--r--  2.0 unx     5102 b- defN 23-Aug-02 07:20 ipykernel/jsonutil.py
+?rw-r--r--  2.0 unx      424 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      539 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/RECORD
+7 files, 14835 bytes uncompressed, 5563 bytes compressed:  62.5%
```

#### ipykernel-6.9.2.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### ipykernel-6.9.2.dist-info/RECORD

```diff
@@ -1,7 +1,7 @@
 ipykernel/__init__.py,sha256=RJFGnC1Jf4urbq3S1FDJmGGbAkyANMuPFftZDR20d2E,133
 ipykernel/comm.py,sha256=wsdtPIjlzPI72CdFqpVn5mJBp4qAI1Ut7tEgBtQ3x8w,7026
 ipykernel/jsonutil.py,sha256=7kInhZjFl4q3WNo9tz10Gy6N5tsbiF7R6buIYh8oCBA,5102
 ipykernel-6.9.2.dist-info/METADATA,sha256=ePjA9gFWVMXeJlT7vSr5Mb7SloZmarODuFFuXRw5484,424
-ipykernel-6.9.2.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+ipykernel-6.9.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 ipykernel-6.9.2.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 ipykernel-6.9.2.dist-info/RECORD,,
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/piplite-0.0.9-py3-none-any.whl`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6720 bytes, number of entries: 7
--rw-r--r--  2.0 unx      155 b- defN 23-May-04 13:01 piplite/__init__.py
--rw-r--r--  2.0 unx     4720 b- defN 23-May-04 13:01 piplite/cli.py
--rw-r--r--  2.0 unx     6574 b- defN 23-May-04 13:01 piplite/piplite.py
-?rw-r--r--  2.0 unx      631 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      523 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/RECORD
-7 files, 14214 bytes uncompressed, 5802 bytes compressed:  59.2%
+Zip file size: 6718 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      155 b- defN 23-Aug-02 07:20 piplite/__init__.py
+-rw-r--r--  2.0 unx     4720 b- defN 23-Aug-02 07:20 piplite/cli.py
+-rw-r--r--  2.0 unx     6574 b- defN 23-Aug-02 07:20 piplite/piplite.py
+?rw-r--r--  2.0 unx      631 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      523 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/RECORD
+7 files, 14214 bytes uncompressed, 5800 bytes compressed:  59.2%
```

#### zipnote «TEMP»/diffoscope_dibrkpdu_/tmp_a6yr48x_.zip

```diff
@@ -3,20 +3,20 @@
 
 Filename: piplite/cli.py
 Comment: 
 
 Filename: piplite/piplite.py
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/METADATA
+Filename: piplite-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/WHEEL
+Filename: piplite-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/licenses/LICENSE
+Filename: piplite-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/RECORD
+Filename: piplite-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### piplite/__init__.py

```diff
@@ -1,6 +1,6 @@
 """A configurable Python package backed by Pyodide's micropip"""
 from .piplite import install
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 __all__ = ["install", "__version__"]
```

#### Comparing `piplite-0.0.8.dist-info/METADATA` & `piplite-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piplite
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Source, https://github.com/jupyterlite/pyodide-kernel
 Author: JupyterLite Contributors
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: <3.12,>=3.11
 Description-Content-Type: text/markdown
```

#### Comparing `piplite-0.0.8.dist-info/licenses/LICENSE` & `piplite-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/pyodide_kernel-0.0.9-py3-none-any.whl`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8221 bytes, number of entries: 11
--rw-r--r--  2.0 unx      712 b- defN 23-May-04 13:01 pyodide_kernel/__init__.py
--rw-r--r--  2.0 unx     2269 b- defN 23-May-04 13:01 pyodide_kernel/display.py
--rw-r--r--  2.0 unx     2454 b- defN 23-May-04 13:01 pyodide_kernel/interpreter.py
--rw-r--r--  2.0 unx     3992 b- defN 23-May-04 13:01 pyodide_kernel/kernel.py
--rw-r--r--  2.0 unx     3197 b- defN 23-May-04 13:01 pyodide_kernel/litetransform.py
--rw-r--r--  2.0 unx     1290 b- defN 23-May-04 13:01 pyodide_kernel/mocks.py
--rw-r--r--  2.0 unx      404 b- defN 23-May-04 13:01 pyodide_kernel/patches.py
-?rw-r--r--  2.0 unx      480 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      910 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/RECORD
-11 files, 17319 bytes uncompressed, 6679 bytes compressed:  61.4%
+Zip file size: 8222 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      712 b- defN 23-Aug-02 07:20 pyodide_kernel/__init__.py
+-rw-r--r--  2.0 unx     2269 b- defN 23-Aug-02 07:20 pyodide_kernel/display.py
+-rw-r--r--  2.0 unx     2454 b- defN 23-Aug-02 07:20 pyodide_kernel/interpreter.py
+-rw-r--r--  2.0 unx     3992 b- defN 23-Aug-02 07:20 pyodide_kernel/kernel.py
+-rw-r--r--  2.0 unx     3197 b- defN 23-Aug-02 07:20 pyodide_kernel/litetransform.py
+-rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 07:20 pyodide_kernel/mocks.py
+-rw-r--r--  2.0 unx      404 b- defN 23-Aug-02 07:20 pyodide_kernel/patches.py
+?rw-r--r--  2.0 unx      480 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      910 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/RECORD
+11 files, 17319 bytes uncompressed, 6680 bytes compressed:  61.4%
```

#### zipnote «TEMP»/diffoscope_dibrkpdu_/tmp6fwqqxdk_.zip

```diff
@@ -15,20 +15,20 @@
 
 Filename: pyodide_kernel/mocks.py
 Comment: 
 
 Filename: pyodide_kernel/patches.py
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/METADATA
+Filename: pyodide_kernel-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/WHEEL
+Filename: pyodide_kernel-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/licenses/LICENSE
+Filename: pyodide_kernel-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/RECORD
+Filename: pyodide_kernel-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### pyodide_kernel/__init__.py

```diff
@@ -1,10 +1,10 @@
 """A Python kernel backed by Pyodide"""
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import sys
 
 # 0. do early mocks that change `sys.modules`
 from . import mocks
 
 mocks.apply_mocks()
```

#### Comparing `pyodide_kernel-0.0.8.dist-info/licenses/LICENSE` & `pyodide_kernel-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

#### Comparing `pyodide_kernel-0.0.8.dist-info/RECORD` & `pyodide_kernel-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyodide_kernel/__init__.py,sha256=dYfAxEhgAibmjAiInRjyrR3pcJf_wRJEJxoGXvwKlAM,712
+pyodide_kernel/__init__.py,sha256=Qnl9_48L6uB-riqcyTHIlruB8qq2ZT0wjThLStcnh4A,712
 pyodide_kernel/display.py,sha256=j_iSs9w55XmCy9XpHReCQR2OGFUMnkMoAKMp_sqBT5I,2269
 pyodide_kernel/interpreter.py,sha256=YFyEXcTpjQqPWExo0MQa8COVraO8Ihz8bobon5Ye-48,2454
 pyodide_kernel/kernel.py,sha256=0ofEqk2yimW6J8wpnCeIdxz6BujUOLxbmeUT3zdaCRo,3992
 pyodide_kernel/litetransform.py,sha256=Iqlxj39Y-P0O1Wjk3kXi1Sqo--IL4ROLV-L_s2jPVbE,3197
 pyodide_kernel/mocks.py,sha256=X49fD89PBn-rVNvkDcbGrDhMpg3Ybc1mhc-Bo0tqI8o,1290
 pyodide_kernel/patches.py,sha256=ApUGlW0FYBdKrLQx8wiqt0jLxrJnm5CxYBVHmlCnSVQ,404
-pyodide_kernel-0.0.8.dist-info/METADATA,sha256=cqQONeS_vb2-now9zyPMLSeS83mDAntDbx41bSUW4PQ,480
-pyodide_kernel-0.0.8.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-pyodide_kernel-0.0.8.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
-pyodide_kernel-0.0.8.dist-info/RECORD,,
+pyodide_kernel-0.0.9.dist-info/METADATA,sha256=SMhPNseQ3MfZP5r3P25ugDZH6fmAfHni7VtbTl79XF8,480
+pyodide_kernel-0.0.9.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+pyodide_kernel-0.0.9.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
+pyodide_kernel-0.0.9.dist-info/RECORD,,
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2337 bytes, number of entries: 5
--rw-r--r--  2.0 unx       55 b- defN 23-May-04 13:01 widgetsnbextension/__init__.py
-?rw-r--r--  2.0 unx      492 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      431 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/RECORD
-5 files, 2589 bytes uncompressed, 1525 bytes compressed:  41.1%
+Zip file size: 2338 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       55 b- defN 23-Aug-02 07:20 widgetsnbextension/__init__.py
+?rw-r--r--  2.0 unx      492 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      431 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/RECORD
+5 files, 2589 bytes uncompressed, 1526 bytes compressed:  41.1%
```

#### widgetsnbextension-3.6.4.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### widgetsnbextension-3.6.4.dist-info/RECORD

```diff
@@ -1,5 +1,5 @@
 widgetsnbextension/__init__.py,sha256=Ehhe-iBe2kPDIVP1GNDa2H2FK8miBEV6ZRcDdsXCwa0,55
 widgetsnbextension-3.6.4.dist-info/METADATA,sha256=POvFnV5PBUrTYnef8n-JNTGFvU2fCsQal6LZSB6cLcg,492
-widgetsnbextension-3.6.4.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+widgetsnbextension-3.6.4.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 widgetsnbextension-3.6.4.dist-info/RECORD,,
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2337 bytes, number of entries: 5
--rw-r--r--  2.0 unx       55 b- defN 23-May-04 13:01 widgetsnbextension/__init__.py
-?rw-r--r--  2.0 unx      493 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      431 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/RECORD
-5 files, 2590 bytes uncompressed, 1525 bytes compressed:  41.1%
+Zip file size: 2338 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       55 b- defN 23-Aug-02 07:20 widgetsnbextension/__init__.py
+?rw-r--r--  2.0 unx      493 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      431 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/RECORD
+5 files, 2590 bytes uncompressed, 1526 bytes compressed:  41.1%
```

#### widgetsnbextension-4.0.7.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### widgetsnbextension-4.0.7.dist-info/RECORD

```diff
@@ -1,5 +1,5 @@
 widgetsnbextension/__init__.py,sha256=FUS4iRrSk7iROOXwaTdKPfC1CChNMdht0P2bZQaBVys,55
 widgetsnbextension-4.0.7.dist-info/METADATA,sha256=ggM19V05p03L7JurOviHELE2nzokq4fT1yrTMODRjlo,493
-widgetsnbextension-4.0.7.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+widgetsnbextension-4.0.7.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 widgetsnbextension-4.0.7.dist-info/RECORD,,
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/schema/kernel.v0.schema.json` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/schema/kernel.v0.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'properties'": "{'pyodideUrl': {'default': "*

 * *                 "'https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js'}}"}*

```diff
@@ -14,15 +14,15 @@
             "format": "uri",
             "items": {
                 "type": "string"
             },
             "type": "array"
         },
         "pyodideUrl": {
-            "default": "https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js",
+            "default": "https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js",
             "description": "The path to the main pyodide.js entry point",
             "format": "uri",
             "type": "string"
         }
     },
     "title": "Pyodide Kernel Settings Schema v0",
     "type": "object"
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/labextension/static/schema/piplite.v0.schema.json` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/labextension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/conftest.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_piplite.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_piplite.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_pyodide.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_pyodide.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/test_repo.py` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/jupyterlite_pyodide_kernel/tests/fixtures/the_smallest_extension-0.1.0-py3-none-any.whl` & `jupyterlite_pyodide_kernel-0.0.9/jupyterlite_pyodide_kernel/tests/fixtures/the_smallest_extension-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/.gitignore` & `jupyterlite_pyodide_kernel-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/LICENSE` & `jupyterlite_pyodide_kernel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/README.md` & `jupyterlite_pyodide_kernel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_pyodide_kernel-0.0.8/pyproject.toml` & `jupyterlite_pyodide_kernel-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,18 @@
     "--self-contained-html",
 ]
 
 [tool.jupyter-releaser.options]
 version_cmd = "python scripts/bump-version.py"
 
 [tool.jupyter-releaser.hooks]
+before-bump-version = [
+    "python -m pip install jupyterlab~=3.5.3",
+    "jlpm"
+]
 before-build-npm = [
     "python -m pip install jupyterlab~=3.5.3 hatch",
     "python -m pip install -e .[dev]",
     "jlpm",
     "jlpm build:prod",
 ]
 before-build-python = [
```

### Comparing `jupyterlite_pyodide_kernel-0.0.8/PKG-INFO` & `jupyterlite_pyodide_kernel-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite-pyodide-kernel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python kernel for JupyterLite powered by Pyodide
 Project-URL: Homepage, https://jupyterlite-pyodide-kernel.readthedocs.io
 Project-URL: Documentation, https://jupyterlite-pyodide-kernel.readthedocs.io
 Project-URL: Source, https://github.com/jupyterlite/pyodide-kernel
 Project-URL: Issues, https://github.com/jupyterlite/pyodide-kernel/issues
 Project-URL: PyPI, https://pypi.org/project/jupyterlite-pyodide-kernel
 Author: JupyterLite Contributors
```

