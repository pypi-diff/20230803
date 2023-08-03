# Comparing `tmp/jupylot-0.1.0.tar.gz` & `tmp/jupylot-0.1.1.tar.gz`

## Comparing `jupylot-0.1.0.tar` & `jupylot-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,32 @@
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupylot-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupylot-0.1.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupylot-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupylot-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 jupylot-0.1.0/RELEASE.md
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 jupylot-0.1.0/Untitled.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupylot-0.1.0/babel.config.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupylot-0.1.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupylot-0.1.0/jest.config.js
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupylot-0.1.0/junit.xml
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 jupylot-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupylot-0.1.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupylot-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupylot-0.1.0/tsconfig.test.json
--rw-r--r--   0        0        0   420699 2020-02-02 00:00:00.000000 jupylot-0.1.0/yarn.lock
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/_version.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/package.json
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/568.2fc7cc4ef210ff0ef700.js
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/747.b43b2818154c113b0160.js
--rw-r--r--   0        0        0    29207 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/865.0de80abf43a3862195b8.js
--rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/remoteEntry.02b4878c8e7dd1f6c74f.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/style.js
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupylot-0.1.0/jupylot/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 jupylot-0.1.0/src/index.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupylot-0.1.0/src/__tests__/jupylot.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupylot-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupylot-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupylot-0.1.0/style/index.js
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupylot-0.1.0/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupylot-0.1.0/LICENSE
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 jupylot-0.1.0/README.md
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 jupylot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 jupylot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupylot-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupylot-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupylot-0.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupylot-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupylot-0.1.1/babel.config.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupylot-0.1.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupylot-0.1.1/jest.config.js
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupylot-0.1.1/junit.xml
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 jupylot-0.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupylot-0.1.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupylot-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupylot-0.1.1/tsconfig.test.json
+-rw-r--r--   0        0        0   420699 2020-02-02 00:00:00.000000 jupylot-0.1.1/yarn.lock
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/_version.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/package.json
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/568.2fc7cc4ef210ff0ef700.js
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/747.b43b2818154c113b0160.js
+-rw-r--r--   0        0        0    29207 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/865.0de80abf43a3862195b8.js
+-rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/remoteEntry.02b4878c8e7dd1f6c74f.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/style.js
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupylot-0.1.1/jupylot/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 jupylot-0.1.1/src/index.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupylot-0.1.1/src/__tests__/jupylot.spec.ts
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupylot-0.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupylot-0.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupylot-0.1.1/style/index.js
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupylot-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupylot-0.1.1/LICENSE
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupylot-0.1.1/README.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 jupylot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 jupylot-0.1.1/PKG-INFO
```

### Comparing `jupylot-0.1.0/jest.config.js` & `jupylot-0.1.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/package.json` & `jupylot-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -179,12 +179,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0",
+    "version": "0.1.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `jupylot-0.1.0/tsconfig.json` & `jupylot-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/yarn.lock` & `jupylot-0.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/__init__.py` & `jupylot-0.1.1/jupylot/__init__.py`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/package.json` & `jupylot-0.1.1/jupylot/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/static/568.2fc7cc4ef210ff0ef700.js` & `jupylot-0.1.1/jupylot/labextension/static/568.2fc7cc4ef210ff0ef700.js`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/static/747.b43b2818154c113b0160.js` & `jupylot-0.1.1/jupylot/labextension/static/747.b43b2818154c113b0160.js`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/static/865.0de80abf43a3862195b8.js` & `jupylot-0.1.1/jupylot/labextension/static/865.0de80abf43a3862195b8.js`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/static/remoteEntry.02b4878c8e7dd1f6c74f.js` & `jupylot-0.1.1/jupylot/labextension/static/remoteEntry.02b4878c8e7dd1f6c74f.js`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/jupylot/labextension/static/third-party-licenses.json` & `jupylot-0.1.1/jupylot/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/src/index.ts` & `jupylot-0.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/.gitignore` & `jupylot-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/LICENSE` & `jupylot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupylot-0.1.0/pyproject.toml` & `jupylot-0.1.1/pyproject.toml`

 * *Files identical despite different names*

