# Comparing `tmp/universal_pathlib-0.0.9.tar.gz` & `tmp/universal_pathlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_pathlib-0.0.9.tar", last modified: Wed May 12 16:34:52 2021, max compression
+gzip compressed data, was "universal_pathlib-0.1.0.tar", last modified: Thu Aug  3 08:08:15 2023, max compression
```

## Comparing `universal_pathlib-0.0.9.tar` & `universal_pathlib-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,65 @@
--rw-r--r--   0        0        0      195 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.flake8
--rw-r--r--   0        0        0     1006 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.github/workflows/python.yml
--rw-r--r--   0        0        0       38 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.gitignore
--rw-r--r--   0        0        0     1065 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/LICENSE
--rw-r--r--   0        0        0      843 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/README.md
--rw-r--r--   0        0        0      308 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/environment.yml
--rw-r--r--   0        0        0    12505 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/notebooks/examples.ipynb
--rw-r--r--   0        0        0      962 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/noxfile.py
--rw-r--r--   0        0        0      859 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      540 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/setup.py
--rw-r--r--   0        0        0      102 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/__init__.py
--rw-r--r--   0        0        0     1535 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/core.py
--rw-r--r--   0        0        0       45 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/errors.py
--rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/__init__.py
--rw-r--r--   0        0        0      893 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/hdfs.py
--rw-r--r--   0        0        0     1189 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/http.py
--rw-r--r--   0        0        0     1228 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/memory.py
--rw-r--r--   0        0        0      734 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/s3.py
--rw-r--r--   0        0        0      742 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/registry.py
--rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/__init__.py
--rw-r--r--   0        0        0     6263 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/cases.py
--rw-r--r--   0        0        0     4796 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/__init__.py
--rw-r--r--   0        0        0      635 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_hdfs.py
--rw-r--r--   0        0        0      226 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_http.py
--rw-r--r--   0        0        0      897 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_memory.py
--rw-r--r--   0        0        0     2638 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_s3.py
--rw-r--r--   0        0        0     1476 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/test_core.py
--rw-r--r--   0        0        0     8582 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/universal_path.py
--rw-r--r--   0        0        0      232 1970-01-01 00:00:00.000000 universal_pathlib-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/notebooks/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/universal_pathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:08:14.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/upath/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/upath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23978 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/tests/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/upath/tests/pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/_test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104167 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_310.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109314 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_311.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138582 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_312.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91139 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_38.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98727 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/upath/tests/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/third_party/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/utils.py
```

### Comparing `universal_pathlib-0.0.9/LICENSE` & `universal_pathlib-0.1.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Quansight
+Copyright (c) 2022, Andrew Fulton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `universal_pathlib-0.0.9/notebooks/examples.ipynb` & `universal_pathlib-0.1.0/notebooks/examples.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9255288938492063%*

 * *Differences: {"'cells'": "{0: {'source': ['import pathlib\\n', 'import warnings\\n', 'from tempfile import "*

 * *            "NamedTemporaryFile\\n', '\\n', 'from upath import UPath\\n', '\\n', "*

 * *            '\'warnings.filterwarnings(action="ignore", message="UPath .*", '*

 * *            'module="upath.core")\']}, 1: {\'source\': {insert: [(0, \'# Local Filesystem\\n\'), '*

 * *            "(2, 'If you give a local path, UPath defaults to `pathlib.PosixPath` or "*

 * *            "`pathlib.WindowsPath`, just as `pathlib.Path`.')], delet […]*

```diff
@@ -9,29 +9,35 @@
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "outputs": [],
             "source": [
-                "from upath import UPath"
+                "import pathlib\n",
+                "import warnings\n",
+                "from tempfile import NamedTemporaryFile\n",
+                "\n",
+                "from upath import UPath\n",
+                "\n",
+                "warnings.filterwarnings(action=\"ignore\", message=\"UPath .*\", module=\"upath.core\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "source": [
-                "# local\n",
+                "# Local Filesystem\n",
                 "\n",
-                "If you give a local path, Upath defaults to `pathlib.PosixPath` or `pathlib.WindowsPath`"
+                "If you give a local path, UPath defaults to `pathlib.PosixPath` or `pathlib.WindowsPath`, just as `pathlib.Path`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "autoscroll": false,
@@ -39,122 +45,182 @@
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "/tmp/tmpdeaokyh7 <class 'str'>\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
-                            "PosixPath('/tmp')"
+                            "PosixPath('/tmp/tmpdeaokyh7')"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "local_path = UPath('/tmp')\n",
+                "tmp = NamedTemporaryFile()\n",
+                "print(tmp.name, type(tmp.name))\n",
+                "local_path = UPath(tmp.name)\n",
+                "assert isinstance(local_path, (pathlib.PosixPath, pathlib.WindowsPath))\n",
                 "local_path"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "source": [
-                "If you give it a scheme registered with fsspec, it will return a UniversalPath which uses fsspec FileSystem backend"
+                "If you give it a scheme registered with fsspec, it will return a UPath which uses fsspec FileSystem backend"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "autoscroll": false,
                 "ein.hycell": false,
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "local_uri='file:///tmp/tmpdeaokyh7'\n",
+                        "local_upath=UPath('file:/tmp/tmpdeaokyh7')\n",
+                        "type(local_upath)=<class 'upath.core.UPath'>\n",
+                        "type(local_upath.fs)=<class 'fsspec.implementations.local.LocalFileSystem'>\n"
+                    ]
+                }
+            ],
             "source": [
-                "local_upath = UPath('file:/tmp')"
+                "local_uri = local_path.absolute().as_uri()\n",
+                "print(f\"{local_uri=}\")\n",
+                "\n",
+                "local_upath = UPath(local_uri)\n",
+                "print(f\"{local_upath=}\")\n",
+                "\n",
+                "print(f\"{type(local_upath)=}\")\n",
+                "assert isinstance(local_upath, UPath)\n",
+                "\n",
+                "print(f\"{type(local_upath.fs)=}\")\n",
+                "tmp.close()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "source": [
-                "# fsspec FileSystems\n",
+                "# `fsspec` FileSystems\n",
                 "\n",
-                "with `UniversalPath` you can cannect to any fsspec FileSystem and interact with it in with it as you would with your local filesystem using pathlib. Connection arguments can be given in a couple of ways:\n",
+                "With `UPath` you can connect to any `fsspec` FileSystem and interact with it in with it as you would with your local filesystem using `pathlib`. Connection arguments can be given in a couple of ways:\n",
                 "\n",
-                "You can give them as keyword arguments as descibed for each filesystem in the fsspec docs:"
+                "You can give them as keyword arguments as described in the `fsspec` [docs](https://filesystem-spec.readthedocs.io/en/latest/api.html#built-in-implementations) for each filesystem implementation:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "autoscroll": false,
                 "ein.hycell": false,
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<fsspec.implementations.github.GithubFileSystem at 0x7f87bfea66b0>"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "gpath = UPath('github:/', org='Quansight', repo='universal_pathlib', sha='main')"
+                "ghpath = UPath('github:/', org='fsspec', repo='universal_pathlib', sha='main')\n",
+                "assert ghpath.exists()\n",
+                "ghpath.fs"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "source": [
-                "or define them in the path/url, in which case they will be appropriately parsed:"
+                "Or define them in the path/url, in which case they will be appropriately parsed:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "autoscroll": false,
                 "ein.hycell": false,
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "UPath('github://fsspec:universal_pathlib@main/')"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "gpath = UPath('github://Quansight:universal_pathlib@main/')"
+                "ghpath = UPath('github://fsspec:universal_pathlib@main/')\n",
+                "ghpath"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "with a UPath object instanciated, you can now interact with the paths with the usual `pathlib.Path` API"
+                "With a `UPath` object instantiated, you can now interact with the paths with the usual `pathlib.Path` API."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "autoscroll": false,
@@ -165,38 +231,30 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "github://Quansight:universal_pathlib@main/.flake8\n",
-                        "github://Quansight:universal_pathlib@main/.github\n",
-                        "github://Quansight:universal_pathlib@main/.gitignore\n",
-                        "github://Quansight:universal_pathlib@main/LICENSE\n",
-                        "github://Quansight:universal_pathlib@main/README.md\n",
-                        "github://Quansight:universal_pathlib@main/environment.yml\n",
-                        "github://Quansight:universal_pathlib@main/notebooks\n",
-                        "github://Quansight:universal_pathlib@main/noxfile.py\n",
-                        "github://Quansight:universal_pathlib@main/pyproject.toml\n",
-                        "github://Quansight:universal_pathlib@main/setup.py\n",
-                        "github://Quansight:universal_pathlib@main/upath\n"
+                        "github://fsspec:universal_pathlib@main/.flake8\n"
                     ]
                 }
             ],
             "source": [
-                "for p in gpath.iterdir():\n",
-                "    print(p)"
+                "for p in ghpath.iterdir():\n",
+                "    print(p)\n",
+                "    break"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The `glob` method is also available. Note the syntax here is as defined in `fsspec`, rather than that of pathlib. "
+                "All the standard path methods and attributes of [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html#pathlib.Path) are available too:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "autoscroll": false,
@@ -204,44 +262,35 @@
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "github://Quansight:universal_pathlib@main/noxfile.py\n",
-                        "github://Quansight:universal_pathlib@main/setup.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/__init__.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/core.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/errors.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/implementations/__init__.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/implementations/http.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/registry.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/tests/__init__.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/tests/conftest.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/tests/implementations/__init__.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/tests/implementations/test_http.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/tests/test_core.py\n",
-                        "github://Quansight:universal_pathlib@main/upath/universal_path.py\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "UPath('github://fsspec:universal_pathlib@main/README.md')"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "for p in gpath.glob('**.py'):\n",
-                "    print(p)"
+                "readme_path = ghpath / \"README.md\"\n",
+                "readme_path"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "All the standard path methods and attributes of `pathlib.Path` are available too:"
+                "To get the full path as a string use:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "autoscroll": false,
@@ -251,32 +300,32 @@
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "UniversalPath('github://Quansight:universal_pathlib@main/README.md')"
+                            "'github://fsspec:universal_pathlib@main/README.md'"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "readme = gpath.joinpath('README.md')\n",
-                "readme"
+                "str(readme_path)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To get the full path as a string use:"
+                "You can also use the path attribute to get just the path:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "autoscroll": false,
@@ -286,31 +335,25 @@
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'github://Quansight:universal_pathlib@main/README.md'"
+                            "'/README.md'"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "str(readme)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "You can also use the path attribute to get just the path:"
+                "# path attribute added\n",
+                "readme_path.path"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "autoscroll": false,
@@ -320,25 +363,24 @@
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'/README.md'"
+                            "('README.md', 'README', '.md')"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# path attribute added\n",
-                "readme.path"
+                "readme_path.name, readme_path.stem, readme_path.suffix"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "autoscroll": false,
@@ -348,51 +390,40 @@
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'README.md'"
+                            "'# Universal Pathlib'"
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "readme.name"
+                "readme_path.read_text().splitlines()[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "autoscroll": false,
                 "ein.hycell": false,
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "'README'"
-                        ]
-                    },
-                    "execution_count": 12,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "readme.stem"
+                "s3path = UPath(\"s3://spacenet-dataset\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "autoscroll": false,
@@ -400,180 +431,217 @@
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "'.md'"
-                        ]
-                    },
-                    "execution_count": 13,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "s3://spacenet-dataset/LICENSE.md\n"
+                    ]
                 }
             ],
             "source": [
-                "readme.suffix"
+                "for p in s3path.iterdir():\n",
+                "    if p.is_file():\n",
+                "        print(p)\n",
+                "        break"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "You can chain paths with the `/` operator and any methods."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "metadata": {
-                "autoscroll": false,
-                "ein.hycell": false,
-                "ein.tags": "worksheet-0",
-                "slideshow": {
-                    "slide_type": "-"
-                }
-            },
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "readme.exists()"
+                "(s3path / \"LICENSE.md\").exists()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "metadata": {
-                "autoscroll": false,
-                "ein.hycell": false,
-                "ein.tags": "worksheet-0",
-                "slideshow": {
-                    "slide_type": "-"
-                }
-            },
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Universal Pathlib\n",
-                        "==================\n",
-                        "\n",
-                        "Universal Pathlib is a python library that aims to extend Python's built-in [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) api to use a variety of backend filesystems using [`fsspec`](https://filesystem-spec.readthedocs.io/en/latest/intro.html)\n",
-                        "\n",
-                        "Installation\n",
-                        "-------------\n",
-                        "\n",
-                        "Universal Pathlib can be installs from conda-forge via:\n",
-                        "\n",
-                        "```bash\n",
-                        "conda install -c conda-forge universal_pathlib\n",
-                        "```\n",
-                        "\n",
-                        "\n"
+                        "The \"SpaceNet Dataset\"\n"
                     ]
                 }
             ],
             "source": [
-                "print(readme.read_text())"
+                "with (s3path / \"LICENSE.md\").open(\"rt\", encoding=\"utf-8\") as f:\n",
+                "    print(f.read(22))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Some filesystems may require extra imports to use."
+                "The `glob` method is also available for most filesystems. Note the syntax here is as detailed in `fsspec` [docs](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.glob), rather than that of `pathlib`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "metadata": {
-                "autoscroll": false,
-                "ein.hycell": false,
-                "ein.tags": "worksheet-0",
-                "slideshow": {
-                    "slide_type": "-"
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "s3://spacenet-dataset/AOIs/AOI_3_Paris/MS/16FEB29111913-M2AS_R01C1-055649178040_01_P001.TIF\n"
+                    ]
                 }
