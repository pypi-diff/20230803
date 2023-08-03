# Comparing `tmp/mkdocs_material_adr-1.1.0a2.tar.gz` & `tmp/mkdocs_material_adr-1.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_material_adr-1.1.0a2.tar", max compression
+gzip compressed data, was "mkdocs_material_adr-1.1.0a3.tar", max compression
```

## Comparing `mkdocs_material_adr-1.1.0a2.tar` & `mkdocs_material_adr-1.1.0a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/LICENSE
--rw-r--r--   0        0        0     1857 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/README.md
--rw-r--r--   0        0        0        0 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/__init__.py
--rw-r--r--   0        0        0      139 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/base_adr.html
--rw-r--r--   0        0        0       30 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/main.html
--rw-r--r--   0        0        0      658 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/mkdocs_theme.yml
--rw-r--r--   0        0        0     1370 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/partials/adr.html
--rw-r--r--   0        0        0      586 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/partials/content.html
--rw-r--r--   0        0        0        0 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/plugins/graph/__init__.py
--rw-r--r--   0        0        0     4706 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/plugins/graph/plugin.py
--rw-r--r--   0        0        0     1553 2023-08-03 14:09:55.155845 mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/stylesheets/adr.css
--rw-r--r--   0        0        0      873 2023-08-03 14:10:11.064087 mkdocs_material_adr-1.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     2949 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a2/setup.py
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 14:18:24.678570 mkdocs_material_adr-1.1.0a3/LICENSE
+-rw-r--r--   0        0        0     1857 2023-08-03 14:18:24.678570 mkdocs_material_adr-1.1.0a3/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/base_adr.html
+-rw-r--r--   0        0        0       30 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/main.html
+-rw-r--r--   0        0        0      658 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1370 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/partials/adr.html
+-rw-r--r--   0        0        0      586 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/partials/content.html
+-rw-r--r--   0        0        0        0 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/plugins/graph/__init__.py
+-rw-r--r--   0        0        0     4736 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/plugins/graph/plugin.py
+-rw-r--r--   0        0        0     1553 2023-08-03 14:18:24.682570 mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/stylesheets/adr.css
+-rw-r--r--   0        0        0      873 2023-08-03 14:18:34.546355 mkdocs_material_adr-1.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2949 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a3/setup.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 mkdocs_material_adr-1.1.0a3/PKG-INFO
```

### Comparing `mkdocs_material_adr-1.1.0a2/LICENSE` & `mkdocs_material_adr-1.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/README.md` & `mkdocs_material_adr-1.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/mkdocs_theme.yml` & `mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/partials/adr.html` & `mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/partials/adr.html`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/partials/content.html` & `mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/partials/content.html`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/plugins/graph/plugin.py` & `mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/plugins/graph/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return datetime.strptime(value, "%d-%b-%Y").date()
 
     @classmethod
     def build_from_page(cls, page) -> "Record":
         return cls(
             title=page.title,
             id=_get_id_from_page(page),
-            url=page.abs_url,
+            url=page.abs_url if page.abs_url else page.url,
             tags=page.meta.get("tags", []),
             **page.meta.get("adr"),
         )
 
 
 class RecordCollection:
     def __init__(self) -> None:
```

### Comparing `mkdocs_material_adr-1.1.0a2/mkdocs_material_adr/stylesheets/adr.css` & `mkdocs_material_adr-1.1.0a3/mkdocs_material_adr/stylesheets/adr.css`

 * *Files identical despite different names*

### Comparing `mkdocs_material_adr-1.1.0a2/pyproject.toml` & `mkdocs_material_adr-1.1.0a3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-material-adr"
-version = "1.1.0-alpha.2"
+version = "1.1.0-alpha.3"
 description = ""
 authors = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 readme = "README.md"
 packages = [{ include = "mkdocs_material_adr" }]
 license = "Apache-2.0"
 repository = "https://github.com/Kl0ven/mkdocs-material-adr"
```

### Comparing `mkdocs_material_adr-1.1.0a2/setup.py` & `mkdocs_material_adr-1.1.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 entry_points = \
 {'mkdocs.plugins': ['mkdocs-material-adr/adr = '
                     'mkdocs_material_adr.plugins.graph.plugin:AdrPlugin'],
  'mkdocs.themes': ['mkdocs-material-adr = mkdocs_material_adr']}
 
 setup_kwargs = {
     'name': 'mkdocs-material-adr',
-    'version': '1.1.0a2',
+    'version': '1.1.0a3',
     'description': '',
     'long_description': "# ADR for MkDocs's Material Theme\n\n[ADR](https://lyz-code.github.io/blue-book/adr/) are short text documents that captures an important architectural decision made along with its context and consequences.\n\n\n[Demo](http://blog.kloven.fr/mkdocs-material-adr/)\n\n## Install\n\n```bash\npip install mkdocs-material-adr\n# or\npoetry add mkdocs-material-adr\n```\n\nIn the `mkdocs.yml` file\n\n```yaml\ntheme:\n  # set the name\n  name: mkdocs-material-adr\n\n  # Configuration for the material theme\n  features:\n    - navigation.instant\n\n\nplugins:\n  - mkdocs-material-adr/adr\n```\n\n## Features\n\n### ADR Headers\nInformation about the ADR are displayed in a header\nDefine information about the ADR in the frontmatter.\n\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/header.png)\n\n\n```md\n---\n    title: 0004 Title\n    adr:\n        author: Jean-Loup Monnier\n        created: 01-Aug-2023\n        status:  draft | proposed | rejected | accepted | superseded\n        superseded_by: 0001-test\n        extends:\n            - 0001-first\n            - 0002-second\n---\n```\nYou can change the colors or add new status using css\n\n```css\n/* Background color */\n.c-pill-<lower_case_status_name> {\n    background: #a3a3a3;\n}\n\n/* Dot color */\n.c-pill-<lower_case_status_name>:before {\n    background: #505050;\n}\n```\n\n### ADR Graph\nAuto generated graph.\nTo enable it add `[GRAPH]` in the markdown file you want the graph to be, Then add th following configuration\n\n```yaml\n\n\nplugins:\n  - mkdocs-material-adr/adr:\n      graph_file: index.md # Change this to your file\n\nmarkdown_extensions:\n  - pymdownx.superfences:\n      custom_fences:\n      - name: mermaid\n        class: mermaid\n        format: !!python/name:pymdownx.superfences.fence_code_format\n```\n![Alt text](https://raw.githubusercontent.com/Kl0ven/mkdocs-material-adr/main/docs/assets/graph.png)\n",
     'author': 'jeanloup.monnier',
     'author_email': 'jean-loup.monnier@spikeelabs.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Kl0ven/mkdocs-material-adr',
```

### Comparing `mkdocs_material_adr-1.1.0a2/PKG-INFO` & `mkdocs_material_adr-1.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-material-adr
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: 
 Home-page: https://github.com/Kl0ven/mkdocs-material-adr
 License: Apache-2.0
 Author: jeanloup.monnier
 Author-email: jean-loup.monnier@spikeelabs.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

