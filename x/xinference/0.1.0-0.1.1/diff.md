# Comparing `tmp/xinference-0.1.0.tar.gz` & `tmp/xinference-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.1.0.tar", last modified: Fri Jul 28 13:13:48 2023, max compression
+gzip compressed data, was "xinference-0.1.1.tar", last modified: Thu Aug  3 15:48:28 2023, max compression
```

## Comparing `xinference-0.1.0.tar` & `xinference-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 13:13:39.000000 xinference-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 13:13:39.000000 xinference-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-28 13:13:48.451522 xinference-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 13:13:39.000000 xinference-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-28 13:13:39.000000 xinference-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-28 13:13:48.455522 xinference-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-28 13:13:39.000000 xinference-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-28 13:13:39.000000 xinference-0.1.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.455522 xinference-0.1.0/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 13:13:48.455522 xinference-0.1.0/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/ggml/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/llm_family.json
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/llm_family.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.264840 xinference-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-03 15:48:14.000000 xinference-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 15:48:14.000000 xinference-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-08-03 15:48:28.264840 xinference-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-08-03 15:48:14.000000 xinference-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-03 15:48:14.000000 xinference-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-03 15:48:28.264840 xinference-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-03 15:48:14.000000 xinference-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-08-03 15:48:14.000000 xinference-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.264840 xinference-0.1.1/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 15:48:28.264840 xinference-0.1.1/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25159 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20309 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/core/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.264840 xinference-0.1.1/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.264840 xinference-0.1.1/xinference/model/llm/ggml/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/ggml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/ggml/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/ggml/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/llm_family.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/llm_family.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.264840 xinference-0.1.1/xinference/model/llm/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/pytorch/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/model/llm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-03 15:48:14.000000 xinference-0.1.1/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:48:28.260840 xinference-0.1.1/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:48:27.000000 xinference-0.1.1/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 15:48:28.000000 xinference-0.1.1/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.1.0/LICENSE` & `xinference-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/PKG-INFO` & `xinference-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: ggml
 Provides-Extra: pytorch
 Provides-Extra: doc
+Provides-Extra: benchmark
 License-File: LICENSE
 
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.1.0 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.1.1 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
-Extra: ggml Provides-Extra: pytorch Provides-Extra: doc License-File: LICENSE
+Extra: ggml Provides-Extra: pytorch Provides-Extra: doc Provides-Extra:
+benchmark License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
```

### Comparing `xinference-0.1.0/README.md` & `xinference-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/setup.cfg` & `xinference-0.1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -65,30 +65,35 @@
 	transformers>=4.31.0
 	torch
 	accelerate>=0.20.3
 	sentencepiece
 	transformers_stream_generator
 	bitsandbytes
 	protobuf
+	einops
 ggml = 
 	chatglm-cpp
 	llama-cpp-python>=0.1.77
 pytorch = 
 	transformers>=4.31.0
 	torch
 	accelerate>=0.20.3
 	sentencepiece
 	transformers_stream_generator
 	bitsandbytes
 	protobuf
+	einops
 doc = 
 	ipython>=6.5.0
 	sphinx>=3.0.0,<5.0.0
 	pydata-sphinx-theme>=0.3.0
 	sphinx-intl>=0.9.9
+benchmark = 
+	psutil
+	pynvml
 
 [options.entry_points]
 console_scripts = 
 	xinference = xinference.deploy.cmdline:cli
 	xinference-supervisor = xinference.deploy.cmdline:supervisor
 	xinference-worker = xinference.deploy.cmdline:worker
```

### Comparing `xinference-0.1.0/setup.py` & `xinference-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/versioneer.py` & `xinference-0.1.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/__init__.py` & `xinference-0.1.1/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/constants.py` & `xinference-0.1.1/xinference/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 XINFERENCE_HOME = str(Path.home() / ".xinference")
 XINFERENCE_CACHE_DIR = os.path.join(XINFERENCE_HOME, "cache")
 XINFERENCE_LOG_DIR = os.path.join(XINFERENCE_HOME, "logs")
 
 XINFERENCE_DEFAULT_LOCAL_HOST = "127.0.0.1"
 XINFERENCE_DEFAULT_DISTRIBUTED_HOST = "0.0.0.0"
 XINFERENCE_DEFAULT_ENDPOINT_PORT = 9997
