# Comparing `tmp/mkdocs_material_adr-1.0.0.tar.gz` & `tmp/mkdocs_material_adr-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_material_adr-1.0.0.tar", max compression
+gzip compressed data, was "mkdocs_material_adr-1.0.1a1.tar", max compression
```

## Comparing `mkdocs_material_adr-1.0.0.tar` & `mkdocs_material_adr-1.0.1a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/LICENSE
--rw-r--r--   0        0        0      849 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/__init__.py
--rw-r--r--   0        0        0      139 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/base_adr.html
--rw-r--r--   0        0        0       30 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/main.html
--rw-r--r--   0        0        0      658 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/mkdocs_theme.yml
--rw-r--r--   0        0        0      592 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/partials/adr.html
--rw-r--r--   0        0        0      564 2023-08-02 13:09:57.909070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/partials/content.html
--rw-r--r--   0        0        0     1400 2023-08-02 13:09:57.913070 mkdocs_material_adr-1.0.0/mkdocs_material_adr/stylesheets/adr.css
--rw-r--r--   0        0        0      553 2023-08-02 13:10:12.909242 mkdocs_material_adr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.0/setup.py
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/LICENSE
+-rw-r--r--   0        0        0     1231 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/base_adr.html
+-rw-r--r--   0        0        0       30 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/main.html
+-rw-r--r--   0        0        0      658 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/mkdocs_theme.yml
+-rw-r--r--   0        0        0      592 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/adr.html
+-rw-r--r--   0        0        0      564 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/content.html
+-rw-r--r--   0        0        0     1400 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/stylesheets/adr.css
+-rw-r--r--   0        0        0      731 2023-08-02 13:49:45.734737 mkdocs_material_adr-1.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     2047 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.1a1/setup.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.1a1/PKG-INFO
```

### Comparing `mkdocs_material_adr-1.0.0/LICENSE` & `mkdocs_material_adr-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.0/README.md` & `mkdocs_material_adr-1.0.1a1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,41 @@
 # ADR for MkDocs's Material Theme
 
 [ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.
 
+
+[Demo](http://blog.kloven.fr/mkdocs-material-adr/)
+
+## Install
+
+```bash
+pip install mkdocs-material-adr
+# or
+poetry add mkdocs-material-adr
+```
+
+In the `mkdocs.yml` file
+
+```yaml
+theme:
+  # set the name
+  name: mkdocs-material-adr
+
+  # Configuration for the material theme
+  features:
+    - navigation.instant
+```
+
 ## Features
 
 ### ADR Headers
 Information about the ADR are displayed in a header
 Define information about the ADR in the frontmatter.
 
-![Alt text](docs/assets/header.png)
+![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/header.png)
 
 
 ```md
 ---
     title: 0004 Title
     adr:
         author: Jean-Loup Monnier
```

### Comparing `mkdocs_material_adr-1.0.0/mkdocs_material_adr/mkdocs_theme.yml` & `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.0/mkdocs_material_adr/partials/adr.html` & `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/adr.html`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.0/mkdocs_material_adr/partials/content.html` & `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/content.html`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.0/mkdocs_material_adr/stylesheets/adr.css` & `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/stylesheets/adr.css`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.0/pyproject.toml` & `mkdocs_material_adr-1.0.1a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 [tool.poetry]
 name = "mkdocs-material-adr"
-version = "1.0.0"
+version = "1.0.1-alpha.1"
 description = ""
 authors = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 readme = "README.md"
 packages = [{ include = "mkdocs_material_adr" }]
+license = "Apache-2.0"
+repository = "https://github.com/Kl0ven/mkdocs-material-adr"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."mkdocs.themes"]
-"mkdocs_material_adr" = "mkdocs_material_adr"
+"mkdocs-material-adr" = "mkdocs_material_adr"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.1"
 pre-commit = "^3.3.3"
 
+
+[tool.poetry.group.demo.dependencies]
+mkdocs = "^1.5.1"
+mkdocs-material = "^9.1.21"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mkdocs_material_adr-1.0.0/setup.py` & `mkdocs_material_adr-1.0.1a1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['mkdocs_material_adr']
 
 package_data = \
 {'': ['*'], 'mkdocs_material_adr': ['partials/*', 'stylesheets/*']}
 
 entry_points = \
-{'mkdocs.themes': ['mkdocs_material_adr = mkdocs_material_adr']}
+{'mkdocs.themes': ['mkdocs-material-adr = mkdocs_material_adr']}
 
 setup_kwargs = {
     'name': 'mkdocs-material-adr',
-    'version': '1.0.0',
+    'version': '1.0.1a1',
     'description': '',
-    'long_description': "# ADR for MkDocs's Material Theme\n\n[ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.\n\n## Features\n\n### ADR Headers\nInformation about the ADR are displayed in a header\nDefine information about the ADR in the frontmatter.\n\n![Alt text](docs/assets/header.png)\n\n\n```md\n---\n    title: 0004 Title\n    adr:\n        author: Jean-Loup Monnier\n        created: 01-Aug-2023\n        status:  draft | proposed | rejected | accepted | superseded\n        superseded_by: 0001-test\n---\n```\nYou can change the colors or add new status using css\n\n```css\n/* Background color */\n.c-pill-<lower_case_status_name> {\n    background: #a3a3a3;\n}\n\n/* Dot color */\n.c-pill-<lower_case_status_name>:before {\n    background: #505050;\n}\n```\n\n### ADR Graph\nWIP\n",
+    'long_description': "# ADR for MkDocs's Material Theme\n\n[ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.\n\n\n[Demo](http://blog.kloven.fr/mkdocs-material-adr/)\n\n## Install\n\n```bash\npip install mkdocs-material-adr\n# or\npoetry add mkdocs-material-adr\n```\n\nIn the `mkdocs.yml` file\n\n```yaml\ntheme:\n  # set the name\n  name: mkdocs-material-adr\n\n  # Configuration for the material theme\n  features:\n    - navigation.instant\n```\n\n## Features\n\n### ADR Headers\nInformation about the ADR are displayed in a header\nDefine information about the ADR in the frontmatter.\n\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/header.png)\n\n\n```md\n---\n    title: 0004 Title\n    adr:\n        author: Jean-Loup Monnier\n        created: 01-Aug-2023\n        status:  draft | proposed | rejected | accepted | superseded\n        superseded_by: 0001-test\n---\n```\nYou can change the colors or add new status using css\n\n```css\n/* Background color */\n.c-pill-<lower_case_status_name> {\n    background: #a3a3a3;\n}\n\n/* Dot color */\n.c-pill-<lower_case_status_name>:before {\n    background: #505050;\n}\n```\n\n### ADR Graph\nWIP\n",
     'author': 'jeanloup.monnier',
     'author_email': 'jean-loup.monnier@spikeelabs.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/Kl0ven/mkdocs-material-adr',
     'packages': packages,
     'package_data': package_data,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

