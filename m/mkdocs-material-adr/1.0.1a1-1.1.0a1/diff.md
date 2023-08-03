# Comparing `tmp/mkdocs_material_adr-1.0.1a1.tar.gz` & `tmp/mkdocs_material_adr-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_material_adr-1.0.1a1.tar", max compression
+gzip compressed data, was "mkdocs_material_adr-1.1.0a1.tar", max compression
```

## Comparing `mkdocs_material_adr-1.0.1a1.tar` & `mkdocs_material_adr-1.1.0a1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     1231 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/README.md
--rw-r--r--   0        0        0        0 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/__init__.py
--rw-r--r--   0        0        0      139 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/base_adr.html
--rw-r--r--   0        0        0       30 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/main.html
--rw-r--r--   0        0        0      658 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/mkdocs_theme.yml
--rw-r--r--   0        0        0      592 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/adr.html
--rw-r--r--   0        0        0      564 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/content.html
--rw-r--r--   0        0        0     1400 2023-08-02 13:49:31.994609 mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/stylesheets/adr.css
--rw-r--r--   0        0        0      731 2023-08-02 13:49:45.734737 mkdocs_material_adr-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     2047 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.1a1/setup.py
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 13:45:29.830490 mkdocs_material_adr-1.1.0a1/LICENSE
+-rw-r--r--   0        0        0     1857 2023-08-03 13:45:29.830490 mkdocs_material_adr-1.1.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/base_adr.html
+-rw-r--r--   0        0        0       30 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/main.html
+-rw-r--r--   0        0        0      658 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1370 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/partials/adr.html
+-rw-r--r--   0        0        0      586 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/partials/content.html
+-rw-r--r--   0        0        0        0 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/plugins/graph/__init__.py
+-rw-r--r--   0        0        0     4702 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/plugins/graph/plugin.py
+-rw-r--r--   0        0        0     1553 2023-08-03 13:45:29.834491 mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/stylesheets/adr.css
+-rw-r--r--   0        0        0      873 2023-08-03 13:45:40.086654 mkdocs_material_adr-1.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2949 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a1/setup.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a1/PKG-INFO
```

### Comparing `mkdocs_material_adr-1.0.1a1/LICENSE` & `mkdocs_material_adr-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.1a1/README.md` & `mkdocs_material_adr-1.1.0a1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 theme:
   # set the name
   name: mkdocs-material-adr
 
   # Configuration for the material theme
   features:
     - navigation.instant
+
+
+plugins:
+  - mkdocs-material-adr/adr
 ```
 
 ## Features
 
 ### ADR Headers
 Information about the ADR are displayed in a header
 Define information about the ADR in the frontmatter.
@@ -38,14 +42,17 @@
 ---
     title: 0004 Title
     adr:
         author: Jean-Loup Monnier
         created: 01-Aug-2023
         status:  draft | proposed | rejected | accepted | superseded
         superseded_by: 0001-test
+        extends:
+            - 0001-first
+            - 0002-second
 ---
 ```
 You can change the colors or add new status using css
 
 ```css
 /* Background color */
 .c-pill-<lower_case_status_name> {
@@ -55,8 +62,25 @@
 /* Dot color */
 .c-pill-<lower_case_status_name>:before {
     background: #505050;
 }
 ```
 
 ### ADR Graph
-WIP
+Auto generated graph.
+To enable it add `[GRAPH]` in the markdown file you want the graph to be, Then add th following configuration
+
+```yaml
+
+
+plugins:
+  - mkdocs-material-adr/adr:
+      graph_file: index.md # Change this to your file
+
+markdown_extensions:
+  - pymdownx.superfences:
+      custom_fences:
+      - name: mermaid
+        class: mermaid
+        format: !!python/name:pymdownx.superfences.fence_code_format
+```
+![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/graph.png)
```

### Comparing `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/mkdocs_theme.yml` & `mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/partials/content.html` & `mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/partials/content.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% if "material/tags" in config.plugins %}
+{% if "material/tags" in config.plugins and not page.meta.adr %}
 {% include "partials/tags.html" %}
 {% endif %}
 {% include "partials/actions.html" %}
 
 {% if "\x3ch1" not in page.content %}
 <h1>{{ page.title | d(config.site_name, true)}}</h1>
 {% endif %}
