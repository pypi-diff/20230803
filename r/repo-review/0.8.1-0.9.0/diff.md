# Comparing `tmp/repo_review-0.8.1.tar.gz` & `tmp/repo_review-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jul 13 17:42:45 2023, max compression
+gzip compressed data, last modified: Thu Aug  3 20:17:05 2023, max compression
```

## Comparing `repo_review-0.8.1.tar` & `repo_review-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0      125 2023-07-13 17:42:45.000000 repo_review-0.8.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-07-13 17:42:45.000000 repo_review-0.8.1/.gitattributes
--rw-r--r--   0        0        0     2045 2023-07-13 17:42:45.000000 repo_review-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-07-13 17:42:45.000000 repo_review-0.8.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      400 2023-07-13 17:42:45.000000 repo_review-0.8.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1216 2023-07-13 17:42:45.000000 repo_review-0.8.1/action.yml
--rw-r--r--   0        0        0     3242 2023-07-13 17:42:45.000000 repo_review-0.8.1/noxfile.py
--rw-r--r--   0        0        0      359 2023-07-13 17:42:45.000000 repo_review-0.8.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2527 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2356 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/.nojekyll
--rw-r--r--   0        0        0      217 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/changelog.md
--rw-r--r--   0        0        0     5910 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/checks.md
--rw-r--r--   0        0        0      990 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/cli.md
--rw-r--r--   0        0        0     1009 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/families.md
--rw-r--r--   0        0        0     2243 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/fixtures.md
--rw-r--r--   0        0        0     1915 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/index.html
--rw-r--r--   0        0        0      253 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/index.md
--rw-r--r--   0        0        0     2248 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/intro.md
--rw-r--r--   0        0        0     2746 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/plugins.md
--rw-r--r--   0        0        0     2821 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/programmatic.md
--rw-r--r--   0        0        0    10563 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/webapp.md
--rw-r--r--   0        0        0     1033 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/api/repo_review.rst
--rw-r--r--   0        0        0      230 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/__init__.py
--rw-r--r--   0        0        0     7626 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/__main__.py
--rw-r--r--   0        0        0      160 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     3576 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/checks.py
--rw-r--r--   0        0        0     1591 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/families.py
--rw-r--r--   0        0        0     3607 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     6010 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2315 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/html.py
--rw-r--r--   0        0        0     7393 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_cmd.py
--rw-r--r--   0        0        0     2429 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_self.py
--rw-r--r--   0        0        0     4029 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-07-13 17:42:45.000000 repo_review-0.8.1/.gitignore
--rw-r--r--   0        0        0     1525 2023-07-13 17:42:45.000000 repo_review-0.8.1/LICENSE
--rw-r--r--   0        0        0     6123 2023-07-13 17:42:45.000000 repo_review-0.8.1/README.md
--rw-r--r--   0        0        0     5359 2023-07-13 17:42:45.000000 repo_review-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8397 2023-07-13 17:42:45.000000 repo_review-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-03 20:17:05.000000 repo_review-0.9.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-08-03 20:17:05.000000 repo_review-0.9.0/.gitattributes
+-rw-r--r--   0        0        0     2045 2023-08-03 20:17:05.000000 repo_review-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-08-03 20:17:05.000000 repo_review-0.9.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      400 2023-08-03 20:17:05.000000 repo_review-0.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1216 2023-08-03 20:17:05.000000 repo_review-0.9.0/action.yml
+-rw-r--r--   0        0        0     3219 2023-08-03 20:17:05.000000 repo_review-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      359 2023-08-03 20:17:05.000000 repo_review-0.9.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2527 2023-08-03 20:17:05.000000 repo_review-0.9.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-08-03 20:17:05.000000 repo_review-0.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-08-03 20:17:05.000000 repo_review-0.9.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-08-03 20:17:05.000000 repo_review-0.9.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-08-03 20:17:05.000000 repo_review-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/.nojekyll
+-rw-r--r--   0        0        0      217 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0     6083 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/cli.md
+-rw-r--r--   0        0        0     2295 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     1445 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/families.md
+-rw-r--r--   0        0        0     2474 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/fixtures.md
+-rw-r--r--   0        0        0     1915 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/index.html
+-rw-r--r--   0        0        0      253 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/index.md
+-rw-r--r--   0        0        0     2248 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/intro.md
+-rw-r--r--   0        0        0     2746 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/plugins.md
+-rw-r--r--   0        0        0     2821 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/programmatic.md
+-rw-r--r--   0        0        0    11110 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/webapp.md
+-rw-r--r--   0        0        0     1033 2023-08-03 20:17:05.000000 repo_review-0.9.0/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     8157 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      160 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     3625 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/checks.py
+-rw-r--r--   0        0        0     2389 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/families.py
+-rw-r--r--   0        0        0     3607 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2449 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/html.py
+-rw-r--r--   0        0        0     7826 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-03 20:17:05.000000 repo_review-0.9.0/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4400 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_cmd.py
+-rw-r--r--   0        0        0      452 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_families.py
+-rw-r--r--   0        0        0     2408 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_package.py
+-rw-r--r--   0        0        0     2712 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_self.py
+-rw-r--r--   0        0        0     4309 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      424 2023-08-03 20:17:05.000000 repo_review-0.9.0/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2095 2023-08-03 20:17:05.000000 repo_review-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1525 2023-08-03 20:17:05.000000 repo_review-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6123 2023-08-03 20:17:05.000000 repo_review-0.9.0/README.md
+-rw-r--r--   0        0        0     5193 2023-08-03 20:17:05.000000 repo_review-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8420 2023-08-03 20:17:05.000000 repo_review-0.9.0/PKG-INFO
```

### Comparing `repo_review-0.8.1/.pre-commit-config.yaml` & `repo_review-0.9.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.15.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.7.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
+    rev: "v0.0.281"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
@@ -50,15 +50,15 @@
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
         files: (src|web|tests)
         args: []
         additional_dependencies:
-          - click==8.1.3
+          - click>=8.1.5
           - markdown-it-py
           - pytest
           - rich
           - tomli
           - types-PyYAML
 
   - repo: https://github.com/codespell-project/codespell
```

### Comparing `repo_review-0.8.1/action.yml` & `repo_review-0.9.0/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/noxfile.py` & `repo_review-0.9.0/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,38 +88,38 @@
         "-b", dest="builder", default="html", help="Build target (default: html)"
     )
     args, posargs = parser.parse_known_args(session.posargs)
 
     if args.builder != "html" and args.serve:
         session.error("Must not specify non-HTML builder with --serve")
 
-    session.install("-e.[docs]")
+    extra_installs = ["sphinx-autobuild"] if args.serve else []
+
+    session.install("-e.[docs]", *extra_installs)
     session.chdir("docs")
 
     if args.builder == "linkcheck":
         session.run(
             "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
         )
         return
 
