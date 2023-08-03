# Comparing `tmp/fastmessage-0.0.0.tar.gz` & `tmp/fastmessage-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmessage-0.0.0.tar", last modified: Thu Aug  3 18:38:26 2023, max compression
+gzip compressed data, was "fastmessage-0.0.1.tar", last modified: Thu Aug  3 20:01:16 2023, max compression
```

## Comparing `fastmessage-0.0.0.tar` & `fastmessage-0.0.1.tar`

### file list

```diff
@@ -1,64 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/
--rw-rw-rw-   0        0        0       77 2022-09-04 06:09:01.000000 fastmessage-0.0.0/.flake8
--rw-rw-rw-   0        0        0     1088 2023-08-03 18:25:23.000000 fastmessage-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      194 2022-10-12 06:38:55.000000 fastmessage-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2177 2023-08-03 18:38:26.753723 fastmessage-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-08-03 18:34:40.000000 fastmessage-0.0.0/README.md
--rw-rw-rw-   0        0        0        5 2023-08-03 18:33:44.000000 fastmessage-0.0.0/VERSION
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.715953 fastmessage-0.0.0/_custom_build/
--rw-rw-rw-   0        0        0        0 2022-10-12 06:21:11.000000 fastmessage-0.0.0/_custom_build/__init__.py
--rw-rw-rw-   0        0        0      264 2022-10-12 07:27:15.000000 fastmessage-0.0.0/_custom_build/backend.py
--rw-rw-rw-   0        0        0     1096 2022-10-12 07:18:57.000000 fastmessage-0.0.0/_custom_build/make_all_extra_requirements.py
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.722460 fastmessage-0.0.0/fastmessage/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:25:43.000000 fastmessage-0.0.0/fastmessage/__init__.py
--rw-rw-rw-   0        0        0        0 2022-09-04 06:22:36.000000 fastmessage-0.0.0/fastmessage/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/fastmessage.egg-info/
--rw-rw-rw-   0        0        0     2177 2023-08-03 18:38:26.000000 fastmessage-0.0.0/fastmessage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1159 2023-08-03 18:38:26.000000 fastmessage-0.0.0/fastmessage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 18:38:26.000000 fastmessage-0.0.0/fastmessage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-08-03 18:38:26.000000 fastmessage-0.0.0/fastmessage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 18:38:26.000000 fastmessage-0.0.0/fastmessage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      301 2023-04-11 06:11:08.000000 fastmessage-0.0.0/mypy.ini
--rw-rw-rw-   0        0        0     1342 2023-08-03 18:36:15.000000 fastmessage-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       34 2023-08-03 18:33:44.000000 fastmessage-0.0.0/pytest.ini
--rw-rw-rw-   0        0        0      125 2023-08-03 18:38:26.000000 fastmessage-0.0.0/requirements-all.txt
--rw-rw-rw-   0        0        0       49 2023-08-03 18:36:07.000000 fastmessage-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       44 2023-08-03 18:34:40.000000 fastmessage-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 18:38:26.753723 fastmessage-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.691418 fastmessage-0.0.0/venv/
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.691418 fastmessage-0.0.0/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.691418 fastmessage-0.0.0/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/build/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:14.000000 fastmessage-0.0.0/venv/Lib/site-packages/build/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/certifi/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:52.000000 fastmessage-0.0.0/venv/Lib/site-packages/certifi/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/charset_normalizer/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:52.000000 fastmessage-0.0.0/venv/Lib/site-packages/charset_normalizer/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/idna/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:50.000000 fastmessage-0.0.0/venv/Lib/site-packages/idna/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/importlib_metadata/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:53.000000 fastmessage-0.0.0/venv/Lib/site-packages/importlib_metadata/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/keyring/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:54.000000 fastmessage-0.0.0/venv/Lib/site-packages/keyring/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.738092 fastmessage-0.0.0/venv/Lib/site-packages/markdown_it/
--rw-rw-rw-   0        0        0       26 2023-08-03 18:37:52.000000 fastmessage-0.0.0/venv/Lib/site-packages/markdown_it/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/mdurl/
--rw-rw-rw-   0        0        0       26 2023-08-03 18:37:50.000000 fastmessage-0.0.0/venv/Lib/site-packages/mdurl/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/more_itertools/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:50.000000 fastmessage-0.0.0/venv/Lib/site-packages/more_itertools/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/packaging/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:13.000000 fastmessage-0.0.0/venv/Lib/site-packages/packaging/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      286 2023-08-03 18:37:29.000000 fastmessage-0.0.0/venv/Lib/site-packages/pip/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/pkginfo/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:50.000000 fastmessage-0.0.0/venv/Lib/site-packages/pkginfo/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/readme_renderer/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:54.000000 fastmessage-0.0.0/venv/Lib/site-packages/readme_renderer/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/rich/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:53.000000 fastmessage-0.0.0/venv/Lib/site-packages/rich/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/tomli/
--rw-rw-rw-   0        0        0       26 2023-08-03 18:37:13.000000 fastmessage-0.0.0/venv/Lib/site-packages/tomli/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/twine/
--rw-rw-rw-   0        0        0        0 2023-08-03 18:37:55.000000 fastmessage-0.0.0/venv/Lib/site-packages/twine/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:26.753723 fastmessage-0.0.0/venv/Lib/site-packages/urllib3/
--rw-rw-rw-   0        0        0       93 2023-08-03 18:37:46.000000 fastmessage-0.0.0/venv/Lib/site-packages/urllib3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:16.503681 fastmessage-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:01:03.000000 fastmessage-0.0.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 20:01:03.000000 fastmessage-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 20:01:03.000000 fastmessage-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 20:01:16.503681 fastmessage-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-03 20:01:03.000000 fastmessage-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 20:01:04.000000 fastmessage-0.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:16.499681 fastmessage-0.0.1/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:03.000000 fastmessage-0.0.1/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 20:01:03.000000 fastmessage-0.0.1/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 20:01:03.000000 fastmessage-0.0.1/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:16.503681 fastmessage-0.0.1/fastmessage/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-03 20:01:03.000000 fastmessage-0.0.1/fastmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-08-03 20:01:03.000000 fastmessage-0.0.1/fastmessage/fastmessage_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:03.000000 fastmessage-0.0.1/fastmessage/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:16.503681 fastmessage-0.0.1/fastmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 20:01:16.000000 fastmessage-0.0.1/fastmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 20:01:16.000000 fastmessage-0.0.1/fastmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:01:16.000000 fastmessage-0.0.1/fastmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 20:01:16.000000 fastmessage-0.0.1/fastmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 20:01:16.000000 fastmessage-0.0.1/fastmessage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 20:01:03.000000 fastmessage-0.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 20:01:03.000000 fastmessage-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 20:01:03.000000 fastmessage-0.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 20:01:16.000000 fastmessage-0.0.1/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 20:01:03.000000 fastmessage-0.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 20:01:03.000000 fastmessage-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:01:16.503681 fastmessage-0.0.1/setup.cfg
```

### Comparing `fastmessage-0.0.0/PKG-INFO` & `fastmessage-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: fastmessage
-Version: 0.0.0
-Author-email: Aviv Salem <avivsalem@gmail.com>
-Maintainer-email: Aviv Salem <avivsalem@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
-Project-URL: Documentation, https://fastmessage.readthedocs.io/
-Platform: win32
-Platform: linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
-# FastMessage
-
-[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
-[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
-[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
-[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
-[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
-[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
-[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
-
-FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
-
-You can find the full documentation [here](https://fastmessage.readthedocs.io/)
-
-## Requirements
-
-Python 3.7+
-
-## Installation
-
-```console
-$ pip install fastmessage
-```
+Metadata-Version: 2.1
+Name: fastmessage
+Version: 0.0.1
+Author-email: Aviv Salem <avivsalem@gmail.com>
+Maintainer-email: Aviv Salem <avivsalem@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
+Project-URL: Documentation, https://fastmessage.readthedocs.io/
+Platform: win32
+Platform: linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+# FastMessage
+
+[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
+[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
+[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
+[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
+[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
+[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
+
+FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
+
+You can find the full documentation [here](https://fastmessage.readthedocs.io/)
+
+## Requirements
+
+Python 3.7+
+
+## Installation
+
+```console
+$ pip install fastmessage
+```
```

### Comparing `fastmessage-0.0.0/README.md` & `fastmessage-0.0.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# FastMessage
-
-[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
-[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
-[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
-[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
-[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
-[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
-[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
-
-FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
-
-You can find the full documentation [here](https://fastmessage.readthedocs.io/)
-
-## Requirements
-
-Python 3.7+
-
-## Installation
-
-```console
-$ pip install fastmessage
-```
+# FastMessage
+
+[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
+[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
+[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
+[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
+[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
+[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
+
+FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
+
+You can find the full documentation [here](https://fastmessage.readthedocs.io/)
+
+## Requirements
+
+Python 3.7+
+
+## Installation
+
+```console
+$ pip install fastmessage
+```
```

### Comparing `fastmessage-0.0.0/_custom_build/make_all_extra_requirements.py` & `fastmessage-0.0.1/_custom_build/make_all_extra_requirements.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import os
-from pathlib import Path
-from typing import List, Set
-
-
-def load_requirements(path: Path, filename) -> List[str]:
-    return (path / filename).read_text().splitlines()
-
-
-def load_all_extra_requirements(path: Path) -> List[str]:
-    import re
-    extra_requirement_pattern = re.compile(r'^requirements[_\-](?P<name>.+?)\.txt$')
-    files = [f for f in path.iterdir() if f.is_file()]
-    all_requirements: Set[str] = set()
-
-    for file in files:
-        match = extra_requirement_pattern.match(file.name)
-        if match:
-            all_requirements.update((path / file.name).read_text().splitlines())
-
-    return sorted([line.strip() for line in all_requirements])
-
-
-def generate_all_requirements(path: Path, output_filename: str = "requirements-all.txt"):
-    all_extras = os.linesep.join(load_all_extra_requirements(path))
-    output_file = (path/output_filename)
-
-    print(f'---------------> Writing the requirements to {output_file}:')
-    print(all_extras)
-    output_file.write_text(all_extras)
-    print()
-    print('---------------> Done!!!')
+import os
+from pathlib import Path
+from typing import List, Set
+
+
+def load_requirements(path: Path, filename) -> List[str]:
+    return (path / filename).read_text().splitlines()
+
+
+def load_all_extra_requirements(path: Path) -> List[str]:
+    import re
+    extra_requirement_pattern = re.compile(r'^requirements[_\-](?P<name>.+?)\.txt$')
+    files = [f for f in path.iterdir() if f.is_file()]
+    all_requirements: Set[str] = set()
+
+    for file in files:
+        match = extra_requirement_pattern.match(file.name)
+        if match:
+            all_requirements.update((path / file.name).read_text().splitlines())
+
+    return sorted([line.strip() for line in all_requirements])
+
+
+def generate_all_requirements(path: Path, output_filename: str = "requirements-all.txt"):
+    all_extras = os.linesep.join(load_all_extra_requirements(path))
+    output_file = (path/output_filename)
+
+    print(f'---------------> Writing the requirements to {output_file}:')
+    print(all_extras)
+    output_file.write_text(all_extras)
+    print()
+    print('---------------> Done!!!')
```

### Comparing `fastmessage-0.0.0/fastmessage.egg-info/PKG-INFO` & `fastmessage-0.0.1/fastmessage.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: fastmessage
-Version: 0.0.0
-Author-email: Aviv Salem <avivsalem@gmail.com>
-Maintainer-email: Aviv Salem <avivsalem@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
-Project-URL: Documentation, https://fastmessage.readthedocs.io/
-Platform: win32
-Platform: linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
-# FastMessage
-
-[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
-[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
-[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
-[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
-[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
-[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
-[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
-
-FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
-
-You can find the full documentation [here](https://fastmessage.readthedocs.io/)
-
-## Requirements
-
-Python 3.7+
-
-## Installation
-
-```console
-$ pip install fastmessage
-```
+Metadata-Version: 2.1
+Name: fastmessage
+Version: 0.0.1
+Author-email: Aviv Salem <avivsalem@gmail.com>
+Maintainer-email: Aviv Salem <avivsalem@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
+Project-URL: Documentation, https://fastmessage.readthedocs.io/
+Platform: win32
+Platform: linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+# FastMessage
+
+[![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
+[![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
+[![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
+[![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
+[![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
+[![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
+
+FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
+
+You can find the full documentation [here](https://fastmessage.readthedocs.io/)
+
+## Requirements
+
+Python 3.7+
+
+## Installation
+
+```console
+$ pip install fastmessage
+```
```

### Comparing `fastmessage-0.0.0/pyproject.toml` & `fastmessage-0.0.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel"
-]
-build-backend = "backend"
-backend-path = ["_custom_build"]
-
-[project]
-name = "fastmessage"
-requires-python = '>=3.7,<3.12'
-readme = "README.md"
-license = { text = "MIT" }
-classifiers = [
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'License :: OSI Approved :: MIT License',
-]
-dynamic = [
-    "dependencies",
-    "version",
-    "optional-dependencies"
-]
-
-[project.urls]
-Homepage = "https://github.com/Avivsalem/FastMessage/"
-Documentation = "https://fastmessage.readthedocs.io/"
-
-[[project.authors]]
-name = "Aviv Salem"
-email = "avivsalem@gmail.com"
-
-[[project.maintainers]]
-name = "Aviv Salem"
-email = "avivsalem@gmail.com"
-
-[tool.setuptools]
-platforms = [
-    "win32",
-    "linux"
-]
-
-[tool.setuptools.packages.find]
-include = ['fastmessage', 'fastmessage.*']
-
-[tool.setuptools.dynamic]
-dependencies = { file = "requirements.txt" }
-version = { file = "VERSION" }
-
-
-[tool.setuptools.dynamic.optional-dependencies]
-dev = { file = "requirements-dev.txt" }
-all = { file = "requirements-all.txt" }
-
-
-
-
+[build-system]
+requires = [
+    "setuptools",
+    "wheel"
+]
+build-backend = "backend"
+backend-path = ["_custom_build"]
+
+[project]
+name = "fastmessage"
+requires-python = '>=3.7,<3.12'
+readme = "README.md"
+license = { text = "MIT" }
+classifiers = [
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'License :: OSI Approved :: MIT License',
+]
+dynamic = [
+    "dependencies",
+    "version",
+    "optional-dependencies"
+]
+
+[project.urls]
+Homepage = "https://github.com/Avivsalem/FastMessage/"
+Documentation = "https://fastmessage.readthedocs.io/"
+
+[[project.authors]]
+name = "Aviv Salem"
+email = "avivsalem@gmail.com"
+
+[[project.maintainers]]
+name = "Aviv Salem"
+email = "avivsalem@gmail.com"
+
+[tool.setuptools]
+platforms = [
+    "win32",
+    "linux"
+]
+
+[tool.setuptools.packages.find]
+include = ['fastmessage', 'fastmessage.*']
+
+[tool.setuptools.dynamic]
+dependencies = { file = "requirements.txt" }
+version = { file = "VERSION" }
+
+
+[tool.setuptools.dynamic.optional-dependencies]
+dev = { file = "requirements-dev.txt" }
+all = { file = "requirements-all.txt" }
+
+
+
+
```

