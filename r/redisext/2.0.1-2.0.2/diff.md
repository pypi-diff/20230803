# Comparing `tmp/redisext-2.0.1.tar.gz` & `tmp/redisext-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redisext-2.0.1.tar", last modified: Mon Oct 25 14:42:13 2021, max compression
+gzip compressed data, was "redisext-2.0.2.tar", last modified: Thu Aug  3 13:52:45 2023, max compression
```

## Comparing `redisext-2.0.1.tar` & `redisext-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.644785 redisext-2.0.1/
--rw-r--r--   0 andrey     (501) staff       (20)     1081 2021-10-25 14:29:59.000000 redisext-2.0.1/LICENSE
--rw-r--r--   0 andrey     (501) staff       (20)      921 2021-10-25 14:42:13.644872 redisext-2.0.1/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      992 2021-10-25 14:39:04.000000 redisext-2.0.1/README.rst
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.643226 redisext-2.0.1/redisext/
--rw-r--r--   0 andrey     (501) staff       (20)       22 2021-10-25 14:41:42.000000 redisext-2.0.1/redisext/__init__.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.644260 redisext-2.0.1/redisext/backend/
--rw-r--r--   0 andrey     (501) staff       (20)        0 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/backend/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)     3569 2021-10-25 14:39:04.000000 redisext-2.0.1/redisext/backend/abc.py
--rw-r--r--   0 andrey     (501) staff       (20)      297 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/backend/redis.py
--rw-r--r--   0 andrey     (501) staff       (20)      326 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/backend/rmredis.py
--rw-r--r--   0 andrey     (501) staff       (20)      615 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/counter.py
--rw-r--r--   0 andrey     (501) staff       (20)     1913 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/hashmap.py
--rw-r--r--   0 andrey     (501) staff       (20)      730 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/key.py
--rw-r--r--   0 andrey     (501) staff       (20)      716 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/lock.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.644443 redisext-2.0.1/redisext/models/
--rw-r--r--   0 andrey     (501) staff       (20)        0 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/models/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)     1917 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/models/abc.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.644630 redisext-2.0.1/redisext/packages/
--rw-r--r--   0 andrey     (501) staff       (20)        0 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/packages/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)     3693 2021-10-25 14:39:04.000000 redisext-2.0.1/redisext/packages/dsnparse.py
--rw-r--r--   0 andrey     (501) staff       (20)     2864 2021-10-25 14:39:04.000000 redisext-2.0.1/redisext/pool.py
--rw-r--r--   0 andrey     (501) staff       (20)     1477 2021-10-25 14:39:04.000000 redisext-2.0.1/redisext/queue.py
--rw-r--r--   0 andrey     (501) staff       (20)      850 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/serializer.py
--rw-r--r--   0 andrey     (501) staff       (20)      509 2021-10-25 14:29:59.000000 redisext-2.0.1/redisext/stack.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2021-10-25 14:42:13.643830 redisext-2.0.1/redisext.egg-info/
--rw-r--r--   0 andrey     (501) staff       (20)      921 2021-10-25 14:42:13.000000 redisext-2.0.1/redisext.egg-info/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      584 2021-10-25 14:42:13.000000 redisext-2.0.1/redisext.egg-info/SOURCES.txt
--rw-r--r--   0 andrey     (501) staff       (20)        1 2021-10-25 14:42:13.000000 redisext-2.0.1/redisext.egg-info/dependency_links.txt
--rw-r--r--   0 andrey     (501) staff       (20)       12 2021-10-25 14:42:13.000000 redisext-2.0.1/redisext.egg-info/requires.txt
--rw-r--r--   0 andrey     (501) staff       (20)        9 2021-10-25 14:42:13.000000 redisext-2.0.1/redisext.egg-info/top_level.txt
--rw-r--r--   0 andrey     (501) staff       (20)      219 2021-10-25 14:42:13.645149 redisext-2.0.1/setup.cfg
--rw-r--r--   0 andrey     (501) staff       (20)     1467 2021-10-25 14:39:04.000000 redisext-2.0.1/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.049649 redisext-2.0.2/
+-rw-r--r--   0 andrey     (501) staff       (20)     1081 2023-08-03 13:43:17.000000 redisext-2.0.2/LICENSE
+-rw-r--r--   0 andrey     (501) staff       (20)      824 2023-08-03 13:52:45.049709 redisext-2.0.2/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      992 2023-08-03 13:43:17.000000 redisext-2.0.2/README.rst
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.045335 redisext-2.0.2/redisext/
+-rw-r--r--   0 andrey     (501) staff       (20)       22 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/__init__.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.047035 redisext-2.0.2/redisext/backend/
+-rw-r--r--   0 andrey     (501) staff       (20)        0 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/backend/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)     3569 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/backend/abc.py
+-rw-r--r--   0 andrey     (501) staff       (20)      297 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/backend/redis.py
+-rw-r--r--   0 andrey     (501) staff       (20)      326 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/backend/rmredis.py
+-rw-r--r--   0 andrey     (501) staff       (20)      615 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/counter.py
+-rw-r--r--   0 andrey     (501) staff       (20)     1913 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/hashmap.py
+-rw-r--r--   0 andrey     (501) staff       (20)      730 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/key.py
+-rw-r--r--   0 andrey     (501) staff       (20)      716 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/lock.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.047363 redisext-2.0.2/redisext/models/
+-rw-r--r--   0 andrey     (501) staff       (20)        0 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/models/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)     1917 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/models/abc.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.047687 redisext-2.0.2/redisext/packages/
+-rw-r--r--   0 andrey     (501) staff       (20)        0 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/packages/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)     3693 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/packages/dsnparse.py
+-rw-r--r--   0 andrey     (501) staff       (20)     2864 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/pool.py
+-rw-r--r--   0 andrey     (501) staff       (20)     1477 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/queue.py
+-rw-r--r--   0 andrey     (501) staff       (20)      850 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/serializer.py
+-rw-r--r--   0 andrey     (501) staff       (20)      509 2023-08-03 13:43:17.000000 redisext-2.0.2/redisext/stack.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.046325 redisext-2.0.2/redisext.egg-info/
+-rw-r--r--   0 andrey     (501) staff       (20)      824 2023-08-03 13:52:45.000000 redisext-2.0.2/redisext.egg-info/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      800 2023-08-03 13:52:45.000000 redisext-2.0.2/redisext.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        1 2023-08-03 13:52:45.000000 redisext-2.0.2/redisext.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       12 2023-08-03 13:52:45.000000 redisext-2.0.2/redisext.egg-info/requires.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        9 2023-08-03 13:52:45.000000 redisext-2.0.2/redisext.egg-info/top_level.txt
+-rw-r--r--   0 andrey     (501) staff       (20)      219 2023-08-03 13:52:45.049965 redisext-2.0.2/setup.cfg
+-rw-r--r--   0 andrey     (501) staff       (20)     1371 2023-08-03 13:43:17.000000 redisext-2.0.2/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2023-08-03 13:52:45.049520 redisext-2.0.2/tests/
+-rw-r--r--   0 andrey     (501) staff       (20)     1335 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_client.py
+-rw-r--r--   0 andrey     (501) staff       (20)      818 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_counter.py
+-rw-r--r--   0 andrey     (501) staff       (20)      574 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_dsn_connection.py
+-rw-r--r--   0 andrey     (501) staff       (20)     5039 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_dsnparse.py
+-rw-r--r--   0 andrey     (501) staff       (20)     1260 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_expire.py
+-rw-r--r--   0 andrey     (501) staff       (20)     3048 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_hashmap.py
+-rw-r--r--   0 andrey     (501) staff       (20)      818 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_lock.py
+-rw-r--r--   0 andrey     (501) staff       (20)     3642 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_pool.py
+-rw-r--r--   0 andrey     (501) staff       (20)     2315 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_queue.py
+-rw-r--r--   0 andrey     (501) staff       (20)     3010 2023-08-03 13:43:17.000000 redisext-2.0.2/tests/test_stack.py
```

### Comparing `redisext-2.0.1/LICENSE` & `redisext-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/PKG-INFO` & `redisext-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: redisext
-Version: 2.0.1
+Version: 2.0.2
 Summary: Data models for Redis
 Home-page: https://github.com/mylokin/redisext
 Author: Andrey Gubarev
 Author-email: mylokin@me.com
 License: MIT
