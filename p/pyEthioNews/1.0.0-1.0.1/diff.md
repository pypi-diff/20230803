# Comparing `tmp/pyEthioNews-1.0.0.tar.gz` & `tmp/pyEthioNews-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEthioNews-1.0.0.tar", last modified: Thu Aug  3 07:38:14 2023, max compression
+gzip compressed data, was "pyEthioNews-1.0.1.tar", last modified: Thu Aug  3 07:40:40 2023, max compression
```

## Comparing `pyEthioNews-1.0.0.tar` & `pyEthioNews-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:38:14.708440 pyEthioNews-1.0.0/
--rw-rw-rw-   0        0        0      228 2023-08-03 07:38:14.708440 pyEthioNews-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1794 2023-08-02 14:38:37.000000 pyEthioNews-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 07:38:14.691467 pyEthioNews-1.0.0/pyEthioNews/
--rw-rw-rw-   0        0        0       31 2023-08-01 07:24:49.000000 pyEthioNews-1.0.0/pyEthioNews/__init__.py
--rw-rw-rw-   0        0        0     1139 2023-08-02 14:31:21.000000 pyEthioNews-1.0.0/pyEthioNews/news.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:38:14.706480 pyEthioNews-1.0.0/pyEthioNews/providers/
--rw-rw-rw-   0        0        0      168 2023-08-01 06:44:31.000000 pyEthioNews-1.0.0/pyEthioNews/providers/__init__.py
--rw-rw-rw-   0        0        0     1666 2023-08-01 07:27:46.000000 pyEthioNews-1.0.0/pyEthioNews/providers/fana.py
--rw-rw-rw-   0        0        0      725 2023-08-01 07:27:46.000000 pyEthioNews-1.0.0/pyEthioNews/providers/mereja.py
--rw-rw-rw-   0        0        0     2939 2023-08-02 14:31:51.000000 pyEthioNews-1.0.0/pyEthioNews/providers/voa.py
--rw-rw-rw-   0        0        0     3564 2023-08-01 07:27:46.000000 pyEthioNews-1.0.0/pyEthioNews/providers/walta.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:38:14.707464 pyEthioNews-1.0.0/pyEthioNews/types/
--rw-rw-rw-   0        0        0     3949 2022-12-07 15:22:06.000000 pyEthioNews-1.0.0/pyEthioNews/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:38:14.702436 pyEthioNews-1.0.0/pyEthioNews.egg-info/
--rw-rw-rw-   0        0        0      228 2023-08-03 07:38:14.000000 pyEthioNews-1.0.0/pyEthioNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-08-03 07:38:14.000000 pyEthioNews-1.0.0/pyEthioNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:38:14.000000 pyEthioNews-1.0.0/pyEthioNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 07:38:14.000000 pyEthioNews-1.0.0/pyEthioNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 07:38:14.000000 pyEthioNews-1.0.0/pyEthioNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:38:14.709447 pyEthioNews-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-08-03 07:37:41.000000 pyEthioNews-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:40:40.982434 pyEthioNews-1.0.1/
+-rw-rw-rw-   0        0        0     2137 2023-08-03 07:40:40.981450 pyEthioNews-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1794 2023-08-02 14:38:37.000000 pyEthioNews-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 07:40:40.969437 pyEthioNews-1.0.1/pyEthioNews/
+-rw-rw-rw-   0        0        0       31 2023-08-01 07:24:49.000000 pyEthioNews-1.0.1/pyEthioNews/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-08-02 14:31:21.000000 pyEthioNews-1.0.1/pyEthioNews/news.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:40:40.979454 pyEthioNews-1.0.1/pyEthioNews/providers/
+-rw-rw-rw-   0        0        0      168 2023-08-01 06:44:31.000000 pyEthioNews-1.0.1/pyEthioNews/providers/__init__.py
+-rw-rw-rw-   0        0        0     1666 2023-08-01 07:27:46.000000 pyEthioNews-1.0.1/pyEthioNews/providers/fana.py
+-rw-rw-rw-   0        0        0      725 2023-08-01 07:27:46.000000 pyEthioNews-1.0.1/pyEthioNews/providers/mereja.py
+-rw-rw-rw-   0        0        0     2939 2023-08-02 14:31:51.000000 pyEthioNews-1.0.1/pyEthioNews/providers/voa.py
+-rw-rw-rw-   0        0        0     3564 2023-08-01 07:27:46.000000 pyEthioNews-1.0.1/pyEthioNews/providers/walta.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:40:40.980457 pyEthioNews-1.0.1/pyEthioNews/types/
+-rw-rw-rw-   0        0        0     3949 2022-12-07 15:22:06.000000 pyEthioNews-1.0.1/pyEthioNews/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:40:40.975432 pyEthioNews-1.0.1/pyEthioNews.egg-info/
+-rw-rw-rw-   0        0        0     2137 2023-08-03 07:40:40.000000 pyEthioNews-1.0.1/pyEthioNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-08-03 07:40:40.000000 pyEthioNews-1.0.1/pyEthioNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:40:40.000000 pyEthioNews-1.0.1/pyEthioNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 07:40:40.000000 pyEthioNews-1.0.1/pyEthioNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 07:40:40.000000 pyEthioNews-1.0.1/pyEthioNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:40:40.982434 pyEthioNews-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      550 2023-08-03 07:40:30.000000 pyEthioNews-1.0.1/setup.py
```

### Comparing `pyEthioNews-1.0.0/README.md` & `pyEthioNews-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/news.py` & `pyEthioNews-1.0.1/pyEthioNews/news.py`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/providers/fana.py` & `pyEthioNews-1.0.1/pyEthioNews/providers/fana.py`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/providers/mereja.py` & `pyEthioNews-1.0.1/pyEthioNews/providers/mereja.py`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/providers/voa.py` & `pyEthioNews-1.0.1/pyEthioNews/providers/voa.py`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/providers/walta.py` & `pyEthioNews-1.0.1/pyEthioNews/providers/walta.py`

 * *Files identical despite different names*

### Comparing `pyEthioNews-1.0.0/pyEthioNews/types/__init__.py` & `pyEthioNews-1.0.1/pyEthioNews/types/__init__.py`

 * *Files identical despite different names*