```

### Comparing `mkdocs_material_adr-1.0.1a1/mkdocs_material_adr/stylesheets/adr.css` & `mkdocs_material_adr-1.1.0a1/mkdocs_material_adr/stylesheets/adr.css`

 * *Files 6% similar despite different names*

```diff
@@ -84,7 +84,18 @@
 .c-pill-superseded {
     background: #ffebb6;
 }
 
 .c-pill-superseded:before {
     background: #ffc400;
 }
+
+
+.adr_header .md-tag {
+    display: inline !important;
+
+}
+
+.adr_header .md-tags {
+    margin-bottom: 0% !important;
+    margin-top: unset !important;
+}
```

### Comparing `mkdocs_material_adr-1.0.1a1/pyproject.toml` & `mkdocs_material_adr-1.1.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 [tool.poetry]
 name = "mkdocs-material-adr"
-version = "1.0.1-alpha.1"
+version = "1.1.0-alpha.1"
 description = ""
 authors = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 readme = "README.md"
 packages = [{ include = "mkdocs_material_adr" }]
 license = "Apache-2.0"
 repository = "https://github.com/Kl0ven/mkdocs-material-adr"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."mkdocs.themes"]
 "mkdocs-material-adr" = "mkdocs_material_adr"
 
 
+[tool.poetry.plugins."mkdocs.plugins"]
+"mkdocs-material-adr/adr" = "mkdocs_material_adr.plugins.graph.plugin:AdrPlugin"
+
+
 [tool.poetry.dependencies]
 python = "^3.9"
+pydantic = "^2.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.1"
 pre-commit = "^3.3.3"
```

### Comparing `mkdocs_material_adr-1.0.1a1/setup.py` & `mkdocs_material_adr-1.1.0a1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mkdocs_material_adr']
+['mkdocs_material_adr', 'mkdocs_material_adr.plugins.graph']
 
 package_data = \
 {'': ['*'], 'mkdocs_material_adr': ['partials/*', 'stylesheets/*']}
 
+install_requires = \
+['pydantic>=2.1.1,<3.0.0']
+
 entry_points = \
