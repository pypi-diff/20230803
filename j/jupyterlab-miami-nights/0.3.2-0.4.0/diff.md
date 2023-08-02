# Comparing `tmp/jupyterlab_miami_nights-0.3.2.tar.gz` & `tmp/jupyterlab_miami_nights-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_miami_nights-0.3.2.tar", last modified: Fri Jun 18 13:25:55 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_miami_nights-0.3.2.tar` & `jupyterlab_miami_nights-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.917787 jupyterlab_miami_nights-0.3.2/
--rw-r--r--   0 theocean154   (501) staff       (20)     1517 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/LICENSE
--rw-r--r--   0 theocean154   (501) staff       (20)      474 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/MANIFEST.in
--rw-r--r--   0 theocean154   (501) staff       (20)     7278 2021-06-18 13:25:55.917263 jupyterlab_miami_nights-0.3.2/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)     5543 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/README.md
--rw-r--r--   0 theocean154   (501) staff       (20)      207 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/install.json
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.899012 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/
--rw-r--r--   0 theocean154   (501) staff       (20)      319 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      441 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/_version.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.903141 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/
--rw-r--r--   0 theocean154   (501) staff       (20)     2913 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/package.json
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.904951 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/static/
--rw-r--r--   0 theocean154   (501) staff       (20)      481 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/static/568.a075ebf77bc1145a8701.js
--rw-r--r--   0 theocean154   (501) staff       (20)     6269 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/static/remoteEntry.145e469029155b53b350.js
--rw-r--r--   0 theocean154   (501) staff       (20)      118 2021-06-18 13:24:41.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/static/style.js
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.893481 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.893640 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.908972 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/
--rw-r--r--   0 theocean154   (501) staff       (20)   120548 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/3b5adc929c114d1cd0fc91cd735847b6.ttf
--rw-r--r--   0 theocean154   (501) staff       (20)    41744 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/662254c8318cbac0ef3bcda7ad0df6ee.woff2
--rw-r--r--   0 theocean154   (501) staff       (20)   120504 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/ff01975bdccf4187dc2b094650d0cf5e.ttf
--rw-r--r--   0 theocean154   (501) staff       (20)    31454 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.css
--rw-r--r--   0 theocean154   (501) staff       (20)        0 2021-06-18 13:24:42.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.js
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.902495 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/
--rw-r--r--   0 theocean154   (501) staff       (20)     7278 2021-06-18 13:25:55.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)     1483 2021-06-18 13:25:55.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/SOURCES.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2021-06-18 13:25:55.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/dependency_links.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2021-06-18 13:21:01.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/not-zip-safe
--rw-r--r--   0 theocean154   (501) staff       (20)       23 2021-06-18 13:25:55.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/requires.txt
--rw-r--r--   0 theocean154   (501) staff       (20)       24 2021-06-18 13:25:55.000000 jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights.egg-info/top_level.txt
--rw-r--r--   0 theocean154   (501) staff       (20)     2797 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/package.json
--rw-r--r--   0 theocean154   (501) staff       (20)      627 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/pyproject.toml
--rw-r--r--   0 theocean154   (501) staff       (20)       38 2021-06-18 13:25:55.917949 jupyterlab_miami_nights-0.3.2/setup.cfg
--rw-r--r--   0 theocean154   (501) staff       (20)     2304 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/setup.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.909383 jupyterlab_miami_nights-0.3.2/src/
--rw-r--r--   0 theocean154   (501) staff       (20)      719 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/src/index.ts
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.914105 jupyterlab_miami_nights-0.3.2/style/
--rw-r--r--   0 theocean154   (501) staff       (20)      210 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/style/base.css
--rw-r--r--   0 theocean154   (501) staff       (20)     1565 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/custom.css
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-06-18 13:25:55.916403 jupyterlab_miami_nights-0.3.2/style/fonts/
--rw-r--r--   0 theocean154   (501) staff       (20)   120504 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/fonts/SourceCodePro-Bold.ttf
--rw-r--r--   0 theocean154   (501) staff       (20)   120548 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 theocean154   (501) staff       (20)    41744 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/fonts/Vibur.woff2
--rw-r--r--   0 theocean154   (501) staff       (20)      923 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/fonts.css
--rw-r--r--   0 theocean154   (501) staff       (20)      409 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/style/index.css
--rw-r--r--   0 theocean154   (501) staff       (20)      142 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/style/index.js
--rw-r--r--   0 theocean154   (501) staff       (20)     2198 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/neondreams.css
--rw-r--r--   0 theocean154   (501) staff       (20)     9383 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/style.css
--rw-r--r--   0 theocean154   (501) staff       (20)    16880 2021-02-27 04:50:21.000000 jupyterlab_miami_nights-0.3.2/style/variables.css
--rw-r--r--   0 theocean154   (501) staff       (20)      554 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/tsconfig.json
--rw-r--r--   0 theocean154   (501) staff       (20)   179400 2021-06-18 13:15:38.000000 jupyterlab_miami_nights-0.3.2/yarn.lock
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/.gitattributes
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/MANIFEST.in
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/Makefile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/setup.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/.eslintrc.js
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/babel.config.js
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/jest.config.js
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/package.json
+-rw-r--r--   0        0        0   371701 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/yarn.lock
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/src/index.js
+-rw-r--r--   0        0        0   120504 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/SourceCodePro-Bold.ttf
+-rw-r--r--   0        0        0   120548 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/SourceCodePro-Regular.ttf
+-rw-r--r--   0        0        0    41744 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/Vibur.woff2
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/base.css
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/custom.css
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/fonts.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/index.css
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/neondreams.css
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/style.css
+-rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/style/variables.css
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/activate.test.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/assetsTransformer.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/export.test.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/fileMock.js
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/setup.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/js/tests/styleMock.js
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/_version.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/extension/install.json
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/package.json
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/static/568.ad42dc24b11b936dd6c7.js
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/static/remoteEntry.504b42f0aac636b2716f.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0   120548 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/2967dd73df838d2a2d39.ttf
+-rw-r--r--   0        0        0   120504 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/80922933add5aaad3870.ttf
+-rw-r--r--   0        0        0    41744 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/b5e5e677f7c3567440b0.woff2
+-rw-r--r--   0        0        0    31440 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.js
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/tests/test_labextension.py
+-rw-r--r--   0        0        0   100802 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/screenshots/Miami Nights.png
+-rw-r--r--   0        0        0   416952 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/screenshots/Neon Night.png
+-rw-r--r--   0        0        0   431553 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/screenshots/Neon Sunset.png
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/README.md
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8680 2020-02-02 00:00:00.000000 jupyterlab_miami_nights-0.4.0/PKG-INFO
```

### Comparing `jupyterlab_miami_nights-0.3.2/LICENSE` & `jupyterlab_miami_nights-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/README.md` & `jupyterlab_miami_nights-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/package.json` & `jupyterlab_miami_nights-0.4.0/js/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.698219696969697%*

 * *Differences: {"'author'": "'the jupyterlab_miami_nights authors'",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/apputils': '^4.1.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.2', 'eslint': '^8.44.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugin-prettier': '^5.0.0', "*

 * *                      "'prettier': '^3.0.0', 'rimraf': '^5.0.1', '@babel/cli': '^7.22.9', "*

 * *                      "'@babel/core': '^7.22.9', '@babel/eslint-parser': '^7.22.9', "*

 * *          […]*

```diff
@@ -1,99 +1,98 @@
 {
-    "author": {
-        "email": "",
-        "name": "Tim P <t.paine154@gmail.com>"
-    },
-    "bugs": {
-        "url": "https://github.com/timkpaine/jupyterlab_miami_nights/issues"
-    },
+    "author": "the jupyterlab_miami_nights authors",
     "dependencies": {
-        "@jupyterlab/application": "^3.0.11",
-        "@jupyterlab/apputils": "^3.0.9",
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/apputils": "^4.1.2",
         "highlight.js": "^10.4.1"
     },
     "description": "A glowing 80s theme based on Synthwave '84 and  JupyterLab's Neon Night theme by yeebc",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "base64-inline-loader": "^1.1.1",
-        "css-loader": "^5.0.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "mini-css-extract-plugin": "^1.3.3",
+        "@babel/cli": "^7.22.9",
+        "@babel/core": "^7.22.9",
+        "@babel/eslint-parser": "^7.22.9",
+        "@babel/preset-env": "^7.22.9",
+        "@jupyterlab/builder": "^4.0.2",
+        "babel-jest": "^29.6.1",
+        "cpx": "^1.5.0",
+        "eslint": "^8.44.0",
+        "eslint-config-airbnb": "^19.0.4",
+        "eslint-config-airbnb-base": "^15.0.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-import": "^2.27.5",
+        "eslint-plugin-jest": "^27.2.2",
+        "eslint-plugin-json": "^3.1.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "isomorphic-fetch": "^3.0.0",
+        "jest": "^29.6.1",
+        "jest-environment-jsdom": "^29.6.1",
+        "jest-junit": "^16.0.0",
+        "jest-transform-css": "^6.0.1",
+        "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typedoc": "^0.15.4",
-        "typescript": "~4.1.3",
-        "webpack": "^5.11.1",
-        "webpack-cli": "^4.3.1"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
         "lib/*.js",
         "lib/*.css",
         "style/*",
         "style/index.js"
     ],
-    "homepage": "https://github.com/timkpaine/jupyterlab_miami_nights",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.145e469029155b53b350.js"
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "jupyterlab_miami_nights"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
         },
-        "extension": true,
-        "outputDir": "jupyterlab_miami_nights/labextension",
-        "themePath": "style/index.css"
+        "extension": "lib/index.js",
+        "outputDir": "../jupyterlab_miami_nights/labextension",
+        "themePath": "lib/index.css"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "jupyterlab-theme",
         "neon",
         "cyberpunk"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@timkpaine/jupyterlab_miami_nights",
-    "publishConfig": {
-        "access": "public"
-    },
     "repository": {
         "type": "git",
-        "url": "https://github.com/timkpaine/jupyterlab_miami_nights.git"
+        "url": "https://github.com/finos/jupyterlab_templates.git"
     },
     "resolutions": {
-        "highlight.js": "^10.4.1"
+        "json5": "^2.2.3",
+        "sanitize-html": "^2.7.1",
+        "ws": "^7.4.6"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter labextension build .",
-        "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_miami_nights/labextension",
-        "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
+        "build": "npm-run-all clean build:*",
+        "build:babel": "babel src/ --source-maps --out-dir lib/",
+        "build:css": "cpx \"style/*\" \"lib/\"",
+        "build:lab": "rimraf ../jupyterlab_templates/labextension && jupyter labextension build .",
+        "clean": "rimraf lib ../jupyterlab_miami_nights/labextension",
+        "fix": "yarn lint --fix",
+        "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
-        "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/static/remoteEntry.145e469029155b53b350.js` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/static/remoteEntry.504b42f0aac636b2716f.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,128 +1,114 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, a, o, u, l, s, p, f, d, c, h, v = {
-            43: (e, r, t) => {
+    var e, r, t, n, i, a, o, u, l, s, f, p, h, c, d, v, m = {
+            39: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
-                            var n = t.S.default,
-                                i = "default";
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[i] = e, t.I(i, r)
+                            var n = "default",
+                                i = t.S[n];
+                            if (i && i !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => i,
                     init: () => a
                 })
             }
         },
-        m = {};
+        g = {};
 
-    function g(e) {
-        var r = m[e];
+    function b(e) {
+        var r = g[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, g), t.exports
+        return m[e](t, t.exports, b), t.exports
     }
-    g.m = v, g.c = m, g.n = e => {
-        var r = e && e.__esModule ? () => e.default : () => e;
-        return g.d(r, {
-            a: r
-        }), r
-    }, g.d = (e, r) => {
-        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
+    b.m = m, b.c = g, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".a075ebf77bc1145a8701.js?v=a075ebf77bc1145a8701", g.g = function() {
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + ".ad42dc24b11b936dd6c7.js?v=ad42dc24b11b936dd6c7", b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@timkpaine/jupyterlab_miami_nights:", g.l = (t, n, i, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@timkpaine/jupyterlab_miami_nights:", b.l = (t, n, i, a) => {
         if (e[t]) e[t].push(n);
         else {
             var o, u;
             if (void 0 !== i)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var p = l[s];
-                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + i) {
-                        o = p;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + i) {
+                        o = f;
                         break
                     }
                 }
-            o || (u = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, g.nc && o.setAttribute("nonce", g.nc), o.setAttribute("data-webpack", r + i), o.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    o.onerror = o.onload = null, clearTimeout(d);
+            o || (u = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, b.nc && o.setAttribute("nonce", b.nc), o.setAttribute("data-webpack", r + i), o.src = t), e[t] = [n];
+            var p = (r, n) => {
+                    o.onerror = o.onload = null, clearTimeout(h);
                     var i = e[t];
                     if (delete e[t], o.parentNode && o.parentNode.removeChild(o), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(f.bind(null, void 0, {
+                h = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), u && document.head.appendChild(o)
+            o.onerror = p.bind(null, o.onerror), o.onload = p.bind(null, o.onload), u && document.head.appendChild(o)
         }
-    }, g.r = e => {
-        "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
-            value: "Module"
-        }), Object.defineProperty(e, "__esModule", {
-            value: !0
-        })
     }, (() => {
-        g.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        g.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
-                g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
                     o = "@timkpaine/jupyterlab_miami_nights",
                     u = [];
-                switch (t) {
-                    case "default":
-                        ((e, r, t, n) => {
-                            var i = a[e] = a[e] || {},
-                                u = i[r];
-                            (!u || !u.loaded && (1 != !u.eager ? n : o > u.from)) && (i[r] = {
-                                get: () => g.e(568).then((() => () => g(568))),
-                                from: o,
-                                eager: !1
-                            })
-                        })("@timkpaine/jupyterlab_miami_nights", "0.3.2")
-                }
-                return e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && ((e, r, t, n) => {
+                    var i = a[e] = a[e] || {},
+                        u = i[r];
+                    (!u || !u.loaded && (1 != !u.eager ? n : o > u.from)) && (i[r] = {
+                        get: () => b.e(568).then((() => () => b(568))),
+                        from: o,
+                        eager: !1
+                    })
+                })("@timkpaine/jupyterlab_miami_nights", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        g.g.importScripts && (e = g.g.location + "");
-        var r = g.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -159,106 +145,111 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
             for (var o = 0, u = 1, l = !0;; u++, o++) {
-                var s, p, f = u < e.length ? (typeof e[u])[0] : "";
-                if (o >= r.length || "o" == (p = (typeof(s = r[o]))[0])) return !l || ("u" == f ? u > n && !i : "" == f != i);
-                if ("u" == p) {
-                    if (!l || "u" != f) return !1
+                var s, f, p = u < e.length ? (typeof e[u])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(s = r[o]))[0])) return !l || ("u" == p ? u > n && !i : "" == p != i);
+                if ("u" == f) {
+                    if (!l || "u" != p) return !1
                 } else if (l)
-                    if (f == p)
+                    if (p == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (i ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != p && "n" != p) {
                     if (i || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || p < f != i) return !1;
+                    if (u <= n || f < p != i) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var h = [],
+            c = h.pop.bind(h);
         for (o = 1; o < e.length; o++) {
-            var h = e[o];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            var d = e[o];
+            h.push(1 == d ? c() | c() : 2 == d ? c() & c() : d ? a(d, r) : !c())
         }
         return !!c()
     }, o = (e, r) => {
-        var t = g.S[e];
-        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + i(t) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", s = (e, r, t, n) => {
         var i = u(e, t);
-        return a(n, i) || "undefined" != typeof console && console.warn && console.warn(l(t, i, n)), p(e[t][i])
-    }, p = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, i) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, i)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (o(e, t), s(r, 0, t, n)))), d = {}, c = {
-        441: () => f("default", "@jupyterlab/apputils", [1, 3, 0, 5])
-    }, h = {
-        568: [441]
-    }, g.f.consumes = (e, r) => {
-        g.o(h, e) && h[e].forEach((e => {
-            if (g.o(d, e)) return r.push(d[e]);
+        return a(n, i) || f(l(e, t, i, n)), p(e[t][i])
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, p = e => (e.loaded = 1, e.get()), h = (e => function(r, t, n, i) {
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (o(e, t), s(r, 0, t, n)))), c = {}, d = {
+        172: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 3])
+    }, v = {
+        568: [172]
+    }, b.f.consumes = (e, r) => {
+        b.o(v, e) && v[e].forEach((e => {
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    d[e] = 0, g.m[e] = t => {
-                        delete g.c[e], t.exports = r()
+                    c[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete d[e], g.m[e] = t => {
-                        throw delete g.c[e], r
+                    delete c[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var i = c[e]();
-                i.then ? r.push(d[e] = i.then(t).catch(n)) : t(i)
+                var i = d[e]();
+                i.then ? r.push(c[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             69: 0
         };
-        g.f.j = (r, t) => {
-            var n = g.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var i = new Promise(((t, i) => n = e[r] = [t, i]));
                     t.push(n[2] = i);
-                    var a = g.p + g.u(r),
+                    var a = b.p + b.u(r),
                         o = new Error;
-                    g.l(a, (t => {
-                        if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    b.l(a, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var i = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             o.message = "Loading chunk " + r + " failed.\n(" + i + ": " + a + ")", o.name = "ChunkLoadError", o.type = i, o.request = a, n[1](o)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, i, [a, o, u] = t,
                     l = 0;
-                for (n in o) g.o(o, n) && (g.m[n] = o[n]);
-                for (u && u(g), r && r(t); l < a.length; l++) i = a[l], g.o(e, i) && e[i] && e[i][0](), e[a[l]] = 0
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in o) b.o(o, n) && (b.m[n] = o[n]);
+                    u && u(b)
+                }
+                for (r && r(t); l < a.length; l++) i = a[l], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunk_timkpaine_jupyterlab_miami_nights = self.webpackChunk_timkpaine_jupyterlab_miami_nights || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = g(43);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@timkpaine/jupyterlab_miami_nights"] = b
+    var y = b(39);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@timkpaine/jupyterlab_miami_nights"] = y
 })();
```

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/3b5adc929c114d1cd0fc91cd735847b6.ttf` & `jupyterlab_miami_nights-0.4.0/js/style/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/662254c8318cbac0ef3bcda7ad0df6ee.woff2` & `jupyterlab_miami_nights-0.4.0/js/style/Vibur.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/ff01975bdccf4187dc2b094650d0cf5e.ttf` & `jupyterlab_miami_nights-0.4.0/js/style/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.css` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -431,31 +431,31 @@
 /*-----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
 |----------------------------------------------------------------------------*/
 
 @font-face {
     font-family: 'Source Code Pro';
-    src: url(3b5adc929c114d1cd0fc91cd735847b6.ttf) format('truetype');
+    src: url(2967dd73df838d2a2d39.ttf) format('truetype');
     font-weight: 400;
     font-style: normal;
 }
 
 @font-face {
     font-family: 'Source Code Pro';
-    src: url(ff01975bdccf4187dc2b094650d0cf5e.ttf) format('truetype');
+    src: url(80922933add5aaad3870.ttf) format('truetype');
     font-weight: 700;
     font-style: normal;
 }
 
 @font-face {
     font-family: 'Vibur';
     font-style: normal;
     font-weight: 400;
-    src: local('Vibur'), url(662254c8318cbac0ef3bcda7ad0df6ee.woff2) format('woff2');
+    src: local('Vibur'), url(b5e5e677f7c3567440b0.woff2) format('woff2');
     unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
   }
 
 
 /* Fix layout color */
 body {
   line-height: 1.3077; /* 17px for 13px font */
@@ -540,16 +540,16 @@
 }
 
 ::-webkit-scrollbar-thumb:vertical:hover, ::-webkit-scrollbar-thumb:vertical:active {
   background: linear-gradient(to bottom, #fafc32, #f45959, #ef1eaf);
 }
 
 .widget-slider .ui-slider {
-  background: linear-gradient(to right, #fafc32, #f45959, #ef1eaf);
-  border-radius: 4px;
+  background: linear-gradient(to right, #fafc32, #f45959, #ef1eaf) !important;
+  border-radius: 4px !important;
 }
 
 /*Fix cursor of horizontal  scrollbar*/
 .CodeMirror-hscrollbar {
   cursor: auto;
 }
```

### Comparing `jupyterlab_miami_nights-0.3.2/package.json` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.698219696969697%*

 * *Differences: {"'author'": "'the jupyterlab_miami_nights authors'",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/apputils': '^4.1.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.2', 'eslint': '^8.44.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugin-prettier': '^5.0.0', "*

 * *                      "'prettier': '^3.0.0', 'rimraf': '^5.0.1', '@babel/cli': '^7.22.9', "*

 * *                      "'@babel/core': '^7.22.9', '@babel/eslint-parser': '^7.22.9', "*

 * *          […]*

```diff
@@ -1,95 +1,102 @@
 {
-    "author": {
-        "email": "",
-        "name": "Tim P <t.paine154@gmail.com>"
-    },
-    "bugs": {
-        "url": "https://github.com/timkpaine/jupyterlab_miami_nights/issues"
-    },
+    "author": "the jupyterlab_miami_nights authors",
     "dependencies": {
-        "@jupyterlab/application": "^3.0.11",
-        "@jupyterlab/apputils": "^3.0.9",
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/apputils": "^4.1.2",
         "highlight.js": "^10.4.1"
     },
     "description": "A glowing 80s theme based on Synthwave '84 and  JupyterLab's Neon Night theme by yeebc",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "base64-inline-loader": "^1.1.1",
-        "css-loader": "^5.0.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "mini-css-extract-plugin": "^1.3.3",
+        "@babel/cli": "^7.22.9",
+        "@babel/core": "^7.22.9",
+        "@babel/eslint-parser": "^7.22.9",
+        "@babel/preset-env": "^7.22.9",
+        "@jupyterlab/builder": "^4.0.2",
+        "babel-jest": "^29.6.1",
+        "cpx": "^1.5.0",
+        "eslint": "^8.44.0",
+        "eslint-config-airbnb": "^19.0.4",
+        "eslint-config-airbnb-base": "^15.0.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-import": "^2.27.5",
+        "eslint-plugin-jest": "^27.2.2",
+        "eslint-plugin-json": "^3.1.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "isomorphic-fetch": "^3.0.0",
+        "jest": "^29.6.1",
+        "jest-environment-jsdom": "^29.6.1",
+        "jest-junit": "^16.0.0",
+        "jest-transform-css": "^6.0.1",
+        "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typedoc": "^0.15.4",
-        "typescript": "~4.1.3",
-        "webpack": "^5.11.1",
-        "webpack-cli": "^4.3.1"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
         "lib/*.js",
         "lib/*.css",
         "style/*",
         "style/index.js"
     ],
-    "homepage": "https://github.com/timkpaine/jupyterlab_miami_nights",
     "jupyterlab": {
-        "extension": true,
-        "outputDir": "jupyterlab_miami_nights/labextension",
-        "themePath": "style/index.css"
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.504b42f0aac636b2716f.js"
+        },
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "jupyterlab_miami_nights"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
+        },
+        "extension": "lib/index.js",
+        "outputDir": "../jupyterlab_miami_nights/labextension",
+        "themePath": "lib/index.css"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "jupyterlab-theme",
         "neon",
         "cyberpunk"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@timkpaine/jupyterlab_miami_nights",
-    "publishConfig": {
-        "access": "public"
-    },
     "repository": {
         "type": "git",
-        "url": "https://github.com/timkpaine/jupyterlab_miami_nights.git"
+        "url": "https://github.com/finos/jupyterlab_templates.git"
     },
     "resolutions": {
-        "highlight.js": "^10.4.1"
+        "json5": "^2.2.3",
+        "sanitize-html": "^2.7.1",
+        "ws": "^7.4.6"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter labextension build .",
-        "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_miami_nights/labextension",
-        "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
+        "build": "npm-run-all clean build:*",
+        "build:babel": "babel src/ --source-maps --out-dir lib/",
+        "build:css": "cpx \"style/*\" \"lib/\"",
+        "build:lab": "rimraf ../jupyterlab_templates/labextension && jupyter labextension build .",
+        "clean": "rimraf lib ../jupyterlab_miami_nights/labextension",
+        "fix": "yarn lint --fix",
+        "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
-        "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_miami_nights-0.3.2/src/index.ts` & `jupyterlab_miami_nights-0.4.0/js/src/index.js`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,36 @@
-00000000: 696d 706f 7274 207b 0a20 204a 7570 7974  import {.  Jupyt
-00000010: 6572 4672 6f6e 7445 6e64 2c0a 2020 4a75  erFrontEnd,.  Ju
-00000020: 7079 7465 7246 726f 6e74 456e 6450 6c75  pyterFrontEndPlu
-00000030: 6769 6e0a 7d20 6672 6f6d 2027 406a 7570  gin.} from '@jup
-00000040: 7974 6572 6c61 622f 6170 706c 6963 6174  yterlab/applicat
-00000050: 696f 6e27 3b0a 0a69 6d70 6f72 7420 7b20  ion';..import { 
-00000060: 4954 6865 6d65 4d61 6e61 6765 7220 7d20  IThemeManager } 
-00000070: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
-00000080: 622f 6170 7075 7469 6c73 273b 0a0a 2f2a  b/apputils';../*
-00000090: 2a0a 202a 2041 2066 6c61 742c 2038 3027  *. * A flat, 80'
-000000a0: 7320 6e65 6f6e 2069 6e73 7069 7265 6420  s neon inspired 
-000000b0: 7468 656d 6520 666f 7220 4a75 7079 7465  theme for Jupyte
-000000c0: 724c 6162 2e0a 202a 2f0a 636f 6e73 7420  rLab.. */.const 
-000000d0: 706c 7567 696e 3a20 4a75 7079 7465 7246  plugin: JupyterF
-000000e0: 726f 6e74 456e 6450 6c75 6769 6e3c 766f  rontEndPlugin<vo
-000000f0: 6964 3e20 3d20 7b0a 2020 6964 3a20 2740  id> = {.  id: '@
-00000100: 7469 6d6b 7061 696e 652f 6a75 7079 7465  timkpaine/jupyte
-00000110: 726c 6162 5f6d 6961 6d69 5f6e 6967 6874  rlab_miami_night
-00000120: 733a 706c 7567 696e 272c 0a20 2072 6571  s:plugin',.  req
-00000130: 7569 7265 733a 205b 4954 6865 6d65 4d61  uires: [IThemeMa
-00000140: 6e61 6765 725d 2c0a 2020 6163 7469 7661  nager],.  activa
-00000150: 7465 3a20 2861 7070 3a20 4a75 7079 7465  te: (app: Jupyte
-00000160: 7246 726f 6e74 456e 642c 206d 616e 6167  rFrontEnd, manag
-00000170: 6572 3a20 4954 6865 6d65 4d61 6e61 6765  er: IThemeManage
-00000180: 7229 203d 3e20 7b0a 2020 2020 636f 6e73  r) => {.    cons
-00000190: 7420 7374 796c 6520 3d20 2740 7469 6d6b  t style = '@timk
-000001a0: 7061 696e 652f 6a75 7079 7465 726c 6162  paine/jupyterlab
-000001b0: 5f6d 6961 6d69 5f6e 6967 6874 732f 696e  _miami_nights/in
-000001c0: 6465 782e 6373 7327 3b0a 0a20 2020 206d  dex.css';..    m
-000001d0: 616e 6167 6572 2e72 6567 6973 7465 7228  anager.register(
-000001e0: 7b0a 2020 2020 2020 6e61 6d65 3a20 274a  {.      name: 'J
-000001f0: 7570 7974 6572 4c61 6220 4d69 616d 6920  upyterLab Miami 
-00000200: 4e69 6768 7473 272c 0a20 2020 2020 2069  Nights',.      i
-00000210: 734c 6967 6874 3a20 6661 6c73 652c 0a20  sLight: false,. 
-00000220: 2020 2020 2074 6865 6d65 5363 726f 6c6c       themeScroll
-00000230: 6261 7273 3a20 7472 7565 2c0a 2020 2020  bars: true,.    
-00000240: 2020 6c6f 6164 3a20 2829 203d 3e20 6d61    load: () => ma
-00000250: 6e61 6765 722e 6c6f 6164 4353 5328 7374  nager.loadCSS(st
-00000260: 796c 6529 2c0a 2020 2020 2020 756e 6c6f  yle),.      unlo
-00000270: 6164 3a20 2829 203d 3e20 5072 6f6d 6973  ad: () => Promis
-00000280: 652e 7265 736f 6c76 6528 756e 6465 6669  e.resolve(undefi
-00000290: 6e65 6429 0a20 2020 207d 293b 0a20 207d  ned).    });.  }
-000002a0: 2c0a 2020 6175 746f 5374 6172 743a 2074  ,.  autoStart: t
-000002b0: 7275 650a 7d3b 0a0a 6578 706f 7274 2064  rue.};..export d
-000002c0: 6566 6175 6c74 2070 6c75 6769 6e3b 0a    efault plugin;.
+00000000: 696d 706f 7274 207b 4954 6865 6d65 4d61  import {IThemeMa
+00000010: 6e61 6765 727d 2066 726f 6d20 2240 6a75  nager} from "@ju
+00000020: 7079 7465 726c 6162 2f61 7070 7574 696c  pyterlab/apputil
+00000030: 7322 3b0a 0a2f 2a2a 0a20 2a20 4120 666c  s";../**. * A fl
+00000040: 6174 2c20 3830 2773 206e 656f 6e20 696e  at, 80's neon in
+00000050: 7370 6972 6564 2074 6865 6d65 2066 6f72  spired theme for
+00000060: 204a 7570 7974 6572 4c61 622e 0a20 2a2f   JupyterLab.. */
+00000070: 0a63 6f6e 7374 2070 6c75 6769 6e20 3d20  .const plugin = 
+00000080: 7b0a 2020 6964 3a20 2240 7469 6d6b 7061  {.  id: "@timkpa
+00000090: 696e 652f 6a75 7079 7465 726c 6162 5f6d  ine/jupyterlab_m
+000000a0: 6961 6d69 5f6e 6967 6874 733a 706c 7567  iami_nights:plug
+000000b0: 696e 222c 0a20 2072 6571 7569 7265 733a  in",.  requires:
+000000c0: 205b 4954 6865 6d65 4d61 6e61 6765 725d   [IThemeManager]
+000000d0: 2c0a 2020 6163 7469 7661 7465 3a20 2861  ,.  activate: (a
+000000e0: 7070 2c20 6d61 6e61 6765 7229 203d 3e20  pp, manager) => 
+000000f0: 7b0a 2020 2020 636f 6e73 7420 7374 796c  {.    const styl
+00000100: 6520 3d20 2240 7469 6d6b 7061 696e 652f  e = "@timkpaine/
+00000110: 6a75 7079 7465 726c 6162 5f6d 6961 6d69  jupyterlab_miami
+00000120: 5f6e 6967 6874 732f 696e 6465 782e 6373  _nights/index.cs
+00000130: 7322 3b0a 0a20 2020 206d 616e 6167 6572  s";..    manager
+00000140: 2e72 6567 6973 7465 7228 7b0a 2020 2020  .register({.    
+00000150: 2020 6e61 6d65 3a20 224a 7570 7974 6572    name: "Jupyter
+00000160: 4c61 6220 4d69 616d 6920 4e69 6768 7473  Lab Miami Nights
+00000170: 222c 0a20 2020 2020 2069 734c 6967 6874  ",.      isLight
+00000180: 3a20 6661 6c73 652c 0a20 2020 2020 2074  : false,.      t
+00000190: 6865 6d65 5363 726f 6c6c 6261 7273 3a20  hemeScrollbars: 
+000001a0: 7472 7565 2c0a 2020 2020 2020 6c6f 6164  true,.      load
+000001b0: 3a20 2829 203d 3e20 6d61 6e61 6765 722e  : () => manager.
+000001c0: 6c6f 6164 4353 5328 7374 796c 6529 2c0a  loadCSS(style),.
+000001d0: 2020 2020 2020 756e 6c6f 6164 3a20 2829        unload: ()
+000001e0: 203d 3e20 5072 6f6d 6973 652e 7265 736f   => Promise.reso
+000001f0: 6c76 6528 756e 6465 6669 6e65 6429 2c0a  lve(undefined),.
+00000200: 2020 2020 7d29 3b0a 2020 7d2c 0a20 2061      });.  },.  a
+00000210: 7574 6f53 7461 7274 3a20 7472 7565 2c0a  utoStart: true,.
+00000220: 7d3b 0a0a 6578 706f 7274 2064 6566 6175  };..export defau
+00000230: 6c74 2070 6c75 6769 6e3b 0a              lt plugin;.
```

### Comparing `jupyterlab_miami_nights-0.3.2/style/custom.css` & `jupyterlab_miami_nights-0.4.0/js/style/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/style/fonts/SourceCodePro-Bold.ttf` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/80922933add5aaad3870.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/style/fonts/SourceCodePro-Regular.ttf` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/2967dd73df838d2a2d39.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/style/fonts/Vibur.woff2` & `jupyterlab_miami_nights-0.4.0/jupyterlab_miami_nights/labextension/themes/@timkpaine/jupyterlab_miami_nights/b5e5e677f7c3567440b0.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/style/fonts.css` & `jupyterlab_miami_nights-0.4.0/js/style/fonts.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 /*-----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
 |----------------------------------------------------------------------------*/
 
 @font-face {
     font-family: 'Source Code Pro';
-    src: url('fonts/SourceCodePro-Regular.ttf') format('truetype');
+    src: url('SourceCodePro-Regular.ttf') format('truetype');
     font-weight: 400;
     font-style: normal;
 }
 
 @font-face {
     font-family: 'Source Code Pro';
-    src: url('fonts/SourceCodePro-Bold.ttf') format('truetype');
+    src: url('SourceCodePro-Bold.ttf') format('truetype');
     font-weight: 700;
     font-style: normal;
 }
 
 @font-face {
     font-family: 'Vibur';
     font-style: normal;
     font-weight: 400;
-    src: local('Vibur'), url('fonts/Vibur.woff2') format('woff2');
+    src: local('Vibur'), url('Vibur.woff2') format('woff2');
     unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
   }
```

### Comparing `jupyterlab_miami_nights-0.3.2/style/neondreams.css` & `jupyterlab_miami_nights-0.4.0/js/style/neondreams.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_miami_nights-0.3.2/style/style.css` & `jupyterlab_miami_nights-0.4.0/js/style/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 }
 
 ::-webkit-scrollbar-thumb:vertical:hover, ::-webkit-scrollbar-thumb:vertical:active {
   background: linear-gradient(to bottom, #fafc32, #f45959, #ef1eaf);
 }
 
 .widget-slider .ui-slider {
-  background: linear-gradient(to right, #fafc32, #f45959, #ef1eaf);
-  border-radius: 4px;
+  background: linear-gradient(to right, #fafc32, #f45959, #ef1eaf) !important;
+  border-radius: 4px !important;
 }
 
 /*Fix cursor of horizontal  scrollbar*/
 .CodeMirror-hscrollbar {
   cursor: auto;
 }
```

### Comparing `jupyterlab_miami_nights-0.3.2/style/variables.css` & `jupyterlab_miami_nights-0.4.0/js/style/variables.css`

 * *Files identical despite different names*

