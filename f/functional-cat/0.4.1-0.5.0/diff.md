# Comparing `tmp/functional-cat-0.4.1.tar.gz` & `tmp/functional-cat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functional-cat-0.4.1.tar", last modified: Mon Jul 10 17:57:19 2023, max compression
+gzip compressed data, was "functional-cat-0.5.0.tar", last modified: Thu Aug  3 02:17:16 2023, max compression
```

## Comparing `functional-cat-0.4.1.tar` & `functional-cat-0.5.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.406034 functional-cat-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.394034 functional-cat-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.394034 functional-cat-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/docker-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/test-catalog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Dockerfile.glip
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-10 17:57:08.000000 functional-cat-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 17:57:19.406034 functional-cat-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 17:57:08.000000 functional-cat-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-10 17:57:08.000000 functional-cat-0.4.1/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/dlib/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/dlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/dlib/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/glip/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/glip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/glip/glip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/tiny_yolov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/yolov4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/torchvision/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 17:57:08.000000 functional-cat-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/sample_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    60686 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   123080 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/gang.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    67910 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/letter_box.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/mona_lisa.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/street_sign.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:57:19.406034 functional-cat-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 17:57:08.000000 functional-cat-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_dlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.402034 functional-cat-0.4.1/web/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/.env
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/create_tasks_and_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/netlify.toml
--rw-r--r--   0 runner    (1001) docker     (123)  1237799 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.402034 functional-cat-0.4.1/web/public/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/_redirects
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)    79636 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.406034 functional-cat-0.4.1/web/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/AboutPage.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/FuncGrid.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/Header.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/HomePage.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/TasksPage.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/TypesPage.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/Wrapper.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/func.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    34380 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/funcs.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/pythonClassMeta.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/reportWebVitals.ts
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/setupTests.ts
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.068830 functional-cat-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.056830 functional-cat-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.056830 functional-cat-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.github/workflows/docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.github/workflows/test-catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.github/workflows/unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 02:17:06.000000 functional-cat-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-03 02:17:06.000000 functional-cat-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-03 02:17:06.000000 functional-cat-0.5.0/Dockerfile.glip
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-03 02:17:06.000000 functional-cat-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 02:17:06.000000 functional-cat-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 02:17:16.068830 functional-cat-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 02:17:06.000000 functional-cat-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-08-03 02:17:06.000000 functional-cat-0.5.0/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/funcs/dlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/dlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/dlib/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/funcs/glip/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/glip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/glip/glip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/funcs/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/onnx/tiny_yolov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/onnx/yolov4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat/funcs/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-08-03 02:17:06.000000 functional-cat-0.5.0/functional_cat/funcs/torchvision/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-03 02:17:07.000000 functional-cat-0.5.0/functional_cat/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-03 02:17:07.000000 functional-cat-0.5.0/functional_cat/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-08-03 02:17:07.000000 functional-cat-0.5.0/functional_cat/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/functional_cat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 02:17:16.000000 functional-cat-0.5.0/functional_cat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-03 02:17:16.000000 functional-cat-0.5.0/functional_cat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:17:16.000000 functional-cat-0.5.0/functional_cat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-03 02:17:16.000000 functional-cat-0.5.0/functional_cat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 02:17:16.000000 functional-cat-0.5.0/functional_cat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-03 02:17:07.000000 functional-cat-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/sample_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    60686 2023-08-03 02:17:07.000000 functional-cat-0.5.0/sample_imgs/cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   123080 2023-08-03 02:17:07.000000 functional-cat-0.5.0/sample_imgs/gang.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    67910 2023-08-03 02:17:07.000000 functional-cat-0.5.0/sample_imgs/letter_box.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-08-03 02:17:07.000000 functional-cat-0.5.0/sample_imgs/mona_lisa.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-08-03 02:17:07.000000 functional-cat-0.5.0/sample_imgs/street_sign.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 02:17:16.068830 functional-cat-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 02:17:07.000000 functional-cat-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.060830 functional-cat-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-03 02:17:07.000000 functional-cat-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 02:17:07.000000 functional-cat-0.5.0/tests/test_dlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-03 02:17:07.000000 functional-cat-0.5.0/tests/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 02:17:07.000000 functional-cat-0.5.0/tests/test_torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.064830 functional-cat-0.5.0/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/.env
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/create_tasks_and_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/netlify.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  1237799 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.064830 functional-cat-0.5.0/web/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/_redirects
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79636 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:17:16.068830 functional-cat-0.5.0/web/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/AboutPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/App.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/FuncGrid.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/Header.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/HomePage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/TasksPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/TypesPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/Wrapper.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/func.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    34380 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/funcs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/pythonClassMeta.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/reportWebVitals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/src/setupTests.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 02:17:07.000000 functional-cat-0.5.0/web/tsconfig.json
```

### Comparing `functional-cat-0.4.1/.github/workflows/docker-image.yml` & `functional-cat-0.5.0/.github/workflows/docker-image.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 on:
   push:
     paths:
       - functional_cat/**
       - setup.py
       - pyproject.toml
       - Dockerfile
+      - Dockerfile.glip
       - .github/workflows/docker-image.yml
     branches: [main]
 
 jobs:
   build-docker:
     runs-on: ubuntu-latest
     env:
       IMAGE_NAME: ghcr.io/ekorman/functional-cat/functional-cat
       IMAGE_NAME_WITH_COMMIT_HASH: $IMAGE_NAME:${{ github.sha }}
     steps:
       - uses: actions/checkout@v3
       - name: build
         run: |
-          docker build . --build-arg packages="[torch,onnx-gpu]" -t $IMAGE_NAME
+          pip3 install setuptools_scm
+          docker build . --build-arg packages="[torch,onnx-gpu]" --build-arg VERSION=$(python -m setuptools_scm) -t $IMAGE_NAME
       - name: push
         run: |
           docker login ghcr.io -u ${{ github.actor }} -p ${{ secrets.GITHUB_TOKEN }}
           docker push $IMAGE_NAME
           IMAGE_NAME_WITH_COMMIT_HASH=$IMAGE_NAME:${{ github.sha }}
           docker tag $IMAGE_NAME $IMAGE_NAME_WITH_COMMIT_HASH
           docker push $IMAGE_NAME_WITH_COMMIT_HASH
@@ -32,15 +34,16 @@
     runs-on: ubuntu-latest
     env:
       IMAGE_NAME: ghcr.io/ekorman/functional-cat/functional-cat-glip
     steps:
       - uses: actions/checkout@v3
       - name: build
         run: |
-          docker build . -f Dockerfile.glip -t $IMAGE_NAME
+          pip3 install setuptools_scm
+          docker build . --build-arg VERSION=$(python -m setuptools_scm) -f Dockerfile.glip -t $IMAGE_NAME
       - name: push
         run: |
           docker login ghcr.io -u ${{ github.actor }} -p ${{ secrets.GITHUB_TOKEN }}
           docker push $IMAGE_NAME
           IMAGE_NAME_WITH_COMMIT_HASH=$IMAGE_NAME:${{ github.sha }}
           docker tag $IMAGE_NAME $IMAGE_NAME_WITH_COMMIT_HASH
           docker push $IMAGE_NAME_WITH_COMMIT_HASH
```

### Comparing `functional-cat-0.4.1/.github/workflows/test-catalog.yml` & `functional-cat-0.5.0/.github/workflows/test-catalog.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # regenerates funcs file (except for example image and except for glip) and
 # checks that git diff is 0
 name: Check catalog is up-to-date
 
-on: push
+on:
+  push:
+    paths:
+      - functional_cat/**
+      - setup.py
+      - pyproject.toml
 
 jobs:
   check-catalog:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.8"
       - run: pip install ".[torch,onnx,catalog,dlib]"
-      - run: python catalog.py create --overwrite-if-exists --frameworks torch,onnx,dlib --fields class,constructorArgs,description,task,framework,installSnippet,devices,classLabels,colabLink
+      - run: python catalog.py create --overwrite-if-exists --frameworks torch,onnx --fields class,constructorArgs,description,task,framework,installSnippet,devices,classLabels,colabLink
       - run: git diff --exit-code
```

### Comparing `functional-cat-0.4.1/.pre-commit-config.yaml` & `functional-cat-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/Dockerfile` & `functional-cat-0.5.0/Dockerfile`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-FROM nvidia/cuda:10.2-devel-ubuntu18.04
+FROM nvidia/cuda:12.2.0-devel-ubuntu22.04
 
 ARG packages
+ARG VERSION
 
+ENV DEBIAN_FRONTEND=noninteractive 
 ENV CUDA_HOME=/usr/local/cuda
 ENV PATH=${CUDA_HOME}/bin:${PATH}
 ENV LD_LIBRARY_PATH=${CUDA_HOME}/lib64:$LD_LIBRARY_PATH
 
 RUN apt update
-RUN apt install -y wget software-properties-common
-RUN add-apt-repository ppa:deadsnakes/ppa
-RUN apt install -y python3.8 python3-pip python3.8-dev
-
-RUN wget https://bootstrap.pypa.io/get-pip.py
-RUN python3.8 get-pip.py
+RUN apt install python3 python3-pip -y
 
 COPY ./setup.py /functional-cat/setup.py
 COPY ./pyproject.toml /functional-cat/pyproject.toml
 COPY ./functional_cat /functional-cat/functional_cat
 
 WORKDIR /functional-cat
-RUN pip3.8 install ".${packages}"
+RUN SETUPTOOLS_SCM_PRETEND_VERSION=${VERSION} pip3 install ".${packages}"
 
 RUN apt-get update
 RUN apt-get install ffmpeg libsm6 libxext6  -y
 
-RUN alias pip=pip3.8
 WORKDIR /
 
 SHELL ["/bin/bash", "-c"]
```

### Comparing `functional-cat-0.4.1/LICENSE` & `functional-cat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/PKG-INFO` & `functional-cat-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional-cat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Catalog of functions
 License: Copyright 2022 Eric O. Korman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `functional-cat-0.4.1/catalog.py` & `functional-cat-0.5.0/catalog.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/data_types.py` & `functional-cat-0.5.0/functional_cat/data_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,14 +148,28 @@
         return Detection(
             boundary=self.boundary.int(),
             class_label=self.class_label,
             score=self.score,
         )
 
 
+def draw_mask_on_image(
+    img: Image.Image, mask: MaskType, color: Tuple[int, int, int]
+) -> None:
+    bin_mask = np.array(mask) > 0.5
+
+    mask_arr = np.zeros(
+        (bin_mask.shape[0], bin_mask.shape[1], 3), dtype=np.uint8
+    )
+    mask_arr[bin_mask] = color
+    mask_img = Image.fromarray(mask_arr)
+    blend = Image.blend(img, mask_img, alpha=0.4)
+    img.paste(blend, (0, 0), mask=Image.fromarray(bin_mask))
+
+
 @dataclass
 class InstanceSegmentation(Detection):
     mask: MaskType
 
     def draw_on_image(
         self,
         img: Image.Image,
@@ -166,23 +180,15 @@
     ) -> Image.Image:
         if draw_bbox:
             img = super().draw_on_image(img, inplace, color=color)
         else:
             img = img if inplace else img.copy()
 
         if draw_mask:
-            bin_mask = np.array(self.mask) > 0.5
-
-            mask_arr = np.zeros(
-                (bin_mask.shape[0], bin_mask.shape[1], 3), dtype=np.uint8
-            )
-            mask_arr[bin_mask] = color
-            mask_img = Image.fromarray(mask_arr)
-            blend = Image.blend(img, mask_img, alpha=0.4)
-            img.paste(blend, (0, 0), mask=Image.fromarray(bin_mask))
+            draw_mask_on_image(img, self.mask, color)
 
         return img
 
 
 @dataclass
 class Keypoint:
     class_label: str
```

### Comparing `functional-cat-0.4.1/functional_cat/funcs/dlib/detection.py` & `functional-cat-0.5.0/functional_cat/funcs/dlib/detection.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/funcs/glip/glip.py` & `functional-cat-0.5.0/functional_cat/funcs/glip/glip.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/funcs/onnx/tiny_yolov3.py` & `functional-cat-0.5.0/functional_cat/funcs/onnx/tiny_yolov3.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/funcs/onnx/yolov4.py` & `functional-cat-0.5.0/functional_cat/funcs/onnx/yolov4.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/funcs/torchvision/__init__.py` & `functional-cat-0.5.0/functional_cat/funcs/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/funcs/torchvision/detection.py` & `functional-cat-0.5.0/functional_cat/funcs/torchvision/detection.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,16 +147,23 @@
 
 
 def torch_box_to_boundary(box: torch.Tensor) -> BoundingPolygon:
     return BoundingPolygon.from_bbox(*box.cpu().tolist())
 
 
 class TorchvisionDetector(ObjectDetector):
-    def __init__(self, model_name: str):
-        self.device = "cuda" if torch.cuda.is_available() else "cpu"
+    def __init__(self, model_name: str, device: str = None):
+        if device is None:
+            if torch.cuda.is_available():
+                device = "cuda"
+            elif torch.backends.mps.is_available():
+                device = "mps"
+            else:
+                device = "cpu"
+        self.device = device
         if model_name not in MODEL_NAME_TO_WEIGHTS:
             raise ValueError(
                 f"Got invalid `model_name`: {model_name}. Available "
                 f"models are {list(MODEL_NAME_TO_WEIGHTS.keys())}"
             )
         self.model = (
             getattr(detection, model_name)(
```

### Comparing `functional-cat-0.4.1/functional_cat/interfaces.py` & `functional-cat-0.5.0/functional_cat/interfaces.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/io.py` & `functional-cat-0.5.0/functional_cat/io.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat/registry.py` & `functional-cat-0.5.0/functional_cat/registry.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/functional_cat.egg-info/PKG-INFO` & `functional-cat-0.5.0/functional_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional-cat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Catalog of functions
 License: Copyright 2022 Eric O. Korman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `functional-cat-0.4.1/functional_cat.egg-info/SOURCES.txt` & `functional-cat-0.5.0/functional_cat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/pyproject.toml` & `functional-cat-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "functional-cat"
 dynamic = ["version"]
 description = "Catalog of functions"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
-dependencies = ["requests", "Pillow >= 9.1.0", "tqdm", "numpy >= 1.23"]
+dependencies = ["requests", "Pillow >= 9.1.0,<=9.5.0", "tqdm", "numpy >= 1.23"]
 
 [build-system]
 requires =  ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 torch = [
```

### Comparing `functional-cat-0.4.1/sample_imgs/cat.jpg` & `functional-cat-0.5.0/sample_imgs/cat.jpg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/sample_imgs/gang.jpg` & `functional-cat-0.5.0/sample_imgs/gang.jpg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/sample_imgs/letter_box.jpg` & `functional-cat-0.5.0/sample_imgs/letter_box.jpg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/sample_imgs/mona_lisa.jpeg` & `functional-cat-0.5.0/sample_imgs/mona_lisa.jpeg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/sample_imgs/street_sign.jpg` & `functional-cat-0.5.0/sample_imgs/street_sign.jpg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/tests/conftest.py` & `functional-cat-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/tests/test_dlib.py` & `functional-cat-0.5.0/tests/test_dlib.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/tests/test_onnx.py` & `functional-cat-0.5.0/tests/test_onnx.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/tests/test_torchvision.py` & `functional-cat-0.5.0/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/README.md` & `functional-cat-0.5.0/web/README.md`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/create_tasks_and_types.py` & `functional-cat-0.5.0/web/create_tasks_and_types.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/package-lock.json` & `functional-cat-0.5.0/web/package-lock.json`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/package.json` & `functional-cat-0.5.0/web/package.json`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/public/apple-touch-icon.png` & `functional-cat-0.5.0/web/public/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/public/favicon.ico` & `functional-cat-0.5.0/web/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/public/index.html` & `functional-cat-0.5.0/web/public/index.html`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/public/logo192.png` & `functional-cat-0.5.0/web/public/logo192.png`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/public/logo512.png` & `functional-cat-0.5.0/web/public/logo512.png`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/AboutPage.tsx` & `functional-cat-0.5.0/web/src/AboutPage.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/App.css` & `functional-cat-0.5.0/web/src/App.css`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/App.tsx` & `functional-cat-0.5.0/web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/FuncGrid.tsx` & `functional-cat-0.5.0/web/src/FuncGrid.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/Header.tsx` & `functional-cat-0.5.0/web/src/Header.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/HomePage.tsx` & `functional-cat-0.5.0/web/src/HomePage.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/func.tsx` & `functional-cat-0.5.0/web/src/func.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/funcs.json` & `functional-cat-0.5.0/web/src/funcs.json`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/logo.svg` & `functional-cat-0.5.0/web/src/logo.svg`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/src/pythonClassMeta.tsx` & `functional-cat-0.5.0/web/src/pythonClassMeta.tsx`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.1/web/tsconfig.json` & `functional-cat-0.5.0/web/tsconfig.json`

 * *Files identical despite different names*

