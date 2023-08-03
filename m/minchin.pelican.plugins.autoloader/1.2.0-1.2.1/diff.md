# Comparing `tmp/minchin.pelican.plugins.autoloader-1.2.0.tar.gz` & `tmp/minchin.pelican.plugins.autoloader-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minchin.pelican.plugins.autoloader-1.2.0.tar", last modified: Wed Jul 12 05:20:47 2023, max compression
+gzip compressed data, was "minchin.pelican.plugins.autoloader-1.2.1.tar", last modified: Thu Aug  3 20:33:56 2023, max compression
```

## Comparing `minchin.pelican.plugins.autoloader-1.2.0.tar` & `minchin.pelican.plugins.autoloader-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/
--rw-rw-rw-   0        0        0      895 2023-07-11 20:36:02.000000 minchin.pelican.plugins.autoloader-1.2.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1092 2023-07-11 20:36:41.000000 minchin.pelican.plugins.autoloader-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       72 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4695 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3280 2023-07-11 20:45:34.000000 minchin.pelican.plugins.autoloader-1.2.0/README.rst
--rw-rw-rw-   0        0        0      464 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/invoke.yaml
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/minchin/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.288687 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/
--rw-rw-rw-   0        0        0     4689 2023-07-12 05:20:45.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/autoloader.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.287685 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/
--rw-rw-rw-   0        0        0     4695 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/pelican/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.289686 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/autoloader/
--rw-rw-rw-   0        0        0       70 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/autoloader/__init__.py
--rw-rw-rw-   0        0        0      460 2023-07-11 20:38:02.000000 minchin.pelican.plugins.autoloader-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      815 2023-07-11 20:47:01.000000 minchin.pelican.plugins.autoloader-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     4567 2023-07-11 21:16:46.000000 minchin.pelican.plugins.autoloader-1.2.0/setup.py
--rw-rw-rw-   0        0        0      127 2023-07-12 05:00:33.000000 minchin.pelican.plugins.autoloader-1.2.0/tasks.py
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.911741 minchin.pelican.plugins.autoloader-1.2.1/
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      996 2023-08-03 20:27:11.000000 minchin.pelican.plugins.autoloader-1.2.1/CHANGELOG.rst
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     1071 2023-08-03 19:51:10.000000 minchin.pelican.plugins.autoloader-1.2.1/LICENSE.txt
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)       67 2023-08-03 19:51:10.000000 minchin.pelican.plugins.autoloader-1.2.1/MANIFEST.in
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     4588 2023-08-03 20:33:56.903741 minchin.pelican.plugins.autoloader-1.2.1/PKG-INFO
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     3185 2023-08-03 19:51:10.000000 minchin.pelican.plugins.autoloader-1.2.1/README.rst
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      446 2023-08-03 19:51:10.000000 minchin.pelican.plugins.autoloader-1.2.1/invoke.yaml
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.635741 minchin.pelican.plugins.autoloader-1.2.1/minchin/
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.635741 minchin.pelican.plugins.autoloader-1.2.1/minchin/pelican/
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.879741 minchin.pelican.plugins.autoloader-1.2.1/minchin/pelican/plugins/
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     4793 2023-08-03 20:33:53.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin/pelican/plugins/autoloader.py
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.863741 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     4588 2023-08-03 20:33:56.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      476 2023-08-03 20:33:56.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/SOURCES.txt
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)        1 2023-08-03 20:33:56.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/dependency_links.txt
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      248 2023-08-03 20:33:56.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/requires.txt
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)       36 2023-08-03 20:33:56.000000 minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/top_level.txt
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.639741 minchin.pelican.plugins.autoloader-1.2.1/pelican/
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.643741 minchin.pelican.plugins.autoloader-1.2.1/pelican/plugins/
+drwxrws---   0 u0_a233  (10233) media_rw  (1023)        0 2023-08-03 20:33:56.891741 minchin.pelican.plugins.autoloader-1.2.1/pelican/plugins/autoloader/
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)       69 2023-08-03 19:51:11.000000 minchin.pelican.plugins.autoloader-1.2.1/pelican/plugins/autoloader/__init__.py
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      445 2023-08-03 19:51:11.000000 minchin.pelican.plugins.autoloader-1.2.1/pyproject.toml
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      775 2023-08-03 19:51:11.000000 minchin.pelican.plugins.autoloader-1.2.1/requirements.txt
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)       38 2023-08-03 20:33:56.911741 minchin.pelican.plugins.autoloader-1.2.1/setup.cfg
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)     4477 2023-08-03 20:30:06.000000 minchin.pelican.plugins.autoloader-1.2.1/setup.py
+-rw-rw----   0 u0_a233  (10233) media_rw  (1023)      123 2023-08-03 19:51:11.000000 minchin.pelican.plugins.autoloader-1.2.1/tasks.py
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/CHANGELOG.rst` & `minchin.pelican.plugins.autoloader-1.2.1/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-AutoLoader Changelog
-====================
-
-1.2.0 -- 2023-07-11
--------------------
-
-- **feature**: include autoloading from additional "private" namespace of
-  ``minchin.pelican.readers``.
-
-1.1.0 -- 2022-04-09
--------------------
-
-- **feature**: allow autoloading of specificed plugins to be skipped via
-  ``AUTOLOADER_PLUGIN_BLACKLIST`` variable (on Pelican 4.5+ only).
-- **bug**: don't try and initialize ``pelican.plugins._utils`` or
-  ``pelican.plugins.signals``
-
-1.0.3 - 2022-03-20
-------------------
-
-- **support**: update to ``minchin.releaser`` 0.8.2, and thus officially support
-  Python 3.10.
-
-1.0.2 - 2021-10-24
-------------------
-
-- **feature**: original implementation
-- **support**: first release to PyPI under `minchin.pelican.plugins.autoloader`_
-
-.. _minchin.pelican.plugins.autoloader: https://pypi.org/project/minchin.pelican.plugins.autoloader/
+AutoLoader Changelog
+====================
+
+1.2.1 -- 2023-08-03
+-------------------
+
+- **bug**: don't break if no plugins exist in the namespace you are trying to load from.
+
+1.2.0 -- 2023-07-11
+-------------------
+
+- **feature**: include autoloading from additional "private" namespace of
+  ``minchin.pelican.readers``.
+
+1.1.0 -- 2022-04-09
+-------------------
+
+- **feature**: allow autoloading of specificed plugins to be skipped via
+  ``AUTOLOADER_PLUGIN_BLACKLIST`` variable (on Pelican 4.5+ only).
+- **bug**: don't try and initialize ``pelican.plugins._utils`` or
+  ``pelican.plugins.signals``
+
+1.0.3 - 2022-03-20
+------------------
+
+- **support**: update to ``minchin.releaser`` 0.8.2, and thus officially support
+  Python 3.10.
+
+1.0.2 - 2021-10-24
+------------------
+
+- **feature**: original implementation
+- **support**: first release to PyPI under `minchin.pelican.plugins.autoloader`_
+
+.. _minchin.pelican.plugins.autoloader: https://pypi.org/project/minchin.pelican.plugins.autoloader/
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/LICENSE.txt` & `minchin.pelican.plugins.autoloader-1.2.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021-23 Wm. Minchin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021-23 Wm. Minchin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/PKG-INFO` & `minchin.pelican.plugins.autoloader-1.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,129 @@
-Metadata-Version: 2.1
-Name: minchin.pelican.plugins.autoloader
-Version: 1.2.0
-Summary: Pelican plugin, used to auto-load my other plugins.
-Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
-Author: W. Minchin
-Author-email: w_minchin@hotmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
-Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: Pelican :: Plugins
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
-Provides-Extra: build
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE.txt
-
-==========
-AutoLoader
-==========
-
-``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
-a static site generator written in Python.
-
-``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
-It can also be extended to autoload
-plugins in other namespaces, for example, to autoload the ``pelican.plugins``
-namespace on versions of Pelican before 4.5 (when autoloading to those plugins
-was added to the Pelican core).
-
-.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
-    :alt: PyPI version number
-
-.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-    :alt: Changelog
-
-.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Supported Python version
-
-.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
-    :alt: License
-
-.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Download Count
-
-
-Installation
-============
-
-The easiest way to install ``AutoLoader`` is through the use of pip. This
-will also install the required dependencies automatically.
-
-.. code-block:: sh
-
-  pip install minchin.pelican.plugins.autoloader
-
-Further configuration will depend on the version of Pelican you are running. On
-version 4.5 or newer and you haven't defined ``PLUGINS`` in your
-``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
-if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
-of plugins in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  PLUGINS = [
-      # ...
-      'minchin.pelican.plugins.autoloader',
-      # ...
-  ]
-
-If you want to auto-load additional namespaces, you'll need to define the
-``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
-      "pelican.plugins",
-      # other namespaces
-  ]
-
-If you need to disallow auto-loading of certain plugins, you'll need to define
-the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
-This only works when autoloading from defined namespaces. E.g.:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
-      "pelican.plugins.misbehaving_plugin",
-      # other plugins
-  ]
-
-Usage Notes
-===========
-
-- the plugins loaded by this plugin will not be shown when you run
-  ``pelican-plugins``
+Metadata-Version: 2.1
+Name: minchin.pelican.plugins.autoloader
+Version: 1.2.1
+Summary: Pelican plugin, used to auto-load my other plugins.
+Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
+Author: W. Minchin
+Author-email: w_minchin@hotmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
+Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/x-rst
+Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: lint
+Provides-Extra: all
+License-File: LICENSE.txt
+
+==========
+AutoLoader
+==========
+
+``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
+a static site generator written in Python.
+
+``AutoLoader`` is designed to autoload the other Pelican plugins in my
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
+plugins in other namespaces, for example, to autoload the ``pelican.plugins``
+namespace on versions of Pelican before 4.5 (when autoloading to those plugins
+was added to the Pelican core).
+
+.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
+    :alt: PyPI version number
+
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
+
+.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Supported Python version
+
+.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Download Count
+
+
+Installation
+============
+
+The easiest way to install ``AutoLoader`` is through the use of pip. This
+will also install the required dependencies automatically.
+
+.. code-block:: sh
+
+  pip install minchin.pelican.plugins.autoloader
+
+Further configuration will depend on the version of Pelican you are running. On
+version 4.5 or newer and you haven't defined ``PLUGINS`` in your
+``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
+if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
+of plugins in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  PLUGINS = [
+      # ...
+      'minchin.pelican.plugins.autoloader',
+      # ...
+  ]
+
+If you want to auto-load additional namespaces, you'll need to define the
+``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
+      "pelican.plugins",
+      # other namespaces
+  ]
+
+If you need to disallow auto-loading of certain plugins, you'll need to define
+the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
+This only works when autoloading from defined namespaces. E.g.:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
+      "pelican.plugins.misbehaving_plugin",
+      # other plugins
+  ]
+
+Usage Notes
+===========
+
+- the plugins loaded by this plugin will not be shown when you run
+  ``pelican-plugins``
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/README.rst` & `minchin.pelican.plugins.autoloader-1.2.1/README.rst`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-==========
-AutoLoader
-==========
-
-``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
-a static site generator written in Python.
-
-``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
-It can also be extended to autoload
-plugins in other namespaces, for example, to autoload the ``pelican.plugins``
-namespace on versions of Pelican before 4.5 (when autoloading to those plugins
-was added to the Pelican core).
-
-.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
-    :alt: PyPI version number
-
-.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-    :alt: Changelog
-
-.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Supported Python version
-
-.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
-    :alt: License
-
-.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Download Count
-
-
-Installation
-============
-
-The easiest way to install ``AutoLoader`` is through the use of pip. This
-will also install the required dependencies automatically.
-
-.. code-block:: sh
-
-  pip install minchin.pelican.plugins.autoloader
-
-Further configuration will depend on the version of Pelican you are running. On
-version 4.5 or newer and you haven't defined ``PLUGINS`` in your
-``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
-if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
-of plugins in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  PLUGINS = [
-      # ...
-      'minchin.pelican.plugins.autoloader',
-      # ...
-  ]
-
-If you want to auto-load additional namespaces, you'll need to define the
-``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
-      "pelican.plugins",
-      # other namespaces
-  ]
-
-If you need to disallow auto-loading of certain plugins, you'll need to define
-the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
-This only works when autoloading from defined namespaces. E.g.:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
-      "pelican.plugins.misbehaving_plugin",
-      # other plugins
-  ]
-
-Usage Notes
-===========
-
-- the plugins loaded by this plugin will not be shown when you run
-  ``pelican-plugins``
+==========
+AutoLoader
+==========
+
+``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
+a static site generator written in Python.
+
+``AutoLoader`` is designed to autoload the other Pelican plugins in my
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
+plugins in other namespaces, for example, to autoload the ``pelican.plugins``
+namespace on versions of Pelican before 4.5 (when autoloading to those plugins
+was added to the Pelican core).
+
+.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
+    :alt: PyPI version number
+
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
+
+.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Supported Python version
+
+.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Download Count
+
+
+Installation
+============
+
+The easiest way to install ``AutoLoader`` is through the use of pip. This
+will also install the required dependencies automatically.
+
+.. code-block:: sh
+
+  pip install minchin.pelican.plugins.autoloader
+
+Further configuration will depend on the version of Pelican you are running. On
+version 4.5 or newer and you haven't defined ``PLUGINS`` in your
+``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
+if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
+of plugins in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  PLUGINS = [
+      # ...
+      'minchin.pelican.plugins.autoloader',
+      # ...
+  ]
+
+If you want to auto-load additional namespaces, you'll need to define the
+``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
+      "pelican.plugins",
+      # other namespaces
+  ]
+
+If you need to disallow auto-loading of certain plugins, you'll need to define
+the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
+This only works when autoloading from defined namespaces. E.g.:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
+      "pelican.plugins.misbehaving_plugin",
+      # other plugins
+  ]
+
+Usage Notes
+===========
+
+- the plugins loaded by this plugin will not be shown when you run
+  ``pelican-plugins``
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/autoloader.py` & `minchin.pelican.plugins.autoloader-1.2.1/minchin/pelican/plugins/autoloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,137 @@
-import importlib
-import logging
-import pkgutil
-
-import semantic_version
-
-from pelican import __version__ as pelican_version
-from pelican import signals
-
-__title__ = "minchin.pelican.plugins.autoloader"
-__version__ = "1.2.0"
-__description__ = "Pelican plugin, used to auto-load my other plugins."
-__author__ = "W. Minchin"
-__email__ = "w_minchin@hotmail.com"
-__url__ = "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader"
-__license__ = "MIT License"
-
-LOG_PREFIX = "[AutoLoader]"
-DEFAULT_NAMESPACE_LIST = [
-    "minchin.pelican.plugins",
-    "minchin.pelican.readers",
-]
-DEFAULT_PLUGIN_BLACKLIST = [
-    "pelican.plugins._utils",
-    "pelican.plugins.signals",
-]
-
-logger = logging.getLogger(__name__)
-
-
-def pelican_namespace_plugin_support():
-    """
-    Determine if the installed version of Pelican natively supports namespace
-    plugins.
-
-    In short, the Pelican version must be greater than or equal to 4.5.0.
-
-    Return:
-        bool: if namespace plugins are supported
-    """
-
-    pelican_semver = semantic_version.Version(pelican_version)
-    if pelican_semver.major > 4:
-        return True
-    elif pelican_semver.major == 4 and pelican_semver.minor >= 5:
-        return True
-    else:
-        return False
-
-
-def initialize(pelican_instance):
-    if "AUTOLOADER_SIGNAL_INITALIZED" not in pelican_instance.settings.keys():
-        logger.debug("%s loading plugins in the selected namespaces." % LOG_PREFIX)
-
-        if "AUTOLOADER_NAMESPACES" in pelican_instance.settings:
-            namespace_list = pelican_instance.settings["AUTOLOADER_NAMESPACES"]
-        else:
-            namespace_list = DEFAULT_NAMESPACE_LIST
-
-        if "AUTOLOADER_PLUGIN_BLACKLIST" in pelican_instance.settings:
-            namespace_blacklist = pelican_instance.settings[
-                "AUTOLOADER_PLUGIN_BLACKLIST"
-            ]
-        else:
-            namespace_blacklist = DEFAULT_PLUGIN_BLACKLIST
-
-        if pelican_namespace_plugin_support():
-            # only namespace plugins otherwise; Pelican 4.5.0 or newer
-
-            for ns in namespace_list:
-                logger.debug("%s     %s" % (LOG_PREFIX, ns))
-
-                ns_module = importlib.import_module(ns)
-                # this differs from Pelican's built-in namespace plugin finder,
-                # in that we don't require plugins to be their own modules
-                namespace_plugins = {
-                    name: importlib.import_module(name)
-                    for _, name, _ in pkgutil.iter_modules(
-                        ns_module.__path__, ns_module.__name__ + "."
-                    )
-                }
-                for plugin_name, plugin_pkg in namespace_plugins.items():
-                    if plugin_name in namespace_blacklist:
-                        logger.debug(
-                            "%s         %s ... skipping!" % (LOG_PREFIX, plugin_name)
-                        )
-                        continue
-
-                    # manually register plugins
-                    logger.debug("%s         %s" % (LOG_PREFIX, plugin_name))
-                    try:
-                        plugin_pkg.register()
-                    except Exception as e:
-                        logger.error(
-                            "Cannot register plugin `%s`\n%s",
-                            plugin_pkg.__name__,
-                            e,
-                        )
-
-        else:
-            if "PLUGINS" not in pelican_instance.settings.keys():
-                pelican_instance.settings["PLUGINS"] = list()
-
-            for ns in namespace_list:
-                logger.debug("%s     %s" % (LOG_PREFIX, ns))
-                ns_module = importlib.import_module(ns)
-                plugin_iter = pkgutil.iter_modules(
-                    ns_module.__path__, ns_module.__name__ + "."
-                )
-
-                for k in plugin_iter:
-                    pelican_instance.settings["PLUGINS"].append(k.name)
-                    logger.debug(
-                        '%s         "%s" appended to PLUGINS' % (LOG_PREFIX, k.name)
-                    )
-            # force update of plugins
-            pelican_instance.init_plugins()
-
-        pelican_instance.settings["AUTOLOADER_SIGNAL_INITALIZED"] = True
-        # needed, in case any of these plugins are calling the "initialized" signal
-        logger.debug("%s signal: initalized" % LOG_PREFIX)
-        signals.initialized.send(pelican_instance)
-    else:
-        # avoid recurssion
-        pass
-
-
-def register():
-    """Register the plugin with Pelican"""
-    signals.initialized.connect(initialize)
+import importlib
+import logging
+import pkgutil
+
+import semantic_version
+
+from pelican import __version__ as pelican_version
+from pelican import signals
+
+__title__ = "minchin.pelican.plugins.autoloader"
+__version__ = "1.2.1"
+__description__ = "Pelican plugin, used to auto-load my other plugins."
+__author__ = "W. Minchin"
+__email__ = "w_minchin@hotmail.com"
+__url__ = "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader"
+__license__ = "MIT License"
+
+LOG_PREFIX = "[AutoLoader]"
+DEFAULT_NAMESPACE_LIST = [
+    "minchin.pelican.plugins",
+    "minchin.pelican.readers",
+]
+DEFAULT_PLUGIN_BLACKLIST = [
+    "pelican.plugins._utils",
+    "pelican.plugins.signals",
+]
+
+logger = logging.getLogger(__name__)
+
+
+def pelican_namespace_plugin_support():
+    """
+    Determine if the installed version of Pelican natively supports namespace
+    plugins.
+
+    In short, the Pelican version must be greater than or equal to 4.5.0.
+
+    Return:
+        bool: if namespace plugins are supported
+    """
+
+    pelican_semver = semantic_version.Version(pelican_version)
+    if pelican_semver.major > 4:
+        return True
+    elif pelican_semver.major == 4 and pelican_semver.minor >= 5:
+        return True
+    else:
+        return False
+
+
+def initialize(pelican_instance):
+    if "AUTOLOADER_SIGNAL_INITALIZED" not in pelican_instance.settings.keys():
+        logger.debug("%s loading plugins in the selected namespaces." % LOG_PREFIX)
+
+        if "AUTOLOADER_NAMESPACES" in pelican_instance.settings:
+            namespace_list = pelican_instance.settings["AUTOLOADER_NAMESPACES"]
+        else:
+            namespace_list = DEFAULT_NAMESPACE_LIST
+
+        if "AUTOLOADER_PLUGIN_BLACKLIST" in pelican_instance.settings:
+            namespace_blacklist = pelican_instance.settings[
+                "AUTOLOADER_PLUGIN_BLACKLIST"
+            ]
+        else:
+            namespace_blacklist = DEFAULT_PLUGIN_BLACKLIST
+
+        if pelican_namespace_plugin_support():
+            # only namespace plugins otherwise; Pelican 4.5.0 or newer
+
+            for ns in namespace_list:
+                logger.debug("%s    %s" % (LOG_PREFIX, ns))
+
+                try:
+                    ns_module = importlib.import_module(ns)
+                except ModuleNotFoundError:
+                    logger.debug(
+                        "%s        Unable to load namespace '%s'." % (LOG_PREFIX, ns)
+                    )
+                    continue
+
+                # this differs from Pelican's built-in namespace plugin finder,
+                # in that we don't require plugins to be their own modules
+                namespace_plugins = {
+                    name: importlib.import_module(name)
+                    for _, name, _ in pkgutil.iter_modules(
+                        ns_module.__path__, ns_module.__name__ + "."
+                    )
+                }
+                for plugin_name, plugin_pkg in namespace_plugins.items():
+                    if plugin_name in namespace_blacklist:
+                        logger.debug(
+                            "%s        %s ... skipping!" % (LOG_PREFIX, plugin_name)
+                        )
+                        continue
+
+                    # manually register plugins
+                    logger.debug("%s    %s" % (LOG_PREFIX, plugin_name))
+                    try:
+                        plugin_pkg.register()
+                    except Exception as e:
+                        logger.error(
+                            "Cannot register plugin `%s`\n%s",
+                            plugin_pkg.__name__,
+                            e,
+                        )
+
+        else:
+            if "PLUGINS" not in pelican_instance.settings.keys():
+                pelican_instance.settings["PLUGINS"] = list()
+
+            for ns in namespace_list:
+                logger.debug("%s     %s" % (LOG_PREFIX, ns))
+                ns_module = importlib.import_module(ns)
+                plugin_iter = pkgutil.iter_modules(
+                    ns_module.__path__, ns_module.__name__ + "."
+                )
+
+                for k in plugin_iter:
+                    pelican_instance.settings["PLUGINS"].append(k.name)
+                    logger.debug(
+                        '%s         "%s" appended to PLUGINS' % (LOG_PREFIX, k.name)
+                    )
+            # force update of plugins
+            pelican_instance.init_plugins()
+
+        pelican_instance.settings["AUTOLOADER_SIGNAL_INITALIZED"] = True
+        # needed, in case any of these plugins are calling the "initialized" signal
+        logger.debug("%s signal: initalized" % LOG_PREFIX)
+        signals.initialized.send(pelican_instance)
+    else:
+        # avoid recurssion
+        pass
+
+
+def register():
+    """Register the plugin with Pelican"""
+    signals.initialized.connect(initialize)
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO` & `minchin.pelican.plugins.autoloader-1.2.1/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,129 @@
-Metadata-Version: 2.1
-Name: minchin.pelican.plugins.autoloader
-Version: 1.2.0
-Summary: Pelican plugin, used to auto-load my other plugins.
-Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
-Author: W. Minchin
-Author-email: w_minchin@hotmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
-Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: Pelican :: Plugins
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
-Provides-Extra: build
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE.txt
-
-==========
-AutoLoader
-==========
-
-``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
-a static site generator written in Python.
-
-``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
-It can also be extended to autoload
-plugins in other namespaces, for example, to autoload the ``pelican.plugins``
-namespace on versions of Pelican before 4.5 (when autoloading to those plugins
-was added to the Pelican core).
-
-.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
-    :alt: PyPI version number
-
-.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-    :alt: Changelog
-
-.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Supported Python version
-
-.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
-    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
-    :alt: License
-
-.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
-    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
-    :alt: Download Count
-
-
-Installation
-============
-
-The easiest way to install ``AutoLoader`` is through the use of pip. This
-will also install the required dependencies automatically.
-
-.. code-block:: sh
-
-  pip install minchin.pelican.plugins.autoloader
-
-Further configuration will depend on the version of Pelican you are running. On
-version 4.5 or newer and you haven't defined ``PLUGINS`` in your
-``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
-if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
-of plugins in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  PLUGINS = [
-      # ...
-      'minchin.pelican.plugins.autoloader',
-      # ...
-  ]
-
-If you want to auto-load additional namespaces, you'll need to define the
-``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
-      "pelican.plugins",
-      # other namespaces
-  ]
-
-If you need to disallow auto-loading of certain plugins, you'll need to define
-the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
-This only works when autoloading from defined namespaces. E.g.:
-
-.. code-block:: python
-
-  # pelicanconf.py
-
-  from minchin.pelican.plugins import autoloader
-
-  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
-      "pelican.plugins.misbehaving_plugin",
-      # other plugins
-  ]
-
-Usage Notes
-===========
-
-- the plugins loaded by this plugin will not be shown when you run
-  ``pelican-plugins``
+Metadata-Version: 2.1
+Name: minchin.pelican.plugins.autoloader
+Version: 1.2.1
+Summary: Pelican plugin, used to auto-load my other plugins.
+Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
+Author: W. Minchin
+Author-email: w_minchin@hotmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
+Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/x-rst
+Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: lint
+Provides-Extra: all
+License-File: LICENSE.txt
+
+==========
+AutoLoader
+==========
+
+``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
+a static site generator written in Python.
+
+``AutoLoader`` is designed to autoload the other Pelican plugins in my
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
+plugins in other namespaces, for example, to autoload the ``pelican.plugins``
+namespace on versions of Pelican before 4.5 (when autoloading to those plugins
+was added to the Pelican core).
+
+.. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
+    :alt: PyPI version number
+
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
+
+.. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Supported Python version
+
+.. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/minchin.pelican.plugins.autoloader.svg?style=flat
+    :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
+    :alt: Download Count
+
+
+Installation
+============
+
+The easiest way to install ``AutoLoader`` is through the use of pip. This
+will also install the required dependencies automatically.
+
+.. code-block:: sh
+
+  pip install minchin.pelican.plugins.autoloader
+
+Further configuration will depend on the version of Pelican you are running. On
+version 4.5 or newer and you haven't defined ``PLUGINS`` in your
+``pelicanconf.py``, nothing more in needed. On earlier versions of Pelican, or
+if you've defined ``PLUGINS``, you'll need to add the autoloader to your list
+of plugins in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  PLUGINS = [
+      # ...
+      'minchin.pelican.plugins.autoloader',
+      # ...
+  ]
+
+If you want to auto-load additional namespaces, you'll need to define the
+``AUTOLOADER_NAMESPACES`` variable in your ``pelicanconf.py`` file:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_NAMESPACES = autoloader.DEFAULT_NAMESPACE_LIST + [
+      "pelican.plugins",
+      # other namespaces
+  ]
+
+If you need to disallow auto-loading of certain plugins, you'll need to define
+the ``AUTOLOADER_PLUGIN_BLACKLIST`` variable in your ``pelicanconf.py`` file.
+This only works when autoloading from defined namespaces. E.g.:
+
+.. code-block:: python
+
+  # pelicanconf.py
+
+  from minchin.pelican.plugins import autoloader
+
+  AUTOLOADER_PLUGIN_BLACKLIST = autoloader.DEFAULT_PLUGIN_BLACKLIST + [
+      "pelican.plugins.misbehaving_plugin",
+      # other plugins
+  ]
+
+Usage Notes
+===========
+
+- the plugins loaded by this plugin will not be shown when you run
+  ``pelican-plugins``
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/requirements.txt` & `minchin.pelican.plugins.autoloader-1.2.1/requirements.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile
-#
-blinker==1.6.2
-    # via pelican
-docutils==0.20.1
-    # via pelican
-feedgenerator==2.1.0
-    # via pelican
-jinja2==3.1.2
-    # via pelican
-markdown-it-py==3.0.0
-    # via rich
-markupsafe==2.1.3
-    # via jinja2
-mdurl==0.1.2
-    # via markdown-it-py
-pelican==4.8.0
-    # via minchin.pelican.plugins.autoloader (setup.py)
-pygments==2.15.1
-    # via
-    #   pelican
-    #   rich
-python-dateutil==2.8.2
-    # via pelican
-pytz==2023.3
-    # via
-    #   feedgenerator
-    #   pelican
-rich==13.4.2
-    # via pelican
-semantic-version==2.10.0
-    # via minchin.pelican.plugins.autoloader (setup.py)
-six==1.16.0
-    # via python-dateutil
-unidecode==1.3.6
-    # via pelican
+#
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
+#
+#    pip-compile
+#
+blinker==1.6.2
+    # via pelican
+docutils==0.20.1
+    # via pelican
+feedgenerator==2.1.0
+    # via pelican
+jinja2==3.1.2
+    # via pelican
+markdown-it-py==3.0.0
+    # via rich
+markupsafe==2.1.3
+    # via jinja2
+mdurl==0.1.2
+    # via markdown-it-py
+pelican==4.8.0
+    # via minchin.pelican.plugins.autoloader (setup.py)
+pygments==2.15.1
+    # via
+    #   pelican
+    #   rich
+python-dateutil==2.8.2
+    # via pelican
+pytz==2023.3
+    # via
+    #   feedgenerator
+    #   pelican
+rich==13.5.2
+    # via pelican
+semantic-version==2.10.0
+    # via minchin.pelican.plugins.autoloader (setup.py)
+six==1.16.0
+    # via python-dateutil
+unidecode==1.3.6
+    # via pelican
```

