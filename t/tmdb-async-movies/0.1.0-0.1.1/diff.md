# Comparing `tmp/tmdb_async_movies-0.1.0.tar.gz` & `tmp/tmdb_async_movies-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmdb_async_movies-0.1.0.tar", max compression
+gzip compressed data, was "tmdb_async_movies-0.1.1.tar", max compression
```

## Comparing `tmdb_async_movies-0.1.0.tar` & `tmdb_async_movies-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-01 21:18:47.615758 tmdb_async_movies-0.1.0/LICENSE
--rw-r--r--   0        0        0     3505 2023-04-01 21:18:47.615758 tmdb_async_movies-0.1.0/README.md
--rw-r--r--   0        0        0     2083 2023-04-01 21:19:03.859867 tmdb_async_movies-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-01 21:18:47.619758 tmdb_async_movies-0.1.0/src/tmdb_async_movies/__init__.py
--rw-r--r--   0        0        0     3883 2023-04-01 21:18:47.619758 tmdb_async_movies-0.1.0/src/tmdb_async_movies/cli.py
--rw-r--r--   0        0        0    21707 2023-04-01 21:18:47.619758 tmdb_async_movies-0.1.0/src/tmdb_async_movies/main.py
--rw-r--r--   0        0        0        0 2023-04-01 21:18:47.619758 tmdb_async_movies-0.1.0/src/tmdb_async_movies/py.typed
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 tmdb_async_movies-0.1.0/setup.py
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 tmdb_async_movies-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-03 20:25:10.733086 tmdb_async_movies-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3487 2023-08-03 20:25:10.733086 tmdb_async_movies-0.1.1/README.md
+-rw-r--r--   0        0        0     2308 2023-08-03 20:25:28.769362 tmdb_async_movies-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-08-03 20:25:10.737086 tmdb_async_movies-0.1.1/src/tmdb_async_movies/__init__.py
+-rw-r--r--   0        0        0     3883 2023-08-03 20:25:10.737086 tmdb_async_movies-0.1.1/src/tmdb_async_movies/cli.py
+-rw-r--r--   0        0        0    21707 2023-08-03 20:25:10.737086 tmdb_async_movies-0.1.1/src/tmdb_async_movies/main.py
+-rw-r--r--   0        0        0        0 2023-08-03 20:25:10.737086 tmdb_async_movies-0.1.1/src/tmdb_async_movies/py.typed
+-rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 tmdb_async_movies-0.1.1/PKG-INFO
```

### Comparing `tmdb_async_movies-0.1.0/LICENSE` & `tmdb_async_movies-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdb_async_movies-0.1.0/README.md` & `tmdb_async_movies-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 
 You can install _tmdb-async-movies_ via [pip] from [PyPI]:
 
 ```console
 $ pip install tmdb-async-movies
 ```
 
-## Usage
+## Documentation
 
-Please see the [Command-line Reference] for details.
+Please see the [documentation] for details.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
@@ -91,8 +91,8 @@
 [file an issue]: https://github.com/tilschuenemann/tmdb-async-movies/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [license]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/LICENSE
 [contributor guide]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/CONTRIBUTING.md