-    session.run(
-        "sphinx-build",
+    shared_args = (
         "-n",  # nitpicky mode
-        "--keep-going",  # show all errors
         "-T",  # full tracebacks
-        "-b",
-        args.builder,
+        f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
     if args.serve:
-        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
-        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+        session.run("sphinx-autobuild", *shared_args)
+    else:
+        session.run("sphinx-build", "--keep-going", *shared_args)
 
 
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
     Build (regenerate) API docs.
     """
```

### Comparing `repo_review-0.8.1/.github/CONTRIBUTING.md` & `repo_review-0.9.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/.github/matchers/pylint.json` & `repo_review-0.9.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/.github/workflows/cd.yml` & `repo_review-0.9.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/.github/workflows/ci.yml` & `repo_review-0.9.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -102,8 +102,8 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Run repo-review action
         uses: ./
         with:
-          plugins: sp-repo-review==2023.06.01
+          plugins: sp-repo-review==2023.07.13
```

### Comparing `repo_review-0.8.1/docs/checks.md` & `repo_review-0.9.0/docs/checks.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 the check passes, or `False` if the check fails. If you want a dynamic error
 explanation instead of the `check()` docstring, you can return a non-empty
 string from the check instead of `False`. Returning `None` makes a check
 "skipped". Docstrings/error messages can access their own object with `{self}`
 and check name with `{name}` (these are processed with `.format()`, so escape `{}`
 as `{{}}`). The error message is in markdown format.
 
+```{versionchanged} 0.9
+The string return value is not processed via `.format`. You can use `self` and
+the `name` fixture directly when constructing the return string.
+```
+
 If the check named in `requires` does not pass, the check is skipped.
 
 A suggested convention for easily writing checks is as follows:
 
 ```python
 class General:
     family = "general"
```

### Comparing `repo_review-0.8.1/docs/cli.md` & `repo_review-0.9.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/docs/families.md` & `repo_review-0.9.0/docs/families.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 # Families
 
-Families are a set of simple strings that group together similar checks. You can provide a nicer user experience, however, by adding a mapping of information for repo-review to improve the ordering and display of families.
+Families are a set of simple strings that group together similar checks. You can
+provide a nicer user experience, however, by adding a mapping of information for
+repo-review to improve the ordering and display of families.
 
 You can construct a dict with the following optional keys:
 
 ```python
 class Family(typing.TypedDict, total=False):
     name: str  # defaults to key
     order: int  # defaults to 0
+    description: str  # defaults to empty
+```
+
+The `name` will be shown instead if given. The families will be sorted by
+`order` then key. And a `description` will be shown after the name if provided;
+it is expected to be in markdown format.
+
+```{versionadded} 0.9
+Descriptions are now supported.
 ```
 
 Then you can provide a function that maps family strings to this extra information:
 
 ```python
 def get_familes() -> dict[str, Family]:
     return {
@@ -22,21 +33,20 @@
         "pyproject": Family(
             name="PyProject",
             order=-2,
         ),
     }
 ```
 
+```{versionchanged} 0.9
+You can request fixtures for this function, like all the other collection functions.
+This allows dynamic descriptions based on repo contents.
+```
+
 And finally, you register this function as an entry-point:
 
 ```toml
 [project.entry-points."repo_review.families"]
 families = "my_plugin_package.my_family_module:get_families"
 ```
 
 The entry-point name doesn't matter.
-
-```{admonition} Fixtures
-Unlike almost all other parts of the API, the family function does not support
-fixtures. This could be added if there is a need, but usually not needed - if a
-check is not present from a family, the family will not be displayed.
-```
```

### Comparing `repo_review-0.8.1/docs/fixtures.md` & `repo_review-0.9.0/docs/fixtures.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 # Fixtures
 
-Like pytest fixtures, fixtures in repo-review are requested by name. There are four built-in fixtures:
+Like pytest fixtures, fixtures in repo-review are requested by name. There are five built-in fixtures:
 
 - `root`: {class}`~importlib.resources.abc.Traversable` - The repository path. All checks or fixtures that depend on the root of the repository should use this.
 - `package`: `~importlib.resources.abc.Traversable` - The path to the package directory. This is the same as `root` unless `--package-dir` is passed.
+- `name`: `str` - The name of the current check. (Special fixture only provided for checks, not collection functions.)
 - {func}`~repo_review.fixtures.pyproject`: `dict[str, Any]` - The `pyproject.toml` in the package if it exists, an empty dict otherwise.
-- {func}`~repo_review.fixtures.list_all`: `bool` - returns True if repo-review is just trying to collect all checks to list them.
+- {func}`~repo_review.fixtures.list_all`: `bool` - Returns `True`` if repo-review is just trying to collect all checks to list them.
+
+```{versionadded} 0.8
+The `list_all` fixture.
+```
+
+```{versionadded} 0.9
+The `name` fixture for checks.
+```
 
 Repo-review doesn't necessarily assume any form or language for your repository,
 but since it already looks for configuration in `pyproject.toml`, this fixture
 is provided.
 
 ## Writing a fixture
```

### Comparing `repo_review-0.8.1/docs/index.html` & `repo_review-0.9.0/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp-repo-review==2023.06.29", "repo-review==0.8.0"]}
+          deps={["sp-repo-review==2023.07.13", "repo-review==0.9.0"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.8.1/docs/intro.md` & `repo_review-0.9.0/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/docs/plugins.md` & `repo_review-0.9.0/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/docs/programmatic.md` & `repo_review-0.9.0/docs/programmatic.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/docs/webapp.js` & `repo_review-0.9.0/docs/webapp.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -204,17 +204,27 @@
             li key = {
                 `section-${key}`
             } >
             <
             ul >
             <
             MaterialUI.ListSubheader > {
-                props.families[key]
+                props.families[key].name
             } <
             /MaterialUI.ListSubheader> {
+                props.families[key].description && ( <
+                    MaterialUI.ListItem >
+                    <
+                    span dangerouslySetInnerHTML = {
+                        props.families[key].description
+                    }
+                    /> <
+                    /MaterialUI.ListItem>
+                )
+            } {
                 results_components
             } <
             /ul> <
             /li>,
         );
     }
 
@@ -313,21 +323,27 @@
         });
         const state = this.state;
         this.pyodide_promise.then((pyodide) => {
             var families_checks;
             try {
                 families_checks = pyodide.runPython(`
           from pyodide.http import open_url
-          from repo_review.processor import process
+          from repo_review.processor import process, md_as_html
           from repo_review.ghpath import GHPath
 
           GHPath.open_url = staticmethod(open_url)
 
           package = GHPath(repo="${state.repo}", branch="${state.branch}")
-          process(package)
+          result = process(package)
+
+          for v in result[0].values():
+              if v.get("description"):
+                  v["description"] = md_as_html(v["description"])
+
+          result
           `);
             } catch (e) {
                 if (e.message.includes("KeyError: 'tree'")) {
                     this.setState({
                         msg: DEFAULT_MSG,
                         progress: false,
                         err_msg: "Invalid repository or branch. Please try again.",
@@ -343,16 +359,20 @@
 
             const families_dict = families_checks.get(0);
             const results_list = families_checks.get(1);
 
             const results = {};
             const families = {};
             for (const val of families_dict) {
+                const descr = families_dict.get(val).get("description");
                 results[val] = [];
-                families[val] = families_dict.get(val).get("name");
+                families[val] = {
+                    name: families_dict.get(val).get("name").toString(),
+                    description: descr && descr.toString(),
+                };
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
@@ -408,15 +428,15 @@
             helperText = "e.g. scikit-hep/hist"
             variant = "outlined"
             autoFocus = {
                 true
             }
             onKeyDown = {
                 (e) => {
-                    if (event.keyCode === 13)
+                    if (e.keyCode === 13)
                         document.getElementById("branch-select").focus();
                 }
             }
             onInput = {
                 (e) => this.setState({
                     repo: e.target.value
                 })
@@ -435,15 +455,15 @@
                 common_branches
             }
             freeSolo = {
                 true
             }
             onKeyDown = {
                 (e) => {
-                    if (event.keyCode === 13) this.handleCompute();
+                    if (e.keyCode === 13) this.handleCompute();
                 }
             }
             onInputChange = {
                 (e, value) => this.setState({
                     branch: value
                 })
             }
```

### Comparing `repo_review-0.8.1/docs/webapp.md` & `repo_review-0.9.0/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/docs/api/repo_review.rst` & `repo_review-0.9.0/docs/api/repo_review.rst`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/src/repo_review/__main__.py` & `repo_review-0.9.0/src/repo_review/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import rich.traceback
 import rich.tree
 
 from . import __version__
 from ._compat.importlib.resources.abc import Traversable
 from ._compat.typing import assert_never
 from .checks import get_check_description, get_check_url
-from .families import Family, get_family_name
+from .families import Family, get_family_description, get_family_name
 from .ghpath import GHPath
 from .html import to_html
 from .processor import Result, as_simple_dict, collect_all, process
 
 __all__ = ["main"]
 
 
@@ -74,16 +74,27 @@
     color: bool = True,
 ) -> None:
     console = rich.console.Console(
         record=svg, quiet=svg, stderr=stderr, color_system="auto" if color else None
     )
 
     for family, results_list in itertools.groupby(processed, lambda r: r.family):
+        # Compute the family name and optional description
         family_name = get_family_name(families, family)
-        tree = rich.tree.Tree(f"[bold]{family_name}[/bold]:")
+        rich_family_name = rich.text.Text.from_markup(f"[bold]{family_name}[/bold]:")
+        family_description = get_family_description(families, family)
+        if family_description:
+            rich_description = rich.markdown.Markdown(family_description)
+            rich_family = rich.console.Group(
+                rich_family_name, rich_description, rich.console.NewLine()
+            )
+            tree = rich.tree.Tree(rich_family)
+        else:
+            tree = rich.tree.Tree(rich_family_name)
+
         for result in results_list:
             style = (
                 "yellow"
                 if result.result is None
                 else "green"
                 if result.result
                 else "red"
```

### Comparing `repo_review-0.8.1/src/repo_review/checks.py` & `repo_review-0.9.0/src/repo_review/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from typing import Any, Protocol
 
 from .fixtures import apply_fixtures
 
 __all__ = ["Check", "collect_checks", "is_allowed", "get_check_url"]
 
 
+def __dir__() -> list[str]:
+    return __all__
+
+
 class Check(Protocol):
     """
     This is the check Protocol. Since Python doesn't support optional Protocol
     members, the two optional members are required if you want to use this
     Protocol in a type checker. The members can be specified as class
     properties if you want.
     """
```

### Comparing `repo_review-0.8.1/src/repo_review/families.py` & `repo_review-0.9.0/src/repo_review/families.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 import importlib.metadata
 import typing
 from collections.abc import Mapping
+from typing import Any
+
+from .fixtures import apply_fixtures
 
 __all__ = ["Family", "collect_families", "get_family_name"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
@@ -20,26 +23,37 @@
     #: key if missing.
     name: str
 
     #: Checks are first sorted by this integer order, then alphabetically by
     #: family key. Treated like 0 if missing.
     order: int
 
+    #: An optional description that shows up under the family name.
+    description: str
+
 
-def collect_families() -> dict[str, Family]:
+def collect_families(fixtures: Mapping[str, Any]) -> dict[str, Family]:
     """
-    Produces a dict mapping family keys to :class:`Family` dicts based on installed
-    entry points. Unlike other similar functions, this one currently does not
-    expect a dict of fixtures; dynamic listing is not usually needed for
-    :class:`Family`'s.
+    Produces a dict mapping family keys to :class:`Family` dicts based on
+    installed entry points. You must provide the evaluated fixtures so that the
+    family functions have access to the fixtures when they are running, usually
+    used for descriptions.
+
+    :param fixtures: Fully evaluated dict of fixtures.
     """
-    return {
-        name: family
+
+    family_functions = (
+        ep.load()
         for ep in importlib.metadata.entry_points(group="repo_review.families")
-        for name, family in ep.load()().items()
+    )
+
+    return {
+        k: v
+        for func in family_functions
+        for k, v in apply_fixtures(fixtures, func).items()
     }
 
 
 def get_family_name(families: Mapping[str, Family], family: str) -> str:
     """
     Returns the "nice" family name if there is one, otherwise the (input)
     family short name.
@@ -47,7 +61,20 @@
     :param families: A dict of family short names to :class:`.Family`'s.
     :param family: The short name of a family.
     :return: The nice family name if there is one, otherwise the short name is returned.
 
     .. versionadded:: 0.8
     """
     return families.get(family, {}).get("name", family)
+
+
+def get_family_description(families: Mapping[str, Family], family: str) -> str:
+    """
+    Returns the description if there is one, otherwise returns an empty string.
+
+    :param families: A dict of family short names to :class:`.Family`'s.
+    :param family: The short name of a family.
+    :return: The de-intended description if there is one, otherwise an empty string.
+
+    .. versionadded:: 0.9
+    """
+    return families.get(family, {}).get("description", "")
```

### Comparing `repo_review-0.8.1/src/repo_review/fixtures.py` & `repo_review-0.9.0/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/src/repo_review/ghpath.py` & `repo_review-0.9.0/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/src/repo_review/html.py` & `repo_review-0.9.0/src/repo_review/html.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,140 +6,149 @@
 00000050: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
 00000060: 6672 6f6d 2063 6f6c 6c65 6374 696f 6e73  from collections
 00000070: 2e61 6263 2069 6d70 6f72 7420 4d61 7070  .abc import Mapp
 00000080: 696e 670a 0a69 6d70 6f72 7420 6d61 726b  ing..import mark
 00000090: 646f 776e 5f69 740a 0a66 726f 6d20 2e66  down_it..from .f
 000000a0: 616d 696c 6965 7320 696d 706f 7274 2046  amilies import F
 000000b0: 616d 696c 792c 2067 6574 5f66 616d 696c  amily, get_famil
-000000c0: 795f 6e61 6d65 0a66 726f 6d20 2e70 726f  y_name.from .pro
-000000d0: 6365 7373 6f72 2069 6d70 6f72 7420 5265  cessor import Re
-000000e0: 7375 6c74 0a0a 5f5f 616c 6c5f 5f20 3d20  sult..__all__ = 
-000000f0: 5b22 746f 5f68 746d 6c22 5d0a 0a0a 6465  ["to_html"]...de
-00000100: 6620 5f5f 6469 725f 5f28 2920 2d3e 206c  f __dir__() -> l
-00000110: 6973 745b 7374 725d 3a0a 2020 2020 7265  ist[str]:.    re
-00000120: 7475 726e 205f 5f61 6c6c 5f5f 0a0a 0a64  turn __all__...d
-00000130: 6566 2074 6f5f 6874 6d6c 2866 616d 696c  ef to_html(famil
-00000140: 6965 733a 204d 6170 7069 6e67 5b73 7472  ies: Mapping[str
-00000150: 2c20 4661 6d69 6c79 5d2c 2070 726f 6365  , Family], proce
-00000160: 7373 6564 3a20 6c69 7374 5b52 6573 756c  ssed: list[Resul
-00000170: 745d 2920 2d3e 2073 7472 3a0a 2020 2020  t]) -> str:.    
-00000180: 2222 220a 2020 2020 436f 6e76 6572 7420  """.    Convert 
-00000190: 7468 6520 7265 7375 6c74 7320 6f66 2061  the results of a
-000001a0: 2072 6570 6f20 7265 7669 6577 2028 6060   repo review (``
-000001b0: 6661 6d69 6c69 6573 6060 2c20 6060 7072  families``, ``pr
-000001c0: 6f63 6573 7365 6460 6029 2074 6f20 4854  ocessed``) to HT
-000001d0: 4d4c 2e0a 0a20 2020 203a 7061 7261 6d20  ML...    :param 
-000001e0: 6661 6d69 6c69 6573 3a20 5468 6520 6661  families: The fa
-000001f0: 6d69 6c79 206d 6170 7069 6e67 2e0a 2020  mily mapping..  
-00000200: 2020 3a70 6172 616d 2070 726f 6365 7373    :param process
-00000210: 6564 3a20 5468 6520 6c69 7374 206f 6620  ed: The list of 
-00000220: 7072 6f63 6573 7365 6420 7265 7375 6c74  processed result
-00000230: 732e 0a20 2020 2022 2222 0a20 2020 206f  s..    """.    o
-00000240: 7574 203d 2069 6f2e 5374 7269 6e67 494f  ut = io.StringIO
-00000250: 2829 0a20 2020 2070 7269 6e74 203d 2066  ().    print = f
-00000260: 756e 6374 6f6f 6c73 2e70 6172 7469 616c  unctools.partial
-00000270: 2862 7569 6c74 696e 732e 7072 696e 742c  (builtins.print,
-00000280: 2066 696c 653d 6f75 7429 0a20 2020 206d   file=out).    m
-00000290: 6420 3d20 6d61 726b 646f 776e 5f69 742e  d = markdown_it.
-000002a0: 4d61 726b 646f 776e 4974 2829 0a0a 2020  MarkdownIt()..  
-000002b0: 2020 666f 7220 6661 6d69 6c79 2c20 7265    for family, re
-000002c0: 7375 6c74 735f 6c69 7374 2069 6e20 6974  sults_list in it
-000002d0: 6572 746f 6f6c 732e 6772 6f75 7062 7928  ertools.groupby(
-000002e0: 7072 6f63 6573 7365 642c 206c 616d 6264  processed, lambd
-000002f0: 6120 723a 2072 2e66 616d 696c 7929 3a0a  a r: r.family):.
-00000300: 2020 2020 2020 2020 6661 6d69 6c79 5f6e          family_n
-00000310: 616d 6520 3d20 6765 745f 6661 6d69 6c79  ame = get_family
-00000320: 5f6e 616d 6528 6661 6d69 6c69 6573 2c20  _name(families, 
-00000330: 6661 6d69 6c79 290a 2020 2020 2020 2020  family).        
-00000340: 7072 696e 7428 6622 3c68 323e 7b66 616d  print(f"<h2>{fam
-00000350: 696c 795f 6e61 6d65 7d3c 2f68 323e 2229  ily_name}</h2>")
-00000360: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00000370: 3c74 6162 6c65 3e22 290a 2020 2020 2020  <table>").      
-00000380: 2020 7072 696e 7428 223c 7472 3e3c 7468    print("<tr><th
-00000390: 3e3f 3c2f 7468 3e3c 7468 3e4e 616d 653c  >?</th><th>Name<
-000003a0: 2f74 683e 3c74 683e 4465 7363 7269 7074  /th><th>Descript
-000003b0: 696f 6e3c 2f74 683e 3c2f 7472 3e22 290a  ion</th></tr>").
-000003c0: 2020 2020 2020 2020 666f 7220 7265 7375          for resu
-000003d0: 6c74 2069 6e20 7265 7375 6c74 735f 6c69  lt in results_li
-000003e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-000003f0: 636f 6c6f 7220 3d20 280a 2020 2020 2020  color = (.      
-00000400: 2020 2020 2020 2020 2020 226f 7261 6e67            "orang
-00000410: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
-00000420: 2020 2069 6620 7265 7375 6c74 2e72 6573     if result.res
-00000430: 756c 7420 6973 204e 6f6e 650a 2020 2020  ult is None.    
-00000440: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000450: 2022 6772 6565 6e22 0a20 2020 2020 2020   "green".       
-00000460: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
-00000470: 6c74 2e72 6573 756c 740a 2020 2020 2020  lt.result.      
-00000480: 2020 2020 2020 2020 2020 656c 7365 2022            else "
-00000490: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
-000004a0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-000004b0: 636f 6e20 3d20 22e2 9aa0 efb8 8f22 2069  con = "......" i
-000004c0: 6620 7265 7375 6c74 2e72 6573 756c 7420  f result.result 
-000004d0: 6973 204e 6f6e 6520 656c 7365 2022 e29c  is None else "..
-000004e0: 8522 2069 6620 7265 7375 6c74 2e72 6573  ." if result.res
-000004f0: 756c 7420 656c 7365 2022 e29d 8c22 0a20  ult else "...". 
-00000500: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00000510: 745f 7478 7420 3d20 280a 2020 2020 2020  t_txt = (.      
-00000520: 2020 2020 2020 2020 2020 2253 6b69 7070            "Skipp
-00000530: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00000540: 2020 2020 6966 2072 6573 756c 742e 7265      if result.re
-00000550: 7375 6c74 2069 7320 4e6f 6e65 0a20 2020  sult is None.   
-00000560: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00000570: 6520 2250 6173 7365 6422 0a20 2020 2020  e "Passed".     
-00000580: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00000590: 7375 6c74 2e72 6573 756c 740a 2020 2020  sult.result.    
-000005a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000005b0: 2022 4661 696c 6564 220a 2020 2020 2020   "Failed".      
-000005c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000005d0: 2020 2020 6465 7363 7269 7074 696f 6e20      description 
-000005e0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000005f0: 2020 2020 6627 3c61 2068 7265 663d 227b      f'<a href="{
-00000600: 7265 7375 6c74 2e75 726c 7d22 3e7b 7265  result.url}">{re
-00000610: 7375 6c74 2e64 6573 6372 6970 7469 6f6e  sult.description
-00000620: 7d3c 2f61 3e27 0a20 2020 2020 2020 2020  }</a>'.         
-00000630: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-00000640: 2e75 726c 0a20 2020 2020 2020 2020 2020  .url.           
-00000650: 2020 2020 2065 6c73 6520 7265 7375 6c74       else result
-00000660: 2e64 6573 6372 6970 7469 6f6e 0a20 2020  .description.   
-00000670: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00000680: 2020 2020 2020 2070 7269 6e74 2866 273c         print(f'<
-00000690: 7472 2073 7479 6c65 3d22 636f 6c6f 723a  tr style="color:
-000006a0: 207b 636f 6c6f 727d 3b22 3e27 290a 2020   {color};">').  
-000006b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000006c0: 6627 3c74 643e 3c73 7061 6e20 726f 6c65  f'<td><span role
-000006d0: 3d22 696d 6722 2061 7269 612d 6c61 6265  ="img" aria-labe
-000006e0: 6c3d 227b 7265 7375 6c74 5f74 7874 7d22  l="{result_txt}"
-000006f0: 3e7b 6963 6f6e 7d3c 2f73 7061 6e3e 3c2f  >{icon}</span></
-00000700: 7464 3e27 290a 2020 2020 2020 2020 2020  td>').          
-00000710: 2020 7072 696e 7428 6622 3c74 643e 7b72    print(f"<td>{r
-00000720: 6573 756c 742e 6e61 6d65 7d3c 2f74 643e  esult.name}</td>
-00000730: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00000740: 6620 7265 7375 6c74 2e72 6573 756c 7420  f result.result 
-00000750: 6973 204e 6f6e 6520 6f72 2072 6573 756c  is None or resul
-00000760: 742e 7265 7375 6c74 3a0a 2020 2020 2020  t.result:.      
-00000770: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00000780: 6622 3c74 643e 7b64 6573 6372 6970 7469  f"<td>{descripti
-00000790: 6f6e 7d3c 2f74 643e 2229 0a20 2020 2020  on}</td>").     
-000007a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000007b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000007c0: 6e74 2822 3c74 643e 2229 0a20 2020 2020  nt("<td>").     
-000007d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000007e0: 2864 6573 6372 6970 7469 6f6e 290a 2020  (description).  
-000007f0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00000800: 696e 7428 223c 6272 2f3e 2229 0a20 2020  int("<br/>").   
-00000810: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00000820: 6e74 286d 642e 7265 6e64 6572 2872 6573  nt(md.render(res
-00000830: 756c 742e 6572 725f 6d73 6729 290a 2020  ult.err_msg)).  
-00000840: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00000850: 696e 7428 223c 2f74 643e 2229 0a20 2020  int("</td>").   
-00000860: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00000870: 3c2f 7472 3e22 290a 2020 2020 2020 2020  </tr>").        
-00000880: 7072 696e 7428 223c 2f74 6162 6c65 3e22  print("</table>"
-00000890: 290a 0a20 2020 2069 6620 6c65 6e28 7072  )..    if len(pr
-000008a0: 6f63 6573 7365 6429 203d 3d20 303a 0a20  ocessed) == 0:. 
-000008b0: 2020 2020 2020 2070 7269 6e74 2827 3c73         print('<s
-000008c0: 7061 6e20 7374 796c 653d 2263 6f6c 6f72  pan style="color
-000008d0: 3a20 7265 643b 223e 4e6f 2063 6865 636b  : red;">No check
-000008e0: 7320 7261 6e2e 3c2f 7370 616e 3e27 290a  s ran.</span>').
-000008f0: 0a20 2020 2072 6574 7572 6e20 6f75 742e  .    return out.
-00000900: 6765 7476 616c 7565 2829 0a              getvalue().
+000000c0: 795f 6465 7363 7269 7074 696f 6e2c 2067  y_description, g
+000000d0: 6574 5f66 616d 696c 795f 6e61 6d65 0a66  et_family_name.f
+000000e0: 726f 6d20 2e70 726f 6365 7373 6f72 2069  rom .processor i
+000000f0: 6d70 6f72 7420 5265 7375 6c74 0a0a 5f5f  mport Result..__
+00000100: 616c 6c5f 5f20 3d20 5b22 746f 5f68 746d  all__ = ["to_htm
+00000110: 6c22 5d0a 0a0a 6465 6620 5f5f 6469 725f  l"]...def __dir_
+00000120: 5f28 2920 2d3e 206c 6973 745b 7374 725d  _() -> list[str]
+00000130: 3a0a 2020 2020 7265 7475 726e 205f 5f61  :.    return __a
+00000140: 6c6c 5f5f 0a0a 0a64 6566 2074 6f5f 6874  ll__...def to_ht
+00000150: 6d6c 2866 616d 696c 6965 733a 204d 6170  ml(families: Map
+00000160: 7069 6e67 5b73 7472 2c20 4661 6d69 6c79  ping[str, Family
+00000170: 5d2c 2070 726f 6365 7373 6564 3a20 6c69  ], processed: li
+00000180: 7374 5b52 6573 756c 745d 2920 2d3e 2073  st[Result]) -> s
+00000190: 7472 3a0a 2020 2020 2222 220a 2020 2020  tr:.    """.    
+000001a0: 436f 6e76 6572 7420 7468 6520 7265 7375  Convert the resu
+000001b0: 6c74 7320 6f66 2061 2072 6570 6f20 7265  lts of a repo re
+000001c0: 7669 6577 2028 6060 6661 6d69 6c69 6573  view (``families
+000001d0: 6060 2c20 6060 7072 6f63 6573 7365 6460  ``, ``processed`
+000001e0: 6029 2074 6f20 4854 4d4c 2e0a 0a20 2020  `) to HTML...   
+000001f0: 203a 7061 7261 6d20 6661 6d69 6c69 6573   :param families
+00000200: 3a20 5468 6520 6661 6d69 6c79 206d 6170  : The family map
+00000210: 7069 6e67 2e0a 2020 2020 3a70 6172 616d  ping..    :param
+00000220: 2070 726f 6365 7373 6564 3a20 5468 6520   processed: The 
+00000230: 6c69 7374 206f 6620 7072 6f63 6573 7365  list of processe
+00000240: 6420 7265 7375 6c74 732e 0a20 2020 2022  d results..    "
+00000250: 2222 0a20 2020 206f 7574 203d 2069 6f2e  "".    out = io.
+00000260: 5374 7269 6e67 494f 2829 0a20 2020 2070  StringIO().    p
+00000270: 7269 6e74 203d 2066 756e 6374 6f6f 6c73  rint = functools
+00000280: 2e70 6172 7469 616c 2862 7569 6c74 696e  .partial(builtin
+00000290: 732e 7072 696e 742c 2066 696c 653d 6f75  s.print, file=ou
+000002a0: 7429 0a20 2020 206d 6420 3d20 6d61 726b  t).    md = mark
+000002b0: 646f 776e 5f69 742e 4d61 726b 646f 776e  down_it.Markdown
+000002c0: 4974 2829 0a0a 2020 2020 666f 7220 6661  It()..    for fa
+000002d0: 6d69 6c79 2c20 7265 7375 6c74 735f 6c69  mily, results_li
+000002e0: 7374 2069 6e20 6974 6572 746f 6f6c 732e  st in itertools.
+000002f0: 6772 6f75 7062 7928 7072 6f63 6573 7365  groupby(processe
+00000300: 642c 206c 616d 6264 6120 723a 2072 2e66  d, lambda r: r.f
+00000310: 616d 696c 7929 3a0a 2020 2020 2020 2020  amily):.        
+00000320: 6661 6d69 6c79 5f6e 616d 6520 3d20 6765  family_name = ge
+00000330: 745f 6661 6d69 6c79 5f6e 616d 6528 6661  t_family_name(fa
+00000340: 6d69 6c69 6573 2c20 6661 6d69 6c79 290a  milies, family).
+00000350: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00000360: 3c68 323e 7b66 616d 696c 795f 6e61 6d65  <h2>{family_name
+00000370: 7d3c 2f68 323e 2229 0a20 2020 2020 2020  }</h2>").       
+00000380: 2069 6620 6465 7363 7269 7074 696f 6e20   if description 
+00000390: 3a3d 2067 6574 5f66 616d 696c 795f 6465  := get_family_de
+000003a0: 7363 7269 7074 696f 6e28 6661 6d69 6c69  scription(famili
+000003b0: 6573 2c20 6661 6d69 6c79 293a 0a20 2020  es, family):.   
+000003c0: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
+000003d0: 642e 7265 6e64 6572 2864 6573 6372 6970  d.render(descrip
+000003e0: 7469 6f6e 2929 0a20 2020 2020 2020 2070  tion)).        p
+000003f0: 7269 6e74 2822 3c74 6162 6c65 3e22 290a  rint("<table>").
+00000400: 2020 2020 2020 2020 7072 696e 7428 223c          print("<
+00000410: 7472 3e3c 7468 3e3f 3c2f 7468 3e3c 7468  tr><th>?</th><th
+00000420: 3e4e 616d 653c 2f74 683e 3c74 683e 4465  >Name</th><th>De
+00000430: 7363 7269 7074 696f 6e3c 2f74 683e 3c2f  scription</th></
+00000440: 7472 3e22 290a 2020 2020 2020 2020 666f  tr>").        fo
+00000450: 7220 7265 7375 6c74 2069 6e20 7265 7375  r result in resu
+00000460: 6c74 735f 6c69 7374 3a0a 2020 2020 2020  lts_list:.      
+00000470: 2020 2020 2020 636f 6c6f 7220 3d20 280a        color = (.
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 226f 7261 6e67 6522 0a20 2020 2020 2020  "orange".       
+000004a0: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
+000004b0: 6c74 2e72 6573 756c 7420 6973 204e 6f6e  lt.result is Non
+000004c0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000004d0: 2020 656c 7365 2022 6772 6565 6e22 0a20    else "green". 
+000004e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000004f0: 6620 7265 7375 6c74 2e72 6573 756c 740a  f result.result.
+00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000510: 656c 7365 2022 7265 6422 0a20 2020 2020  else "red".     
+00000520: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000530: 2020 2020 2069 636f 6e20 3d20 22e2 9aa0       icon = "...
+00000540: efb8 8f22 2069 6620 7265 7375 6c74 2e72  ..." if result.r
+00000550: 6573 756c 7420 6973 204e 6f6e 6520 656c  esult is None el
+00000560: 7365 2022 e29c 8522 2069 6620 7265 7375  se "..." if resu
+00000570: 6c74 2e72 6573 756c 7420 656c 7365 2022  lt.result else "
+00000580: e29d 8c22 0a20 2020 2020 2020 2020 2020  ...".           
+00000590: 2072 6573 756c 745f 7478 7420 3d20 280a   result_txt = (.
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 2253 6b69 7070 6564 220a 2020 2020 2020  "Skipped".      
+000005c0: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+000005d0: 756c 742e 7265 7375 6c74 2069 7320 4e6f  ult.result is No
+000005e0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+000005f0: 2020 2065 6c73 6520 2250 6173 7365 6422     else "Passed"
+00000600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000610: 2069 6620 7265 7375 6c74 2e72 6573 756c   if result.resul
+00000620: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00000630: 2020 656c 7365 2022 4661 696c 6564 220a    else "Failed".
+00000640: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000650: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00000660: 7074 696f 6e20 3d20 280a 2020 2020 2020  ption = (.      
+00000670: 2020 2020 2020 2020 2020 6627 3c61 2068            f'<a h
+00000680: 7265 663d 227b 7265 7375 6c74 2e75 726c  ref="{result.url
+00000690: 7d22 3e7b 7265 7375 6c74 2e64 6573 6372  }">{result.descr
+000006a0: 6970 7469 6f6e 7d3c 2f61 3e27 0a20 2020  iption}</a>'.   
+000006b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000006c0: 7265 7375 6c74 2e75 726c 0a20 2020 2020  result.url.     
+000006d0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000006e0: 7265 7375 6c74 2e64 6573 6372 6970 7469  result.descripti
+000006f0: 6f6e 0a20 2020 2020 2020 2020 2020 2029  on.            )
+00000700: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00000710: 6e74 2866 273c 7472 2073 7479 6c65 3d22  nt(f'<tr style="
+00000720: 636f 6c6f 723a 207b 636f 6c6f 727d 3b22  color: {color};"
+00000730: 3e27 290a 2020 2020 2020 2020 2020 2020  >').            
+00000740: 7072 696e 7428 6627 3c74 643e 3c73 7061  print(f'<td><spa
+00000750: 6e20 726f 6c65 3d22 696d 6722 2061 7269  n role="img" ari
+00000760: 612d 6c61 6265 6c3d 227b 7265 7375 6c74  a-label="{result
+00000770: 5f74 7874 7d22 3e7b 6963 6f6e 7d3c 2f73  _txt}">{icon}</s
+00000780: 7061 6e3e 3c2f 7464 3e27 290a 2020 2020  pan></td>').    
+00000790: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+000007a0: 3c74 643e 7b72 6573 756c 742e 6e61 6d65  <td>{result.name
+000007b0: 7d3c 2f74 643e 2229 0a20 2020 2020 2020  }</td>").       
+000007c0: 2020 2020 2069 6620 7265 7375 6c74 2e72       if result.r
+000007d0: 6573 756c 7420 6973 204e 6f6e 6520 6f72  esult is None or
+000007e0: 2072 6573 756c 742e 7265 7375 6c74 3a0a   result.result:.
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 7072 696e 7428 6622 3c74 643e 7b64 6573  print(f"<td>{des
+00000810: 6372 6970 7469 6f6e 7d3c 2f74 643e 2229  cription}</td>")
+00000820: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00000830: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00000840: 2020 2070 7269 6e74 2822 3c74 643e 2229     print("<td>")
+00000850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000860: 2070 7269 6e74 2864 6573 6372 6970 7469   print(descripti
+00000870: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+00000880: 2020 2020 7072 696e 7428 223c 6272 2f3e      print("<br/>
+00000890: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000008a0: 2020 2070 7269 6e74 286d 642e 7265 6e64     print(md.rend
+000008b0: 6572 2872 6573 756c 742e 6572 725f 6d73  er(result.err_ms
+000008c0: 6729 290a 2020 2020 2020 2020 2020 2020  g)).            
+000008d0: 2020 2020 7072 696e 7428 223c 2f74 643e      print("</td>
+000008e0: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
+000008f0: 7269 6e74 2822 3c2f 7472 3e22 290a 2020  rint("</tr>").  
+00000900: 2020 2020 2020 7072 696e 7428 223c 2f74        print("</t
+00000910: 6162 6c65 3e22 290a 0a20 2020 2069 6620  able>")..    if 
+00000920: 6c65 6e28 7072 6f63 6573 7365 6429 203d  len(processed) =
+00000930: 3d20 303a 0a20 2020 2020 2020 2070 7269  = 0:.        pri
+00000940: 6e74 2827 3c73 7061 6e20 7374 796c 653d  nt('<span style=
+00000950: 2263 6f6c 6f72 3a20 7265 643b 223e 4e6f  "color: red;">No
+00000960: 2063 6865 636b 7320 7261 6e2e 3c2f 7370   checks ran.</sp
+00000970: 616e 3e27 290a 0a20 2020 2072 6574 7572  an>')..    retur
+00000980: 6e20 6f75 742e 6765 7476 616c 7565 2829  n out.getvalue()
+00000990: 0a                                       .
```

### Comparing `repo_review-0.8.1/src/repo_review/processor.py` & `repo_review-0.9.0/src/repo_review/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,24 +19,35 @@
     "CollectionReturn",
     "ProcessReturn",
     "Result",
     "ResultDict",
     "as_simple_dict",
     "collect_all",
     "process",
+    "md_as_html",
 ]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 md = markdown_it.MarkdownIt()
 
 
+def md_as_html(md_text: str) -> str:
+    """
+    Heler function that converts markdown text to HTML. Strips paragraph tags from the result.
+
+    :param md_text: The markdown text to convert.
+    """
+    result: str = md.render(md_text).strip()
+    return result.removeprefix("<p>").removesuffix("</p>").strip()
+
+
 class ResultDict(typing.TypedDict):
     """
     Helper to get the type in the JSON style returns. Basically identical to
     :class:`Result` but in dict form and without the name.
     """
 
     family: str  #: The family string
@@ -59,16 +70,15 @@
     err_msg: str = ""  #: The error message if the result is false, in markdown format
     url: str = ""  #: An optional URL (empty string if missing)
 
     def err_as_html(self) -> str:
         """
         Produces HTML from the error message, assuming it is in markdown.
         """
-        result: str = md.render(self.err_msg).strip()
-        return result.removeprefix("<p>").removesuffix("</p>").strip()
+        return md_as_html(self.err_msg)
 
 
 class ProcessReturn(typing.NamedTuple):
     """
     Return type for :func:`process`.
     """
 
@@ -139,15 +149,15 @@
     fixture_functions = collect_fixtures()
     fixtures = compute_fixtures(root, package, fixture_functions)
 
     # Collect the checks
     checks = collect_checks(fixtures)
 
     # Collect families.
-    families = collect_families()
+    families = collect_families(fixtures)
 
     # These are optional, so fill in missing families.
     for name in {c.family for c in checks.values()}:
         if name not in families:
             families[name] = Family()
 
     # Sort results
@@ -190,17 +200,23 @@
     # Keep track of which checks have been completed
     completed: dict[str, str | None] = {}
 
     # Run all the checks in topological order based on their dependencies
     ts = graphlib.TopologicalSorter(graph)
     for name in ts.static_order():
         if all(completed.get(n, "") == "" for n in graph[name]):
-            result = apply_fixtures(fixtures, tasks[name].check)
+            result = apply_fixtures({"name": name, **fixtures}, tasks[name].check)
             if isinstance(result, bool):
-                completed[name] = "" if result else tasks[name].check.__doc__
+                completed[name] = (
+                    ""
+                    if result
+                    else (tasks[name].check.__doc__ or "Check failed").format(
+                        name=name, self=tasks[name].check
+                    )
+                )
             else:
                 completed[name] = result
         else:
             completed[name] = None
 
     # Collect the results
     result_list = []
@@ -212,17 +228,17 @@
         if not is_allowed(select_checks, skip_checks, task_name):
             continue
 
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
-                description=doc.format(self=check, name=task_name),
+                description=doc.format(self=check, name=task_name).strip(),
                 result=result,
-                err_msg=textwrap.dedent(err_msg.format(self=check, name=task_name)),
+                err_msg=textwrap.dedent(err_msg),
                 url=get_check_url(task_name, check),
             )
         )
 
     return ProcessReturn(families, result_list)
```

### Comparing `repo_review-0.8.1/tests/test_checks.py` & `repo_review-0.9.0/tests/test_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     @staticmethod
     def check(package: Traversable) -> bool:
         """
         Requires Path(".") to be passed
         """
 
-        return package == Path(".")
+        return package == Path()
 
 
 class D200:
     "Always true"
     family = "pyproject"
 
     @staticmethod
@@ -41,50 +41,50 @@
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class C100:
     "Can compute custom output strings"
     fail: bool
     family: ClassVar[str] = "custom"
 
-    def check(self) -> str:
+    def check(self, name: str) -> str:
         "Never see me"
-        return "I'm a custom error message" if self.fail else ""
+        return f"I'm a custom error message from {name}" if self.fail else ""
 
 
 def test_no_checks(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         importlib.metadata, "entry_points", lambda group: []  # noqa: ARG005
     )
 
-    _, results = repo_review.processor.process(Path("."))
+    _, results = repo_review.processor.process(Path())
     assert len(results) == 0
 
 
 def test_load_entry_point(monkeypatch: pytest.MonkeyPatch) -> None:
     ep = importlib.metadata.EntryPoint(name="x", group="y", value="test_module:f")
     sys.modules["test_module"] = ModuleType("test_module")
     sys.modules["test_module"].f = lambda: {"D100": D100, "D200": D200}  # type: ignore[attr-defined]
     monkeypatch.setattr(
         importlib.metadata, "entry_points", lambda group: [ep]  # noqa: ARG005
     )
-    checks = collect_checks({"package": Path(".")})
+    checks = collect_checks({"package": Path()})
 
     assert len(checks) == 2
     assert "D100" in checks
     assert "D200" in checks
     assert checks["D200"] == D200  # type: ignore[comparison-overlap]
 
 
 def test_custom_checks(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100, "D200": D200},
     )
-    _, results = repo_review.processor.process(Path("."))
+    _, results = repo_review.processor.process(Path())
 
     assert len(results) == 2
     assert results[0].name == "D100"
     assert results[0].result
     assert results[0].url == "https://example.com"
     assert results[1].name == "D200"
     assert results[1].result
@@ -94,66 +94,66 @@
 
 def test_ignore_filter_single(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100, "D200": D200},
     )
-    _, results = repo_review.processor.process(Path("."), ignore={"D100"})
+    _, results = repo_review.processor.process(Path(), ignore={"D100"})
 
     assert len(results) == 1
     assert results[0].name == "D200"
     assert results[0].result
 
 
 def test_ignore_filter_letter(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100(), "D200": D200()},
     )
-    _, results = repo_review.processor.process(Path("."), ignore={"D"})
+    _, results = repo_review.processor.process(Path(), ignore={"D"})
 
     assert not results
 
 
 def test_select_filter_letter(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100(), "D200": D200(), "C100": C100(fail=True)},
     )
-    _, results = repo_review.processor.process(Path("."), select={"D"})
+    _, results = repo_review.processor.process(Path(), select={"D"})
 
     assert len(results) == 2
 
 
 def test_select_filter_exact(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100(), "D200": D200()},
     )
