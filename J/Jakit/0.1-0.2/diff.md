# Comparing `tmp/Jakit-0.1.tar.gz` & `tmp/Jakit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jakit-0.1.tar", last modified: Tue Aug  1 16:56:11 2023, max compression
+gzip compressed data, was "Jakit-0.2.tar", last modified: Thu Aug  3 14:15:22 2023, max compression
```

## Comparing `Jakit-0.1.tar` & `Jakit-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:56:11.334680 Jakit-0.1/
-drwxrwxrwx   0        0        0        0 2023-08-01 16:56:11.308684 Jakit-0.1/Jakit/
--rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.1/Jakit/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-08-01 16:42:45.000000 Jakit-0.1/Jakit/jakit_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:56:11.330685 Jakit-0.1/Jakit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-01 16:56:11.000000 Jakit-0.1/Jakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-08-01 16:56:11.000000 Jakit-0.1/Jakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:56:11.000000 Jakit-0.1/Jakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 16:56:11.000000 Jakit-0.1/Jakit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.1/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-01 16:56:11.333687 Jakit-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 16:56:11.334680 Jakit-0.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-08-01 16:50:26.000000 Jakit-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.757667 Jakit-0.2/
+drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.737671 Jakit-0.2/Jakit/
+-rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.2/Jakit/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-08-03 13:26:48.000000 Jakit-0.2/Jakit/jakit_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.750671 Jakit-0.2/Jakit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      752 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.2/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-03 14:15:22.752673 Jakit-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:15:22.760667 Jakit-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1951 2023-08-03 14:15:07.000000 Jakit-0.2/setup.py
```

### Comparing `Jakit-0.1/Jakit/jakit_jobs.py` & `Jakit-0.2/Jakit/jakit_jobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pymongo
 from bson.objectid import ObjectId
 from Dager.dager_data import Database
+import requests
 
 Dager_client = "mongodb://DaggerData_rw:eEsQcKvMgKfH5Di@p1ir1mon019.ger.corp.intel.com:7174,p2ir1mon019.ger.corp.intel.com:7174,p3ir1mon019.ger.corp.intel.com:7174/DaggerData?ssl=true&replicaSet=mongo7174"
 Dager_conn = 'DaggerData'
 Jobs_status_coll = 'Jobs'
 
 ConnectionStringDager = pymongo.MongoClient(Dager_client)
 DatabaseDager = ConnectionStringDager[Dager_conn]
@@ -22,14 +23,22 @@
         """ Read from Mongo and Store into DataFrame """
 
         jobs = CollectionJobs.find({"_id": {"$in": jobids}})
         list_jobs = list(jobs)
 
         return list_jobs
     
+    def report_info(self,reportid,toolid):
+        """call jakit api"""
+        # get request to jakit api
+        report_info = requests.get(f'https://JakitAPI.apps1-ir-int.icloud.intel.com/args?reportID={reportid}&toolID={toolid}')
+        
+        return report_info.json()
+
+
     def job_info(self,jobids,indicator_names):
         jobids = [ObjectId(jobid) for jobid in jobids]
         dager_data = Database()
         jobs_info = self.get_jobs(jobids)
 
 
         for job in jobs_info:
```

### Comparing `Jakit-0.1/Jakit.egg-info/PKG-INFO` & `Jakit-0.2/Jakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.1
+Version: 0.2
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.1/LICENSE` & `Jakit-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Jakit-0.1/PKG-INFO` & `Jakit-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.1
+Version: 0.2
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

