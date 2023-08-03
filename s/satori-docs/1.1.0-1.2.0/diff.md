# Comparing `tmp/satori_docs-1.1.0.tar.gz` & `tmp/satori_docs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_docs-1.1.0.tar", last modified: Thu Aug  3 00:49:30 2023, max compression
+gzip compressed data, was "satori_docs-1.2.0.tar", last modified: Thu Aug  3 01:14:33 2023, max compression
```

## Comparing `satori_docs-1.1.0.tar` & `satori_docs-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0    35149 2023-08-03 00:49:16.035056 satori_docs-1.1.0/LICENSE
--rw-r--r--   0        0        0       54 2023-08-03 00:49:16.035056 satori_docs-1.1.0/README.md
--rw-r--r--   0        0        0      520 2023-08-03 00:49:30.950983 satori_docs-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/Dockerfile
--rw-r--r--   0        0        0     3132 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/README.md
--rw-r--r--   0        0        0        0 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/__init__.py
--rw-r--r--   0        0        0      474 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/_sidebar.md
--rw-r--r--   0        0        0     2591 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/asynchronous_and_synchronous_executions.md
--rw-r--r--   0        0        0      597 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/config.md
--rw-r--r--   0        0        0     1518 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/examples/hello_world.md
--rw-r--r--   0        0        0      438 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/examples/monitor.yml
--rw-r--r--   0        0        0      146 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/examples/ping.yml
--rw-r--r--   0        0        0     2145 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/github_ci.md
--rw-r--r--   0        0        0      636 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/gitlab.md
--rw-r--r--   0        0        0   152994 2023-08-03 00:49:16.035056 satori_docs-1.1.0/src/docs/img/async.png
--rw-r--r--   0        0        0  2393400 2023-08-03 00:49:16.047056 satori_docs-1.1.0/src/docs/img/sync-output.png
--rw-r--r--   0        0        0   379295 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/img/sync-report.png
--rw-r--r--   0        0        0   194316 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/img/sync.png
--rw-r--r--   0        0        0     1386 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/index.html
--rw-r--r--   0        0        0     1416 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/install.md
--rw-r--r--   0        0        0     2655 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language.md
--rw-r--r--   0        0        0    12198 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language_asserts.md
--rw-r--r--   0        0        0      994 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language_execution.md
--rw-r--r--   0        0        0     1422 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language_inputs.md
--rw-r--r--   0        0        0     4742 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language_playbooks.md
--rw-r--r--   0        0        0     6062 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/language_settings.md
--rw-r--r--   0        0        0     1282 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/mode.md
--rw-r--r--   0        0        0     2404 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/monitor.md
--rw-r--r--   0        0        0     2807 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/notifications.md
--rw-r--r--   0        0        0      813 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/playbook.md
--rw-r--r--   0        0        0     4820 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/repo.md
--rw-r--r--   0        0        0     3101 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/report.md
--rw-r--r--   0        0        0     2136 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/run.md
--rw-r--r--   0        0        0     1208 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/team.md
--rw-r--r--   0        0        0    16108 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/theme.css
--rw-r--r--   0        0        0     1491 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/docs/user_accounts.md
--rw-r--r--   0        0        0        0 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/satori_help/__init__.py
--rw-r--r--   0        0        0     1646 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/satori_help/gui.py
--rw-r--r--   0        0        0      887 2023-08-03 00:49:16.051056 satori_docs-1.1.0/src/satori_help/main.py
--rw-r--r--   0        0        0    40907 1970-01-01 00:00:00.000000 satori_docs-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 01:14:19.138469 satori_docs-1.2.0/LICENSE
+-rw-r--r--   0        0        0       54 2023-08-03 01:14:19.138469 satori_docs-1.2.0/README.md
+-rw-r--r--   0        0        0      520 2023-08-03 01:14:33.438568 satori_docs-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/Dockerfile
+-rw-r--r--   0        0        0     3132 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/__init__.py
+-rw-r--r--   0        0        0      474 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/_sidebar.md
+-rw-r--r--   0        0        0     2591 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/asynchronous_and_synchronous_executions.md
+-rw-r--r--   0        0        0      597 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/config.md
+-rw-r--r--   0        0        0     1518 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/examples/hello_world.md
+-rw-r--r--   0        0        0      438 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/examples/monitor.yml
+-rw-r--r--   0        0        0      146 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/examples/ping.yml
+-rw-r--r--   0        0        0     2145 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/github_ci.md
+-rw-r--r--   0        0        0      636 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/gitlab.md
+-rw-r--r--   0        0        0   152994 2023-08-03 01:14:19.138469 satori_docs-1.2.0/src/docs/img/async.png
+-rw-r--r--   0        0        0  2393400 2023-08-03 01:14:19.154469 satori_docs-1.2.0/src/docs/img/sync-output.png
+-rw-r--r--   0        0        0   379295 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/img/sync-report.png
+-rw-r--r--   0        0        0   194316 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/img/sync.png
+-rw-r--r--   0        0        0     1778 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/index.html
+-rw-r--r--   0        0        0     1416 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/install.md
+-rw-r--r--   0        0        0     2655 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language.md
+-rw-r--r--   0        0        0    12198 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language_asserts.md
+-rw-r--r--   0        0        0      994 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language_execution.md
+-rw-r--r--   0        0        0     1422 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language_inputs.md
+-rw-r--r--   0        0        0     4742 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language_playbooks.md
+-rw-r--r--   0        0        0     6062 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/language_settings.md
+-rw-r--r--   0        0        0     1282 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/mode.md
+-rw-r--r--   0        0        0     2404 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/monitor.md
+-rw-r--r--   0        0        0     2807 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/notifications.md
+-rw-r--r--   0        0        0      813 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/playbook.md
+-rw-r--r--   0        0        0     4820 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/repo.md
+-rw-r--r--   0        0        0     3101 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/report.md
+-rw-r--r--   0        0        0     2136 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/run.md
+-rw-r--r--   0        0        0     1208 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/team.md
+-rw-r--r--   0        0        0     1491 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/docs/user_accounts.md
+-rw-r--r--   0        0        0        0 2023-08-03 01:14:19.158469 satori_docs-1.2.0/src/satori_help/__init__.py
+-rw-r--r--   0        0        0     1646 2023-08-03 01:14:19.162469 satori_docs-1.2.0/src/satori_help/gui.py
+-rw-r--r--   0        0        0      887 2023-08-03 01:14:19.162469 satori_docs-1.2.0/src/satori_help/main.py
+-rw-r--r--   0        0        0    40907 1970-01-01 00:00:00.000000 satori_docs-1.2.0/PKG-INFO
```

### Comparing `satori_docs-1.1.0/LICENSE` & `satori_docs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/pyproject.toml` & `satori_docs-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-docs"
-version = "1.1.0"
+version = "1.2.0"
 description = "Satori CI - Automated Software Testing Platform Documents"
 authors = [
     { name = "Satori CI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "textual>=0.27.0",
 ]
```

### Comparing `satori_docs-1.1.0/src/docs/README.md` & `satori_docs-1.2.0/src/docs/README.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/asynchronous_and_synchronous_executions.md` & `satori_docs-1.2.0/src/docs/asynchronous_and_synchronous_executions.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/config.md` & `satori_docs-1.2.0/src/docs/config.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/examples/hello_world.md` & `satori_docs-1.2.0/src/docs/examples/hello_world.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/github_ci.md` & `satori_docs-1.2.0/src/docs/github_ci.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/gitlab.md` & `satori_docs-1.2.0/src/docs/gitlab.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/img/async.png` & `satori_docs-1.2.0/src/docs/img/async.png`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/img/sync-output.png` & `satori_docs-1.2.0/src/docs/img/sync-output.png`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/img/sync-report.png` & `satori_docs-1.2.0/src/docs/img/sync-report.png`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/img/sync.png` & `satori_docs-1.2.0/src/docs/img/sync.png`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/index.html` & `satori_docs-1.2.0/src/docs/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -2,40 +2,46 @@
 <html lang="en">
 <head>
   <meta charset="UTF-8">
   <title>Satori-CI Documentation</title>
   <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
   <meta name="description" content="Description">
   <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
-  <link rel="stylesheet" href="theme.css">
+  <link rel="stylesheet" media="(prefers-color-scheme: dark)" href="https://cdn.jsdelivr.net/npm/docsify-themeable@0/dist/css/theme-simple-dark.css">
+  <link rel="stylesheet" media="(prefers-color-scheme: light)" href="https://cdn.jsdelivr.net/npm/docsify-themeable@0/dist/css/theme-simple.css">
+  <style>
+    :root {
+      --theme-hue: 76;
+    }
+  </style>
 </head>
 <body>
   <nav>
     <a href="https://satori-ci.com">satori-ci.com</a>
   </nav>
   <div id="app"></div>
   <script>
     window.$docsify = {
       name: 'Satori CI Documentation',
       repo: '',
       loadSidebar: true,
-      mergeNavbar: true,//TODO: check this
       auto2top: true,
       autoHeader: true,
       maxLevel   : 3,
       subMaxLevel: 3,
       search: {
         depth      : 3,
         noData     : 'No results!',
         placeholder: 'Search...'
       },
     }
   </script>
   <!-- Docsify v4 -->
   <script src="https://cdn.jsdelivr.net/npm/docsify@4"></script>
+  <script src="https://cdn.jsdelivr.net/npm/docsify-themeable@0/dist/js/docsify-themeable.min.js"></script>
   <script src="https://unpkg.com/docsify-pagination/dist/docsify-pagination.min.js"></script>
   <script src="https://cdn.jsdelivr.net/npm/docsify@4/lib/plugins/search.js"></script>
   <script src="https://cdn.jsdelivr.net/npm/docsify-copy-code@2"></script>
-  <script src="//cdn.jsdelivr.net/npm/prismjs@1/components/prism-bash.min.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/prismjs@1/components/prism-yaml.min.js"></script>
+  <script src="https://cdn.jsdelivr.net/npm/prismjs@1/components/prism-bash.min.js"></script>
+  <script src="https://cdn.jsdelivr.net/npm/prismjs@1/components/prism-yaml.min.js"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 
 
 
+
  satori-ci.com
```

### Comparing `satori_docs-1.1.0/src/docs/install.md` & `satori_docs-1.2.0/src/docs/install.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language.md` & `satori_docs-1.2.0/src/docs/language.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language_asserts.md` & `satori_docs-1.2.0/src/docs/language_asserts.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language_execution.md` & `satori_docs-1.2.0/src/docs/language_execution.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language_inputs.md` & `satori_docs-1.2.0/src/docs/language_inputs.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language_playbooks.md` & `satori_docs-1.2.0/src/docs/language_playbooks.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/language_settings.md` & `satori_docs-1.2.0/src/docs/language_settings.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/mode.md` & `satori_docs-1.2.0/src/docs/mode.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/monitor.md` & `satori_docs-1.2.0/src/docs/monitor.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/notifications.md` & `satori_docs-1.2.0/src/docs/notifications.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/playbook.md` & `satori_docs-1.2.0/src/docs/playbook.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/repo.md` & `satori_docs-1.2.0/src/docs/repo.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/report.md` & `satori_docs-1.2.0/src/docs/report.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/run.md` & `satori_docs-1.2.0/src/docs/run.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/team.md` & `satori_docs-1.2.0/src/docs/team.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/docs/user_accounts.md` & `satori_docs-1.2.0/src/docs/user_accounts.md`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/satori_help/gui.py` & `satori_docs-1.2.0/src/satori_help/gui.py`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/src/satori_help/main.py` & `satori_docs-1.2.0/src/satori_help/main.py`

 * *Files identical despite different names*

### Comparing `satori_docs-1.1.0/PKG-INFO` & `satori_docs-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-docs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Satori CI - Automated Software Testing Platform Documents
 Author-Email: Satori CI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