### Comparing `minchin.pelican.plugins.autoloader-1.2.0/setup.py` & `minchin.pelican.plugins.autoloader-1.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,149 @@
-import codecs
-import os
-import re
-
-import setuptools
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-
-def read(*parts):
-    # intentionally *not* adding an encoding option to open
-    return codecs.open(os.path.join(here, *parts), "r").read()
-
-
-def find_meta(*meta_file_parts, meta_key):
-    """
-    Extract __*meta*__ from meta_file
-    """
-    meta_file = read(*meta_file_parts)
-    meta_match = re.search(
-        r"^__{}__ = ['\"]([^'\"]*)['\"]".format(meta_key), meta_file, re.M
-    )
-    if meta_match:
-        return meta_match.group(1)
-    raise RuntimeError("Unable to find __{}__ string.".format(meta_key))
-
-
-##############################################################################
-#                          PACKAGE METADATA                                  #
-##############################################################################
-META_PATH = ["minchin", "pelican", "plugins", "autoloader.py"]
-
-NAME = find_meta(*META_PATH, meta_key="title").lower()
-VERSION = find_meta(*META_PATH, meta_key="version")
-SHORT_DESC = find_meta(*META_PATH, meta_key="description")
-LONG_DESC = read("README.rst")
-AUTHOR = find_meta(*META_PATH, meta_key="author")
-AUTHOR_EMAIL = find_meta(*META_PATH, meta_key="email")
-URL = find_meta(*META_PATH, meta_key="url")
-LICENSE = find_meta(*META_PATH, meta_key="license")
-
-PACKAGES = setuptools.find_namespace_packages(
-    exclude=(
-        "test",
-        "docs",
-    )
-)
-
-INSTALL_REQUIRES = [
-    "pelican",
-    "semantic_version",
-]
-
-EXTRA_REQUIRES = {
-    "build": [
-        "pip-tools",
-        "minchin.releaser >= 0.8.2",
-        # less, installed via npm  # npm install less -g
-    ],
-    "docs": [
-        # 'sphinx >= 1.4',  # theme requires at least 1.4
-        # 'cloud_sptheme >= 1.8',
-        # 'releases',
-        # 'Babel >= 1.3, != 2.0',  # 2.0 breaks on Windows
-    ],
-    "test": [
-        # 'green >= 1.9.4',  # v2 works
-        # 'coverage',
-        # 'isort',
-        # 'pydocstyle',
-        # 'pycodestyle',
-        # 'check-manifest'
-    ],
-    "dev": [
-        "markdown",
-        "minchin.pelican.plugins.nojekyll",
-    ],
-}
-
-# full list of Classifiers at
-# https://pypi.python.org/pypi?%3Aaction=list_classifiers
-CLASSIFIERS = [
-    #   having an unknown classifier should keep PyPI from accepting the
-    #   package as an upload
-    # 'Private :: Do Not Upload',
-    # 'Development Status :: 1 - Planning',
-    # 'Development Status :: 2 - Pre-Alpha',
-    # 'Development Status :: 3 - Alpha',
-    # "Development Status :: 4 - Beta",
-    'Development Status :: 5 - Production/Stable',
-    # 'Development Status :: 6 - Mature',
-    # 'Development Status :: 7 - Inactive',
-    "Environment :: Console",
-    "Framework :: Pelican :: Plugins",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-    "Natural Language :: English",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-##############################################################################
-
-if LICENSE in ["MIT License"]:
-    CLASSIFIERS += ["License :: OSI Approved :: {}".format(LICENSE)]
-
-# add 'all' key to EXTRA_REQUIRES
-all_requires = []
-for k, v in EXTRA_REQUIRES.items():
-    all_requires.extend(v)
-EXTRA_REQUIRES["all"] = all_requires
-
-
-setuptools.setup(
-    name=NAME,
-    version=VERSION,
-    url=URL,
-    project_urls={
-        "Bug Tracker": "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues",
-        "Changelog": "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst",
-    },
-    license=LICENSE,
-    author=AUTHOR,
-    author_email=AUTHOR_EMAIL,
-    description=SHORT_DESC,
-    long_description=LONG_DESC,
-    long_description_content_type="text/x-rst",
-    packages=PACKAGES,
-    package_data={"": ["README.rst", "CHANGELOG.rst", "LICENSE.txt"]},
-    include_package_data=True,
-    install_requires=INSTALL_REQUIRES,
-    extras_require=EXTRA_REQUIRES,
-    platforms="any",
-    classifiers=CLASSIFIERS,
-    # namespace_packages=[
-    #     # "pelican",
-    #     # "pelican.plugins",
-    #     "pelican.plugins.seafoam",
-    # ],
-    # zip_save=False,  # use wheel instead
-)
+import codecs
+import os
+import re
+
+import setuptools
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+
+def read(*parts):
+    # intentionally *not* adding an encoding option to open
+    return codecs.open(os.path.join(here, *parts), "r").read()
+
+
+def find_meta(*meta_file_parts, meta_key):
+    """
+    Extract __*meta*__ from meta_file
+    """
+    meta_file = read(*meta_file_parts)
+    meta_match = re.search(
+        r"^__{}__ = ['\"]([^'\"]*)['\"]".format(meta_key), meta_file, re.M
+    )
+    if meta_match:
+        return meta_match.group(1)
+    raise RuntimeError("Unable to find __{}__ string.".format(meta_key))
+
+
+##############################################################################
+#                          PACKAGE METADATA                                  #
+##############################################################################
+META_PATH = ["minchin", "pelican", "plugins", "autoloader.py"]
+
+NAME = find_meta(*META_PATH, meta_key="title").lower()
+VERSION = find_meta(*META_PATH, meta_key="version")
+SHORT_DESC = find_meta(*META_PATH, meta_key="description")
+LONG_DESC = read("README.rst")
+AUTHOR = find_meta(*META_PATH, meta_key="author")
+AUTHOR_EMAIL = find_meta(*META_PATH, meta_key="email")
+URL = find_meta(*META_PATH, meta_key="url")
+LICENSE = find_meta(*META_PATH, meta_key="license")
+
+PACKAGES = setuptools.find_namespace_packages(
+    exclude=(
+        "test",
+        "docs",
+    )
+)
+
+INSTALL_REQUIRES = [
+    "pelican",
+    "semantic_version",
+]
+
+EXTRA_REQUIRES = {
+    "build": [
+        "pip-tools",
+        "minchin.releaser >= 0.8.2",
+        # less, installed via npm  # npm install less -g
+    ],
+    "docs": [
+        # 'sphinx >= 1.4',  # theme requires at least 1.4
+        # 'cloud_sptheme >= 1.8',
+        # 'releases',
+        # 'Babel >= 1.3, != 2.0',  # 2.0 breaks on Windows
+    ],
+    "test": [
+        # 'green >= 1.9.4',  # v2 works
+        # 'coverage',
+        # 'isort',
+        # 'pydocstyle',
+        # 'pycodestyle',
+        # 'check-manifest'
+    ],
+    "dev": [
+        "markdown",
+        "minchin.pelican.plugins.nojekyll",
+    ],
+    "lint": [
+        "black",
+        "isort",
+    ],
+}
+
+# full list of Classifiers at
+# https://pypi.python.org/pypi?%3Aaction=list_classifiers
+CLASSIFIERS = [
+    #   having an unknown classifier should keep PyPI from accepting the
+    #   package as an upload
+    # 'Private :: Do Not Upload',
+    # 'Development Status :: 1 - Planning',
+    # 'Development Status :: 2 - Pre-Alpha',
+    # 'Development Status :: 3 - Alpha',
+    # "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
+    # 'Development Status :: 6 - Mature',
+    # 'Development Status :: 7 - Inactive',
+    "Environment :: Console",
+    "Framework :: Pelican :: Plugins",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "Natural Language :: English",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+##############################################################################
+
+if LICENSE in ["MIT License"]:
+    CLASSIFIERS += ["License :: OSI Approved :: {}".format(LICENSE)]
+
+# add 'all' key to EXTRA_REQUIRES
+all_requires = []
+for k, v in EXTRA_REQUIRES.items():
+    all_requires.extend(v)
+EXTRA_REQUIRES["all"] = all_requires
+
+
+setuptools.setup(
+    name=NAME,
+    version=VERSION,
+    url=URL,
+    project_urls={
+        "Bug Tracker": "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues",
+        "Changelog": "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst",
+    },
+    license=LICENSE,
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    description=SHORT_DESC,
+    long_description=LONG_DESC,
+    long_description_content_type="text/x-rst",
+    packages=PACKAGES,
+    package_data={"": ["README.rst", "CHANGELOG.rst", "LICENSE.txt"]},
+    include_package_data=True,
+    install_requires=INSTALL_REQUIRES,
+    extras_require=EXTRA_REQUIRES,
+    platforms="any",
+    classifiers=CLASSIFIERS,
+    # namespace_packages=[
+    #     # "pelican",
+    #     # "pelican.plugins",
+    #     "pelican.plugins.seafoam",
+    # ],
+    # zip_save=False,  # use wheel instead
+)
```