-{'mkdocs.themes': ['mkdocs-material-adr = mkdocs_material_adr']}
+{'mkdocs.plugins': ['mkdocs-material-adr/adr = '
+                    'mkdocs_material_adr.plugins.graph.plugin:AdrPlugin'],
+ 'mkdocs.themes': ['mkdocs-material-adr = mkdocs_material_adr']}
 
 setup_kwargs = {
     'name': 'mkdocs-material-adr',
-    'version': '1.0.1a1',
+    'version': '1.1.0a1',
     'description': '',
-    'long_description': "# ADR for MkDocs's Material Theme\n\n[ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.\n\n\n[Demo](http://blog.kloven.fr/mkdocs-material-adr/)\n\n## Install\n\n```bash\npip install mkdocs-material-adr\n# or\npoetry add mkdocs-material-adr\n```\n\nIn the `mkdocs.yml` file\n\n```yaml\ntheme:\n  # set the name\n  name: mkdocs-material-adr\n\n  # Configuration for the material theme\n  features:\n    - navigation.instant\n```\n\n## Features\n\n### ADR Headers\nInformation about the ADR are displayed in a header\nDefine information about the ADR in the frontmatter.\n\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/header.png)\n\n\n```md\n---\n    title: 0004 Title\n    adr:\n        author: Jean-Loup Monnier\n        created: 01-Aug-2023\n        status:  draft | proposed | rejected | accepted | superseded\n        superseded_by: 0001-test\n---\n```\nYou can change the colors or add new status using css\n\n```css\n/* Background color */\n.c-pill-<lower_case_status_name> {\n    background: #a3a3a3;\n}\n\n/* Dot color */\n.c-pill-<lower_case_status_name>:before {\n    background: #505050;\n}\n```\n\n### ADR Graph\nWIP\n",
+    'long_description': "# ADR for MkDocs's Material Theme\n\n[ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.\n\n\n[Demo](http://blog.kloven.fr/mkdocs-material-adr/)\n\n## Install\n\n```bash\npip install mkdocs-material-adr\n# or\npoetry add mkdocs-material-adr\n```\n\nIn the `mkdocs.yml` file\n\n```yaml\ntheme:\n  # set the name\n  name: mkdocs-material-adr\n\n  # Configuration for the material theme\n  features:\n    - navigation.instant\n\n\nplugins:\n  - mkdocs-material-adr/adr\n```\n\n## Features\n\n### ADR Headers\nInformation about the ADR are displayed in a header\nDefine information about the ADR in the frontmatter.\n\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/header.png)\n\n\n```md\n---\n    title: 0004 Title\n    adr:\n        author: Jean-Loup Monnier\n        created: 01-Aug-2023\n        status:  draft | proposed | rejected | accepted | superseded\n        superseded_by: 0001-test\n        extends:\n            - 0001-first\n            - 0002-second\n---\n```\nYou can change the colors or add new status using css\n\n```css\n/* Background color */\n.c-pill-<lower_case_status_name> {\n    background: #a3a3a3;\n}\n\n/* Dot color */\n.c-pill-<lower_case_status_name>:before {\n    background: #505050;\n}\n```\n\n### ADR Graph\nAuto generated graph.\nTo enable it add `[GRAPH]` in the markdown file you want the graph to be, Then add th following configuration\n\n```yaml\n\n\nplugins:\n  - mkdocs-material-adr/adr:\n      graph_file: index.md # Change this to your file\n\nmarkdown_extensions:\n  - pymdownx.superfences:\n      custom_fences:\n      - name: mermaid\n        class: mermaid\n        format: !!python/name:pymdownx.superfences.fence_code_format\n```\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/graph.png)\n",
     'author': 'jeanloup.monnier',
     'author_email': 'jean-loup.monnier@spikeelabs.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Kl0ven/mkdocs-material-adr',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mkdocs_material_adr-1.0.1a1/PKG-INFO` & `mkdocs_material_adr-1.1.0a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mkdocs-material-adr
-Version: 1.0.1a1
+Version: 1.1.0a1
 Summary: 
 Home-page: https://github.com/Kl0ven/mkdocs-material-adr
 License: Apache-2.0
 Author: jeanloup.monnier
 Author-email: jean-loup.monnier@spikeelabs.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Kl0ven/mkdocs-material-adr
 Description-Content-Type: text/markdown
 
 # ADR for MkDocs's Material Theme
 
 [ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.
 
@@ -36,14 +37,18 @@
 theme:
   # set the name
   name: mkdocs-material-adr
 
   # Configuration for the material theme
   features:
     - navigation.instant
+
+
+plugins:
+  - mkdocs-material-adr/adr
 ```
 
 ## Features
 
 ### ADR Headers
 Information about the ADR are displayed in a header
 Define information about the ADR in the frontmatter.
@@ -55,14 +60,17 @@
 ---
     title: 0004 Title
     adr:
         author: Jean-Loup Monnier
         created: 01-Aug-2023
         status:  draft | proposed | rejected | accepted | superseded
         superseded_by: 0001-test
+        extends:
+            - 0001-first
+            - 0002-second
 ---
 ```
 You can change the colors or add new status using css
 
 ```css
 /* Background color */
 .c-pill-<lower_case_status_name> {
@@ -72,9 +80,26 @@
 /* Dot color */
 .c-pill-<lower_case_status_name>:before {
     background: #505050;
 }
 ```
 
 ### ADR Graph
-WIP
+Auto generated graph.
+To enable it add `[GRAPH]` in the markdown file you want the graph to be, Then add th following configuration
+
+```yaml
+
+
+plugins:
+  - mkdocs-material-adr/adr:
+      graph_file: index.md # Change this to your file
+
+markdown_extensions:
+  - pymdownx.superfences:
+      custom_fences:
+      - name: mermaid
+        class: mermaid
+        format: !!python/name:pymdownx.superfences.fence_code_format
+```
+![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/graph.png)
```

