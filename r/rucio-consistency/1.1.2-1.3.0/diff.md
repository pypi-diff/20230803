# Comparing `tmp/rucio-consistency-1.1.2.tar.gz` & `tmp/rucio-consistency-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.1.2.tar", last modified: Tue Jun 27 14:49:51 2023, max compression
+gzip compressed data, was "rucio-consistency-1.3.0.tar", last modified: Thu Aug  3 14:02:42 2023, max compression
```

## Comparing `rucio-consistency-1.1.2.tar` & `rucio-consistency-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.485765 rucio-consistency-1.1.2/
--rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/LICENSE
--rw-r--r--   0 ivm        (503) staff       (20)      369 2023-06-27 14:49:51.485478 rucio-consistency-1.1.2/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/README.rst
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.479040 rucio-consistency-1.1.2/rucio_consistency/
--rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.483772 rucio-consistency-1.1.2/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (503) staff       (20)      124 2023-06-27 14:49:47.000000 rucio-consistency-1.1.2/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.484959 rucio-consistency-1.1.2/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    27550 2023-06-27 14:40:37.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.481296 rucio-consistency-1.1.2/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (503) staff       (20)      369 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)      850 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (503) staff       (20)      388 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (503) staff       (20)       22 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (503) staff       (20)       18 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (503) staff       (20)       38 2023-06-27 14:49:51.485885 rucio-consistency-1.1.2/setup.cfg
--rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/setup.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.218605 rucio-consistency-1.3.0/
+-rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/LICENSE
+-rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-03 14:02:42.218277 rucio-consistency-1.3.0/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/README.rst
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.210999 rucio-consistency-1.3.0/rucio_consistency/
+-rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.216381 rucio-consistency-1.3.0/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (503) staff       (20)      125 2023-08-03 14:02:11.000000 rucio-consistency-1.3.0/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.217788 rucio-consistency-1.3.0/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    27819 2023-08-03 14:02:11.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.213330 rucio-consistency-1.3.0/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)      850 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (503) staff       (20)      388 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (503) staff       (20)       22 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       18 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       38 2023-08-03 14:02:42.218901 rucio-consistency-1.3.0/setup.cfg
+-rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/setup.py
```

### Comparing `rucio-consistency-1.1.2/LICENSE` & `rucio-consistency-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/README.rst` & `rucio-consistency-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/cmplib.py` & `rucio-consistency-1.3.0/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/config.py` & `rucio-consistency-1.3.0/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/part.py` & `rucio-consistency-1.3.0/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.3.0/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/stats.py` & `rucio-consistency-1.3.0/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pythreader import TaskQueue, Task, DEQueue, PyThread, synchronized, ShellCommand, Primitive
 import re, json, os, os.path, traceback, sys
 import subprocess, time, random, gzip
 
 from rucio_consistency import to_str, Stats, PartitionedList, ScannerConfiguration
-from .xrootd_client import XRootDClient
+from rucio_consistency.xrootd import XRootDClient
 
 Version = "4.0"
 
 GB = 1024*1024*1024
 
 try:
     import tqdm
@@ -123,15 +123,15 @@
 
 class Scanner(Task):
     
     MAX_ATTEMPTS_REC = 3
     MAX_ATTEMPTS_FLAT = 3
     MAX_REC_ZERO_RETRY = 1
 
-    def __init__(self, master, client, timeout, location, recursive, include_sizes = True, report_empty_top = True):
+    def __init__(self, master, client, timeout, location, recursive, include_sizes=True, report_empty_top=True, list_empty_dirs=False):
         Task.__init__(self)
         self.Client = client
         self.Master = master
         self.Location = canonic_path(location)
         self.ForcedFlat = not recursive
         self.WasRecursive = recursive
         self.Subprocess = None
