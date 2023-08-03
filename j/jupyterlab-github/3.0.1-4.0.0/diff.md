# Comparing `tmp/jupyterlab_github-3.0.1.tar.gz` & `tmp/jupyterlab_github-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/krassowski/jupyterlab-github/dist/tmpe6aycxuo/jupyterlab_github-3.0.1.tar", last modified: Sat Nov 27 16:59:05 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_github-3.0.1.tar` & `jupyterlab_github-4.0.0.tar`

### file list

```diff
@@ -1,53 +1,46 @@
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.638158 jupyterlab_github-3.0.1/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     1514 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/LICENSE
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      470 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/MANIFEST.in
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     8456 2021-11-27 16:59:05.638158 jupyterlab_github-3.0.1/PKG-INFO
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     7417 2021-11-27 16:58:08.000000 jupyterlab_github-3.0.1/README.md
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      195 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/install.json
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyter-config/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       92 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/jupyter-config/jupyterlab_github.json
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyterlab_github/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     5390 2021-11-27 16:58:08.000000 jupyterlab_github-3.0.1/jupyterlab_github/__init__.py
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      441 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/jupyterlab_github/_version.py
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyterlab_github/labextension/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     3754 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/package.json
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.630158 jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.630158 jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/@jupyterlab/
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/@jupyterlab/github/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      679 2021-11-27 16:59:04.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/@jupyterlab/github/drive.json
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     3612 2021-11-27 16:59:04.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/@jupyterlab/github/package.json.orig
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    35407 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/060d51417beb0f47daa10a4dcb2e147d.png
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    11786 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/534.06ec9cb816bf9170af66.js
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     1493 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/742.c0343f89d61252c41791.js
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    13743 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/784.7af3b56872a0f8721f0b.js
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     7783 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/remoteEntry.e0263a028853908ae4bb.js
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      161 2021-11-27 16:59:04.000000 jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/style.js
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     8456 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/PKG-INFO
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     1255 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/SOURCES.txt
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)        1 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/dependency_links.txt
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)        1 2021-11-27 15:23:39.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/not-zip-safe
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       16 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/requires.txt
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       18 2021-11-27 16:59:05.000000 jupyterlab_github-3.0.1/jupyterlab_github.egg-info/top_level.txt
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     3612 2021-11-27 16:58:08.000000 jupyterlab_github-3.0.1/package.json
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      145 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/pyproject.toml
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       73 2021-11-27 16:59:05.638158 jupyterlab_github-3.0.1/setup.cfg
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     2711 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/setup.py
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    21980 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/setupbase.py
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/src/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    12232 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/src/browser.ts
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    22907 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/src/contents.ts
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     5273 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/src/github.ts
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     4288 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/src/index.ts
-drwxrwxr-x   0 krassowski  (1000) krassowski  (1000)        0 2021-11-27 16:59:05.634158 jupyterlab_github-3.0.1/style/
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     2741 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/base.css
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     2396 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/binder.svg
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       25 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/index.css
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)       21 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/index.js
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     2142 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/octocat-dark.svg
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      940 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/octocat-light.svg
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)    35407 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/style/octocat_error.png
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)      554 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/tsconfig.json
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)     2969 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/tslint.json
--rw-rw-r--   0 krassowski  (1000) krassowski  (1000)   230182 2021-10-22 22:38:52.000000 jupyterlab_github-3.0.1/yarn.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.eslintignore
+-rw-r--r--   0        0        0    13361 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.prettierrc
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.stylelintrc
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.travis.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0    24242 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0   474836 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/gitception.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/install.json
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/tsconfig.json
+-rw-r--r--   0        0        0   210563 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/yarn.lock
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyter-config/jupyter_notebook_config.d/jupyterlab_github.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyter-config/jupyter_server_config.d/jupyterlab_github.json
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/_version.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/api/api.yaml
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/package.json
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/schemas/@jupyterlab/github/drive.json
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/schemas/@jupyterlab/github/package.json.orig
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/742.36b89fd7ee003ea0f9f1.js
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/747.600d6a58e8387735fc09.js
+-rw-r--r--   0        0        0    14766 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/958.22edf3675e77b075de5c.js
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/remoteEntry.3bfd9366a4d281640860.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/style.js
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/schema/drive.json
+-rw-r--r--   0        0        0    12262 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/src/browser.ts
+-rw-r--r--   0        0        0    22925 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/src/contents.ts
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/src/github.ts
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/src/svg.d.ts
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/base.css
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/binder.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/index.js
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/octocat-dark.svg
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/octocat-light.svg
+-rw-r--r--   0        0        0    35407 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/style/octocat_error.png
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/LICENSE
+-rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/README.md
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 jupyterlab_github-4.0.0/PKG-INFO
```

### Comparing `jupyterlab_github-3.0.1/LICENSE` & `jupyterlab_github-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/PKG-INFO` & `jupyterlab_github-4.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,24 @@
-Metadata-Version: 2.1
-Name: jupyterlab_github
-Version: 3.0.1
-Summary: JupyterLab viewer for GitHub repositories
-Home-page: https://github.com/jupyterlab/jupyterlab-github
-Author: Ian Rose
-Author-email: jupyter@googlegroups.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JupyterLab GitHub
 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab/jupyterlab-github/main?urlpath=lab)
+
 A JupyterLab extension for accessing GitHub repositories.
 
 ### What this extension is
 
 When you install this extension, an additional filebrowser tab will be added
 to the left area of JupyterLab. This filebrowser allows you to select GitHub
 organizations and users, browse their repositories, and open the files in those
 repositories. If those files are notebooks, you can run them just as you would
 any other notebook. You can also attach a kernel to text files and run those.
 Basically, you should be able to open any file in a repository that JupyterLab can handle.
 
 Here is a screenshot of the plugin opening this very file on GitHub:
