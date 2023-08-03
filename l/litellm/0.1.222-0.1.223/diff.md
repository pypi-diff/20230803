# Comparing `tmp/litellm-0.1.222.tar.gz` & `tmp/litellm-0.1.223.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.222.tar", last modified: Thu Aug  3 13:28:32 2023, max compression
+gzip compressed data, was "litellm-0.1.223.tar", last modified: Thu Aug  3 15:09:34 2023, max compression
```

## Comparing `litellm-0.1.222.tar` & `litellm-0.1.223.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.089393 litellm-0.1.222/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.222/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 13:28:32.089276 litellm-0.1.222/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.222/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.088179 litellm-0.1.222/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.222/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.222/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.222/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14924 2023-08-03 12:53:34.000000 litellm-0.1.222/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.089102 litellm-0.1.222/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.222/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 13:28:32.089452 litellm-0.1.222/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 13:27:36.000000 litellm-0.1.222/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.431698 litellm-0.1.223/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.223/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:09:34.431554 litellm-0.1.223/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.223/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.430451 litellm-0.1.223/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.223/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.223/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.223/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    15044 2023-08-03 13:49:40.000000 litellm-0.1.223/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.431271 litellm-0.1.223/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.223/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:09:34.431753 litellm-0.1.223/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 15:09:15.000000 litellm-0.1.223/setup.py
```

### Comparing `litellm-0.1.222/LICENSE` & `litellm-0.1.223/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.222/README.md` & `litellm-0.1.223/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.1-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
 [![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere-blue?color=green)](https://github.com/BerriAI/litellm)
 
 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
-a simple & light 100 line package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
+a simple & light package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
 - guarantees consistent output, text responses will always be available at `['choices'][0]['message']['content']`
 
 # usage
```

### Comparing `litellm-0.1.222/litellm/__init__.py` & `litellm-0.1.223/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.222/litellm/main.py` & `litellm-0.1.223/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.222/litellm/timeout.py` & `litellm-0.1.223/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.222/litellm/utils.py` & `litellm-0.1.223/litellm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         try:
             import sentry_sdk
         except ImportError:
             print_verbose("Package 'sentry_sdk' is missing. Installing it...")
             subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'sentry_sdk'])
             import sentry_sdk
         sentry_sdk_instance = sentry_sdk
+        sentry_trace_rate = os.environ.get("SENTRY_API_TRACE_RATE") if "SENTRY_API_TRACE_RATE" in os.environ else "1.0"
         sentry_sdk_instance.init(dsn=os.environ.get("SENTRY_API_URL"), traces_sample_rate=float(os.environ.get("SENTRY_API_TRACE_RATE")))
         capture_exception = sentry_sdk_instance.capture_exception
         add_breadcrumb = sentry_sdk_instance.add_breadcrumb 
       elif callback == "posthog":
         try:
             from posthog import Posthog
         except ImportError:
```

