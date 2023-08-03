# Comparing `tmp/dj-monaco-1.0.2.tar.gz` & `tmp/dj-monaco-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-monaco-1.0.2.tar", last modified: Wed Aug  2 09:25:03 2023, max compression
+gzip compressed data, was "dj-monaco-1.0.3.tar", last modified: Thu Aug  3 06:13:52 2023, max compression
```

## Comparing `dj-monaco-1.0.2.tar` & `dj-monaco-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.630602 dj-monaco-1.0.2/
--rw-r--r--   0 karel     (1000) karel     (1000)      173 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/AUTHORS.rst
--rw-r--r--   0 karel     (1000) karel     (1000)     3239 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 karel     (1000) karel     (1000)       97 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/HISTORY.rst
--rw-r--r--   0 karel     (1000) karel     (1000)     1091 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/LICENSE
--rw-rw-r--   0 karel     (1000) karel     (1000)      260 2022-07-27 23:30:41.000000 dj-monaco-1.0.2/MANIFEST.in
--rw-rw-r--   0 karel     (1000) karel     (1000)     2335 2023-08-02 09:25:03.630602 dj-monaco-1.0.2/PKG-INFO
--rw-r--r--   0 karel     (1000) karel     (1000)     1633 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/README.rst
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/dj_monaco.egg-info/
--rw-r--r--   0 karel     (1000) karel     (1000)     2335 2023-08-02 09:25:03.000000 dj-monaco-1.0.2/dj_monaco.egg-info/PKG-INFO
--rw-r--r--   0 karel     (1000) karel     (1000)      990 2023-08-02 09:25:03.000000 dj-monaco-1.0.2/dj_monaco.egg-info/SOURCES.txt
--rw-r--r--   0 karel     (1000) karel     (1000)        1 2023-08-02 09:25:03.000000 dj-monaco-1.0.2/dj_monaco.egg-info/dependency_links.txt
--rw-r--r--   0 karel     (1000) karel     (1000)        1 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/dj_monaco.egg-info/not-zip-safe
--rw-r--r--   0 karel     (1000) karel     (1000)        7 2023-08-02 09:25:03.000000 dj-monaco-1.0.2/dj_monaco.egg-info/requires.txt
--rw-r--r--   0 karel     (1000) karel     (1000)        9 2023-08-02 09:25:03.000000 dj-monaco-1.0.2/dj_monaco.egg-info/top_level.txt
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/
--rw-rw-r--   0 karel     (1000) karel     (1000)       22 2023-08-02 09:23:03.000000 dj-monaco-1.0.2/djmonaco/__init__.py
--rw-rw-r--   0 karel     (1000) karel     (1000)     1334 2023-08-02 09:18:08.000000 dj-monaco-1.0.2/djmonaco/admin.py
--rw-r--r--   0 karel     (1000) karel     (1000)      111 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/apps.py
--rw-rw-r--   0 karel     (1000) karel     (1000)      933 2023-08-02 09:18:17.000000 dj-monaco-1.0.2/djmonaco/forms.py
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/migrations/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/migrations/__init__.py
--rw-rw-r--   0 karel     (1000) karel     (1000)      873 2023-08-02 09:18:24.000000 dj-monaco-1.0.2/djmonaco/models.py
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.622603 dj-monaco-1.0.2/djmonaco/static/
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/static/css/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/static/css/djmonaco.css
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/static/djmonaco/
--rw-rw-r--   0 karel     (1000) karel     (1000)      320 2023-08-02 09:20:39.000000 dj-monaco-1.0.2/djmonaco/static/djmonaco/monaco-editor.css
--rw-rw-r--   0 karel     (1000) karel     (1000)     5585 2023-08-01 01:24:13.000000 dj-monaco-1.0.2/djmonaco/static/djmonaco/monaco-editor.js
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/static/js/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/static/js/djmonaco.js
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.622603 dj-monaco-1.0.2/djmonaco/templates/
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/templates/djmonaco/
--rw-r--r--   0 karel     (1000) karel     (1000)      108 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/templates/djmonaco/monaco.html
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/test_utils/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/__init__.py
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/test_utils/test_app/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/test_app/__init__.py
--rw-r--r--   0 karel     (1000) karel     (1000)       70 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/test_app/admin.py
--rw-r--r--   0 karel     (1000) karel     (1000)       90 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/test_app/apps.py
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/djmonaco/test_utils/test_app/migrations/
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/test_app/migrations/__init__.py
--rw-r--r--   0 karel     (1000) karel     (1000)       58 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/test_utils/test_app/models.py
--rw-r--r--   0 karel     (1000) karel     (1000)      116 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/urls.py
--rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/djmonaco/views.py
--rw-rw-r--   0 karel     (1000) karel     (1000)      814 2023-08-01 01:24:13.000000 dj-monaco-1.0.2/djmonaco/widgets.py
--rw-r--r--   0 karel     (1000) karel     (1000)      100 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/pyproject.toml
--rw-r--r--   0 karel     (1000) karel     (1000)       41 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/requirements.txt
--rw-r--r--   0 karel     (1000) karel     (1000)       51 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/requirements_dev.txt
--rw-r--r--   0 karel     (1000) karel     (1000)      109 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/requirements_test.txt
--rw-r--r--   0 karel     (1000) karel     (1000)      248 2023-08-02 09:25:03.630602 dj-monaco-1.0.2/setup.cfg
--rwxrwxr-x   0 karel     (1000) karel     (1000)     2139 2022-07-27 23:35:56.000000 dj-monaco-1.0.2/setup.py
-drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-02 09:25:03.626603 dj-monaco-1.0.2/tests/
--rw-r--r--   0 karel     (1000) karel     (1000)      333 2022-07-17 05:53:01.000000 dj-monaco-1.0.2/tests/test_models.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/
+-rw-r--r--   0 karel     (1000) karel     (1000)      173 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/AUTHORS.rst
+-rw-r--r--   0 karel     (1000) karel     (1000)     3239 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 karel     (1000) karel     (1000)       97 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/HISTORY.rst
+-rw-r--r--   0 karel     (1000) karel     (1000)     1091 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/LICENSE
+-rw-rw-r--   0 karel     (1000) karel     (1000)      260 2022-07-27 23:30:41.000000 dj-monaco-1.0.3/MANIFEST.in
+-rw-rw-r--   0 karel     (1000) karel     (1000)     2335 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/PKG-INFO
+-rw-r--r--   0 karel     (1000) karel     (1000)     1633 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/README.rst
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/dj_monaco.egg-info/
+-rw-r--r--   0 karel     (1000) karel     (1000)     2335 2023-08-03 06:13:52.000000 dj-monaco-1.0.3/dj_monaco.egg-info/PKG-INFO
+-rw-r--r--   0 karel     (1000) karel     (1000)      990 2023-08-03 06:13:52.000000 dj-monaco-1.0.3/dj_monaco.egg-info/SOURCES.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)        1 2023-08-03 06:13:52.000000 dj-monaco-1.0.3/dj_monaco.egg-info/dependency_links.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)        1 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/dj_monaco.egg-info/not-zip-safe
+-rw-r--r--   0 karel     (1000) karel     (1000)        7 2023-08-03 06:13:52.000000 dj-monaco-1.0.3/dj_monaco.egg-info/requires.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)        9 2023-08-03 06:13:52.000000 dj-monaco-1.0.3/dj_monaco.egg-info/top_level.txt
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/
+-rw-rw-r--   0 karel     (1000) karel     (1000)       22 2023-08-03 06:13:18.000000 dj-monaco-1.0.3/djmonaco/__init__.py
+-rw-rw-r--   0 karel     (1000) karel     (1000)     1334 2023-08-03 06:07:10.000000 dj-monaco-1.0.3/djmonaco/admin.py
+-rw-r--r--   0 karel     (1000) karel     (1000)      111 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/apps.py
+-rw-rw-r--   0 karel     (1000) karel     (1000)      933 2023-08-03 06:07:01.000000 dj-monaco-1.0.3/djmonaco/forms.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/migrations/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/migrations/__init__.py
+-rw-rw-r--   0 karel     (1000) karel     (1000)      873 2023-08-03 06:06:53.000000 dj-monaco-1.0.3/djmonaco/models.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/static/
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/static/css/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/static/css/djmonaco.css
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/static/djmonaco/
+-rw-rw-r--   0 karel     (1000) karel     (1000)      320 2023-08-02 09:20:39.000000 dj-monaco-1.0.3/djmonaco/static/djmonaco/monaco-editor.css
+-rw-rw-r--   0 karel     (1000) karel     (1000)     5848 2023-08-03 06:10:26.000000 dj-monaco-1.0.3/djmonaco/static/djmonaco/monaco-editor.js
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/djmonaco/static/js/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/static/js/djmonaco.js
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.477710 dj-monaco-1.0.3/djmonaco/templates/
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/djmonaco/templates/djmonaco/
+-rw-r--r--   0 karel     (1000) karel     (1000)      108 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/templates/djmonaco/monaco.html
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/djmonaco/test_utils/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/__init__.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/djmonaco/test_utils/test_app/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/test_app/__init__.py
+-rw-r--r--   0 karel     (1000) karel     (1000)       70 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/test_app/admin.py
+-rw-r--r--   0 karel     (1000) karel     (1000)       90 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/test_app/apps.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/djmonaco/test_utils/test_app/migrations/
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/test_app/migrations/__init__.py
+-rw-r--r--   0 karel     (1000) karel     (1000)       58 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/test_utils/test_app/models.py
+-rw-r--r--   0 karel     (1000) karel     (1000)      116 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/urls.py
+-rw-r--r--   0 karel     (1000) karel     (1000)        0 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/djmonaco/views.py
+-rw-rw-r--   0 karel     (1000) karel     (1000)      814 2023-08-01 01:24:13.000000 dj-monaco-1.0.3/djmonaco/widgets.py
+-rw-r--r--   0 karel     (1000) karel     (1000)      100 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/pyproject.toml
+-rw-r--r--   0 karel     (1000) karel     (1000)       41 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/requirements.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)       51 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/requirements_dev.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)      109 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/requirements_test.txt
+-rw-r--r--   0 karel     (1000) karel     (1000)      248 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/setup.cfg
+-rwxrwxr-x   0 karel     (1000) karel     (1000)     2139 2022-07-27 23:35:56.000000 dj-monaco-1.0.3/setup.py
+drwxrwxr-x   0 karel     (1000) karel     (1000)        0 2023-08-03 06:13:52.481710 dj-monaco-1.0.3/tests/
+-rw-r--r--   0 karel     (1000) karel     (1000)      333 2022-07-17 05:53:01.000000 dj-monaco-1.0.3/tests/test_models.py
```

### Comparing `dj-monaco-1.0.2/CONTRIBUTING.rst` & `dj-monaco-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/LICENSE` & `dj-monaco-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/PKG-INFO` & `dj-monaco-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-monaco
-Version: 1.0.2
+Version: 1.0.3
 Summary: django widget for monaco editor
 Home-page: https://github.com/kverdecia/dj-monaco
 Author: Karel Antonio Verdecia Ortiz
 Author-email: kverdecia@gmail.com
 License: MIT
 Keywords: dj-monaco
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dj-monaco-1.0.2/README.rst` & `dj-monaco-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/dj_monaco.egg-info/PKG-INFO` & `dj-monaco-1.0.3/dj_monaco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-monaco
-Version: 1.0.2
+Version: 1.0.3
 Summary: django widget for monaco editor
 Home-page: https://github.com/kverdecia/dj-monaco
 Author: Karel Antonio Verdecia Ortiz
 Author-email: kverdecia@gmail.com
 License: MIT
 Keywords: dj-monaco
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dj-monaco-1.0.2/dj_monaco.egg-info/SOURCES.txt` & `dj-monaco-1.0.3/dj_monaco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/djmonaco/admin.py` & `dj-monaco-1.0.3/djmonaco/admin.py`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/djmonaco/forms.py` & `dj-monaco-1.0.3/djmonaco/forms.py`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/djmonaco/models.py` & `dj-monaco-1.0.3/djmonaco/models.py`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/djmonaco/static/djmonaco/monaco-editor.js` & `dj-monaco-1.0.3/djmonaco/static/djmonaco/monaco-editor.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -78,24 +78,32 @@
                         diagnosticsOptions.enableSchemaRequest = true;
                 }
 
                 if (Object.keys(diagnosticsOptions).length > 1) {
                     monaco.languages.json.jsonDefaults.setDiagnosticsOptions(diagnosticsOptions);
                 }
 
-                var editor = monaco.editor.create(document.getElementById(container.id + '--editor'), {
+                const editor = monaco.editor.create(document.getElementById(container.id + '--editor'), {
                     renderWhitespace: true,
                     language: container.dataset.language,
                     wordWrap: container.dataset.wordwrap || 'off',
                     minimap: {
                         enabled: container.dataset.minimap === 'true'
                     },
                     fontSize: 12 + 1,
                     value: container.value
                 });
+                const event = new CustomEvent('monaco:editor-created', {
+                    detail: {
+                        editor,
+                        container,
+                    },
+                });
+                document.dispatchEvent(event);
+
 
                 if (container.dataset.language === 'html') {
                     emmetMonaco.emmetHTML(monaco);
                 } else if (container.dataset.language === 'css') {
                     emmetMonaco.emmetCSS(monaco);
                 }
```

### Comparing `dj-monaco-1.0.2/djmonaco/widgets.py` & `dj-monaco-1.0.3/djmonaco/widgets.py`

 * *Files identical despite different names*

### Comparing `dj-monaco-1.0.2/setup.py` & `dj-monaco-1.0.3/setup.py`

 * *Files identical despite different names*