-![gitception](https://raw.githubusercontent.com/jupyterlab/jupyterlab-github/master/gitception.png 'Gitception')
+![gitception](https://raw.githubusercontent.com/jupyterlab/jupyterlab-github/main/gitception.png 'Gitception')
 
 ### What this extension is not
 
 This is not an extension that provides full GitHub access, such as
 saving files, making commits, forking repositories, etc.
 For it to be so, it would need to more-or-less reinvent the GitHub website,
 which represents a huge increase in complexity for the extension.
@@ -61,38 +35,48 @@
 
 For that reason, we recommend that you take the time and effort to set up the server
 extension as well as the lab extension, which will allow you to access higher rate-limits.
 This process is described in the [installation](#Installation) section.
 
 ## Prerequisites
 
-- JupyterLab 3.0
+- JupyterLab > 3.0
 - A GitHub account for the server extension
 
 ## Installation
 
 As discussed above, this extension has both a server extension and a lab extension.
 Both extensions will be installed by default when installing from PyPI, but you may
-have only lab extension installed if you used the Extension Manager in JupyterLab 3.x.
+have only lab extension installed if you used the Extension Manager in JupyterLab.
 
 We recommend completing the steps described below as to not be rate-limited.
 The purpose of the server extension is to add GitHub credentials that you will need to acquire
 from https://github.com/settings/developers, and then to proxy your request to GitHub.
 
 For JupyterLab version older than 3 please see the instructions on the
 [2.x branch](https://github.com/jupyterlab/jupyterlab-github/tree/2.x).
 
 ### 1. Installing both server and prebuilt lab extension
 
+#### JupyterLab 4.x
+
 To install the both the server extension and (prebuilt) lab extension, enter the following in your terminal:
 
 ```bash
 pip install jupyterlab-github
 ```
 
+#### JupyterLab 3.x
+
+We need to pin the extension version to `3.0.1` for making it work on the JupyterLab 3.x.
+
+```bash
+pip install 'jupyterlab-github==3.0.1'
+```
+
 After restarting JupyterLab, the extension should work, and you can experience
 the joys of being rate-limited first-hand!
 
 ### 2. Getting your credentials from GitHub
 
 There are two approaches to getting credentials from GitHub:
 (1) you can get an access token, (2) you can register an OAuth app.
@@ -133,28 +117,28 @@
 
 It is important to note that the "Client Secret" string is, as the name suggests, a secret.
 _Do not_ share this value online, as people may be able to use it to impersonate you on GitHub.
 
 ### 3. Enabling and configuring the server extension
 
 The server extension will be enabled by default on new JupyterLab installations
-if you installed it with pip. If you used Extension Manager in JupyterLab 3.x,
+if you installed it with pip. If you used Extension Manager in JupyterLab,
 please uninstall the extension and install it again with the instructions from point (1).
 
 Confirm that the server extension is installed and enabled with:
 
 ```bash
 jupyter server extension list
 ```
 
 you should see the following:
 
 ```
 - Validating jupyterlab_github...
-     jupyterlab_github 3.0.0 OK
+     jupyterlab_github 4.0.0 OK
 ```
 
 On some older installations (e.g. old JupyterHub versions) which use jupyter
 `notebook` server instead of the new `jupyter-server`, the extension needs to
 show up on the legacy `serverextensions` list (note: no space between _server_ and _extension_):
 
 ```bash
@@ -204,9 +188,7 @@
 {
   "defaultRepo": "owner/repository"
 }
 ```
 
 where `owner` is the GitHub user/org,
 and `repository` is the name of the repository you want to open.
-
-
```

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/__init__.py` & `jupyterlab_github-4.0.0/jupyterlab_github/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 import re, json, copy
 
-import tornado.gen as gen
+from tornado import web
 from tornado.httputil import url_concat
 from tornado.httpclient import AsyncHTTPClient, HTTPRequest, HTTPError
 
 from traitlets import Unicode, Bool
 from traitlets.config import Configurable
 
-from notebook.utils import url_path_join, url_escape
-from notebook.base.handlers import APIHandler
+from jupyter_server.utils import url_path_join, url_escape
+from jupyter_server.base.handlers import APIHandler
 
 from ._version import __version__
 
 
 link_regex = re.compile(r'<([^>]*)>;\s*rel="([\w]*)\"')
 
 
 class GitHubConfig(Configurable):
     """
     Allows configuration of access to the GitHub api
     """
     allow_client_side_access_token = Bool(
-        False, config=True,
+        False,
         help=(
             "If True the access token specified in the JupyterLab settings "
             "will take precedence. If False the token specified in JupyterLab "
             "will be ignored. Storing your access token in the client can "
             "present a security risk so be careful if enabling this setting."
         )
-    )
+    ).tag(config=True)
+
     api_url = Unicode(
-        'https://api.github.com', config=True,
+        'https://api.github.com',
         help="The url for the GitHub api"
-    )
+    ).tag(config=True)
+
     access_token = Unicode(
-        '', config=True,
+        '',
         help="A personal access token for GitHub."
-    )
+    ).tag(config=True)
+
     validate_cert = Bool(
-        True, config=True,
+        True,
         help=(
             "Whether to validate the servers' SSL certificate on requests "
             "made to the GitHub api. In general this is a bad idea so only "
             "disable SSL validation if you know what you are doing!"
         )
-    )
+    ).tag(config=True)
 
 
 class GitHubHandler(APIHandler):
     """
     A proxy for the GitHub API v3.
 
     The purpose of this proxy is to provide authentication to the API requests
     which allows for a higher rate limit. Without this, the rate limit on
     unauthenticated calls is so limited as to be practically useless.
     """
-    @gen.coroutine
-    def get(self, path):
+
+    client = AsyncHTTPClient()
+
+    @web.authenticated
+    async def get(self, path):
         """
         Proxy API requests to GitHub, adding authentication parameter(s) if
         they have been set.
         """
 
         # Get access to the notebook config object
         c = GitHubConfig(config=self.config)
@@ -81,34 +87,36 @@
                     "your notebook configuration file:\n"
                     "c.GitHubConfig.access_token = '<TOKEN>'\n"
                 )
                 raise HTTPError(403, msg)
             elif c.access_token != '':
                 # Preferentially use the config access_token if set
                 token = c.access_token
+            else:
+                token = ''
 
             api_path = url_concat(api_path, params)
-            client = AsyncHTTPClient()
+            
             request = HTTPRequest(
                 api_path,
                 validate_cert=c.validate_cert,
                 user_agent='JupyterLab GitHub',
                 headers={"Authorization": "token {}".format(token)}
             )
-            response = yield client.fetch(request)
+            response = await self.client.fetch(request)
             data = json.loads(response.body.decode('utf-8'))
 
             # Check if we need to paginate results.
             # If so, get pages until all the results
             # are loaded into the data buffer.
             next_page_path = self._maybe_get_next_page_path(response)
             while next_page_path:
                 request = copy.copy(request)
                 request.url = next_page_path
-                response = yield client.fetch(request)
+                response = await self.client.fetch(request)
                 next_page_path = self._maybe_get_next_page_path(response)
                 data.extend(json.loads(response.body.decode('utf-8')))
 
             # Send the results back.
             self.finish(json.dumps(data))
 
         except HTTPError as err:
@@ -126,19 +134,30 @@
             matched = link_regex.findall(link_headers[0])
             for match in matched:
                 links[match[1]] = match[0]
             next_page_path = links.get('next', None)
 
         return next_page_path
 
+    
+def _jupyter_labextension_paths():
+    return [
+        {
+            "src": "labextension",
+            "dest": "@jupyterlab/github",
+        }
+    ]
+
+
 def _jupyter_server_extension_paths():
     return [{
         'module': 'jupyterlab_github'
     }]
 
+
 def load_jupyter_server_extension(nb_server_app):
     """
     Called when the extension is loaded.
 
     Args:
         nb_server_app (NotebookWebApplication): handle to the Notebook webserver instance.
     """
```

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/labextension/schemas/@jupyterlab/github/drive.json` & `jupyterlab_github-4.0.0/jupyterlab_github/labextension/schemas/@jupyterlab/github/drive.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/060d51417beb0f47daa10a4dcb2e147d.png` & `jupyterlab_github-4.0.0/style/octocat_error.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/742.c0343f89d61252c41791.js` & `jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/742.36b89fd7ee003ea0f9f1.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,41 @@
+"use strict";
 (self.webpackChunk_jupyterlab_github = self.webpackChunk_jupyterlab_github || []).push([
     [742], {
         742: (r, t) => {
-            "use strict";
             t.byteLength = function(r) {
-                var t = c(r),
+                var t = h(r),
                     e = t[0],
                     n = t[1];
                 return 3 * (e + n) / 4 - n
             }, t.toByteArray = function(r) {
-                var t, e, o = c(r),
-                    h = o[0],
-                    u = o[1],
+                var t, e, o = h(r),
+                    u = o[0],
+                    c = o[1],
                     i = new a(function(r, t, e) {
                         return 3 * (t + e) / 4 - e
-                    }(0, h, u)),
+                    }(0, u, c)),
                     f = 0,
-                    A = u > 0 ? h - 4 : h;
+                    A = c > 0 ? u - 4 : u;
                 for (e = 0; e < A; e += 4) t = n[r.charCodeAt(e)] << 18 | n[r.charCodeAt(e + 1)] << 12 | n[r.charCodeAt(e + 2)] << 6 | n[r.charCodeAt(e + 3)], i[f++] = t >> 16 & 255, i[f++] = t >> 8 & 255, i[f++] = 255 & t;
-                return 2 === u && (t = n[r.charCodeAt(e)] << 2 | n[r.charCodeAt(e + 1)] >> 4, i[f++] = 255 & t), 1 === u && (t = n[r.charCodeAt(e)] << 10 | n[r.charCodeAt(e + 1)] << 4 | n[r.charCodeAt(e + 2)] >> 2, i[f++] = t >> 8 & 255, i[f++] = 255 & t), i
+                return 2 === c && (t = n[r.charCodeAt(e)] << 2 | n[r.charCodeAt(e + 1)] >> 4, i[f++] = 255 & t), 1 === c && (t = n[r.charCodeAt(e)] << 10 | n[r.charCodeAt(e + 1)] << 4 | n[r.charCodeAt(e + 2)] >> 2, i[f++] = t >> 8 & 255, i[f++] = 255 & t), i
             }, t.fromByteArray = function(r) {
-                for (var t, n = r.length, a = n % 3, o = [], h = 16383, u = 0, c = n - a; u < c; u += h) o.push(i(r, u, u + h > c ? c : u + h));
+                for (var t, n = r.length, a = n % 3, o = [], u = 16383, h = 0, i = n - a; h < i; h += u) o.push(c(r, h, h + u > i ? i : h + u));
                 return 1 === a ? (t = r[n - 1], o.push(e[t >> 2] + e[t << 4 & 63] + "==")) : 2 === a && (t = (r[n - 2] << 8) + r[n - 1], o.push(e[t >> 10] + e[t >> 4 & 63] + e[t << 2 & 63] + "=")), o.join("")
             };
-            for (var e = [], n = [], a = "undefined" != typeof Uint8Array ? Uint8Array : Array, o = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", h = 0, u = o.length; h < u; ++h) e[h] = o[h], n[o.charCodeAt(h)] = h;
+            for (var e = [], n = [], a = "undefined" != typeof Uint8Array ? Uint8Array : Array, o = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", u = 0; u < 64; ++u) e[u] = o[u], n[o.charCodeAt(u)] = u;
 
-            function c(r) {
+            function h(r) {
                 var t = r.length;
                 if (t % 4 > 0) throw new Error("Invalid string. Length must be a multiple of 4");
                 var e = r.indexOf("=");
                 return -1 === e && (e = t), [e, e === t ? 0 : 4 - e % 4]
             }
 
-            function i(r, t, n) {
-                for (var a, o, h = [], u = t; u < n; u += 3) a = (r[u] << 16 & 16711680) + (r[u + 1] << 8 & 65280) + (255 & r[u + 2]), h.push(e[(o = a) >> 18 & 63] + e[o >> 12 & 63] + e[o >> 6 & 63] + e[63 & o]);
-                return h.join("")
+            function c(r, t, n) {
+                for (var a, o, u = [], h = t; h < n; h += 3) a = (r[h] << 16 & 16711680) + (r[h + 1] << 8 & 65280) + (255 & r[h + 2]), u.push(e[(o = a) >> 18 & 63] + e[o >> 12 & 63] + e[o >> 6 & 63] + e[63 & o]);
+                return u.join("")
             }
             n["-".charCodeAt(0)] = 62, n["_".charCodeAt(0)] = 63
         }
     }
 ]);
```

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/784.7af3b56872a0f8721f0b.js` & `jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/958.22edf3675e77b075de5c.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,40 @@
+"use strict";
 (self.webpackChunk_jupyterlab_github = self.webpackChunk_jupyterlab_github || []).push([
-    [784], {
-        784: (e, t, s) => {
-            "use strict";
+    [958], {
+        958: (e, t, s) => {
             s.r(t), s.d(t, {
-                default: () => R
+                default: () => x,
+                gitHubIcon: () => R
             });
-            var r = s(458),
-                i = s(825),
-                n = s(790),
-                o = s(579),
-                a = s(260),
-                h = s(168),
-                l = s(387),
-                d = s(473),
-                u = s(584);
+            var r = s(4),
+                i = s(172),
+                n = s(580),
+                o = s(237),
+                a = s(154),
+                h = s(663),
+                c = s(901),
+                l = s(987),
+                d = s(1),
+                u = s(790);
 
-            function c(e, t) {
+            function p(e, t) {
                 return u.ServerConnection.makeRequest(e, {}, t).then((e => 200 !== e.status ? e.json().then((t => {
                     throw new u.ServerConnection.ResponseError(e, t.message)
                 })) : e.json()))
             }
-            var p = s(959);
-            const m = "https://github.com";
-            class b {
+            var m = s(282);
+            const b = "https://github.com";
+            class _ {
                 constructor(e) {
-                    this._baseUrl = "github", this._validUser = !1, this._isDisposed = !1, this._fileChanged = new h.Signal(this), this._serverSettings = u.ServerConnection.makeSettings(), this._fileTypeForPath = t => {
+                    this._baseUrl = "github", this._validUser = !1, this._isDisposed = !1, this._fileChanged = new c.Signal(this), this._serverSettings = u.ServerConnection.makeSettings(), this._fileTypeForPath = t => {
                         const s = e.getFileTypesForPath(t);
                         return 0 === s.length ? e.getFileType("text") : s[0]
-                    }, this.baseUrl = m, this._useProxy = new Promise((e => {
-                        c(l.URLExt.join(this._serverSettings.baseUrl, "github"), this._serverSettings).then((() => {
+                    }, this.baseUrl = b, this._useProxy = new Promise((e => {
+                        p(l.URLExt.join(this._serverSettings.baseUrl, "github"), this._serverSettings).then((() => {
                             e(!0)
                         })).catch((() => {
                             console.warn("The JupyterLab GitHub server extension appears to be missing. If you do not install it with application credentials, you are likely to be rate limited by GitHub very quickly"), e(!1)
                         }))
                     })), this.rateLimitedState = new d.ObservableValue(!1)
                 }
                 get name() {
@@ -47,45 +49,45 @@
                 get fileChanged() {
                     return this._fileChanged
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, h.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, c.Signal.clearData(this))
                 }
                 get baseUrl() {
                     return this._baseUrl
                 }
                 set baseUrl(e) {
                     this._baseUrl = e
                 }
                 get accessToken() {
                     return this._accessToken
                 }
                 set accessToken(e) {
                     this._accessToken = e
                 }
                 get(e, t) {
-                    const s = _(e);
-                    if ("" === s.user) return this._validUser = !1, Promise.resolve(g.dummyDirectory);
+                    const s = g(e);
+                    if ("" === s.user) return this._validUser = !1, Promise.resolve(y.dummyDirectory);
                     if (s.user && !s.repository) return this._listRepos(s.user);
                     const r = l.URLExt.encodeParts(l.URLExt.join("repos", s.user, s.repository, "contents", s.path));
-                    return this._apiRequest(r).then((t => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), g.gitHubContentsToJupyterContents(e, t, this._fileTypeForPath)))).catch((t => 404 === t.response.status ? (console.warn("GitHub: cannot find org/repo. Perhaps you misspelled something?"), this._validUser = !1, g.dummyDirectory) : 403 === t.response.status && -1 !== t.message.indexOf("rate limit") ? (!0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0), console.error(t.message), Promise.reject(t)) : 403 === t.response.status && -1 !== t.message.indexOf("blob") ? (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), this._getBlob(e)) : (console.error(t.message), Promise.reject(t))))
+                    return this._apiRequest(r).then((t => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), y.gitHubContentsToJupyterContents(e, t, this._fileTypeForPath)))).catch((t => 404 === t.response.status ? (console.warn("GitHub: cannot find org/repo. Perhaps you misspelled something?"), this._validUser = !1, y.dummyDirectory) : 403 === t.response.status && -1 !== t.message.indexOf("rate limit") ? (!0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0), console.error(t.message), Promise.reject(t)) : 403 === t.response.status && -1 !== t.message.indexOf("blob") ? (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), this._getBlob(e)) : (console.error(t.message), Promise.reject(t))))
                 }
                 getDownloadUrl(e) {
-                    const t = _(e);
+                    const t = g(e);
                     if (!t.user) return Promise.reject("GitHub: no active organization");
                     if (!t.path) return Promise.reject("GitHub: No file selected");
                     const s = l.PathExt.dirname(t.path),
                         r = l.URLExt.encodeParts(l.URLExt.join("repos", t.user, t.repository, "contents", s));
                     return this._apiRequest(r).then((e => {
-                        for (let s of e)
+                        for (const s of e)
                             if (s.path === t.path) return s.download_url;
-                        throw g.makeError(404, `Cannot find file at ${t.path}`)
+                        throw y.makeError(404, `Cannot find file at ${t.path}`)
                     }))
                 }
                 newUntitled(e = {}) {
                     return Promise.reject("Repository is read only")
                 }
                 delete(e) {
                     return Promise.reject("Repository is read only")
@@ -109,25 +111,25 @@
                     return Promise.reject("Repository is read only")
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.reject("Read only")
                 }
                 _getBlob(e) {
                     let t;
-                    const s = _(e),
+                    const s = g(e),
                         r = l.PathExt.dirname(s.path),
                         i = l.URLExt.encodeParts(l.URLExt.join("repos", s.user, s.repository, "contents", r));
                     return this._apiRequest(i).then((e => {
-                        for (let r of e)
+                        for (const r of e)
                             if (r.path === s.path) return t = r, r.sha;
                         throw Error("Cannot find sha for blob")
                     })).then((e => {
                         const t = l.URLExt.encodeParts(l.URLExt.join("repos", s.user, s.repository, "git", "blobs", e));
                         return this._apiRequest(t)
-                    })).then((s => (t.content = s.content, g.gitHubContentsToJupyterContents(e, t, this._fileTypeForPath))))
+                    })).then((s => (t.content = s.content, y.gitHubContentsToJupyterContents(e, t, this._fileTypeForPath))))
                 }
                 _listRepos(e) {
                     const t = l.URLExt.encodeParts(l.URLExt.join("orgs", e, "repos"));
                     return this._apiRequest(t).catch((t => {
                         if (404 === t.response.status) return this._apiRequest("user").then((t => {
                             let s;
                             return s = t.login === e ? "user/repos?type=owner" : l.URLExt.encodeParts(l.URLExt.join("users", e, "repos")), this._apiRequest(s)
@@ -135,43 +137,44 @@
                             if (401 === t.response.status) {
                                 const t = l.URLExt.encodeParts(l.URLExt.join("users", e, "repos"));
                                 return this._apiRequest(t)
                             }
                             throw t
                         }));
                         throw t
-                    })).then((e => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), g.reposToDirectory(e)))).catch((e => (403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? !0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0) : (console.error(e.message), console.warn("GitHub: cannot find user. Perhaps you misspelled something?"), this._validUser = !1), g.dummyDirectory)))
+                    })).then((e => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), y.reposToDirectory(e)))).catch((e => (403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? !0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0) : (console.error(e.message), console.warn("GitHub: cannot find user. Perhaps you misspelled something?"), this._validUser = !1), y.dummyDirectory)))
                 }
                 _apiRequest(e) {
                     return this._useProxy.then((t => {
-                        let s, r = e.split("?"),
-                            i = r[0],
-                            n = (r[1] || "").split("&"),
-                            o = {};
-                        for (const e of n)
+                        const s = e.split("?"),
+                            r = s[0],
+                            i = (s[1] || "").split("&"),
+                            n = {};
+                        for (const e of i)
                             if (e) {
-                                let [t, s] = e.split("=");
-                                o[t] = s
-                            } return !0 === t ? (s = l.URLExt.join(this._serverSettings.baseUrl, "github"), this.accessToken && (o.access_token = this.accessToken)) : s = "https://api.github.com", i && (s = l.URLExt.join(s, i)), s += "?" + Object.keys(o).map((e => `${e}=${o[e]}`)).join("&"), !0 === t ? c(s, this._serverSettings) : (a = s, window.fetch(a).then((e => 200 !== e.status ? e.json().then((t => {
+                                const [t, s] = e.split("=");
+                                n[t] = s
+                            } let o;
+                        return !0 === t ? (o = l.URLExt.join(this._serverSettings.baseUrl, "github"), this.accessToken && (n.access_token = this.accessToken)) : o = "https://api.github.com", r && (o = l.URLExt.join(o, r)), o += "?" + Object.keys(n).map((e => `${e}=${n[e]}`)).join("&"), !0 === t ? p(o, this._serverSettings) : (a = o, window.fetch(a).then((e => 200 !== e.status ? e.json().then((t => {
                             throw new u.ServerConnection.ResponseError(e, t.message)
                         })) : e.json())));
                         var a
                     }))
                 }
             }
 
-            function _(e) {
+            function g(e) {
                 const t = e.split("/");
                 return {
                     user: t.length > 0 ? t[0] : "",
                     repository: t.length > 1 ? t[1] : "",
                     path: t.length > 2 ? l.URLExt.join(...t.slice(2)) : ""
                 }
             }
-            var g;
+            var y;
             ! function(e) {
                 function t(e, t) {
                     const s = new Response(t, {
                         status: e,
                         statusText: t
                     });
                     return new u.ServerConnection.ResponseError(s, t)
@@ -260,79 +263,78 @@
                             mimetype: "",
                             content: null
                         })))
                     }
                 }, e.makeError = t;
                 const s = new TextDecoder("utf8");
                 e.b64DecodeUTF8 = function(e) {
-                    const t = p.toByteArray(e.replace(/\n/g, ""));
+                    const t = m.toByteArray(e.replace(/\n/g, ""));
                     return s.decode(t)
                 }
-            }(g || (g = {}));
-            var y = s(971),
-                w = s(850),
-                f = s(706);
-            const v = "jp-MyBinderButton-disabled";
-            class P extends f.Widget {
+            }(y || (y = {}));
+            var w = s(697),
+                v = s(778);
+            const f = "jp-MyBinderButton-disabled";
+            class P extends v.Widget {
                 constructor(e, t) {
-                    super(), this._errorPanel = null, this._binderActive = !1, this._changeGuard = !1, this.addClass("jp-GitHubBrowser"), this.layout = new f.PanelLayout, this.layout.addWidget(e), this._browser = e, this._drive = t, this.userName = new j, this.userName.node.title = "Click to edit user/organization", this._browser.toolbar.addItem("user", this.userName), this.userName.nameChanged.connect(this._onUserChanged, this), this._openGitHubButton = new i.ToolbarButton({
+                    super(), this._errorPanel = null, this._binderActive = !1, this._changeGuard = !1, this.addClass("jp-GitHubBrowser"), this.layout = new v.PanelLayout, this.layout.addWidget(e), this._browser = e, this._drive = t, this.userName = new C, this.userName.node.title = "Click to edit user/organization", this._browser.toolbar.addItem("user", this.userName), this.userName.nameChanged.connect(this._onUserChanged, this), this._openGitHubButton = new i.ToolbarButton({
                         onClick: () => {
                             let e = this._drive.baseUrl;
                             if (!this._drive.validUser) return void window.open(e);
-                            const t = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
+                            const t = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
                             e = l.URLExt.join(e, t.user), t.repository && (e = l.URLExt.join(e, t.repository, "tree", "master", t.path)), window.open(e)
                         },
                         iconClass: "jp-GitHub-icon jp-Icon jp-Icon-16",
                         tooltip: "Open this repository on GitHub"
                     }), this._openGitHubButton.addClass("jp-GitHub-toolbar-item"), this._browser.toolbar.addItem("GitHub", this._openGitHubButton), this._launchBinderButton = new i.ToolbarButton({
                         onClick: () => {
                             if (!this._binderActive) return;
-                            const e = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
+                            const e = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
                                 t = l.URLExt.join("https://mybinder.org/v2/gh", e.user, e.repository, "master"),
                                 s = l.URLExt.join("lab", "tree", e.path);
                             window.open(t + `?urlpath=${s}`)
                         },
                         tooltip: "Launch this repository on mybinder.org",
                         iconClass: "jp-MyBinderButton jp-Icon jp-Icon-16"
                     }), this._launchBinderButton.addClass("jp-GitHub-toolbar-item"), this._browser.toolbar.addItem("binder", this._launchBinderButton);
-                    let s = new i.ToolbarButton({
-                        icon: y.refreshIcon,
+                    const s = new i.ToolbarButton({
+                        icon: n.refreshIcon,
                         onClick: () => {
                             this._browser.model.refresh()
                         },
                         tooltip: "Refresh File List"
                     });
                     s.addClass("jp-GitHub-toolbar-item"), this._browser.toolbar.addItem("gh-refresher", s), this._browser.model.pathChanged.connect(this._onPathChanged, this), this._onPathChanged(), this._drive.rateLimitedState.changed.connect(this._updateErrorPanel, this)
                 }
                 _onUserChanged() {
                     this._changeGuard || (this._changeGuard = !0, this._browser.model.cd(`/${this.userName.name}`).then((() => {
-                        this._changeGuard = !1, this._updateErrorPanel(), document.activeElement === document.body && this._browser.layout.widgets[2].node.focus()
+                        this._changeGuard = !1, this._updateErrorPanel(), document.activeElement === document.body && this._browser.layout.widgets[1].node.focus()
                     })))
                 }
                 _onPathChanged() {
-                    const e = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
-                    return this._changeGuard || (this._changeGuard = !0, this.userName.name = e.user, this._changeGuard = !1, this._updateErrorPanel()), this._drive.validUser && e.repository ? "" === e.path ? (0, w.find)(this._browser.model.items(), (e => "requirements.txt" === e.name || "environment.yml" === e.name || "apt.txt" === e.name || "REQUIRE" === e.name || "Dockerfile" === e.name || "binder" === e.name && "directory" === e.type)) ? (this._launchBinderButton.removeClass(v), void(this._binderActive = !0)) : (this._launchBinderButton.addClass(v), void(this._binderActive = !1)) : void 0 : (this._launchBinderButton.addClass(v), void(this._binderActive = !1))
+                    const e = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
+                    return this._changeGuard || (this._changeGuard = !0, this.userName.name = e.user, this._changeGuard = !1, this._updateErrorPanel()), this._drive.validUser && e.repository ? "" === e.path ? (0, w.find)(this._browser.model.items(), (e => "requirements.txt" === e.name || "environment.yml" === e.name || "apt.txt" === e.name || "REQUIRE" === e.name || "Dockerfile" === e.name || "binder" === e.name && "directory" === e.type)) ? (this._launchBinderButton.removeClass(f), void(this._binderActive = !0)) : (this._launchBinderButton.addClass(f), void(this._binderActive = !1)) : void 0 : (this._launchBinderButton.addClass(f), void(this._binderActive = !1))
                 }
                 _updateErrorPanel() {
-                    const e = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
+                    const e = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
                         t = this._drive.rateLimitedState.get(),
                         s = this._drive.validUser;
-                    if (this._errorPanel && (this._browser.layout.widgets[2].node.removeChild(this._errorPanel.node), this._errorPanel.dispose(), this._errorPanel = null), t) this._errorPanel = new C("You have been rate limited by GitHub! You will need to wait about an hour before continuing"), this._browser.layout.widgets[2].node.appendChild(this._errorPanel.node);
+                    if (this._errorPanel && (this._browser.layout.widgets[1].node.removeChild(this._errorPanel.node), this._errorPanel.dispose(), this._errorPanel = null), t) this._errorPanel = new j("You have been rate limited by GitHub! You will need to wait about an hour before continuing"), this._browser.layout.widgets[1].node.appendChild(this._errorPanel.node);
                     else if (s);
                     else {
                         const t = e.user ? `"${e.user}" appears to be an invalid user name!` : "Please enter a GitHub user name";
-                        this._errorPanel = new C(t), this._browser.layout.widgets[2].node.appendChild(this._errorPanel.node)
+                        this._errorPanel = new j(t), this._browser.layout.widgets[1].node.appendChild(this._errorPanel.node)
                     }
                 }
             }
-            class j extends f.Widget {
+            class C extends v.Widget {
                 constructor() {
-                    super(), this._name = "", this._nameChanged = new h.Signal(this), this.addClass("jp-GitHubUserInput");
-                    const e = this.layout = new f.PanelLayout,
-                        t = new f.Widget;
+                    super(), this._name = "", this._nameChanged = new c.Signal(this), this.addClass("jp-GitHubUserInput");
+                    const e = this.layout = new v.PanelLayout,
+                        t = new v.Widget;
                     t.addClass("jp-GitHubUserInput-wrapper"), this._input = document.createElement("input"), this._input.placeholder = "GitHub User", this._input.className = "jp-GitHubUserInput-input", t.node.appendChild(this._input), e.addWidget(t)
                 }
                 get name() {
                     return this._name
                 }
                 set name(e) {
                     if (e === this._name) return;
@@ -344,18 +346,15 @@
                 }
                 get nameChanged() {
                     return this._nameChanged
                 }
                 handleEvent(e) {
                     switch (e.type) {
                         case "keydown":
-                            switch (e.keyCode) {
-                                case 13:
-                                    e.stopPropagation(), e.preventDefault(), this.name = this._input.value, this._input.blur()
-                            }
+                            13 === e.keyCode && (e.stopPropagation(), e.preventDefault(), this.name = this._input.value, this._input.blur());
                             break;
                         case "blur":
                             e.stopPropagation(), e.preventDefault(), this.name = this._input.value;
                             break;
                         case "focus":
                             e.stopPropagation(), e.preventDefault(), this._input.select()
                     }
@@ -363,69 +362,74 @@
                 onAfterAttach(e) {
                     this._input.addEventListener("keydown", this), this._input.addEventListener("blur", this), this._input.addEventListener("focus", this)
                 }
                 onBeforeDetach(e) {
                     this._input.removeEventListener("keydown", this), this._input.removeEventListener("blur", this), this._input.removeEventListener("focus", this)
                 }
             }
-            class C extends f.Widget {
+            class j extends v.Widget {
                 constructor(e) {
                     super(), this.addClass("jp-GitHubErrorPanel");
                     const t = document.createElement("div"),
                         s = document.createElement("div");
                     t.className = "jp-GitHubErrorImage", s.className = "jp-GitHubErrorText", s.textContent = e, this.node.appendChild(t), this.node.appendChild(s)
                 }
             }
             const E = "github-filebrowser",
                 U = "@jupyterlab/github:drive",
-                R = {
+                R = new n.LabIcon({
+                    name: `${E}:icon`,
+                    svgstr: '<svg width="16" height="16" xmlns="http://www.w3.org/2000/svg" xmlns:svg="http://www.w3.org/2000/svg">\n   <g>\n      <path id="path2" fill="#616161" fill-rule="evenodd" d="m8,0c-4.42,0 -8,3.58 -8,8c0,3.54 2.29,6.53 5.47,7.59c0.4,0.07 0.55,-0.17 0.55,-0.38c0,-0.19 -0.01,-0.82 -0.01,-1.49c-2.01,0.37 -2.53,-0.49 -2.69,-0.94c-0.09,-0.23 -0.48,-0.94 -0.82,-1.13c-0.28,-0.15 -0.68,-0.52 -0.01,-0.53c0.63,-0.01 1.08,0.58 1.23,0.82c0.72,1.21 1.87,0.87 2.33,0.66c0.07,-0.52 0.28,-0.87 0.51,-1.07c-1.78,-0.2 -3.64,-0.89 -3.64,-3.95c0,-0.87 0.31,-1.59 0.82,-2.15c-0.08,-0.2 -0.36,-1.02 0.08,-2.12c0,0 0.67,-0.21 2.2,0.82c0.64,-0.18 1.32,-0.27 2,-0.27c0.68,0 1.36,0.09 2,0.27c1.53,-1.04 2.2,-0.82 2.2,-0.82c0.44,1.1 0.16,1.92 0.08,2.12c0.51,0.56 0.82,1.27 0.82,2.15c0,3.07 -1.87,3.75 -3.65,3.95c0.29,0.25 0.54,0.73 0.54,1.48c0,1.07 -0.01,1.93 -0.01,2.2c0,0.21 0.15,0.46 0.55,0.38a8.013,8.013 0 0 0 5.45,-7.59c0,-4.42 -3.58,-8 -8,-8z" />\n   </g>\n</svg>'
+                }),
+                x = {
                     id: U,
-                    requires: [n.IDocumentManager, o.IFileBrowserFactory, r.ILayoutRestorer, a.ISettingRegistry],
+                    requires: [o.IDocumentManager, a.IFileBrowserFactory, h.ISettingRegistry],
+                    optional: [r.ILayoutRestorer],
                     activate: function(e, t, s, r, i) {
-                        const n = new b(e.docRegistry);
+                        const n = new _(e.docRegistry);
                         t.services.contents.addDrive(n);
                         const o = s.createFileBrowser(E, {
                                 driveName: n.name,
                                 refreshInterval: 3e5
                             }),
                             a = new P(o, n);
-                        a.title.iconClass = "jp-GitHub-icon jp-SideBar-tabIcon", a.title.caption = "Browse GitHub", a.id = "github-file-browser", r.add(a, E), e.shell.add(a, "left", {
+                        a.title.icon = R, a.title.iconClass = "jp-SideBar-tabIcon", a.title.caption = "Browse GitHub", a.id = "github-file-browser", i && i.add(a, E), e.shell.add(a, "left", {
                             rank: 102
                         });
                         let h = !1;
-                        const l = async e => {
+                        const c = async e => {
                             const t = e.get("baseUrl").composite,
                                 s = e.get("accessToken").composite;
-                            if (n.baseUrl = t || m, s) {
+                            if (n.baseUrl = t || b, s) {
                                 let t = !0;
-                                h && (t = await x.showWarning()), t ? n.accessToken = s : e.remove("accessToken")
+                                h && (t = await L.showWarning()), t ? n.accessToken = s : e.remove("accessToken")
                             } else n.accessToken = null
                         };
-                        Promise.all([i.load(U), e.restored]).then((([e]) => {
-                            e.changed.connect(l), l(e), h = !0;
+                        Promise.all([r.load(U), e.restored]).then((([e]) => {
+                            e.changed.connect(c), c(e), h = !0;
                             const t = e.get("defaultRepo").composite;
                             t && o.model.restored.then((() => {
                                 o.model.cd(`/${t}`)
                             }))
                         })).catch((e => {
                             console.error(e.message)
                         }))
                     },
                     autoStart: !0
                 };
-            var x;
+            var L;
             ! function(e) {
                 e.showWarning = async function() {
                     return (0, i.showDialog)({
                         title: "Security Alert!",
                         body: "Adding a client side access token can pose a security risk! Please consider using the server extension instead.Do you want to continue?",
                         buttons: [i.Dialog.cancelButton({
                             label: "CANCEL"
                         }), i.Dialog.warnButton({
                             label: "PROCEED"
                         })]
                     }).then((e => !!e.button.accept))
                 }
-            }(x || (x = {}))
+            }(L || (L = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github/labextension/static/remoteEntry.e0263a028853908ae4bb.js` & `jupyterlab_github-4.0.0/jupyterlab_github/labextension/static/remoteEntry.3bfd9366a4d281640860.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,115 +1,136 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, h, b, v, g, y, m, j, w, S = {},
-        E = {};
+    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, h, b, v, g, y, m, j, w, S, E = {
+            10: (e, r, t) => {
+                var n = {
+                        "./index": () => t.e(958).then((() => () => t(958))),
+                        "./extension": () => t.e(958).then((() => () => t(958))),
+                        "./style": () => t.e(747).then((() => () => t(747)))
+                    },
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                        throw new Error('Module "' + e + '" does not exist in container.')
+                    })), t.R = void 0, r),
+                    o = (e, r) => {
+                        if (t.S) {
+                            var n = "default",
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
+                        }
+                    };
+                t.d(r, {
+                    get: () => a,
+                    init: () => o
+                })
+            }
+        },
+        k = {};
 
-    function k(e) {
-        if (E[e]) return E[e].exports;
-        var r = E[e] = {
+    function P(e) {
+        var r = k[e];
+        if (void 0 !== r) return r.exports;
+        var t = k[e] = {
             id: e,
             exports: {}
         };
-        return S[e](r, r.exports, k), r.exports
+        return E[e](t, t.exports, P), t.exports
     }
-    k.m = S, k.n = e => {
+    P.m = E, P.c = k, P.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return k.d(r, {
+        return P.d(r, {
             a: r
         }), r
-    }, k.d = (e, r) => {
-        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
+    }, P.d = (e, r) => {
+        for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        534: "06ec9cb816bf9170af66",
-        742: "c0343f89d61252c41791",
-        784: "7af3b56872a0f8721f0b"
+    }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
+        742: "36b89fd7ee003ea0f9f1",
+        747: "600d6a58e8387735fc09",
+        958: "22edf3675e77b075de5c"
     } [e] + ".js?v=" + {
-        534: "06ec9cb816bf9170af66",
-        742: "c0343f89d61252c41791",
-        784: "7af3b56872a0f8721f0b"
-    } [e], k.g = function() {
+        742: "36b89fd7ee003ea0f9f1",
+        747: "600d6a58e8387735fc09",
+        958: "22edf3675e77b075de5c"
+    } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/github:", k.l = (t, n, a, o) => {
+    }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/github:", P.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, k.r = e => {
+    }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        k.S = {};
+        P.S = {};
         var e = {},
             r = {};
-        k.I = (t, n) => {
+        P.I = (t, n) => {
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
-                k.o(k.S, t) || (k.S[t] = {});
-                var o = k.S[t],
+                P.o(P.S, t) || (P.S[t] = {});
+                var o = P.S[t],
                     i = "@jupyterlab/github",
                     u = (e, r, t, n) => {
                         var a = o[e] = o[e] || {},
                             u = a[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                switch (t) {
-                    case "default":
-                        u("@jupyterlab/github", "3.0.1", (() => k.e(784).then((() => () => k(784))))), u("base64-js", "1.3.1", (() => k.e(742).then((() => () => k(742)))))
-                }
-                return e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupyterlab/github", "4.0.0", (() => P.e(958).then((() => () => P(958))))), u("base64-js", "1.5.1", (() => P.e(742).then((() => () => P(742)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        k.g.importScripts && (e = k.g.location + "");
-        var r = k.g.document;
+        P.g.importScripts && (e = P.g.location + "");
+        var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), P.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -175,126 +196,108 @@
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = k.S[e];
-        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = P.S[e];
+        if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + a(t) + ")", f = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(t, a, n)), h(e[t][a])
+        return o(n, a) || c(s(e, t, a, n)), b(e[t][a])
     }, d = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, p = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, c = (e, r, t, n) => {
-        "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), v = (b = e => function(r, t, n, a) {
-        var o = k.I(r);
-        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || c(r, e, t, n) || u(r, t))))), g = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = b(((e, r, t, n, a) => {
-        var o = r && k.o(r, t) && d(r, t, n);
-        return o ? h(o) : a()
-    })), m = {}, j = {
-        168: () => g("default", "@lumino/signaling", [1, 1, 4, 3]),
-        260: () => g("default", "@jupyterlab/settingregistry", [1, 3, 2, 4]),
-        387: () => g("default", "@jupyterlab/coreutils", [1, 5, 2, 4]),
-        458: () => g("default", "@jupyterlab/application", [1, 3, 2, 4]),
-        473: () => v("default", "@jupyterlab/observables", [1, 4, 2, 4]),
-        579: () => g("default", "@jupyterlab/filebrowser", [1, 3, 2, 4]),
-        584: () => g("default", "@jupyterlab/services", [1, 6, 2, 4]),
-        706: () => g("default", "@lumino/widgets", [1, 1, 19, 0]),
-        790: () => g("default", "@jupyterlab/docmanager", [1, 3, 2, 4]),
-        825: () => g("default", "@jupyterlab/apputils", [1, 3, 2, 4]),
-        850: () => g("default", "@lumino/algorithm", [1, 1, 3, 3]),
-        959: () => y("default", "base64-js", [1, 1, 3, 0], (() => k.e(742).then((() => () => k(742))))),
-        971: () => g("default", "@jupyterlab/ui-components", [1, 3, 2, 4])
-    }, w = {
-        784: [168, 260, 387, 458, 473, 579, 584, 706, 790, 825, 850, 959, 971]
-    }, k.f.consumes = (e, r) => {
-        k.o(w, e) && w[e].forEach((e => {
-            if (k.o(m, e)) return r.push(m[e]);
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, h = (e, r, t, n) => {
+        c(p(e, r, t, n))
+    }, b = e => (e.loaded = 1, e.get()), g = (v = e => function(r, t, n, a) {
+        var o = P.I(r);
+        return o && o.then ? o.then(e.bind(e, r, P.S[r], t, n, a)) : e(r, P.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), b(d(r, t, n) || h(r, e, t, n) || u(r, t))))), y = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = v(((e, r, t, n, a) => {
+        var o = r && P.o(r, t) && d(r, t, n);
+        return o ? b(o) : a()
+    })), j = {}, w = {
+        1: () => g("default", "@jupyterlab/observables", [1, 5, 0, 3]),
+        4: () => y("default", "@jupyterlab/application", [1, 4, 0, 3]),
+        154: () => y("default", "@jupyterlab/filebrowser", [1, 4, 0, 3]),
+        172: () => y("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
+        237: () => y("default", "@jupyterlab/docmanager", [1, 4, 0, 3]),
+        282: () => m("default", "base64-js", [1, 1, 5, 0], (() => P.e(742).then((() => () => P(742))))),
+        580: () => y("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
+        663: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
+        697: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
+        790: () => y("default", "@jupyterlab/services", [1, 7, 0, 3]),
+        901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
+        987: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 3])
+    }, S = {
+        958: [1, 4, 154, 172, 237, 282, 580, 663, 697, 778, 790, 901, 987]
+    }, P.f.consumes = (e, r) => {
+        P.o(S, e) && S[e].forEach((e => {
+            if (P.o(j, e)) return r.push(j[e]);
             var t = r => {
-                    m[e] = 0, S[e] = t => {
-                        delete E[e], t.exports = r()
+                    j[e] = 0, P.m[e] = t => {
+                        delete P.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete m[e], S[e] = t => {
-                        throw delete E[e], r
+                    delete j[e], P.m[e] = t => {
+                        throw delete P.c[e], r
                     }
                 };
             try {
-                var a = j[e]();
-                a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                var a = w[e]();
+                a.then ? r.push(j[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             879: 0
         };
-        k.f.j = (r, t) => {
-            var n = k.o(e, r) ? e[r] : void 0;
+        P.f.j = (r, t) => {
+            var n = P.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => {
-                        n = e[r] = [t, a]
-                    }));
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
                     t.push(n[2] = a);
-                    var o = k.p + k.u(r),
+                    var o = P.p + P.u(r),
                         i = new Error;
-                    k.l(o, (t => {
-                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    P.l(o, (t => {
+                        if (P.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                for (var n, a, [o, i, u] = t, l = 0, s = []; l < o.length; l++) a = o[l], k.o(e, a) && e[a] && s.push(e[a][0]), e[a] = 0;
-                for (n in i) k.o(i, n) && (k.m[n] = i[n]);
-                for (u && u(k), r && r(t); s.length;) s.shift()()
+                var n, a, [o, i, u] = t,
+                    l = 0;
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in i) P.o(i, n) && (P.m[n] = i[n]);
+                    u && u(P)
+                }
+                for (r && r(t); l < o.length; l++) a = o[l], P.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyterlab_github = self.webpackChunk_jupyterlab_github || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var P = {};
-    (() => {
-        var e = P,
-            r = {
-                "./index": () => k.e(784).then((() => () => k(784))),
-                "./extension": () => k.e(784).then((() => () => k(784))),
-                "./style": () => k.e(534).then((() => () => k(534)))
-            },
-            t = (e, t) => (k.R = t, t = k.o(r, e) ? r[e]() : Promise.resolve().then((() => {
-                throw new Error('Module "' + e + '" does not exist in container.')
-            })), k.R = void 0, t),
-            n = (e, r) => {
-                if (k.S) {
-                    var t = k.S.default,
-                        n = "default";
-                    if (t && t !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                    return k.S[n] = e, k.I(n, r)
-                }
-            };
-        k.d(e, {
-            get: () => t,
-            init: () => n
-        })
-    })(), (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/github"] = P
+    })(), P.nc = void 0;
+    var T = P(10);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/github"] = T
 })();
```

### Comparing `jupyterlab_github-3.0.1/jupyterlab_github.egg-info/PKG-INFO` & `jupyterlab_github-4.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,76 @@
 Metadata-Version: 2.1
-Name: jupyterlab-github
-Version: 3.0.1
+Name: jupyterlab_github
+Version: 4.0.0
 Summary: JupyterLab viewer for GitHub repositories
-Home-page: https://github.com/jupyterlab/jupyterlab-github
-Author: Ian Rose
-Author-email: jupyter@googlegroups.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
+Project-URL: Homepage, https://github.com/jupyterlab/jupyterlab-github
+Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyterlab-github/issues
+Project-URL: Repository, https://github.com/jupyterlab/jupyterlab-github.git
+Author-email: Ian Rose <jupyter@googlegroups.com>
+License: Copyright (c) 2017, Project Jupyter Contributors
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: jupyterlab<5,>=4.0.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # JupyterLab GitHub
 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab/jupyterlab-github/main?urlpath=lab)
+
 A JupyterLab extension for accessing GitHub repositories.
 
 ### What this extension is
 
 When you install this extension, an additional filebrowser tab will be added
 to the left area of JupyterLab. This filebrowser allows you to select GitHub
 organizations and users, browse their repositories, and open the files in those
 repositories. If those files are notebooks, you can run them just as you would
 any other notebook. You can also attach a kernel to text files and run those.
 Basically, you should be able to open any file in a repository that JupyterLab can handle.
 
 Here is a screenshot of the plugin opening this very file on GitHub:
-![gitception](https://raw.githubusercontent.com/jupyterlab/jupyterlab-github/master/gitception.png 'Gitception')
+![gitception](https://raw.githubusercontent.com/jupyterlab/jupyterlab-github/main/gitception.png 'Gitception')
 
 ### What this extension is not
 
 This is not an extension that provides full GitHub access, such as
 saving files, making commits, forking repositories, etc.
 For it to be so, it would need to more-or-less reinvent the GitHub website,
 which represents a huge increase in complexity for the extension.
@@ -61,38 +87,48 @@
 
 For that reason, we recommend that you take the time and effort to set up the server
 extension as well as the lab extension, which will allow you to access higher rate-limits.
 This process is described in the [installation](#Installation) section.
 
 ## Prerequisites
 
-- JupyterLab 3.0
+- JupyterLab > 3.0
 - A GitHub account for the server extension
 
 ## Installation
 
 As discussed above, this extension has both a server extension and a lab extension.
 Both extensions will be installed by default when installing from PyPI, but you may
-have only lab extension installed if you used the Extension Manager in JupyterLab 3.x.
+have only lab extension installed if you used the Extension Manager in JupyterLab.
 
 We recommend completing the steps described below as to not be rate-limited.
 The purpose of the server extension is to add GitHub credentials that you will need to acquire
 from https://github.com/settings/developers, and then to proxy your request to GitHub.
 
 For JupyterLab version older than 3 please see the instructions on the
 [2.x branch](https://github.com/jupyterlab/jupyterlab-github/tree/2.x).
 
 ### 1. Installing both server and prebuilt lab extension
 
+#### JupyterLab 4.x
+
 To install the both the server extension and (prebuilt) lab extension, enter the following in your terminal:
 
 ```bash
 pip install jupyterlab-github
 ```
 
+#### JupyterLab 3.x
+
+We need to pin the extension version to `3.0.1` for making it work on the JupyterLab 3.x.
+
+```bash
+pip install 'jupyterlab-github==3.0.1'
+```
+
 After restarting JupyterLab, the extension should work, and you can experience
 the joys of being rate-limited first-hand!
 
 ### 2. Getting your credentials from GitHub
 
 There are two approaches to getting credentials from GitHub:
 (1) you can get an access token, (2) you can register an OAuth app.
@@ -133,28 +169,28 @@
 
 It is important to note that the "Client Secret" string is, as the name suggests, a secret.
 _Do not_ share this value online, as people may be able to use it to impersonate you on GitHub.
 
 ### 3. Enabling and configuring the server extension
 
 The server extension will be enabled by default on new JupyterLab installations
-if you installed it with pip. If you used Extension Manager in JupyterLab 3.x,
+if you installed it with pip. If you used Extension Manager in JupyterLab,
 please uninstall the extension and install it again with the instructions from point (1).
 
 Confirm that the server extension is installed and enabled with:
 
 ```bash
 jupyter server extension list
 ```
 
 you should see the following:
 
 ```
 - Validating jupyterlab_github...
-     jupyterlab_github 3.0.0 OK
+     jupyterlab_github 4.0.0 OK
 ```
 
 On some older installations (e.g. old JupyterHub versions) which use jupyter
 `notebook` server instead of the new `jupyter-server`, the extension needs to
 show up on the legacy `serverextensions` list (note: no space between _server_ and _extension_):
 
 ```bash
@@ -204,9 +240,7 @@
 {
   "defaultRepo": "owner/repository"
 }
 ```
 
 where `owner` is the GitHub user/org,
 and `repository` is the name of the repository you want to open.
-
-
```

### Comparing `jupyterlab_github-3.0.1/src/browser.ts` & `jupyterlab_github-4.0.0/src/browser.ts`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,18 @@
       onClick: () => {
         let url = this._drive.baseUrl;
         // If there is no valid user, open the GitHub homepage.
         if (!this._drive.validUser) {
           window.open(url);
           return;
         }
-        const localPath = this._browser.model.manager.services.contents.localPath(
-          this._browser.model.path
-        );
+        const localPath =
+          this._browser.model.manager.services.contents.localPath(
+            this._browser.model.path
+          );
         const resource = parsePath(localPath);
         url = URLExt.join(url, resource.user);
         if (resource.repository) {
           url = URLExt.join(
             url,
             resource.repository,
             'tree',
@@ -81,17 +82,18 @@
     // Create a button the opens MyBinder to the appropriate repo.
     this._launchBinderButton = new ToolbarButton({
       onClick: () => {
         // If binder is not active for this directory, do nothing.
         if (!this._binderActive) {
           return;
         }
-        const localPath = this._browser.model.manager.services.contents.localPath(
-          this._browser.model.path
-        );
+        const localPath =
+          this._browser.model.manager.services.contents.localPath(
+            this._browser.model.path
+          );
         const resource = parsePath(localPath);
         const url = URLExt.join(
           MY_BINDER_BASE_URL,
           resource.user,
           resource.repository,
           'master'
         );
@@ -103,15 +105,15 @@
       iconClass: 'jp-MyBinderButton jp-Icon jp-Icon-16'
     });
     this._launchBinderButton.addClass('jp-GitHub-toolbar-item');
     this._browser.toolbar.addItem('binder', this._launchBinderButton);
 
     // Add our own refresh button, since the other one is hidden
     // via CSS.
-    let refresher = new ToolbarButton({
+    const refresher = new ToolbarButton({
       icon: refreshIcon,
       onClick: () => {
         this._browser.model.refresh();
       },
       tooltip: 'Refresh File List'
     });
     refresher.addClass('jp-GitHub-toolbar-item');
@@ -142,15 +144,15 @@
       this._changeGuard = false;
       this._updateErrorPanel();
       // Once we have the new listing, maybe give the file listing
       // focus. Once the input element is removed, the active element
       // appears to revert to document.body. If the user has subsequently
       // focused another element, don't focus the browser listing.
       if (document.activeElement === document.body) {
-        const listing = (this._browser.layout as PanelLayout).widgets[2];
+        const listing = (this._browser.layout as PanelLayout).widgets[1];
         listing.node.focus();
       }
     });
   }
 
   /**
    * React to the path changing for the browser.
@@ -221,39 +223,39 @@
     );
     const resource = parsePath(localPath);
     const rateLimited = this._drive.rateLimitedState.get();
     const validUser = this._drive.validUser;
 
     // If we currently have an error panel, remove it.
     if (this._errorPanel) {
-      const listing = (this._browser.layout as PanelLayout).widgets[2];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.removeChild(this._errorPanel.node);
       this._errorPanel.dispose();
       this._errorPanel = null;
     }
 
     // If we are being rate limited, make an error panel.
     if (rateLimited) {
       this._errorPanel = new GitHubErrorPanel(
         'You have been rate limited by GitHub! ' +
           'You will need to wait about an hour before ' +
           'continuing'
       );
-      const listing = (this._browser.layout as PanelLayout).widgets[2];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.appendChild(this._errorPanel.node);
       return;
     }
 
     // If we have an invalid user, make an error panel.
     if (!validUser) {
       const message = resource.user
         ? `"${resource.user}" appears to be an invalid user name!`
         : 'Please enter a GitHub user name';
       this._errorPanel = new GitHubErrorPanel(message);
-      const listing = (this._browser.layout as PanelLayout).widgets[2];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.appendChild(this._errorPanel.node);
       return;
     }
   }
 
   private _browser: FileBrowser;
   private _drive: GitHubDrive;
```

### Comparing `jupyterlab_github-3.0.1/src/contents.ts` & `jupyterlab_github-4.0.0/src/contents.ts`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         resource.repository,
         'contents',
         dirname
       )
     );
     return this._apiRequest<GitHubDirectoryListing>(dirApiPath).then(
       dirContents => {
-        for (let item of dirContents) {
+        for (const item of dirContents) {
           if (item.path === resource.path) {
             return item.download_url;
           }
         }
         throw Private.makeError(404, `Cannot find file at ${resource.path}`);
       }
     );
@@ -417,15 +417,15 @@
         resource.repository,
         'contents',
         dirname
       )
     );
     return this._apiRequest<GitHubDirectoryListing>(dirApiPath)
       .then(dirContents => {
-        for (let item of dirContents) {
+        for (const item of dirContents) {
           if (item.path === resource.path) {
             blobData = item as GitHubFileContents;
             return item.sha;
           }
         }
         throw Error('Cannot find sha for blob');
       })
@@ -524,21 +524,21 @@
 
   /**
    * Determine whether to make the call via the
    * notebook server proxy or not.
    */
   private _apiRequest<T>(apiPath: string): Promise<T> {
     return this._useProxy.then(result => {
-      let parts = apiPath.split('?');
-      let path = parts[0];
-      let query = (parts[1] || '').split('&');
-      let params: { [key: string]: string } = {};
+      const parts = apiPath.split('?');
+      const path = parts[0];
+      const query = (parts[1] || '').split('&');
+      const params: { [key: string]: string } = {};
       for (const param of query) {
         if (param) {
-          let [key, value] = param.split('=');
+          const [key, value] = param.split('=');
           params[key] = value;
         }
       }
       let requestUrl: string;
       if (result === true) {
         requestUrl = URLExt.join(this._serverSettings.baseUrl, 'github');
         // add the access token if defined
@@ -547,15 +547,15 @@
         }
       } else {
         requestUrl = DEFAULT_GITHUB_API_URL;
       }
       if (path) {
         requestUrl = URLExt.join(requestUrl, path);
       }
-      let newQuery = Object.keys(params)
+      const newQuery = Object.keys(params)
         .map(key => `${key}=${params[key]}`)
         .join('&');
       requestUrl += '?' + newQuery;
       if (result === true) {
         return proxiedApiRequest<T>(requestUrl, this._serverSettings);
       } else {
         return browserApiRequest<T>(requestUrl);
@@ -737,15 +737,15 @@
    *
    * @param repo - the GitHubRepo object.
    *
    * @returns a Contents.IModel object.
    */
   export function reposToDirectory(repos: GitHubRepo[]): Contents.IModel {
     // If it is a directory, convert to that.
-    let content: Contents.IModel[] = repos.map(repo => {
+    const content: Contents.IModel[] = repos.map(repo => {
       return {
         name: repo.name,
         path: repo.full_name,
         format: 'json',
         type: 'directory',
         created: '',
         writable: false,
```

### Comparing `jupyterlab_github-3.0.1/src/github.ts` & `jupyterlab_github-4.0.0/src/github.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/src/index.ts` & `jupyterlab_github-4.0.0/src/index.ts`

 * *Files 5% similar despite different names*

```diff
@@ -5,58 +5,66 @@
   ILayoutRestorer,
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 
+import { LabIcon } from '@jupyterlab/ui-components';
+
 import { IDocumentManager } from '@jupyterlab/docmanager';
 
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 
 import { GitHubDrive, DEFAULT_GITHUB_BASE_URL } from './contents';
 
 import { GitHubFileBrowser } from './browser';
 
+import GitHubSvgStr from '../style/octocat-light.svg';
+
 /**
  * GitHub filebrowser plugin state namespace.
  */
 const NAMESPACE = 'github-filebrowser';
 
 /**
  * The ID for the plugin.
  */
 const PLUGIN_ID = '@jupyterlab/github:drive';
 
 /**
+ * GitHub Icon class.
+ */
+export const gitHubIcon = new LabIcon({
+  name: `${NAMESPACE}:icon`,
+  svgstr: GitHubSvgStr
+});
+
+/**
  * The JupyterLab plugin for the GitHub Filebrowser.
  */
 const fileBrowserPlugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
-  requires: [
-    IDocumentManager,
-    IFileBrowserFactory,
-    ILayoutRestorer,
-    ISettingRegistry
-  ],
+  requires: [IDocumentManager, IFileBrowserFactory, ISettingRegistry],
+  optional: [ILayoutRestorer],
   activate: activateFileBrowser,
   autoStart: true
 };
 
 /**
  * Activate the file browser.
  */
 function activateFileBrowser(
   app: JupyterFrontEnd,
   manager: IDocumentManager,
   factory: IFileBrowserFactory,
-  restorer: ILayoutRestorer,
-  settingRegistry: ISettingRegistry
+  settingRegistry: ISettingRegistry,
+  restorer: ILayoutRestorer | null
 ): void {
   // Add the GitHub backend to the contents manager.
   const drive = new GitHubDrive(app.docRegistry);
   manager.services.contents.addDrive(drive);
 
   // Create the embedded filebrowser. GitHub repos likely
   // don't need as often of a refresh interval as normal ones,
@@ -65,21 +73,24 @@
   const browser = factory.createFileBrowser(NAMESPACE, {
     driveName: drive.name,
     refreshInterval: 300000
   });
 
   const gitHubBrowser = new GitHubFileBrowser(browser, drive);
 
-  gitHubBrowser.title.iconClass = 'jp-GitHub-icon jp-SideBar-tabIcon';
+  gitHubBrowser.title.icon = gitHubIcon;
+  gitHubBrowser.title.iconClass = 'jp-SideBar-tabIcon';
   gitHubBrowser.title.caption = 'Browse GitHub';
 
   gitHubBrowser.id = 'github-file-browser';
 
   // Add the file browser widget to the application restorer.
-  restorer.add(gitHubBrowser, NAMESPACE);
+  if (restorer) {
+    restorer.add(gitHubBrowser, NAMESPACE);
+  }
   app.shell.add(gitHubBrowser, 'left', { rank: 102 });
 
   let shouldWarn = false;
   const onSettingsUpdated = async (settings: ISettingRegistry.ISettings) => {
     const baseUrl = settings.get('baseUrl').composite as
       | string
       | null
```

### Comparing `jupyterlab_github-3.0.1/style/base.css` & `jupyterlab_github-4.0.0/style/base.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/*-----------------------------------------------------------------------------
+/* -----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
-|----------------------------------------------------------------------------*/
+|---------------------------------------------------------------------------- */
 
 [data-jp-theme-light='true'] .jp-GitHub-icon {
-  background-image: url(octocat-light.svg);
+  background-image: 'url(octocat-light.svg)';
 }
 
 [data-jp-theme-light='false'] .jp-GitHub-icon {
-  background-image: url(octocat-dark.svg);
+  background-image: 'url(octocat-dark.svg)';
 }
 
 .jp-GitHubBrowser {
   background-color: var(--jp-layout-color1);
   height: 100%;
 }
 
@@ -22,15 +22,15 @@
 }
 
 .jp-GitHubUserInput {
   overflow: hidden;
   white-space: nowrap;
   text-align: center;
   font-size: large;
-  padding: 0px;
+  padding: 0;
   background-color: var(--jp-layout-color1);
 }
 
 .jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item.jp-GitHubUserInput {
   flex: 8 8;
 }
 
@@ -94,26 +94,26 @@
   background: var(--jp-layout-color2);
 }
 
 .jp-GitHubErrorImage {
   background-size: 100%;
   width: 200px;
   height: 165px;
-  background-image: url(octocat_error.png);
+  background-image: 'url(octocat_error.png)';
 }
 
 .jp-GitHubErrorText {
   font-size: var(--jp-ui-font-size3);
   color: var(--jp-ui-font-color1);
   text-align: center;
   padding: 12px;
 }
 
 .jp-GitHubBrowser .jp-MyBinderButton {
-  background-image: url(binder.svg);
+  background-image: 'url(binder.svg)';
 }
 
 .jp-GitHubBrowser .jp-MyBinderButton-disabled {
   opacity: 0.3;
 }
 
 #setting-editor .jp-PluginList-icon.jp-GitHub-icon {
```

### Comparing `jupyterlab_github-3.0.1/style/binder.svg` & `jupyterlab_github-4.0.0/style/binder.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/style/octocat-dark.svg` & `jupyterlab_github-4.0.0/style/octocat-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/style/octocat-light.svg` & `jupyterlab_github-4.0.0/style/octocat-light.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_github-3.0.1/tsconfig.json` & `jupyterlab_github-4.0.0/tsconfig.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "es2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