-    _, results = repo_review.processor.process(Path("."), select={"D100"})
+    _, results = repo_review.processor.process(Path(), select={"D100"})
 
     assert len(results) == 1
 
 
 def test_string_result(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"C100": C100(fail=False), "C101": C100(fail=True)},
     )
-    _, results = repo_review.processor.process(Path("."))
+    _, results = repo_review.processor.process(Path())
 
     assert len(results) == 2
     check_c100 = results[0]
     check_c101 = results[1]
 
     assert check_c100.name == "C100"
     assert check_c100.result is True
     assert not check_c100.err_msg
 
     assert check_c101.name == "C101"
     assert check_c101.result is False
-    assert check_c101.err_msg == "I'm a custom error message"
+    assert check_c101.err_msg == "I'm a custom error message from C101"
```

### Comparing `repo_review-0.8.1/tests/test_cmd.py` & `repo_review-0.9.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/tests/test_fixtures.py` & `repo_review-0.9.0/tests/test_fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     @staticmethod
     def check(package: Traversable) -> bool:
         """
         Requires Path(".") to be passed
         """
 
-        return package == Path(".")
+        return package == Path()
 
 
 class D200:
     "Always true"
     family = "pyproject"
 
     @staticmethod
@@ -50,44 +50,44 @@
 
 def get_checks(some_bool: bool) -> dict[str, type]:
     return {"D100": D100, "D200": D200} if some_bool else {"D100": D100}
 
 
 def test_process_fixtures() -> None:
     fixtures = compute_fixtures(
-        Path("."),
-        Path("."),
+        Path(),
+        Path(),
         {"simple": simple, "nothing": nothing, "not_simple": not_simple},
     )
 
     assert apply_fixtures(fixtures, nothing) == 42
     assert apply_fixtures(fixtures, simple) == "."
     assert apply_fixtures(fixtures, not_simple) == ". ."
 
 
 def test_process_fixtures_with_package() -> None:
     fixtures = compute_fixtures(
-        Path("."),
-        Path("."),
+        Path(),
+        Path(),
         {
             "simple": simple,
             "nothing": nothing,
             "not_simple": not_simple,
         },
     )
 
     assert apply_fixtures(fixtures, nothing) == 42
     assert apply_fixtures(fixtures, simple) == "."
