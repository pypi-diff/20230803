# Comparing `tmp/pih-mio-1.48022.tar.gz` & `tmp/pih-mio-1.48023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48022.tar", last modified: Wed Aug  2 07:45:03 2023, max compression
+gzip compressed data, was "pih-mio-1.48023.tar", last modified: Thu Aug  3 07:26:27 2023, max compression
```

## Comparing `pih-mio-1.48022.tar` & `pih-mio-1.48023.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:01.137763 pih-mio-1.48022/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:01.950268 pih-mio-1.48022/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48022/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48022/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48022/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48022/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48022/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48022/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-02 07:45:03.342405 pih-mio-1.48022/PKG-INFO
--rw-rw-rw-   0        0        0     1628 2023-08-02 06:40:52.000000 pih-mio-1.48022/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:03.264296 pih-mio-1.48022/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 07:45:03.358033 pih-mio-1.48022/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:25.652731 pih-mio-1.48023/
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.387111 pih-mio-1.48023/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48023/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48023/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165345 2023-08-03 07:25:43.000000 pih-mio-1.48023/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48023/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48023/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48023/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:26:27.921293 pih-mio-1.48023/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48023/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:27.530673 pih-mio-1.48023/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:26:23.000000 pih-mio-1.48023/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-03 07:26:25.000000 pih-mio-1.48023/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:26:23.000000 pih-mio-1.48023/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:26:27.968204 pih-mio-1.48023/setup.cfg
```

### Comparing `pih-mio-1.48022/MobileHelperCore/api.py` & `pih-mio-1.48023/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,19 @@
                             Note, ActionDescription, StorageValue, 
                             IntStorageValue, TimeStorageValue, BoolStorageValue,
                             CommandMenuItem)
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
+class MIO:
+
+    NAME: str = "mio"       
+    VERSION: str = "1.48023"  
+
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
 
 class AddressedInterruption(Exception):
@@ -1307,28 +1312,27 @@
         dump_name: str = PolibaseDBApi.get_default_name()
         answer: bool = self.input.yes_no(
             f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(dump_name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
         if A.A_P.DB.backup(self.input.answer if answer else dump_name):
             self.write_line(i(f"{self.user_given_name}, ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе {b('Backup Console')}"))
 
     def robocopy_job_run_handler(self) -> None:
-        from BackupCore.api import BackupApi
         forced: bool = self.is_forced
         source_job_name: str | None = self.first_arg()
         if not A.D_C.empty(source_job_name):
             source_job_name = source_job_name.lower()
         job_name_set: set = set()
         job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = defaultdict(list)
         job_status_list: list[RobocopyJobStatus] = A.R_B.robocopy_job_status_list().data
         job_status_map: dict[str, RobocopyJobStatus] = {}
         for job_status in job_status_list:
             job_name: str = job_status.name
             job_name_set.add(job_name)
             job_status_map_by_name[job_name].append(job_status)
-            job_status_map[BackupApi.get_job_full_name(
+            job_status_map[A.D_B.get_job_full_name(
                 job_status.name, job_status.source, job_status.destination)] = job_status
         job_name_list: list[str] = list(job_name_set)
         job_name_list.sort()
         if not A.D_C.empty(source_job_name) and source_job_name not in job_name_list:
             source_job_name = None
 
         def is_active(job_name: str) -> bool:
@@ -1347,15 +1351,15 @@
                 self.write_line(f"{b('Список Robocopy-заданий:')}\n")
 
             def job_status_list_label_function(name: str) -> str:
                 job_list: list[RobocopyJobStatus] = job_status_map_by_name[name]
                 def job_status_item_label_function(job_status: RobocopyJobStatus) -> str:
                     source: str = job_status.source
                     destination: str = job_status.destination
-                    job_status = job_status_map[BackupApi.get_job_full_name(
+                    job_status = job_status_map[A.D_B.get_job_full_name(
                         name, source, destination)]
                     status: int | None = None
                     date: str | None = None
                     if job_status.active:
                         date = "выполняется"
                     else:
                         if job_status.last_created is not None:
```

### Comparing `pih-mio-1.48022/MobileHelperCore/service.py` & `pih-mio-1.48023/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48022/MobileHelperCore/service_api.py` & `pih-mio-1.48023/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48022/MobileHelperCore/tools.py` & `pih-mio-1.48023/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48022/pih-mio_setup.py` & `pih-mio-1.48023/pih-mio_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import importlib.util
 import sys
 from setuptools import setup
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih import PIH
+from pih import A
 from pih.tools import j
+from MobileHelperCore.api import MIO
 
 #########################################################################################################
 """
 1. python mio_setup.py sdist --dist-dir mio_dist bdist_wheel --dist-dir mio_dist build --build-base pih_mio_build
 2. twine upload --repository pypi mio_dist/*
 3. pip install pih_mio -U
 """
@@ -24,23 +25,23 @@
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
-name: str = j((PIH.NAME, PIH.MIO.NAME), "-")
+name: str = j((A.root.NAME, MIO.NAME), "-")
 setup(
     name=name,
     entry_points={
         "console_scripts": [
             f"{name}=MobileHelperCore.__main__:start",
         ]
     },
-    version=PIH.VERSION.MIO.local(),
+    version=MIO.VERSION,
     description="PIH Mobile Helper library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
```

