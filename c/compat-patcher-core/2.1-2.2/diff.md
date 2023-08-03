# Comparing `tmp/compat-patcher-core-2.1.tar.gz` & `tmp/compat-patcher-core-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\compat-patcher-core-2.1.tar", last modified: Wed Jun 15 20:40:55 2022, max compression
+gzip compressed data, was "compat-patcher-core-2.2.tar", last modified: Thu Aug  3 15:33:11 2023, max compression
```

## Comparing `compat-patcher-core-2.1.tar` & `compat-patcher-core-2.2.tar`

### file list

```diff
@@ -1,79 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.360431 compat-patcher-core-2.1/
--rw-rw-rw-   0        0        0       92 2016-11-29 21:54:32.000000 compat-patcher-core-2.1/AUTHORS
--rw-rw-rw-   0        0        0      621 2022-06-15 20:34:26.000000 compat-patcher-core-2.1/CHANGELOG
--rw-rw-rw-   0        0        0     1082 2015-03-17 13:13:45.000000 compat-patcher-core-2.1/LICENSE
--rw-rw-rw-   0        0        0      410 2019-06-22 19:51:01.000000 compat-patcher-core-2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4512 2022-06-15 20:40:55.360431 compat-patcher-core-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3030 2022-06-15 13:19:47.000000 compat-patcher-core-2.1/README.rst
--rw-rw-rw-   0        0        0        4 2022-06-15 20:32:09.000000 compat-patcher-core-2.1/VERSION
--rw-rw-rw-   0        0        0      437 2019-06-20 21:53:15.000000 compat-patcher-core-2.1/cookiecutter.json
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.270494 compat-patcher-core-2.1/docs/
--rw-rw-rw-   0        0        0     7895 2019-06-16 15:01:46.000000 compat-patcher-core-2.1/docs/Makefile
--rw-rw-rw-   0        0        0     1526 2019-06-22 20:18:26.000000 compat-patcher-core-2.1/docs/api.rst
--rw-rw-rw-   0        0        0    10206 2019-06-18 17:50:36.000000 compat-patcher-core-2.1/docs/conf.py
--rw-rw-rw-   0        0        0     2404 2019-06-22 18:02:31.000000 compat-patcher-core-2.1/docs/guidelines.rst
--rw-rw-rw-   0        0        0      605 2019-06-22 18:16:22.000000 compat-patcher-core-2.1/docs/index.rst
--rwxrwxrwx   0        0        0     7502 2019-06-16 15:01:46.000000 compat-patcher-core-2.1/docs/make.bat
--rw-rw-rw-   0        0        0     3823 2019-06-22 18:20:44.000000 compat-patcher-core-2.1/docs/startup.rst
--rw-rw-rw-   0        0        0      663 2022-06-15 14:27:42.000000 compat-patcher-core-2.1/pytest.ini
--rw-rw-rw-   0        0        0      390 2022-06-15 14:21:45.000000 compat-patcher-core-2.1/requirements.txt
--rw-rw-rw-   0        0        0      146 2022-06-15 20:40:55.363430 compat-patcher-core-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1924 2022-06-15 15:46:35.000000 compat-patcher-core-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.271491 compat-patcher-core-2.1/src/
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.283482 compat-patcher-core-2.1/src/compat_patcher_core/
--rw-rw-rw-   0        0        0     2259 2022-06-15 11:43:26.000000 compat-patcher-core-2.1/src/compat_patcher_core/__init__.py
--rw-rw-rw-   0        0        0      144 2020-11-04 15:31:13.000000 compat-patcher-core-2.1/src/compat_patcher_core/exceptions.py
--rw-rw-rw-   0        0        0     6472 2021-01-19 19:54:09.000000 compat-patcher-core-2.1/src/compat_patcher_core/import_proxifier.py
--rw-rw-rw-   0        0        0     3174 2020-11-04 15:31:13.000000 compat-patcher-core-2.1/src/compat_patcher_core/readme_generator.py
--rw-rw-rw-   0        0        0    14804 2020-11-04 15:31:13.000000 compat-patcher-core-2.1/src/compat_patcher_core/registry.py
--rw-rw-rw-   0        0        0     4510 2022-06-13 22:10:16.000000 compat-patcher-core-2.1/src/compat_patcher_core/runner.py
--rw-rw-rw-   0        0        0     3892 2022-06-15 11:59:37.000000 compat-patcher-core-2.1/src/compat_patcher_core/scaffolding.py
--rw-rw-rw-   0        0        0    10979 2022-06-15 11:45:15.000000 compat-patcher-core-2.1/src/compat_patcher_core/utilities.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.314462 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/
--rw-rw-rw-   0        0        0     4512 2022-06-15 20:40:55.000000 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2477 2022-06-15 20:40:55.000000 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-15 20:40:55.000000 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2022-06-15 20:40:55.000000 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-06-15 20:40:55.000000 compat-patcher-core-2.1/src/compat_patcher_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       94 2019-06-17 21:10:41.000000 compat-patcher-core-2.1/src/conftest.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.326480 compat-patcher-core-2.1/tests/
--rw-rw-rw-   0        0        0     4056 2019-06-18 18:33:45.000000 compat-patcher-core-2.1/tests/dummy_fixers.py
--rw-rw-rw-   0        0        0       81 2019-06-14 06:27:45.000000 compat-patcher-core-2.1/tests/dummy_module.py
--rw-rw-rw-   0        0        0     3296 2022-06-15 13:31:19.000000 compat-patcher-core-2.1/tests/test_cookiecutter_recipe.py
--rw-rw-rw-   0        0        0     3600 2021-01-19 21:03:59.000000 compat-patcher-core-2.1/tests/test_import_proxifier.py
--rw-rw-rw-   0        0        0    10903 2019-06-18 18:22:39.000000 compat-patcher-core-2.1/tests/test_patching_registry.py
--rw-rw-rw-   0        0        0     4891 2019-06-18 18:33:45.000000 compat-patcher-core-2.1/tests/test_patching_runner.py
--rw-rw-rw-   0        0        0     6080 2019-06-20 20:40:03.000000 compat-patcher-core-2.1/tests/test_patching_utilities.py
--rw-rw-rw-   0        0        0      804 2019-06-18 18:22:39.000000 compat-patcher-core-2.1/tests/test_readme_generator.py
--rw-rw-rw-   0        0        0     1880 2019-06-22 17:03:09.000000 compat-patcher-core-2.1/tests/test_scaffolding.py
--rw-rw-rw-   0        0        0      531 2022-06-15 16:19:13.000000 compat-patcher-core-2.1/tox.ini
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.347438 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/
--rw-rw-rw-   0        0        0     1172 2019-06-18 20:02:08.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/.gitignore
--rw-rw-rw-   0        0        0      144 2022-06-15 14:58:05.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/.travis.yml
--rw-rw-rw-   0        0        0      178 2018-10-14 04:01:22.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/AUTHORS.rst
--rw-rw-rw-   0        0        0      117 2018-10-14 04:01:22.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/CHANGELOG
--rw-rw-rw-   0        0        0     3450 2019-06-18 21:36:18.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1082 2019-06-18 20:09:05.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/LICENSE
--rw-rw-rw-   0        0        0      363 2019-06-20 21:47:31.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/MANIFEST.in
--rw-rw-rw-   0        0        0     1073 2019-06-18 20:56:58.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/README.in
--rw-rw-rw-   0        0        0       71 2019-06-21 21:13:34.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/README.rst
--rw-rw-rw-   0        0        0       27 2019-06-20 20:52:52.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/VERSION
--rw-rw-rw-   0        0        0      482 2019-06-20 20:51:36.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/generate_readme.py
--rw-rw-rw-   0        0        0      547 2019-06-18 20:09:47.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/pytest.ini
--rw-rw-rw-   0        0        0       78 2019-06-20 21:57:24.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/requirements-dev.txt
--rw-rw-rw-   0        0        0      118 2019-06-18 20:20:31.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/setup.cfg
--rw-rw-rw-   0        0        0     2001 2019-06-20 21:33:10.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.348437 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/
--rw-rw-rw-   0        0        0       94 2019-06-17 21:10:41.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/conftest.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.352436 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/
--rw-rw-rw-   0        0        0      662 2019-06-22 17:45:57.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/__init__.py
--rw-rw-rw-   0        0        0      425 2019-06-22 18:05:29.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/deprecation.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.354435 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/fixers/
--rw-rw-rw-   0        0        0      740 2019-06-18 21:45:30.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/fixers/__init__.py
--rw-rw-rw-   0        0        0      729 2019-06-18 21:47:29.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/src/{{cookiecutter.project_slug}}/registry.py
-drwxrwxrwx   0        0        0        0 2022-06-15 20:40:55.359431 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tests/
--rw-rw-rw-   0        0        0      150 2019-06-18 21:16:43.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tests/_test_utilities.py
--rw-rw-rw-   0        0        0      360 2019-06-20 20:28:04.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tests/conftest.py
--rw-rw-rw-   0        0        0      992 2019-06-22 17:07:36.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tests/test_scaffolding.py
--rw-rw-rw-   0        0        0      236 2019-06-18 21:23:58.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tests/test_software_fixers.py
--rw-rw-rw-   0        0        0      511 2019-06-22 17:10:55.000000 compat-patcher-core-2.1/{{cookiecutter.root_directory_name}}/tox.ini
+drwxrwxrwx   0        0        0        0 2023-08-03 15:33:11.961855 compat-patcher-core-2.2/
+-rw-rw-rw-   0        0        0       92 2016-11-29 21:54:32.000000 compat-patcher-core-2.2/AUTHORS
+-rw-rw-rw-   0        0        0     1082 2015-03-17 13:13:45.000000 compat-patcher-core-2.2/LICENSE
+-rw-rw-rw-   0        0        0     4170 2023-08-03 15:33:11.960855 compat-patcher-core-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3030 2022-06-15 13:19:47.000000 compat-patcher-core-2.2/README.rst
+-rw-rw-rw-   0        0        0     1437 2023-08-03 15:32:10.000000 compat-patcher-core-2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:33:11.961855 compat-patcher-core-2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 15:33:11.937671 compat-patcher-core-2.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 15:33:11.957855 compat-patcher-core-2.2/src/compat_patcher_core/
+-rw-rw-rw-   0        0        0     2259 2022-06-15 11:43:26.000000 compat-patcher-core-2.2/src/compat_patcher_core/__init__.py
+-rw-rw-rw-   0        0        0      144 2020-11-04 15:31:13.000000 compat-patcher-core-2.2/src/compat_patcher_core/exceptions.py
+-rw-rw-rw-   0        0        0     6472 2021-01-19 19:54:09.000000 compat-patcher-core-2.2/src/compat_patcher_core/import_proxifier.py
+-rw-rw-rw-   0        0        0     3174 2020-11-04 15:31:13.000000 compat-patcher-core-2.2/src/compat_patcher_core/readme_generator.py
+-rw-rw-rw-   0        0        0    14804 2020-11-04 15:31:13.000000 compat-patcher-core-2.2/src/compat_patcher_core/registry.py
+-rw-rw-rw-   0        0        0     4510 2022-06-13 22:10:16.000000 compat-patcher-core-2.2/src/compat_patcher_core/runner.py
+-rw-rw-rw-   0        0        0     3892 2022-06-15 11:59:37.000000 compat-patcher-core-2.2/src/compat_patcher_core/scaffolding.py
+-rw-rw-rw-   0        0        0    10979 2022-06-15 11:45:15.000000 compat-patcher-core-2.2/src/compat_patcher_core/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:33:11.960855 compat-patcher-core-2.2/src/compat_patcher_core.egg-info/
+-rw-rw-rw-   0        0        0     4170 2023-08-03 15:33:11.000000 compat-patcher-core-2.2/src/compat_patcher_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-08-03 15:33:11.000000 compat-patcher-core-2.2/src/compat_patcher_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:33:11.000000 compat-patcher-core-2.2/src/compat_patcher_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 15:33:11.000000 compat-patcher-core-2.2/src/compat_patcher_core.egg-info/top_level.txt
```

### Comparing `compat-patcher-core-2.1/LICENSE` & `compat-patcher-core-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/PKG-INFO` & `compat-patcher-core-2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: compat-patcher-core
-Version: 2.1
-Summary: A patcher system to allow easy and lasting API compatibility.
-Home-page: https://github.com/pakal/compat-patcher-core
-Author: Pascal Chambon & others
-Author-email: pythoniks@gmail.com
+Version: 2.2
+Summary: A patcher system to allow easy and lasting API compatibility
+Author-email: Pascal Chambon <pythoniks@gmail.com>
 License: MIT