-    assert apply_fixtures(fixtures, lambda package: package) == Path(".")
+    assert apply_fixtures(fixtures, lambda package: package) == Path()
     assert apply_fixtures(fixtures, not_simple) == ". ."
 
 
 @pytest.mark.parametrize("some_bool", [True, False])
 def test_process_checks(monkeypatch: pytest.MonkeyPatch, some_bool: bool) -> None:
     ep = importlib.metadata.EntryPoint(name="x", group="y", value="test_module:f")
     sys.modules["test_module"] = ModuleType("test_module")
     sys.modules["test_module"].f = get_checks  # type: ignore[attr-defined]
     monkeypatch.setattr(
         importlib.metadata, "entry_points", lambda group: [ep]  # noqa: ARG005
     )
-    checks = collect_checks({"package": Path("."), "some_bool": some_bool})
+    checks = collect_checks({"package": Path(), "some_bool": some_bool})
     assert len(checks) == 1 + some_bool
```

### Comparing `repo_review-0.8.1/tests/test_package.py` & `repo_review-0.9.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/tests/test_self.py` & `repo_review-0.9.0/tests/test_self.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,45 +5,61 @@
 
 import repo_review.processor
 
 
 @pytest.fixture(autouse=True)
 def patch_entry_points(monkeypatch: pytest.MonkeyPatch) -> None:
     orig_ep = importlib.metadata.entry_points