@@ -139,14 +139,15 @@
         self.Elapsed = None
         self.RecAttempts = self.MAX_ATTEMPTS_REC if recursive else 0
         self.FlatAttempts = self.MAX_ATTEMPTS_FLAT
         self.ZeroAttempts = self.MAX_REC_ZERO_RETRY
         self.IncludeSizes = include_sizes
         self.ReportEmptyTop = report_empty_top
         self.Timeout = timeout
+        self.ListEmptyDirs = list_empty_dirs                # whether to produce the list of empty dirs or just count them
         #print("Scanner create for location:", self.Location)
 
     def __str__(self):
         return "Scanner(%s)" % (self.Location,)
 
     def message(self, status, stats):
         if self.Master is not None:
@@ -204,30 +205,34 @@
                 while dirpath and dirpath != '/' and dirpath in empty_dirs:
                     empty_dirs.remove(dirpath)
                     dirpath = self.parent(dirpath)
 
         if self.ReportEmptyTop and (recursive or not dirs) and not files:
             empty_dirs.add(self.Location)
 
-        counts = " files: %-8d dirs: %-8d empty: %-8d" % (len(files), len(dirs), len(empty_dirs))
+        empty_dir_count = len(empty_dirs)
+        if not self.ListEmptyDirs:
+            empty_dirs = None
+
+        counts = " files: %-8d dirs: %-8d empty: %-8d" % (len(files), len(dirs), empty_dir_count)
         if self.IncludeSizes:
             total_size = sum(size for _, size in files) + sum(size for _, size in dirs)
             counts += " size: %10.3fGB" % (total_size/GB,)
         self.message("done", stats+counts)
         if self.Master is not None:
-            self.Master.scanner_succeeded(self, location, self.WasRecursive, files, dirs, empty_dirs)
+            self.Master.scanner_succeeded(self, location, self.WasRecursive, files, dirs, empty_dir_count, empty_dirs)
 
 class ScannerMaster(PyThread):
     
     MAX_RECURSION_FAILED_COUNT = 5
     REPORT_INTERVAL = 10.0
     RESULTS_BUFFER_SISZE = 100
     
     def __init__(self, client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress, max_files = None,
-                include_sizes=True, ignore_list=[]):
+                include_sizes=True, ignore_list=[], list_empty_dirs=False):
         PyThread.__init__(self)
         self.RecursiveThreshold = recursive_threshold
         self.PathConverter = path_converter
         self.Client = client
         self.Root = root
         self.MaxScanners = max_scanners
         self.Results = DEQueue(self.RESULTS_BUFFER_SISZE)
@@ -249,27 +254,29 @@
         self.MaxFiles = max_files       # will stop after number of files found exceeds this number. Used for debugging
         self.IgnoreList = ignore_list
         self.IgnoredFiles = self.IgnoredDirs = 0
         self.IncludeSizes = include_sizes
         self.TotalSize = 0.0 if include_sizes else None                  # Megabytes
         self.Timeout = timeout
         self.RootExpected = root_expected
+        self.ListEmptyDirs = list_empty_dirs
 
     def taskFailed(self, queue, task, exc_type, exc_value, tb):
         traceback.print_exception(exc_type, exc_value, tb, file=sys.stderr)
 
     def taskFailed(self, queue, task, exc_type, exc_value, tb):
         traceback.print_exception(exc_type, exc_value, tb, file=sys.stderr)
 
     def run(self):
         #
         # scan Root non-recursovely first, if failed, return immediarely
         #
         #server, location, recursive, timeout
-        scanner_task = Scanner(self, self.Client, self.Timeout, self.Root, self.RecursiveThreshold == 0, include_sizes=self.IncludeSizes, report_empty_top=False)
+        scanner_task = Scanner(self, self.Client, self.Timeout, self.Root, self.RecursiveThreshold == 0, include_sizes=self.IncludeSizes, 
+                report_empty_top=False, list_empty_dirs=self.ListEmptyDirs)
         self.ScannerQueue.addTask(scanner_task)
         self.ScannerQueue.waitUntilEmpty()
         self.Results.close()
         self.ScannerQueue.Delegate = None       # detach for garbage collection
         self.ScannerQueue = None
         
     def dir_ignored(self, logpath):