-            },
-            "outputs": [],
+            ],
             "source": [
-                "import s3fs"
+                "for p in (s3path / \"AOIs\" / \"AOI_3_Paris\").glob(\"**.TIF\"):\n",
+                "    print(p)\n",
+                "    break"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 17,
-            "metadata": {
-                "autoscroll": false,
-                "ein.hycell": false,
-                "ein.tags": "worksheet-0",
-                "slideshow": {
-                    "slide_type": "-"
-                }
-            },
-            "outputs": [],
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "s3path = UPath(\"s3:/spacenet-dataset\")"
+                "### Works with fsspec filesystems\n",
+                "\n",
+                "Some filesystems may require additional packages to be installed.\n",
+                "\n",
+                "Check out some of the known implementations:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
-            "metadata": {
-                "autoscroll": false,
-                "ein.hycell": false,
-                "ein.tags": "worksheet-0",
-                "slideshow": {
-                    "slide_type": "-"
-                }
-            },
+            "execution_count": 17,
+            "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "s3:/spacenet-dataset/\n",
-                        "s3:/spacenet-dataset/AOIs\n",
-                        "s3:/spacenet-dataset/Hosted-Datasets\n",
-                        "s3:/spacenet-dataset/SpaceNet_Off-Nadir_Dataset\n",
-                        "s3:/spacenet-dataset/spacenet-model-weights\n",
-                        "s3:/spacenet-dataset/spacenet-stac\n",
-                        "s3:/spacenet-dataset/spacenet\n"
-                    ]
+                    "data": {
+                        "text/markdown": [
+                            "| Name | Class |\n",
+                            "| --- | --- |\n",
+                            "| abfs | adlfs.AzureBlobFileSystem |\n",
+                            "| abfss | adlfs.AzureBlobFileSystem |\n",
+                            "| adl | adlfs.AzureDatalakeFileSystem |\n",
+                            "| arrow_hdfs | fsspec.implementations.arrow.HadoopFileSystem |\n",
+                            "| asynclocal | morefs.asyn_local.AsyncLocalFileSystem |\n",
+                            "| az | adlfs.AzureBlobFileSystem |\n",
+                            "| blockcache | fsspec.implementations.cached.CachingFileSystem |\n",
+                            "| cached | fsspec.implementations.cached.CachingFileSystem |\n",
+                            "| dask | fsspec.implementations.dask.DaskWorkerFileSystem |\n",
+                            "| dbfs | fsspec.implementations.dbfs.DatabricksFileSystem |\n",
+                            "| dir | fsspec.implementations.dirfs.DirFileSystem |\n",
+                            "| dropbox | dropboxdrivefs.DropboxDriveFileSystem |\n",
+                            "| dvc | dvc.api.DVCFileSystem |\n",
+                            "| file | fsspec.implementations.local.LocalFileSystem |\n",
+                            "| filecache | fsspec.implementations.cached.WholeFileCacheFileSystem |\n",
+                            "| ftp | fsspec.implementations.ftp.FTPFileSystem |\n",
+                            "| gcs | gcsfs.GCSFileSystem |\n",
+                            "| gdrive | gdrivefs.GoogleDriveFileSystem |\n",
+                            "| generic | fsspec.generic.GenericFileSystem |\n",
+                            "| git | fsspec.implementations.git.GitFileSystem |\n",
+                            "| github | fsspec.implementations.github.GithubFileSystem |\n",
+                            "| gs | gcsfs.GCSFileSystem |\n",
+                            "| hdfs | fsspec.implementations.arrow.HadoopFileSystem |\n",
+                            "| hf | huggingface_hub.HfFileSystem |\n",
+                            "| http | fsspec.implementations.http.HTTPFileSystem |\n",
+                            "| https | fsspec.implementations.http.HTTPFileSystem |\n",
+                            "| jlab | fsspec.implementations.jupyter.JupyterFileSystem |\n",
+                            "| jupyter | fsspec.implementations.jupyter.JupyterFileSystem |\n",
+                            "| libarchive | fsspec.implementations.libarchive.LibArchiveFileSystem |\n",
+                            "| memory | fsspec.implementations.memory.MemoryFileSystem |\n",
+                            "| oci | ocifs.OCIFileSystem |\n",
+                            "| oss | ossfs.OSSFileSystem |\n",
+                            "| reference | fsspec.implementations.reference.ReferenceFileSystem |\n",
+                            "| root | fsspec_xrootd.XRootDFileSystem |\n",
+                            "| s3 | s3fs.S3FileSystem |\n",
+                            "| s3a | s3fs.S3FileSystem |\n",
+                            "| sftp | fsspec.implementations.sftp.SFTPFileSystem |\n",
+                            "| simplecache | fsspec.implementations.cached.SimpleCacheFileSystem |\n",
+                            "| smb | fsspec.implementations.smb.SMBFileSystem |\n",
+                            "| ssh | fsspec.implementations.sftp.SFTPFileSystem |\n",
+                            "| tar | fsspec.implementations.tar.TarFileSystem |\n",
+                            "| wandb | wandbfs.WandbFS |\n",
+                            "| webdav | webdav4.fsspec.WebdavFileSystem |\n",
+                            "| webhdfs | fsspec.implementations.webhdfs.WebHDFS |\n",
+                            "| zip | fsspec.implementations.zip.ZipFileSystem |"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.Markdown object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "for p in s3path.iterdir():\n",
-                "    print(p)"
+                "from fsspec.registry import known_implementations\n",
+                "from IPython.display import Markdown, display\n",
+                "\n",
+                "known = [\n",
+                "    f\"| {name} | {d['class']} |\" for name, d in sorted(known_implementations.items())\n",
+                "]\n",
+                "known = \"\\n\".join([\"| Name | Class |\\n| --- | --- |\", *known])\n",
+                "display(Markdown(known))"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "fsspec",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.7"
+            "version": "3.10.10"
         },
-        "name": "Untitled.ipynb"
+        "name": "Untitled.ipynb",
+        "vscode": {
+            "interpreter": {
+                "hash": "d4d4510d3a243cfb62b62dec561eb2191aad85ef77736fec7cfe79076e15c84c"
+            }
+        }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `universal_pathlib-0.0.9/upath/implementations/s3.py` & `universal_pathlib-0.1.0/upath/implementations/hdfs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
-import re
+from __future__ import annotations
 
-from upath.universal_path import _FSSpecAccessor, UniversalPath
+import upath.core
 
 
-class _S3Accessor(_FSSpecAccessor):
+class _HDFSAccessor(upath.core._FSSpecAccessor):
     def __init__(self, parsed_url, *args, **kwargs):
         super().__init__(parsed_url, *args, **kwargs)
+        self._fs.root_marker = "/"
 
-    def _format_path(self, s):
-        s = os.path.join(self._url.netloc, s.lstrip("/"))
-        return s
-
-
-class S3Path(UniversalPath):
-    _default_accessor = _S3Accessor
-
-    def _sub_path(self, name):
-        """s3fs returns path as `{bucket}/<path>` with listdir
-        and glob, so here we can add the netloc to the sub string
-        so it gets subbed out as well
-        """
-        sp = self.path
-        subed = re.sub(f"^{self._url.netloc}/({sp}|{sp[1:]})/?", "", name)
-        return subed
+    def touch(self, path, **kwargs):
+        kwargs.pop("truncate", None)
+        super().touch(path, **kwargs)
+
+    def mkdir(self, path, create_parents=True, **kwargs):
+        pth = self._format_path(path)
+        if create_parents:
+            return self._fs.makedirs(pth, **kwargs)
+        else:
+            if not kwargs.get("exist_ok", False) and self._fs.exists(pth):
+                raise FileExistsError(pth)
+            return self._fs.mkdir(pth, create_parents=create_parents, **kwargs)
+
+
+class HDFSPath(upath.core.UPath):
+    _default_accessor = _HDFSAccessor
```

### Comparing `universal_pathlib-0.0.9/upath/tests/implementations/test_hdfs.py` & `universal_pathlib-0.1.0/upath/tests/implementations/test_hdfs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """see upath/tests/conftest.py for fixtures
 """
 import pytest  # noqa: F401
 
 from upath import UPath
 from upath.implementations.hdfs import HDFSPath
-from upath.tests.cases import BaseTests
+
+from ..cases import BaseTests
 
 
 @pytest.mark.hdfs
 class TestUPathHDFS(BaseTests):
     @pytest.fixture(autouse=True)
     def path(self, local_testdir, hdfs):
         host, user, port = hdfs
```