-[command-line reference]: https://tmdb-async-movies.readthedocs.io/en/latest/cli.html
+[documentation]: https://tmdb-async-movies.readthedocs.io/en/latest/
```

### Comparing `tmdb_async_movies-0.1.0/pyproject.toml` & `tmdb_async_movies-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "tmdb_async_movies"
-version = "0.1.0"
-description = "tmdb_async_movies"
+version = "0.1.1"
+description = "tmdb-async-movies is an asynchronous utility for fetching bulk movie data from TMDB using movie title and optionally release year."
 authors = ["Til Schünemann <til.schuenemann@mailbox.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tilschuenemann/tmdb-async-movies"
 repository = "https://github.com/tilschuenemann/tmdb-async-movies"
 documentation = "https://tmdb-async-movies.readthedocs.io"
 classifiers = [
     "Development Status :: 3 - Alpha",
 ]
+keywords = ["tmdb","api","movies","bulk","async","tmdb-api","tmdb-movie","movie","aiohttp","tmdb-async-movies"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/tilschuenemann/tmdb-async-movies/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = ">=8.0.1"
```

### Comparing `tmdb_async_movies-0.1.0/src/tmdb_async_movies/cli.py` & `tmdb_async_movies-0.1.1/src/tmdb_async_movies/cli.py`

 * *Files identical despite different names*

### Comparing `tmdb_async_movies-0.1.0/src/tmdb_async_movies/main.py` & `tmdb_async_movies-0.1.1/src/tmdb_async_movies/main.py`

 * *Files identical despite different names*

### Comparing `tmdb_async_movies-0.1.0/setup.py` & `tmdb_async_movies-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tmdb-async-movies
+Version: 0.1.1
+Summary: tmdb-async-movies is an asynchronous utility for fetching bulk movie data from TMDB using movie title and optionally release year.
+Home-page: https://github.com/tilschuenemann/tmdb-async-movies
+License: MIT
+Keywords: tmdb,api,movies,bulk,async,tmdb-api,tmdb-movie,movie,aiohttp,tmdb-async-movies
+Author: Til Schünemann
+Author-email: til.schuenemann@mailbox.org
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Requires-Dist: pathlib (>=1.0.1,<2.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Changelog, https://github.com/tilschuenemann/tmdb-async-movies/releases
+Project-URL: Documentation, https://tmdb-async-movies.readthedocs.io
+Project-URL: Repository, https://github.com/tilschuenemann/tmdb-async-movies
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# tmdb-async-movies
 
-packages = \
-['tmdb_async_movies']
+[![PyPI](https://img.shields.io/pypi/v/tmdb-async-movies.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/tmdb-async-movies.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/tmdb-async-movies)][python version]
+[![License](https://img.shields.io/pypi/l/tmdb-async-movies)][license]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp-retry>=2.8.3,<3.0.0',
- 'aiohttp>=3.8.3,<4.0.0',
- 'click>=8.0.1',
- 'numpy>=1.23.5,<2.0.0',
- 'pandas>=1.5.1,<2.0.0',
- 'pathlib>=1.0.1,<2.0.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['tmdbasyncmovies = tmdb_async_movies.cli:tmdbasyncmovies']}
-
-setup_kwargs = {
-    'name': 'tmdb-async-movies',
-    'version': '0.1.0',
-    'description': 'tmdb_async_movies',
-    'long_description': '# tmdb-async-movies\n\n[![PyPI](https://img.shields.io/pypi/v/tmdb-async-movies.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/tmdb-async-movies.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/tmdb-async-movies)][python version]\n[![License](https://img.shields.io/pypi/l/tmdb-async-movies)][license]\n\n[![Read the documentation at https://tmdb-async-movies.readthedocs.io/](https://img.shields.io/readthedocs/tmdb-async-movies/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/tilschuenemann/tmdb-async-movies/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/tilschuenemann/tmdb-async-movies/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/tmdb-async-movies/\n[status]: https://pypi.org/project/tmdb-async-movies/\n[python version]: https://pypi.org/project/tmdb-async-movies\n[read the docs]: https://tmdb-async-movies.readthedocs.io/\n[tests]: https://github.com/tilschuenemann/tmdb-async-movies/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/tilschuenemann/tmdb-async-movies\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n`tmdb-async-movies` is an asynchronous utility for fetching bulk movie data from [TMDB](https://www.themoviedb.org/) using movie title and optionally release year.\n\n- Designed for bulk usage: Pipe in a list of queries and get results immediately.\n- Blazing fast: Asynchronous calls enable you to get metadata from hundreds of movies in a couple of seconds.\n- Typed: Metadata dataframes are strictly cast so you don\'t have to do it yourself.\n- Hackable: It\'s a small project with ~500 LOC.\n- Accessible: It has both a Python API and a CLI.\n\n## Requirements\n\nYou\'ll need to have a TMDB API key in order to make API requests.\n\nDefault environment variable:\n\n```bash\n$ export TMDB_API_KEY="your_api_key_here"\n```\n\nPython:\n\n```python\nfrom tmdb_async_movies.main import TmdbAsyncMovies\nt = TmdbAsyncMovies(tmdb_api_key="your_api_key_here")\n```\n\nCLI:\n\n```bash\ntmdb-async-movies -t "your_api_key_here" from_input "1999 The Matrix"\n```\n\n## Installation\n\nYou can install _tmdb-async-movies_ via [pip] from [PyPI]:\n\n```console\n$ pip install tmdb-async-movies\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_tmdb_async_movies_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/tilschuenemann/tmdb-async-movies/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/LICENSE\n[contributor guide]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/CONTRIBUTING.md\n[command-line reference]: https://tmdb-async-movies.readthedocs.io/en/latest/cli.html\n',
-    'author': 'Til Schünemann',
-    'author_email': 'til.schuenemann@mailbox.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tilschuenemann/tmdb-async-movies',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+[![Read the documentation at https://tmdb-async-movies.readthedocs.io/](https://img.shields.io/readthedocs/tmdb-async-movies/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/tilschuenemann/tmdb-async-movies/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/tilschuenemann/tmdb-async-movies/branch/main/graph/badge.svg)][codecov]
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/tmdb-async-movies/
+[status]: https://pypi.org/project/tmdb-async-movies/
+[python version]: https://pypi.org/project/tmdb-async-movies
+[read the docs]: https://tmdb-async-movies.readthedocs.io/
+[tests]: https://github.com/tilschuenemann/tmdb-async-movies/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/tilschuenemann/tmdb-async-movies
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Features
+
+`tmdb-async-movies` is an asynchronous utility for fetching bulk movie data from [TMDB](https://www.themoviedb.org/) using movie title and optionally release year.
+
+- Designed for bulk usage: Pipe in a list of queries and get results immediately.
+- Blazing fast: Asynchronous calls enable you to get metadata from hundreds of movies in a couple of seconds.
+- Typed: Metadata dataframes are strictly cast so you don't have to do it yourself.
+- Hackable: It's a small project with ~500 LOC.
+- Accessible: It has both a Python API and a CLI.
+
+## Requirements
+
+You'll need to have a TMDB API key in order to make API requests.
+
+Default environment variable:
+
+```bash
+$ export TMDB_API_KEY="your_api_key_here"
+```
+
+Python:
+
+```python
+from tmdb_async_movies.main import TmdbAsyncMovies
+t = TmdbAsyncMovies(tmdb_api_key="your_api_key_here")
+```
+
+CLI:
+
+```bash
+tmdb-async-movies -t "your_api_key_here" from_input "1999 The Matrix"
+```
+
+## Installation
+
+You can install _tmdb-async-movies_ via [pip] from [PyPI]:
+
+```console
+$ pip install tmdb-async-movies
+```
+
+## Documentation
+
+Please see the [documentation] for details.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_tmdb_async_movies_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/tilschuenemann/tmdb-async-movies/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/LICENSE
+[contributor guide]: https://github.com/tilschuenemann/tmdb-async-movies/blob/main/CONTRIBUTING.md
+[documentation]: https://tmdb-async-movies.readthedocs.io/en/latest/
 
-setup(**setup_kwargs)
```