@@ -299,15 +306,14 @@
 
     def addEmptyDirectories(self, paths):
         if not self.Failed:
             for path in paths:
                 if path != self.Root:
                     # do not report root even if it is empty
                     self.Results.append(('e', path))
-                    self.NEmptyDirs += 1
                 else:
                     print("Empty root", path,"removed from empty list")
 
     @synchronized
     def report(self):
         if time.time() > self.LastReport + self.REPORT_INTERVAL:
             waiting, active = self.ScannerQueue.tasks()
@@ -325,15 +331,15 @@
             print("Gave up:", scanner.Location)
             self.GaveUp[scanner.Location] = error
             self.NScanned += 1  
             #sys.stderr.write("Gave up on: %s\n" % (path,))
             self.show_progress()            #"Error scanning %s: %s -- retrying" % (scanner.Location, error))
 
     @synchronized
-    def scanner_succeeded(self, scanner, location, was_recursive, files, dirs, empty_dirs):
+    def scanner_succeeded(self, scanner, location, was_recursive, files, dirs, empty_dir_count, empty_dirs):
         if not files and not dirs and was_recursive and scanner.ZeroAttempts > 0:
             scanner.ZeroAttempts -= 1
             print("resubmitted because recursive scan found nothing:", scanner.Location)
             self.ScannerQueue.addTask(scanner)
             return
 
         self.NScanned += 1
@@ -346,26 +352,31 @@
             else:
                 self.IgnoredFiles += 1
 
         scan = not was_recursive
         allow_recursive = scan #and len(dirs) > 1
         #print("scanner_succeeded: loop over dirs... scan:", scan)
         for path, size in dirs:
-            logpath = self.PathConverter.path_to_logpath(path)
             self.NDirectories += 1
-            if self.dir_ignored(logpath):
-                self.IgnoredDirs += 1
-                if scan:    print(logpath, " - directory ignored")
-            else:
-                self.Results.append(('d', logpath))
-                if scan:
+            if scan:
+                logpath = self.PathConverter.path_to_logpath(path)
+                if self.dir_ignored(logpath):
+                    self.IgnoredDirs += 1
+                    print(logpath, " - directory ignored")
+                else:
                     self.addDirectoryToScan(logpath, allow_recursive)
 
+        self.NEmptyDirs += empty_dir_count
         if empty_dirs:
-            self.addEmptyDirectories(empty_dirs)            # do not convert to LFN
+            for path in empty_dirs:
+                if path != self.Root:
+                    # do not report root even if it is empty
+                    self.Results.append(('e', path))
+                else:
+                    print("Empty root", path,"removed from empty list")
 
         self.show_progress()
 
     def paths(self):
         # log paths, e.g. /store/mc/...
         for t, path in self.Results:
             yield t, path
@@ -440,15 +451,15 @@
             sys.exit(1)
         lfn = rewrite_path.sub(rewrite_out, lfn)   
     return lfn
 
 def scan_root(rse, config, client, root, root_expected, my_stats, stats, stats_key, 
             quiet, display_progress, max_files,
             recursive_threshold, max_scanners, timeout,
-            file_list, dir_list, empty_dirs_file,
+            file_list, empty_dirs_file,
             ignore_failed_directories, include_sizes):
 
     failed = root_failed = False
     
     server = config.Server
     server_root = config.ServerRoot
     ignore_subdirs = config.ignore_subdirs(root)
@@ -472,15 +483,15 @@
         stats.update_section(stats_key, my_stats)
 
     remove_prefix = config.RemovePrefix
     add_prefix = config.AddPrefix
     path_converter = PathConverter(server_root, remove_prefix, add_prefix, root)
 
     master = ScannerMaster(client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress,
-            max_files = max_files, include_sizes=include_sizes,
+            max_files = max_files, include_sizes=include_sizes, list_empty_dirs=empty_dirs_file is not None,
             ignore_list = ignore_list)
 
     path_filter = None          # -- obsolete -- config.scanner_filter(rse)
     #if path_filter is not None:
     #    path_filter = re.compile(path_filter)
     rewrite_path, rewrite_out = None, None      # -- obsolete -- config.scanner_rewrite(rse)
     if rewrite_path is not None:
