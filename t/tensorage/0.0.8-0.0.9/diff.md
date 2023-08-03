# Comparing `tmp/tensorage-0.0.8.tar.gz` & `tmp/tensorage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.8.tar", last modified: Wed Aug  2 09:24:10 2023, max compression
+gzip compressed data, was "tensorage-0.0.9.tar", last modified: Thu Aug  3 06:14:08 2023, max compression
```

## Comparing `tensorage-0.0.8.tar` & `tensorage-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-02 09:23:55.000000 tensorage-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-02 09:23:55.000000 tensorage-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-02 09:24:10.029866 tensorage-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-02 09:23:55.000000 tensorage-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-02 09:23:55.000000 tensorage-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 09:24:10.029866 tensorage-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-02 09:23:55.000000 tensorage-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/db_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     9570 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-03 06:13:57.000000 tensorage-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-03 06:13:57.000000 tensorage-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-03 06:14:08.458240 tensorage-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-03 06:13:57.000000 tensorage-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-03 06:13:57.000000 tensorage-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 06:14:08.458240 tensorage-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-03 06:13:57.000000 tensorage-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.8/LICENSE` & `tensorage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.8/setup.py` & `tensorage-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.8/tensorage/auth.py` & `tensorage-0.0.9/tensorage/auth.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.8/tensorage/db_init.py` & `tensorage-0.0.9/tensorage/db_init.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.8/tensorage/session.py` & `tensorage-0.0.9/tensorage/session.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.8/tensorage/store.py` & `tensorage-0.0.9/tensorage/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
             _iterator = tqdm(batches, desc=f'Uploading {key} [{len(batches)} batches of {batch_size}]') if not self.quiet else batches
 
             # insert the tensor
             for offset, batch in _iterator:
                 context.insert_tensor(dataset.id, [tensor for tensor in batch], offset=offset)
 
     def __delitem__(self, key: str):
-        raise NotImplementedError
+        with self._session as context:
+            context.remove_dataset(key)
     
     def __contains__(self, key: str):
         # get the keys
         keys = self.keys()
 
         # check if key is in keys
         return key in keys
```