-Description: .. image:: https://travis-ci.com/pakal/compat-patcher-core.svg?branch=master
-            :target: https://travis-ci.com/pakal/compat-patcher-core
-        
-        
-        *Long term API compatibility for fast-moving projects*
-        
-        
-        Welcome to **Compat Patcher Core**, a mini-framework to build **Compatibility Patchers**. These companion applications
-        allow your favorite software (a framework, a library...) to keep long term API stability towards its ecosystem
-        (plugins, bridges to other applications...), while still keeping the main codebase clean, and getting new features at
-        a good pace.
-        
-        Compatibility Patchers inject backward/forward compatibility shims (like class/function/attribute aliases), restore
-        features which were dropped/externalized because "not used enough" or "outside the scope of the library", and tweak
-        the signatures and behaviour of callables (eg. for arguments which disappeared, or which became mandatory). It can
-        even setup lazy "import aliases", so that code can import a moved module both from its old and new location.
-        
-        These shims allows you to upgrade your dependencies one at a time, when their maintainer finally had some time for a
-        code update, or when missing features and bugfixes justify a fork. Most importantly, they allow you to not get stuck,
-        when deadlines are tight, and crucial dependencies have conflicting expectations regarding the software version.
-        
-        Note that compatibility Patchers are not supposed to undo changes related to security (default access permissions,
-        markup escaping, cookie parameters...), because of the risks involved. Also, changes that only impact project-level
-        code (eg. new mandatory *settings*) should not get patched, since it's easier and cleaner for to simply update project
-        code.
-        
-        Technically, Compatibility Patchers are packages which manage a set of **fixers**, tiny utilities (often less than 10
-        lines of code) which advertise the change that they make, the software versions that they support, and which patch the
-        target code on demand. By applying these fixers in a proper order (sometimes before, sometimes after the
-        initialization of the patched software itself), Compatibility Patchers can easily "time travel", and work around multiple
-        breaking changes which target the same part of the code (e.g. a content handler being added and then removed).
-        
-        Compat Patcher Core holds the core logice of that system, via easily extendable classes: a registry system,
-        monkey-patching utilities, and a generic runner to be called at the very start of your application. It also contains
-        a **cookiecutter recipe** to setup your own Compatibility Patcher in a few minutes, with test scaffolding and packaging
-        metadata ready for launch.
-        
-        Documentation is available on `Read The Docs <https://compat-patcher-core.readthedocs.io/en/latest/index.html>`_
-        
-        Sources are available on `Github <https://github.com/pakal/compat-patcher-core>`_
-        
-        
-        Which applications currently benefit from this system?
-        
-        - The Django Web Framework via `Django-Compat-Patcher <https://github.com/pakal/django-compat-patcher>`_
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Provides-Extra: build_sphinx
-Provides-Extra: run_pylint
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+.. image:: https://travis-ci.com/pakal/compat-patcher-core.svg?branch=master
+    :target: https://travis-ci.com/pakal/compat-patcher-core
+
+
+*Long term API compatibility for fast-moving projects*
+
+
+Welcome to **Compat Patcher Core**, a mini-framework to build **Compatibility Patchers**. These companion applications
+allow your favorite software (a framework, a library...) to keep long term API stability towards its ecosystem
+(plugins, bridges to other applications...), while still keeping the main codebase clean, and getting new features at
+a good pace.
+
+Compatibility Patchers inject backward/forward compatibility shims (like class/function/attribute aliases), restore
+features which were dropped/externalized because "not used enough" or "outside the scope of the library", and tweak
+the signatures and behaviour of callables (eg. for arguments which disappeared, or which became mandatory). It can
+even setup lazy "import aliases", so that code can import a moved module both from its old and new location.
+
+These shims allows you to upgrade your dependencies one at a time, when their maintainer finally had some time for a
+code update, or when missing features and bugfixes justify a fork. Most importantly, they allow you to not get stuck,
+when deadlines are tight, and crucial dependencies have conflicting expectations regarding the software version.
+
+Note that compatibility Patchers are not supposed to undo changes related to security (default access permissions,
+markup escaping, cookie parameters...), because of the risks involved. Also, changes that only impact project-level
+code (eg. new mandatory *settings*) should not get patched, since it's easier and cleaner for to simply update project
+code.
+
+Technically, Compatibility Patchers are packages which manage a set of **fixers**, tiny utilities (often less than 10
+lines of code) which advertise the change that they make, the software versions that they support, and which patch the
+target code on demand. By applying these fixers in a proper order (sometimes before, sometimes after the
+initialization of the patched software itself), Compatibility Patchers can easily "time travel", and work around multiple
+breaking changes which target the same part of the code (e.g. a content handler being added and then removed).
+
+Compat Patcher Core holds the core logice of that system, via easily extendable classes: a registry system,
+monkey-patching utilities, and a generic runner to be called at the very start of your application. It also contains
+a **cookiecutter recipe** to setup your own Compatibility Patcher in a few minutes, with test scaffolding and packaging
+metadata ready for launch.
+
+Documentation is available on `Read The Docs <https://compat-patcher-core.readthedocs.io/en/latest/index.html>`_
+
+Sources are available on `Github <https://github.com/pakal/compat-patcher-core>`_
+
+
+Which applications currently benefit from this system?
+
+- The Django Web Framework via `Django-Compat-Patcher <https://github.com/pakal/django-compat-patcher>`_
```

### Comparing `compat-patcher-core-2.1/README.rst` & `compat-patcher-core-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/__init__.py` & `compat-patcher-core-2.2/src/compat_patcher_core/__init__.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/import_proxifier.py` & `compat-patcher-core-2.2/src/compat_patcher_core/import_proxifier.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/readme_generator.py` & `compat-patcher-core-2.2/src/compat_patcher_core/readme_generator.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/registry.py` & `compat-patcher-core-2.2/src/compat_patcher_core/registry.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/runner.py` & `compat-patcher-core-2.2/src/compat_patcher_core/runner.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/scaffolding.py` & `compat-patcher-core-2.2/src/compat_patcher_core/scaffolding.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core/utilities.py` & `compat-patcher-core-2.2/src/compat_patcher_core/utilities.py`

 * *Files identical despite different names*

### Comparing `compat-patcher-core-2.1/src/compat_patcher_core.egg-info/PKG-INFO` & `compat-patcher-core-2.2/src/compat_patcher_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: compat-patcher-core
-Version: 2.1
-Summary: A patcher system to allow easy and lasting API compatibility.
-Home-page: https://github.com/pakal/compat-patcher-core
-Author: Pascal Chambon & others
-Author-email: pythoniks@gmail.com
+Version: 2.2
+Summary: A patcher system to allow easy and lasting API compatibility
+Author-email: Pascal Chambon <pythoniks@gmail.com>
 License: MIT