-    ep = importlib.metadata.EntryPoint(
+    ep1 = importlib.metadata.EntryPoint(
         name="pyproject",
         group="repo_review.checks",
         value="pyproject:repo_review_checks",
     )
+    ep2 = importlib.metadata.EntryPoint(
+        name="pyproject",
+        group="repo_review.families",
+        value="pyproject:repo_review_families",
+    )
 
     def new_ep(*, group: str) -> list[importlib.metadata.EntryPoint]:
         if group == "repo_review.checks":
-            return [ep]
-        if group in {"repo_review.fixtures", "repo_review.families"}:
+            return [ep1]
+        if group == "repo_review.families":
+            return [ep2]
+        if group == "repo_review.fixtures":
             return [
                 e for e in orig_ep(group=group) if e.module.startswith("repo_review.")
             ]
         return orig_ep(group=group)
 
     monkeypatch.setattr(importlib.metadata, "entry_points", new_ep)
 
 
 def test_pyproject() -> None:
-    families, results = repo_review.processor.process(Path("."))
+    families, results = repo_review.processor.process(Path())
 
-    assert families == {"general": {}, "pyproject": {}}
+    assert families == {
+        "general": {},
+        "pyproject": {
+            "description": "Has hatchling.build backend",
+            "name": "PyProject",
+        },
+    }
     assert len(results) == 9
 
     assert all(result.result for result in results)
 
 
 def test_no_pyproject() -> None:
     families, results = repo_review.processor.process(Path("tests"))
 
-    assert families == {"general": {}, "pyproject": {}}
+    assert families == {
+        "general": {},
+        "pyproject": {"description": "Has unknown backend", "name": "PyProject"},
+    }
     assert len(results) == 9
 
     assert (
         sum(result.result is None for result in results if result.family == "pyproject")
         == 4
     )
     assert (
@@ -53,18 +69,24 @@
         sum(result.result is None for result in results if result.family == "general")
         == 0
     )
 
 
 def test_empty_pyproject() -> None:
     families, results = repo_review.processor.process(
-        Path("."), subdir="tests/test_utilities"
+        Path(), subdir="tests/test_utilities"
     )
 
-    assert families == {"general": {}, "pyproject": {}}
+    assert families == {
+        "general": {},
+        "pyproject": {
+            "description": "Has flit_core.buildapi backend",
+            "name": "PyProject",
+        },
+    }
     assert len(results) == 9
 
     assert (
         sum(result.result is None for result in results if result.family == "pyproject")
         == 1
     )
     assert (
```

### Comparing `repo_review-0.8.1/tests/test_utilities/pyproject.py` & `repo_review-0.9.0/tests/test_utilities/pyproject.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,7 +141,16 @@
         return "minversion" in options and float(options["minversion"]) >= 6
 
 
 def repo_review_checks() -> dict[str, PyProject | General]:
     return {p.__name__: p() for p in PyProject.__subclasses__()} | {
         p.__name__: p() for p in General.__subclasses__()
     }
+
+
+def repo_review_families(pyproject: dict[str, Any]) -> dict[str, dict[str, str]]:
+    return {
+        "pyproject": {
+            "name": "PyProject",
+            "description": f"Has {pyproject.get('build-system', {}).get('build-backend', 'unknown')} backend",
+        }
+    }
```

### Comparing `repo_review-0.8.1/.gitignore` & `repo_review-0.9.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -137,7 +137,8 @@
 # Cython debug symbols
 cython_debug/
 
 # setuptools_scm
 src/*/_version.py
 
 node_modules/
+/.vscode
```

### Comparing `repo_review-0.8.1/LICENSE` & `repo_review-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/README.md` & `repo_review-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.1/pyproject.toml` & `repo_review-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "markdown-it-py",
-  "pyyaml",
+  "pyyaml!=6.0.0,!=5.4.0,!=5.4.1", # pyyaml is broken with cython 3
   "tomli; python_version < '3.11'",
   "typing-extensions; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 cli = [
   "click >=8",
@@ -84,15 +84,14 @@
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config", "--import-mode=importlib"]
 xfail_strict = true
 log_cli_level = "INFO"
 filterwarnings = [
   'error',
-  'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 testpaths = ["tests"]
 pythonpath = ["tests/test_utilities"]
 
 
 [tool.mypy]
 mypy_path = ["src"]
@@ -131,15 +130,15 @@
   "unnecessary-ellipsis",  # Not correct for typing
 ]
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
+  "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "EM",          # flake8-errmsg
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
@@ -156,15 +155,14 @@
   "YTT",         # flake8-2020
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
   "PT004",  # Incorrect check, usefixtures is the correct way to do this
 ]
-target-version = "py310"
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 typing-modules = ["repo_review._compat.typing"]
 flake8-unused-arguments.ignore-variadic-names = true
@@ -178,10 +176,7 @@
 "typing.assert_never".msg = "Use repo_review._compat.typing.assert_never instead."
 "importlib.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 "importlib.resources.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 
 [tool.ruff.per-file-ignores]
 "src/repo_review/_compat/**.py" = ["TID251"]
 "src/**/__main__.py" = ["T20"]
-
-[tool.repo-review]
-ignore = ["PC190"]  # Remove after first July 2023 release of sp-repo-review
```

### Comparing `repo_review-0.8.1/PKG-INFO` & `repo_review-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.8.1
+Version: 0.9.0
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
 Project-URL: Documentation, https://repo-review.readthedocs.io
 Project-URL: Homepage, https://repo-review.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: markdown-it-py
-Requires-Dist: pyyaml
+Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == 'cli'
 Requires-Dist: rich-click; extra == 'cli'
 Requires-Dist: rich>=12.2; extra == 'cli'
 Provides-Extra: dev
```

