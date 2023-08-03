# Comparing `tmp/dkist-sphinx-theme-1.1.1.tar.gz` & `tmp/dkist-sphinx-theme-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-sphinx-theme-1.1.1.tar", last modified: Thu Dec  8 22:20:15 2022, max compression
+gzip compressed data, was "dkist-sphinx-theme-1.1.2.tar", last modified: Thu Aug  3 08:18:40 2023, max compression
```

## Comparing `dkist-sphinx-theme-1.1.1.tar` & `dkist-sphinx-theme-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      764 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    19617 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      207 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      350 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      512 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/
--rw-rw-rw-   0 root         (0) root         (0)      288 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.080663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/autoapi_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/autoapi_templates/python/
--rw-rw-rw-   0 root         (0) root         (0)     2441 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/autoapi_templates/python/module.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/autoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/core.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/verify_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     6191 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_intersphinx_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_requirements_table.py
--rw-rw-rw-   0 root         (0) root         (0)     6662 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_workflow_diagram.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/layout.html
--rw-rw-rw-   0 root         (0) root         (0)     1949 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/navbar.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/
--rw-rw-rw-   0 root         (0) root         (0)     6685 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/dkist.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/
--rw-rw-rw-   0 root         (0) root         (0)   147435 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg
--rw-rw-rw-   0 root         (0) root         (0)    18231 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/NSOlogo.gif
--rw-rw-rw-   0 root         (0) root         (0)    41662 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/favico.ico
--rw-rw-rw-   0 root         (0) root         (0)    10027 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/forkme.png
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/pdf_icon.png
--rw-rw-rw-   0 root         (0) root         (0)      322 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/theme.conf
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/tests/test_import.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-12-08 22:20:15.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1175 2022-12-08 22:20:15.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-12-08 22:20:15.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2022-12-08 22:20:15.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-12-08 22:20:15.000000 dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-12-08 22:20:15.084663 dkist-sphinx-theme-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-12-08 22:20:10.000000 dkist-sphinx-theme-1.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    19617 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/module.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/autoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/verify_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     6191 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_intersphinx_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_requirements_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     6662 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_workflow_diagram.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/navbar.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/dkist.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)   147435 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    18231 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/NSOlogo.gif
+-rw-rw-rw-   0 root         (0) root         (0)    41662 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/favico.ico
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/forkme.png
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/pdf_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/theme.conf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/test_import.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/setup.py
```

### Comparing `dkist-sphinx-theme-1.1.1/.gitignore` & `dkist-sphinx-theme-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/LICENSE.rst` & `dkist-sphinx-theme-1.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/bitbucket-pipelines.yml` & `dkist-sphinx-theme-1.1.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/autoapi_templates/python/module.rst` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/autoapi.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/autoapi.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/core.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/core.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/theme.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/theme.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/conf/verify_requirements.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/verify_requirements.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_intersphinx_mapping.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_intersphinx_mapping.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_requirements_table.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_requirements_table.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/create_workflow_diagram.py` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_workflow_diagram.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/layout.html` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/layout.html`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/navbar.html` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/navbar.html`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/dkist.css` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/dkist.css`

 * *Files 8% similar despite different names*

```diff
@@ -378,7 +378,25 @@
     }
 }
 
 /* Custom Stuff */
 ul.spec-table-ul {
     padding-left: 15px;
 }
+
+div.container.cell,
+div.container.cell_input,
+div.container.cell_output {
+    width: 100%;
+    display: block;
+    overflow-x: auto;
+}
+
+div.container.cell_input {
+    margin-bottom: 0;
+}
+
+div.container.cell_output {
+    overflow-y: auto;
+    max-height: 800px;
+    margin-top: 0;
+}
```

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/NSOlogo.gif` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/NSOlogo.gif`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/favico.ico` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/favico.ico`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/forkme.png` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/forkme.png`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme/dkist/static/img/pdf_icon.png` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/pdf_icon.png`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/dkist_sphinx_theme.egg-info/SOURCES.txt` & `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.1/setup.py` & `dkist-sphinx-theme-1.1.2/setup.py`

 * *Files identical despite different names*