-Description: .. image:: https://travis-ci.com/pakal/compat-patcher-core.svg?branch=master
-            :target: https://travis-ci.com/pakal/compat-patcher-core
-        
-        
-        *Long term API compatibility for fast-moving projects*
-        
-        
-        Welcome to **Compat Patcher Core**, a mini-framework to build **Compatibility Patchers**. These companion applications
-        allow your favorite software (a framework, a library...) to keep long term API stability towards its ecosystem
-        (plugins, bridges to other applications...), while still keeping the main codebase clean, and getting new features at
-        a good pace.
-        
-        Compatibility Patchers inject backward/forward compatibility shims (like class/function/attribute aliases), restore
-        features which were dropped/externalized because "not used enough" or "outside the scope of the library", and tweak
-        the signatures and behaviour of callables (eg. for arguments which disappeared, or which became mandatory). It can
-        even setup lazy "import aliases", so that code can import a moved module both from its old and new location.
-        
-        These shims allows you to upgrade your dependencies one at a time, when their maintainer finally had some time for a
-        code update, or when missing features and bugfixes justify a fork. Most importantly, they allow you to not get stuck,
-        when deadlines are tight, and crucial dependencies have conflicting expectations regarding the software version.
-        
-        Note that compatibility Patchers are not supposed to undo changes related to security (default access permissions,
-        markup escaping, cookie parameters...), because of the risks involved. Also, changes that only impact project-level
-        code (eg. new mandatory *settings*) should not get patched, since it's easier and cleaner for to simply update project
-        code.
-        
-        Technically, Compatibility Patchers are packages which manage a set of **fixers**, tiny utilities (often less than 10
-        lines of code) which advertise the change that they make, the software versions that they support, and which patch the
-        target code on demand. By applying these fixers in a proper order (sometimes before, sometimes after the
-        initialization of the patched software itself), Compatibility Patchers can easily "time travel", and work around multiple
-        breaking changes which target the same part of the code (e.g. a content handler being added and then removed).
-        
-        Compat Patcher Core holds the core logice of that system, via easily extendable classes: a registry system,
-        monkey-patching utilities, and a generic runner to be called at the very start of your application. It also contains
-        a **cookiecutter recipe** to setup your own Compatibility Patcher in a few minutes, with test scaffolding and packaging
-        metadata ready for launch.
-        
-        Documentation is available on `Read The Docs <https://compat-patcher-core.readthedocs.io/en/latest/index.html>`_
-        
-        Sources are available on `Github <https://github.com/pakal/compat-patcher-core>`_
-        
-        
-        Which applications currently benefit from this system?
-        
-        - The Django Web Framework via `Django-Compat-Patcher <https://github.com/pakal/django-compat-patcher>`_
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Provides-Extra: build_sphinx
-Provides-Extra: run_pylint
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+.. image:: https://travis-ci.com/pakal/compat-patcher-core.svg?branch=master
+    :target: https://travis-ci.com/pakal/compat-patcher-core
+
+
+*Long term API compatibility for fast-moving projects*
+
+
+Welcome to **Compat Patcher Core**, a mini-framework to build **Compatibility Patchers**. These companion applications
+allow your favorite software (a framework, a library...) to keep long term API stability towards its ecosystem
+(plugins, bridges to other applications...), while still keeping the main codebase clean, and getting new features at
+a good pace.
+
+Compatibility Patchers inject backward/forward compatibility shims (like class/function/attribute aliases), restore
+features which were dropped/externalized because "not used enough" or "outside the scope of the library", and tweak
+the signatures and behaviour of callables (eg. for arguments which disappeared, or which became mandatory). It can
+even setup lazy "import aliases", so that code can import a moved module both from its old and new location.
+
+These shims allows you to upgrade your dependencies one at a time, when their maintainer finally had some time for a
+code update, or when missing features and bugfixes justify a fork. Most importantly, they allow you to not get stuck,
+when deadlines are tight, and crucial dependencies have conflicting expectations regarding the software version.
+
+Note that compatibility Patchers are not supposed to undo changes related to security (default access permissions,
+markup escaping, cookie parameters...), because of the risks involved. Also, changes that only impact project-level
+code (eg. new mandatory *settings*) should not get patched, since it's easier and cleaner for to simply update project
+code.
+
+Technically, Compatibility Patchers are packages which manage a set of **fixers**, tiny utilities (often less than 10
+lines of code) which advertise the change that they make, the software versions that they support, and which patch the
+target code on demand. By applying these fixers in a proper order (sometimes before, sometimes after the
+initialization of the patched software itself), Compatibility Patchers can easily "time travel", and work around multiple
+breaking changes which target the same part of the code (e.g. a content handler being added and then removed).
+
+Compat Patcher Core holds the core logice of that system, via easily extendable classes: a registry system,
+monkey-patching utilities, and a generic runner to be called at the very start of your application. It also contains
+a **cookiecutter recipe** to setup your own Compatibility Patcher in a few minutes, with test scaffolding and packaging
+metadata ready for launch.
+
+Documentation is available on `Read The Docs <https://compat-patcher-core.readthedocs.io/en/latest/index.html>`_
+
+Sources are available on `Github <https://github.com/pakal/compat-patcher-core>`_
+
+
+Which applications currently benefit from this system?
+
+- The Django Web Framework via `Django-Compat-Patcher <https://github.com/pakal/django-compat-patcher>`_
```