@@ -503,16 +514,14 @@
     if not path_prefix.endswith("/"):
         path_prefix += "/"
 
     for t, logpath in master.paths():
         # here, path is absolute path, which includes site root
         if t == 'f':
             file_list.add(logpath)             
-        elif t == 'd' and dir_list is not None:
-            dir_list.add(logpath)
         elif t == 'e' and empty_dirs_file is not None:
             empty_dirs_file.write(logpath)
             empty_dirs_file.write("\n")
 
     if display_progress:
         master.close_progress()
 
@@ -569,15 +578,15 @@
             stats["error"] = root_stats.get("error")
     return failed
     
 def main():
     import getopt, sys, time
 
     t0 = time.time()    
-    opts, args = getopt.getopt(sys.argv[1:], "t:m:o:R:n:c:vqM:s:S:zd:kxe:r:")
+    opts, args = getopt.getopt(sys.argv[1:], "t:m:o:R:n:c:vqM:s:S:zkxe:r:")
     opts = dict(opts)
     
     if len(args) != 1 or not "-c" in opts:
         print(Usage)
         sys.exit(2)
 
     rse = args[0]
@@ -615,17 +624,14 @@
             print (Usage)
             sys.exit(2)
 
     output = opts.get("-o","out.list")
 
     out_list = PartitionedList.create(nparts, output, zout)
 
-    dir_output = opts.get("-d")
-    dir_list = PartitionedList.create(nparts, dir_output, zout) if dir_output else None
-    
     empty_dirs_file = None
     empty_dir_output = opts.get("-e")
     if empty_dir_output:
         if zout:
             if not empty_dir_output.endswith(".gz"):    empty_dir_output += ".gz"
             empty_dirs_file = gzip.open(empty_dir_output, "wt")
         else:
@@ -647,15 +653,14 @@
         "server_root":server_root,
         "server":server,
         "roots":[], 
         "start_time":time.time(),
         "end_time": None,
         "status":   "started",
         "files_output_prefix":          output,
-        "dirs_output_prefix":           dir_output,
         "empty_dirs_output_file":       empty_dir_output
     }
     
     if stats is not None:
         stats[stats_key] = my_stats
     
     root_paths = [canonic_path(root if root.startswith("/") else server_root + "/" + root) for root in config.RootList]
@@ -687,31 +692,29 @@
         for client, root in good_roots:
             try:
                 print(f"Scanning root {root} ...", file=sys.stderr)
                 expected = root_file_counts.get(root, 0) > 0
                 failed = scan_root(rse, config, client, root, expected, my_stats, stats, stats_key, 
                         quiet, display_progress, max_files,
                         recursive_threshold, max_scanners, timeout,
-                        out_list, dir_list, empty_dirs_file,
+                        out_list, empty_dirs_file,
                         ignore_directory_scan_errors, include_sizes)
             except:
                 exc = traceback.format_exc()
                 print(exc)
                 lines = exc.split("\n")
                 scanning = my_stats.setdefault("scanning", {"root":root})
                 scanning["exception"] = lines
                 scanning["exception_time"] = time.time()
                 failed = True
 
             if failed:
                 break
 
         out_list.close()
-        if dir_list is not None:
-            dir_list.close()
         if empty_dirs_file is not None:
             empty_dirs_file.close()
 
         total_files = sum(root_stats["files"] for root_stats in my_stats["roots"])
 
     if failed or all_roots_failed or total_files == 0:
         my_stats["status"] = "failed"
```

### Comparing `rucio-consistency-1.1.2/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.3.0/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.2/setup.py` & `rucio-consistency-1.3.0/setup.py`

 * *Files identical despite different names*