+XINFERENCE_ENV_ENDPOINT = "XINFERENCE_ENDPOINT"
```

### Comparing `xinference-0.1.0/xinference/core/__init__.py` & `xinference-0.1.1/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/core/api.py` & `xinference-0.1.1/xinference/core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import asyncio
 from typing import Any, Dict, Optional
 
 import xoscar as xo
 
 from ..isolation import Isolation
 from . import ModelActor
-from .service import SupervisorActor
+from .supervisor import SupervisorActor
 
 
 class AsyncSupervisorAPI:
     def __init__(self, supervisor_address: str):
         self._supervisor_address = supervisor_address
         self._supervisor_ref = None
```

### Comparing `xinference-0.1.0/xinference/core/gradio.py` & `xinference-0.1.1/xinference/core/gradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from ..types import ChatCompletionChunk, ChatCompletionMessage
 
 MODEL_TO_FAMILIES: Dict[str, LLMFamilyV1] = dict(
     (model_family.model_name, model_family)
     for model_family in LLM_FAMILIES
-    if model_family.model_name not in ["baichuan", "baichuan-base", "llama-2"]
+    if "chat" in model_family.model_ability
 )
 
 
 class GradioApp:
     def __init__(
         self,
         supervisor_address: str,
```

### Comparing `xinference-0.1.0/xinference/core/model.py` & `xinference-0.1.1/xinference/core/model.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/core/resource.py` & `xinference-0.1.1/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/core/restful_api.py` & `xinference-0.1.1/xinference/core/restful_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, Field
 from sse_starlette.sse import EventSourceResponse
 from typing_extensions import NotRequired, TypedDict
 from uvicorn import Config, Server
 
 from ..types import ChatCompletion, Completion, Embedding
-from .service import SupervisorActor
+from .supervisor import SupervisorActor
 
 logger = logging.getLogger(__name__)
 
 max_tokens_field = Field(
     default=128, ge=1, le=2048, description="The maximum number of tokens to generate."
 )
```

### Comparing `xinference-0.1.0/xinference/deploy/__init__.py` & `xinference-0.1.1/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/deploy/cmdline.py` & `xinference-0.1.1/xinference/deploy/cmdline.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
+import os
+from typing import Optional
 
 import click
 from xoscar.utils import get_next_port
 
 from .. import __version__
 from ..client import RESTfulClient
 from ..constants import (
     XINFERENCE_DEFAULT_DISTRIBUTED_HOST,
     XINFERENCE_DEFAULT_ENDPOINT_PORT,
     XINFERENCE_DEFAULT_LOCAL_HOST,
+    XINFERENCE_ENV_ENDPOINT,
 )
 
 
+def get_endpoint(endpoint: Optional[str]) -> str:
+    # user didn't specify the endpoint.
+    if endpoint is None:
+        if XINFERENCE_ENV_ENDPOINT in os.environ:
+            return os.environ[XINFERENCE_ENV_ENDPOINT]
+        else:
+            default_endpoint = f"http://{XINFERENCE_DEFAULT_LOCAL_HOST}:{XINFERENCE_DEFAULT_ENDPOINT_PORT}"
+            return default_endpoint
+    else:
+        return endpoint
+
+
 @click.group(invoke_without_command=True, name="xinference")
 @click.pass_context
 @click.version_option(__version__, "--version", "-v")
 @click.option("--log-level", default="INFO", type=str)
 @click.option("--host", "-H", default=XINFERENCE_DEFAULT_LOCAL_HOST, type=str)
 @click.option("--port", "-p", default=XINFERENCE_DEFAULT_ENDPOINT_PORT, type=int)
 def cli(
@@ -77,25 +92,26 @@
 
 
 @click.command()
 @click.option("--log-level", default="INFO", type=str)
 @click.option(
     "--endpoint",
     "-e",
-    default=f"http://{XINFERENCE_DEFAULT_LOCAL_HOST}:{XINFERENCE_DEFAULT_ENDPOINT_PORT}",
     type=str,
 )
 @click.option("--host", "-H", default=XINFERENCE_DEFAULT_DISTRIBUTED_HOST, type=str)
-def worker(log_level: str, endpoint: str, host: str):
+def worker(log_level: str, endpoint: Optional[str], host: str):
     from ..deploy.worker import main
 
     if log_level:
         logging.basicConfig(level=logging.getLevelName(log_level.upper()))
     logging_conf = dict(level=log_level.upper())
 
+    endpoint = get_endpoint(endpoint)
+
     client = RESTfulClient(base_url=endpoint)
     supervisor_internal_addr = client._get_supervisor_internal_address()
 
     address = f"{host}:{get_next_port()}"
     main(
         address=address,
         supervisor_address=supervisor_internal_addr,
@@ -103,28 +119,29 @@
     )
 
 
 @cli.command("launch")
 @click.option(
     "--endpoint",
     "-e",
-    default=f"http://{XINFERENCE_DEFAULT_LOCAL_HOST}:{XINFERENCE_DEFAULT_ENDPOINT_PORT}",
     type=str,
 )
 @click.option("--model-name", "-n", type=str)
 @click.option("--size-in-billions", "-s", default=None, type=int)
 @click.option("--model-format", "-f", default=None, type=str)
 @click.option("--quantization", "-q", default=None, type=str)
 def model_launch(
-    endpoint: str,
+    endpoint: Optional[str],
     model_name: str,
     size_in_billions: int,
     model_format: str,
     quantization: str,
 ):
+    endpoint = get_endpoint(endpoint)
+
     client = RESTfulClient(base_url=endpoint)
     model_uid = client.launch_model(
         model_name=model_name,
         model_size_in_billions=size_in_billions,
         model_format=model_format,
         quantization=quantization,
     )
@@ -132,26 +149,27 @@
     print(f"Model uid: {model_uid}")
 
 
 @cli.command("list")
 @click.option(
     "--endpoint",
     "-e",
-    default=f"http://{XINFERENCE_DEFAULT_LOCAL_HOST}:{XINFERENCE_DEFAULT_ENDPOINT_PORT}",
     type=str,
 )
 @click.option("--all", is_flag=True)
-def model_list(endpoint: str, all: bool):
+def model_list(endpoint: Optional[str], all: bool):
     import sys
 
     from tabulate import tabulate
 
     # TODO: get from the supervisor
     from ..model.llm import LLM_FAMILIES
 
+    endpoint = get_endpoint(endpoint)
+
     table = []
     if all:
         for model_family in LLM_FAMILIES:
             table.append(
                 [
                     model_family.model_name,
                     model_family.model_lang,
@@ -191,21 +209,22 @@
         )
 
 
 @cli.command("terminate")
 @click.option(
     "--endpoint",
     "-e",
-    default=f"http://{XINFERENCE_DEFAULT_LOCAL_HOST}:{XINFERENCE_DEFAULT_ENDPOINT_PORT}",
     type=str,
 )
 @click.option("--model-uid", type=str)
 def model_terminate(
-    endpoint: str,
+    endpoint: Optional[str],
     model_uid: str,
 ):
+    endpoint = get_endpoint(endpoint)
+
     client = RESTfulClient(base_url=endpoint)
     client.terminate_model(model_uid=model_uid)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `xinference-0.1.0/xinference/deploy/local.py` & `xinference-0.1.1/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/deploy/supervisor.py` & `xinference-0.1.1/xinference/deploy/supervisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import xoscar as xo
 from xoscar.utils import get_next_port
 
 from ..constants import XINFERENCE_DEFAULT_ENDPOINT_PORT
 from ..core.gradio import GradioApp
 from ..core.restful_api import RESTfulAPIActor
-from ..core.service import SupervisorActor
+from ..core.supervisor import SupervisorActor
 
 logger = logging.getLogger("xinference")
 
 
 async def start_supervisor_components(address: str, host: str, port: int):
     await xo.create_actor(SupervisorActor, address=address, uid=SupervisorActor.uid())
     gradio_block = GradioApp(address).build()
```

### Comparing `xinference-0.1.0/xinference/deploy/test/__init__.py` & `xinference-0.1.1/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/deploy/utils.py` & `xinference-0.1.1/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/deploy/worker.py` & `xinference-0.1.1/xinference/deploy/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import asyncio
 import logging
 from typing import Dict, Optional
 
 import xoscar as xo
 
-from ..core.service import WorkerActor
+from ..core.worker import WorkerActor
 
 logger = logging.getLogger(__name__)
 
 
 async def start_worker_components(address: str, supervisor_address: str):
     actor_pool_config = await xo.get_pool_config(address)
     subpool_addresses = []
```

### Comparing `xinference-0.1.0/xinference/isolation.py` & `xinference-0.1.1/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/locale/__init__.py` & `xinference-0.1.1/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/locale/utils.py` & `xinference-0.1.1/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/locale/zh_CN.json` & `xinference-0.1.1/xinference/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/__init__.py` & `xinference-0.1.1/xinference/model/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/core.py` & `xinference-0.1.1/xinference/model/core.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/__init__.py` & `xinference-0.1.1/xinference/model/llm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -104,26 +104,32 @@
             return cls
     return None
 
 
 def _install():
     from .ggml.chatglm import ChatglmCppChatModel
     from .ggml.llamacpp import LlamaCppChatModel, LlamaCppModel
-    from .pytorch.baichuan import BaichuanPytorchChatModel, BaichuanPytorchModel
+    from .pytorch.baichuan import BaichuanPytorchChatModel
+    from .pytorch.chatglm import ChatglmPytorchChatModel
     from .pytorch.core import PytorchChatModel, PytorchModel
+    from .pytorch.falcon import FalconPytorchChatModel, FalconPytorchModel
+    from .pytorch.vicuna import VicunaPytorchChatModel
 
     _LLM_CLASSES.extend(
         [
             ChatglmCppChatModel,
             LlamaCppModel,
             LlamaCppChatModel,
             PytorchModel,
             PytorchChatModel,
-            BaichuanPytorchModel,
             BaichuanPytorchChatModel,
+            VicunaPytorchChatModel,
+            FalconPytorchModel,
+            FalconPytorchChatModel,
+            ChatglmPytorchChatModel,
         ]
     )
 
     json_path = os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "llm_family.json"
     )
     for json_obj in json.load(open(json_path)):
```

### Comparing `xinference-0.1.0/xinference/model/llm/core.py` & `xinference-0.1.1/xinference/model/llm/core.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/ggml/__init__.py` & `xinference-0.1.1/xinference/model/llm/ggml/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/ggml/chatglm.py` & `xinference-0.1.1/xinference/model/llm/ggml/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/ggml/llamacpp.py` & `xinference-0.1.1/xinference/model/llm/ggml/llamacpp.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/llm_family.py` & `xinference-0.1.1/xinference/model/llm/llm_family.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,19 +74,15 @@
 def get_legacy_cache_path(
     model_name: str,
     model_format: str,
     model_size_in_billions: Optional[int] = None,
     quantization: Optional[str] = None,
 ) -> str:
     full_name = f"{model_name}-{model_format}-{model_size_in_billions}b-{quantization}"
-    save_dir = os.path.join(XINFERENCE_CACHE_DIR, full_name)
-    if not os.path.exists(save_dir):
-        os.makedirs(save_dir, exist_ok=True)
-    save_path = os.path.join(save_dir, "model.bin")
-    return save_path
+    return os.path.join(XINFERENCE_CACHE_DIR, full_name, "model.bin")
 
 
 def cache(
     llm_family: LLMFamilyV1,
     llm_spec: "LLMSpecV1",
     quantization: Optional[str] = None,
 ) -> str:
```

### Comparing `xinference-0.1.0/xinference/model/llm/pytorch/__init__.py` & `xinference-0.1.1/xinference/model/llm/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference/model/llm/pytorch/baichuan.py` & `xinference-0.1.1/xinference/model/llm/pytorch/baichuan.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,74 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
-from ....constants import XINFERENCE_CACHE_DIR
 from ..llm_family import LLMFamilyV1, LLMSpecV1
-from .core import PytorchChatModel, PytorchModel, PytorchModelConfig
-
-
-class BaichuanPytorchModel(PytorchModel):
-    def __init__(
-        self,
-        model_uid: str,
-        model_family: "LLMFamilyV1",
-        model_spec: "LLMSpecV1",
-        quantization: str,
-        model_path: str,
-        pytorch_model_config: Optional[PytorchModelConfig] = None,
-    ):
-        super().__init__(
-            model_uid,
-            model_family,
-            model_spec,
-            quantization,
-            model_path,
-            pytorch_model_config=pytorch_model_config,
-        )
-
-    def _load_model(self, kwargs: dict):
-        try:
-            from transformers import AutoModelForCausalLM, AutoTokenizer
-        except ImportError:
-            error_message = "Failed to import module 'transformers'"
-            installation_guide = [
-                "Please make sure 'transformers' is installed. ",
-                "You can install it by `pip install transformers`\n",
-            ]
-
-            raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
-
-        tokenizer = AutoTokenizer.from_pretrained(
-            self.model_path,
-            trust_remote_code=True,
-            revision=kwargs["revision"],
-            cache_dir=XINFERENCE_CACHE_DIR,
-        )
-        model = AutoModelForCausalLM.from_pretrained(
-            self.model_path,
-            trust_remote_code=True,
-            low_cpu_mem_usage=True,
-            cache_dir=XINFERENCE_CACHE_DIR,
-            **kwargs,
-        )
-        return model, tokenizer
-
-    @classmethod
-    def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
-        if llm_spec.model_format != "pytorch":
-            return False
-        if "baichuan" not in llm_family.model_name:
-            return False
-        if "generate" not in llm_family.model_ability:
-            return False
-        return True
+from .core import PytorchChatModel, PytorchModelConfig
 
 
 class BaichuanPytorchChatModel(PytorchChatModel):
     def __init__(
         self,
         model_uid: str,
         model_family: "LLMFamilyV1",
@@ -110,27 +52,25 @@
             raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
         tokenizer = AutoTokenizer.from_pretrained(
             self.model_path,
             use_fast=self._use_fast_tokenizer,
             trust_remote_code=True,
             revision=kwargs["revision"],
-            cache_dir=XINFERENCE_CACHE_DIR,
         )
         model = AutoModelForCausalLM.from_pretrained(
             self.model_path,
             trust_remote_code=True,
-            cache_dir=XINFERENCE_CACHE_DIR,
             **kwargs,
         )
         model.generation_config = GenerationConfig.from_pretrained(self.model_path)
         return model, tokenizer
 
     @classmethod
     def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
         if llm_spec.model_format != "pytorch":
             return False
-        if "baichuan" not in llm_family.model_name:
+        if "baichuan-chat" not in llm_family.model_name:
             return False
         if "chat" not in llm_family.model_ability:
             return False
         return True
```

### Comparing `xinference-0.1.0/xinference/model/llm/pytorch/compression.py` & `xinference-0.1.1/xinference/model/llm/pytorch/compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 import torch.nn as nn
 from huggingface_hub import snapshot_download
 from torch import Tensor
 from torch.nn import functional as F
 from tqdm import tqdm
 from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 
-from ....constants import XINFERENCE_CACHE_DIR
-
 
 @dataclasses.dataclass
 class CompressionConfig:
     """Group-wise quantization."""
 
     num_bits: int
     group_size: int
@@ -113,37 +111,33 @@
 
     # partially load model
     tokenizer = AutoTokenizer.from_pretrained(
         model_path,
         use_fast=use_fast,
         trust_remote_code=True,
         revision=revision,
-        cache_dir=XINFERENCE_CACHE_DIR,
     )
 
     with init_empty_weights():
         config = AutoConfig.from_pretrained(
             model_path,
             low_cpu_mem_usage=True,
             torch_dtype=torch_dtype,
             trust_remote_code=True,
             revision=revision,
-            cache_dir=XINFERENCE_CACHE_DIR,
         )
         model = AutoModelForCausalLM.from_config(config, trust_remote_code=True)
         linear_weights = get_compressed_list(model)
 
     if os.path.exists(model_path):
         # `model_path` is a local folder
         base_pattern = os.path.join(model_path, "pytorch_model*.bin")
     else:
         # `model_path` is a cached Hugging Face repo
-        model_path = snapshot_download(
-            model_path, revision=revision, cache_dir=XINFERENCE_CACHE_DIR
-        )
+        model_path = snapshot_download(model_path, revision=revision)
         base_pattern = os.path.join(model_path, "pytorch_model*.bin")
 
     files = glob.glob(base_pattern)
 
     compressed_state_dict = {}
 
     for filename in tqdm(files):
```

### Comparing `xinference-0.1.0/xinference/model/llm/pytorch/core.py` & `xinference-0.1.1/xinference/model/llm/pytorch/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,30 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from typing import Iterator, List, Optional, TypedDict, Union
 
-import torch
-
-from ....constants import XINFERENCE_CACHE_DIR
 from ....types import (
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionMessage,
     Completion,
     CompletionChunk,
     Embedding,
+    EmbeddingData,
+    EmbeddingUsage,
 )
 from ..core import LLM
 from ..llm_family import LLMFamilyV1, LLMSpecV1
 from ..utils import ChatModelMixin
-from .compression import load_compress_model
-from .utils import generate_stream
 
 logger = logging.getLogger(__name__)
 
 
 class PytorchGenerateConfig(TypedDict, total=False):
     temperature: float
     repetition_penalty: float
@@ -119,26 +116,34 @@
             ]
 
             raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
         tokenizer = AutoTokenizer.from_pretrained(
             self.model_path,
             use_fast=self._use_fast_tokenizer,
+            trust_remote_code=True,
             revision=kwargs["revision"],
-            cache_dir=XINFERENCE_CACHE_DIR,
         )
         model = AutoModelForCausalLM.from_pretrained(
             self.model_path,
+            trust_remote_code=True,
             low_cpu_mem_usage=True,
-            cache_dir=XINFERENCE_CACHE_DIR,
             **kwargs,
         )
         return model, tokenizer
 
     def load(self):
+        try:
+            import torch
+        except ImportError:
+            raise ImportError(
+                f"Failed to import module 'torch'. Please make sure 'torch' is installed.\n\n"
+            )
+        from .compression import load_compress_model
+
         quantization = self.quantization
         num_gpus = self._pytorch_model_config.get("num_gpus", 1)
         if self._is_darwin_and_apple_silicon():
             device = self._pytorch_model_config.get("device", "mps")
         else:
             device = self._pytorch_model_config.get("device", "cuda")
 
@@ -189,30 +194,55 @@
             self._model.to(device)
         logger.debug(f"Model Memory: {self._model.get_memory_footprint()}")
 
     @classmethod
     def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
         if llm_spec.model_format != "pytorch":
             return False
-        if "baichuan" in llm_family.model_name:
+        if llm_family.model_name in [
+            "baichuan-chat",
+            "vicuna-v1.3",
+            "falcon",
+            "falcon-instruct",
+            "chatglm",
+            "chatglm2",
+            "chatglm2-32k",
+        ]:
             return False
         if "generate" not in llm_family.model_ability:
             return False
         return True
 
     def generate(
         self, prompt: str, generate_config: Optional[PytorchGenerateConfig] = None
     ) -> Union[Completion, Iterator[CompletionChunk]]:
+        from .utils import (
+            generate_stream,
+            generate_stream_chatglm,
+            generate_stream_falcon,
+        )
+
         def generator_wrapper(
             prompt: str, device: str, generate_config: PytorchGenerateConfig
         ) -> Iterator[CompletionChunk]:
-            for completion_chunk, _ in generate_stream(
-                self._model, self._tokenizer, prompt, device, generate_config
-            ):
-                yield completion_chunk
+            if "falcon" in self.model_family.model_name:
+                for completion_chunk, _ in generate_stream_falcon(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    yield completion_chunk
+            elif "chatglm" in self.model_family.model_name:
+                for completion_chunk, _ in generate_stream_chatglm(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    yield completion_chunk
+            else:
+                for completion_chunk, _ in generate_stream(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    yield completion_chunk
 
         logger.debug(
             "Enter generate, prompt: %s, generate config: %s", prompt, generate_config
         )
 
         generate_config = self._sanitize_generate_config(generate_config)
 
@@ -221,32 +251,121 @@
 
         stream = generate_config.get("stream", False)
         if self._is_darwin_and_apple_silicon():
             device = self._pytorch_model_config.get("device", "mps")
         else:
             device = self._pytorch_model_config.get("device", "cuda")
         if not stream:
-            for completion_chunk, completion_usage in generate_stream(
-                self._model, self._tokenizer, prompt, device, generate_config
-            ):
-                pass
+            if "falcon" in self.model_family.model_name:
+                for completion_chunk, completion_usage in generate_stream_falcon(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    pass
+            elif "chatglm" in self.model_family.model_name:
+                for completion_chunk, completion_usage in generate_stream_chatglm(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    pass
+            else:
+                for completion_chunk, completion_usage in generate_stream(
+                    self._model, self._tokenizer, prompt, device, generate_config
+                ):
+                    pass
             completion = Completion(
                 id=completion_chunk["id"],
                 object=completion_chunk["object"],
                 created=completion_chunk["created"],
                 model=completion_chunk["model"],
                 choices=completion_chunk["choices"],
                 usage=completion_usage,
             )
             return completion
         else:
             return generator_wrapper(prompt, device, generate_config)
 
     def create_embedding(self, input: Union[str, List[str]]) -> Embedding:
-        raise NotImplementedError
+        try:
+            import torch
+            import torch.nn.functional as F
+        except ImportError as e:
+            raise ImportError(
+                "Could not import torch. Please install it with `pip install torch`."
+            ) from e
+
+        if self._is_darwin_and_apple_silicon():
+            device = self._pytorch_model_config.get("device", "mps")
+        else:
+            device = self._pytorch_model_config.get("device", "cuda")
+
+        if isinstance(input, str):
+            inputs = [input]
+        else:
+            inputs = input
+
+        tokenizer = self._tokenizer
+        is_llama = "llama" in str(type(self._model))  # llama supports batch inference
+        is_chatglm = "chatglm" in str(type(self._model))
+        if is_llama:
+            encoding = tokenizer.batch_encode_plus(
+                inputs, padding=True, return_tensors="pt"
+            )
+            input_ids = encoding["input_ids"].to(device)
+            attention_mask = encoding["attention_mask"].to(device)
+            model_output = self._model(
+                input_ids, attention_mask, output_hidden_states=True
+            )
+            data = model_output.hidden_states[-1]
+            mask = attention_mask.unsqueeze(-1).expand(data.size()).float()
+            masked_embeddings = data * mask
+            sum_embeddings = torch.sum(masked_embeddings, dim=1)
+            seq_length = torch.sum(mask, dim=1)
+            embedding = sum_embeddings / seq_length
+            normalized_embeddings = F.normalize(embedding, p=2, dim=1)
+            normalized_embeddings = normalized_embeddings.tolist()
+            token_num = torch.sum(attention_mask).item()
+
+            embedding_list = []
+            for index, data in enumerate(normalized_embeddings):
+                embedding_list.append(
+                    EmbeddingData(index=index, object="embedding", embedding=data)
+                )
+
+            usage = EmbeddingUsage(prompt_tokens=token_num, total_tokens=token_num)
+
+            ret = Embedding(
+                object="list",
+                model=self.model_uid,
+                data=embedding_list,
+                usage=usage,
+            )
+
+        else:
+            embedding = []
+            token_num = 0
+            for index, text in enumerate(inputs):
+                input_ids = tokenizer.encode(text, return_tensors="pt").to(device)
+                model_output = self._model(input_ids, output_hidden_states=True)
+                if is_chatglm:
+                    data = (model_output.hidden_states[-1].transpose(0, 1))[0]
+                else:
+                    data = model_output.hidden_states[-1][0]
+                data = F.normalize(torch.mean(data, dim=0), p=2, dim=0)
+                data = data.tolist()
+
+                embedding.append(
+                    EmbeddingData(index=index, object="embedding", embedding=data)
+                )
+                token_num += len(input_ids[0])
+
+            usage = EmbeddingUsage(prompt_tokens=token_num, total_tokens=token_num)
+            ret = Embedding(
+                object="list", model=self.model_uid, data=embedding, usage=usage
+            )
+
+        return ret
 
 
 class PytorchChatModel(PytorchModel, ChatModelMixin):
     def __init__(
         self,
         model_uid: str,
         model_family: "LLMFamilyV1",
@@ -288,15 +407,23 @@
 
         return pytorch_generate_config
 
     @classmethod
     def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
         if llm_spec.model_format != "pytorch":
             return False
-        if "baichuan" in llm_family.model_name:
+        if llm_family.model_name in [
+            "baichuan-chat",
+            "vicuna-v1.3",
+            "falcon",
+            "falcon-instruct",
+            "chatglm",
+            "chatglm2",
+            "chatglm2-32k",
+        ]:
             return False
         if "chat" not in llm_family.model_ability:
             return False
         return True
 
     def chat(
         self,
```

### Comparing `xinference-0.1.0/xinference/model/llm/pytorch/vicuna.py` & `xinference-0.1.1/xinference/model/llm/pytorch/vicuna.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,37 +22,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, Optional
+from typing import Optional
 
-if TYPE_CHECKING:
-    from .. import LLMFamilyV1, LLMSpecV1
-    from .core import PytorchChatModel, PytorchModelConfig
+from .. import LLMFamilyV1, LLMSpecV1
+from .core import PytorchChatModel, PytorchModelConfig
 
 
-class VicunaCensoredPytorch(PytorchChatModel):
+class VicunaPytorchChatModel(PytorchChatModel):
     def __init__(
         self,
         model_uid: str,
         model_family: "LLMFamilyV1",
         model_spec: "LLMSpecV1",
         quantization: str,
         model_path: str,
         pytorch_model_config: Optional["PytorchModelConfig"] = None,
     ):
         super().__init__(
             model_uid,
             model_family,
             model_spec,
-            model_path,
             quantization,
+            model_path,
             pytorch_model_config=pytorch_model_config,
         )
         self._use_fast_tokenizer = False
 
     @classmethod
     def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
         if llm_spec.model_format != "pytorch":
```

### Comparing `xinference-0.1.0/xinference/types.py` & `xinference-0.1.1/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.1.0/xinference.egg-info/PKG-INFO` & `xinference-0.1.1/xinference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: ggml
 Provides-Extra: pytorch
 Provides-Extra: doc
+Provides-Extra: benchmark
 License-File: LICENSE
 
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.1.0 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.1.1 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
-Extra: ggml Provides-Extra: pytorch Provides-Extra: doc License-File: LICENSE
+Extra: ggml Provides-Extra: pytorch Provides-Extra: doc Provides-Extra:
+benchmark License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
```

### Comparing `xinference-0.1.0/xinference.egg-info/SOURCES.txt` & `xinference-0.1.1/xinference.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 xinference.egg-info/top_level.txt
 xinference/core/__init__.py
 xinference/core/api.py
 xinference/core/gradio.py
 xinference/core/model.py
 xinference/core/resource.py
 xinference/core/restful_api.py
-xinference/core/service.py
+xinference/core/supervisor.py
+xinference/core/utils.py
+xinference/core/worker.py
 xinference/deploy/__init__.py
 xinference/deploy/cmdline.py
 xinference/deploy/local.py
 xinference/deploy/supervisor.py
 xinference/deploy/utils.py
 xinference/deploy/worker.py
 xinference/deploy/test/__init__.py
@@ -43,11 +45,13 @@
 xinference/model/llm/llm_family.py
 xinference/model/llm/utils.py
 xinference/model/llm/ggml/__init__.py
 xinference/model/llm/ggml/chatglm.py
 xinference/model/llm/ggml/llamacpp.py
 xinference/model/llm/pytorch/__init__.py
 xinference/model/llm/pytorch/baichuan.py
+xinference/model/llm/pytorch/chatglm.py
 xinference/model/llm/pytorch/compression.py
 xinference/model/llm/pytorch/core.py
+xinference/model/llm/pytorch/falcon.py
 xinference/model/llm/pytorch/utils.py
 xinference/model/llm/pytorch/vicuna.py
```

### Comparing `xinference-0.1.0/xinference.egg-info/requires.txt` & `xinference-0.1.1/xinference.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 transformers>=4.31.0
 torch
 accelerate>=0.20.3
 sentencepiece
 transformers_stream_generator
 bitsandbytes
 protobuf
+einops
+
+[benchmark]
+psutil
+pynvml
 
 [dev]
 cython>=0.29
 pytest>=3.5.0
 pytest-cov>=2.5.0
 pytest-timeout>=1.2.0
 pytest-forked>=1.0
@@ -52,7 +57,8 @@
 transformers>=4.31.0
 torch
 accelerate>=0.20.3
 sentencepiece
 transformers_stream_generator
 bitsandbytes
 protobuf
+einops
```