-Description: UNKNOWN
 Keywords: redis,orm,models
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
+License-File: LICENSE
```

### Comparing `redisext-2.0.1/README.rst` & `redisext-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/backend/abc.py` & `redisext-2.0.2/redisext/backend/abc.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/counter.py` & `redisext-2.0.2/redisext/counter.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/hashmap.py` & `redisext-2.0.2/redisext/hashmap.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/key.py` & `redisext-2.0.2/redisext/key.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/lock.py` & `redisext-2.0.2/redisext/lock.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/models/abc.py` & `redisext-2.0.2/redisext/models/abc.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/packages/dsnparse.py` & `redisext-2.0.2/redisext/packages/dsnparse.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/pool.py` & `redisext-2.0.2/redisext/pool.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/queue.py` & `redisext-2.0.2/redisext/queue.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext/serializer.py` & `redisext-2.0.2/redisext/serializer.py`

 * *Files identical despite different names*

### Comparing `redisext-2.0.1/redisext.egg-info/PKG-INFO` & `redisext-2.0.2/redisext.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: redisext
-Version: 2.0.1
+Version: 2.0.2
 Summary: Data models for Redis
 Home-page: https://github.com/mylokin/redisext
 Author: Andrey Gubarev
 Author-email: mylokin@me.com
 License: MIT
-Description: UNKNOWN
 Keywords: redis,orm,models
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
+License-File: LICENSE
```

