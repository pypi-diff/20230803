# Comparing `tmp/ghcr_badge-0.3.2.tar.gz` & `tmp/ghcr_badge-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghcr_badge-0.3.2.tar", max compression
+gzip compressed data, was "ghcr_badge-0.3.3.tar", max compression
```

## Comparing `ghcr_badge-0.3.2.tar` & `ghcr_badge-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     3802 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/README.md
--rw-r--r--   0        0        0      125 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/__init__.py
--rw-r--r--   0        0        0     1282 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/dicts.py
--rw-r--r--   0        0        0    13055 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/generate.py
--rw-r--r--   0        0        0     2859 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/main.py
--rw-r--r--   0        0        0        0 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/py.typed
--rw-r--r--   0        0        0     7454 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/server.py
--rw-r--r--   0        0        0    32038 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/static/favicon.ico
--rw-r--r--   0        0        0    28398 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/static/favicon.png
--rw-r--r--   0        0        0      721 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/svg/mark-github.svg
--rw-r--r--   0        0        0      540 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/svg/package-16.svg
--rw-r--r--   0        0        0     7236 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/templates/index.j2
--rw-r--r--   0        0        0     1798 2023-07-30 18:13:59.890952 ghcr_badge-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     3802 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/README.md
+-rw-r--r--   0        0        0      125 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/__init__.py
+-rw-r--r--   0        0        0     1282 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/dicts.py
+-rw-r--r--   0        0        0    13055 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/generate.py
+-rw-r--r--   0        0        0     2859 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/main.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/py.typed
+-rw-r--r--   0        0        0     7454 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/server.py
+-rw-r--r--   0        0        0    32038 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/static/favicon.ico
+-rw-r--r--   0        0        0    28398 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/static/favicon.png
+-rw-r--r--   0        0        0      721 2023-08-03 14:35:13.632424 ghcr_badge-0.3.3/ghcr_badge/svg/mark-github.svg
+-rw-r--r--   0        0        0      540 2023-08-03 14:35:13.636424 ghcr_badge-0.3.3/ghcr_badge/svg/package-16.svg
+-rw-r--r--   0        0        0     7248 2023-08-03 14:35:13.636424 ghcr_badge-0.3.3/ghcr_badge/templates/index.j2
+-rw-r--r--   0        0        0     1787 2023-08-03 14:35:13.636424 ghcr_badge-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.3/PKG-INFO
```

### Comparing `ghcr_badge-0.3.2/LICENSE.txt` & `ghcr_badge-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/README.md` & `ghcr_badge-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/dicts.py` & `ghcr_badge-0.3.3/ghcr_badge/dicts.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/generate.py` & `ghcr_badge-0.3.3/ghcr_badge/generate.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/main.py` & `ghcr_badge-0.3.3/ghcr_badge/main.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/server.py` & `ghcr_badge-0.3.3/ghcr_badge/server.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/static/favicon.ico` & `ghcr_badge-0.3.3/ghcr_badge/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/static/favicon.png` & `ghcr_badge-0.3.3/ghcr_badge/static/favicon.png`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/svg/mark-github.svg` & `ghcr_badge-0.3.3/ghcr_badge/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/svg/package-16.svg` & `ghcr_badge-0.3.3/ghcr_badge/svg/package-16.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.2/ghcr_badge/templates/index.j2` & `ghcr_badge-0.3.3/ghcr_badge/templates/index.j2`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         <label for="tags-trim">trim:</label>
         <input type="text" name="trim" class="trim" id="tags-trim" value="">
         <button type="submit" onclick="updateImages('tags')">Apply</button>
       </div>
       <hr>
       <h2>latest_tag</h2>
       <img alt="latest_tags-badge" id="latest_tag" src="data:,">
-      <div class="options" id="latest_tags-options">
+      <div class="options" id="latest_tag-options">
         <label for="latest_tag-color">color:</label>
         <input type="color"
                name="color"
                class="color"
                id="latest_tag-color"
                value="#44cc11">
         /
@@ -142,15 +142,15 @@
                name="label"
                class="label"
                id="latest_tag-label"
                value="version">
         /
         <label for="latest_tag-trim">trim:</label>
         <input type="text" name="trim" class="trim" id="latest_tag-trim" value="">
-        <button type="submit" onclick="updateImages('tags')">Apply</button>
+        <button type="submit" onclick="updateImages('latest_tag')">Apply</button>
       </div>
       <hr>
       <h2>develop_tag</h2>
       <img alt="develop_tag-badge" id="develop_tag" src="data:,">
       <div class="options" id="develop_tag-options">
         <label for="develop_tag-color">color:</label>
         <input type="color"
@@ -161,15 +161,15 @@
         /
         <label for="develop_tag-label">label:</label>
         <input type="text"
                name="label"
                class="label"
                id="develop_tag-label"
                value="image tags">
-        <button type="submit" onclick="updateImages('tags')">Apply</button>
+        <button type="submit" onclick="updateImages('develop_tag')">Apply</button>
       </div>
       <hr>
       <h2>size</h2>
       <img alt="size-badge" id="size" src="data:,">
       <div class="options" id="size-options">
         <label for="size-color">color:</label>
         <input type="color"
@@ -186,15 +186,15 @@
                name="label"
                class="label"
                id="size-label"
                value="image size">
         /
         <label for="size-trim">trim:</label>
         <input type="text" name="trim" class="trim" id="size-trim" value="">
-        <button type="submit" onclick="updateImages('tags')">Apply</button>
+        <button type="submit" onclick="updateImages('size')">Apply</button>
       </div>
       <hr>
     </main>
     <footer>
       <span>
         <a href="{{ repo_link }}" target="_blank">eggplants/ghcr-badge</a> / v{{ version }}
       </span>
```

### Comparing `ghcr_badge-0.3.2/pyproject.toml` & `ghcr_badge-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "Generate ghcr.io container's status badge"
 keywords = ["github-container-registry", "badge", "ghcr"]
 name = "ghcr_badge"
 packages = [{include = "ghcr_badge"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/ghcr-badge"
-version = "0.3.2"
+version = "0.3.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anybadge="^1.9.0"
 flask="^2.1.2"
 gunicorn=">=20.1,<22.0"
 humanfriendly="^10.0"
@@ -74,8 +74,8 @@
 js.indent_size = 2
 
 [tool.poetry_bumpversion.file."ghcr_badge/__init__.py"]
 
 [tool.taskipy.tasks]
 lint = "pre-commit run -a"
 profile = "python -m cProfile"
-dev = "flask --app ghcr_badge.server run --debug --reload"
+dev = "FLASK_ENV=development gunicorn --reload"
```

### Comparing `ghcr_badge-0.3.2/PKG-INFO` & `ghcr_badge-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghcr-badge
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate ghcr.io container's status badge
 Home-page: https://github.com/eggplants/ghcr-badge
 License: MIT
 Keywords: github-container-registry,badge,ghcr
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<3.12
```

