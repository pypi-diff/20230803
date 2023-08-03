# Comparing `tmp/bigstream-1.1.5.tar.gz` & `tmp/bigstream-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.1.5.tar", last modified: Mon Jul 31 23:01:31 2023, max compression
+gzip compressed data, was "bigstream-1.1.6.tar", last modified: Thu Aug  3 21:07:13 2023, max compression
```

## Comparing `bigstream-1.1.5.tar` & `bigstream-1.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.607052 bigstream-1.1.5/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.5/LICENSE.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 23:01:20.606032 bigstream-1.1.5/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.5/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.583721 bigstream-1.1.5/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40218 2023-07-31 22:58:52.000000 bigstream-1.1.5/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.5/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.5/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16819 2023-07-31 22:57:06.000000 bigstream-1.1.5/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22197 2023-07-31 21:22:57.000000 bigstream-1.1.5/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.5/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14215 2023-07-31 22:47:55.000000 bigstream-1.1.5/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21985 2023-07-31 22:58:23.000000 bigstream-1.1.5/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.601528 bigstream-1.1.5/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-31 23:01:20.608339 bigstream-1.1.5/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-31 23:00:51.000000 bigstream-1.1.5/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.677801 bigstream-1.1.6/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.6/LICENSE.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-03 21:07:01.676772 bigstream-1.1.6/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.6/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.651989 bigstream-1.1.6/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40218 2023-07-31 23:04:13.000000 bigstream-1.1.6/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.6/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.6/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16819 2023-07-31 22:57:06.000000 bigstream-1.1.6/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22638 2023-08-03 21:05:07.000000 bigstream-1.1.6/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-08-01 18:43:55.000000 bigstream-1.1.6/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14215 2023-07-31 22:47:55.000000 bigstream-1.1.6/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21985 2023-08-02 14:31:12.000000 bigstream-1.1.6/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.672164 bigstream-1.1.6/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-08-03 21:07:01.679075 bigstream-1.1.6/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-08-03 21:06:40.000000 bigstream-1.1.6/setup.py
```

### Comparing `bigstream-1.1.5/LICENSE.txt` & `bigstream-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/README.md` & `bigstream-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/align.py` & `bigstream-1.1.6/bigstream/align.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/application_pipelines.py` & `bigstream-1.1.6/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/configure_irm.py` & `bigstream-1.1.6/bigstream/configure_irm.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/features.py` & `bigstream-1.1.6/bigstream/features.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/level_set.py` & `bigstream-1.1.6/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/metrics.py` & `bigstream-1.1.6/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/motion_correct.py` & `bigstream-1.1.6/bigstream/motion_correct.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/piecewise_align.py` & `bigstream-1.1.6/bigstream/piecewise_align.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dask.distributed import as_completed, wait
 from ClusterWrap.decorator import cluster
 import bigstream.utility as ut
 from bigstream.align import alignment_pipeline
 from bigstream.transform import apply_transform, compose_transform_list
 from bigstream.transform import apply_transform_to_coordinates
 from bigstream.transform import compose_transforms
+from distributed import Lock, MultiLock
 
 
 @cluster
 def distributed_piecewise_alignment_pipeline(
     fix,
     mov,
     fix_spacing,
@@ -164,14 +165,16 @@
     if write_path:
         output_transform = ut.create_zarr(
             write_path,
             fix.shape + (fix.ndim,),
             tuple(blocksize) + (fix.ndim,),
             np.float32,
         )
+        # chunks will need locks for parallel writing
+        locks = [Lock(f'{x}') for x in np.ndindex(*output_transform.cdata_shape)]
 
     # determine fixed image slices for blocking
     blocksize = np.array(blocksize)
     nblocks = np.ceil(np.array(fix.shape) / blocksize).astype(int)
     overlaps = np.round(blocksize * overlap).astype(int)
     indices, slices = [], []
     for (i, j, k) in np.ndindex(*nblocks):
@@ -335,25 +338,34 @@
         if np.any( weights.shape != transform.shape[:-1] ):
             crop = tuple(slice(0, s) for s in transform.shape[:-1])
             weights = weights[crop]
 
         # apply weights
         transform = transform * weights[..., None]
 
-        # return or write the data
+        # if there's no write path, just return the transform block
         if not write_path:
             return transform
+
+        # otherwise, coordinate with neighboring blocks
         else:
-            # wait until the correct write window for this write group
-            # TODO: if a worker can query the set of running tasks, I may be able to skip
-            #       groups that are completely written
-            write_group = np.sum(np.array(block_index) % 3 * (9, 3, 1))
-            while not (write_group < time.time() / write_group_interval % 27 < write_group + .5):
-                time.sleep(1)
+            # block until locks for all write blocks are acquired
+            lock_strs = []
+            for delta in product((-1, 0, 1,), repeat=3):
+                lock_strs.append(str(tuple(a + b for a, b in zip(block_index, delta))))
+            lock = MultiLock(lock_strs)
+            lock.acquire()
+
+            # write result to disk
+            print(f'WRITING BLOCK {block_index} at {time.ctime(time.time())}', flush=True)
             output_transform[fix_slices] = output_transform[fix_slices] + transform
+            print(f'FINISHED WRITING BLOCK {block_index} at {time.ctime(time.time())}', flush=True)
+
+            # release the lock
+            lock.release()
             return True
     # END CLOSURE
 
 
     # submit all alignments to cluster
     futures = cluster.client.map(
         align_single_block, indices,
```

### Comparing `bigstream-1.1.5/bigstream/piecewise_transform.py` & `bigstream-1.1.6/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/stitch.py` & `bigstream-1.1.6/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/transform.py` & `bigstream-1.1.6/bigstream/transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream/utility.py` & `bigstream-1.1.6/bigstream/utility.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/bigstream.egg-info/SOURCES.txt` & `bigstream-1.1.6/bigstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.5/setup.py` & `bigstream-1.1.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.1.5",
+    version="1.1.6",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/GFleishman/bigstream",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

