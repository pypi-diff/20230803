# Comparing `tmp/robotcloud-client-0.0.7.tar.gz` & `tmp/robotcloud-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotcloud-client-0.0.7.tar", last modified: Thu Jul  6 06:46:32 2023, max compression
+gzip compressed data, was "dist/robotcloud-client-0.0.8.tar", last modified: Thu Aug  3 13:16:06 2023, max compression
```

## Comparing `robotcloud-client-0.0.7.tar` & `robotcloud-client-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.364198 robotcloud-client-0.0.7/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-07-06 06:46:32.364198 robotcloud-client-0.0.7/PKG-INFO
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      582 2023-03-22 07:06:52.000000 robotcloud-client-0.0.7/README.md
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.360198 robotcloud-client-0.0.7/robotcloud/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-16 08:53:35.000000 robotcloud-client-0.0.7/robotcloud/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     5103 2022-07-08 06:05:41.000000 robotcloud-client-0.0.7/robotcloud/api.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      765 2022-03-22 07:09:51.000000 robotcloud-client-0.0.7/robotcloud/authenticator.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      261 2022-07-08 06:21:11.000000 robotcloud-client-0.0.7/robotcloud/constants.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.360198 robotcloud-client-0.0.7/robotcloud/endpoints/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      306 2022-07-08 10:10:07.000000 robotcloud-client-0.0.7/robotcloud/endpoints/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1100 2023-03-27 10:21:54.000000 robotcloud-client-0.0.7/robotcloud/endpoints/applications.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2760 2022-04-21 07:37:05.000000 robotcloud-client-0.0.7/robotcloud/endpoints/configurationtypes.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2199 2023-03-16 07:43:25.000000 robotcloud-client-0.0.7/robotcloud/endpoints/devices.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1157 2023-03-20 11:23:25.000000 robotcloud-client-0.0.7/robotcloud/endpoints/locations.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      630 2023-03-16 08:34:00.000000 robotcloud-client-0.0.7/robotcloud/endpoints/login.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1935 2022-07-08 06:51:48.000000 robotcloud-client-0.0.7/robotcloud/endpoints/organizations.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3036 2023-03-31 05:38:34.000000 robotcloud-client-0.0.7/robotcloud/endpoints/projects.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     7334 2023-06-29 07:44:27.000000 robotcloud-client-0.0.7/robotcloud/endpoints/services.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1604 2023-06-30 11:41:21.000000 robotcloud-client-0.0.7/robotcloud/endpoints/services_classifiers.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3705 2022-06-06 05:41:10.000000 robotcloud-client-0.0.7/robotcloud/endpoints/services_data.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1167 2022-04-08 09:23:38.000000 robotcloud-client-0.0.7/robotcloud/endpoints/subsystems.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1141 2022-07-08 05:52:20.000000 robotcloud-client-0.0.7/robotcloud/endpoints/tags.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2347 2023-03-16 08:37:33.000000 robotcloud-client-0.0.7/robotcloud/endpoints/users.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1255 2022-07-08 08:22:31.000000 robotcloud-client-0.0.7/robotcloud/exceptions.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.360198 robotcloud-client-0.0.7/robotcloud/utils/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      117 2022-07-08 08:22:45.000000 robotcloud-client-0.0.7/robotcloud/utils/__init__.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.360198 robotcloud-client-0.0.7/robotcloud/utils/datatables/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2022-05-10 13:46:31.000000 robotcloud-client-0.0.7/robotcloud/utils/datatables/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      428 2022-07-08 06:17:40.000000 robotcloud-client-0.0.7/robotcloud/utils/datatables/request.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      551 2022-07-08 06:17:51.000000 robotcloud-client-0.0.7/robotcloud/utils/datatables/response.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      235 2022-05-10 13:46:31.000000 robotcloud-client-0.0.7/robotcloud/utils/paginated_response.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      286 2023-03-16 08:04:55.000000 robotcloud-client-0.0.7/robotcloud/utils/pagination.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-07-06 06:46:32.364198 robotcloud-client-0.0.7/robotcloud_client.egg-info/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-07-06 06:46:32.000000 robotcloud-client-0.0.7/robotcloud_client.egg-info/PKG-INFO
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1058 2023-07-06 06:46:32.000000 robotcloud-client-0.0.7/robotcloud_client.egg-info/SOURCES.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        1 2023-07-06 06:46:32.000000 robotcloud-client-0.0.7/robotcloud_client.egg-info/dependency_links.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       15 2023-07-06 06:46:32.000000 robotcloud-client-0.0.7/robotcloud_client.egg-info/requires.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       11 2023-07-06 06:46:32.000000 robotcloud-client-0.0.7/robotcloud_client.egg-info/top_level.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      157 2023-07-06 06:46:32.364198 robotcloud-client-0.0.7/setup.cfg
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1408 2023-07-06 06:43:58.000000 robotcloud-client-0.0.7/setup.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/PKG-INFO
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      582 2023-03-22 07:06:52.000000 robotcloud-client-0.0.8/README.md
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.348526 robotcloud-client-0.0.8/robotcloud/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-16 08:53:35.000000 robotcloud-client-0.0.8/robotcloud/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     5103 2022-07-08 06:05:41.000000 robotcloud-client-0.0.8/robotcloud/api.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      765 2022-03-22 07:09:51.000000 robotcloud-client-0.0.8/robotcloud/authenticator.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      261 2022-07-08 06:21:11.000000 robotcloud-client-0.0.8/robotcloud/constants.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/robotcloud/endpoints/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      306 2022-07-08 10:10:07.000000 robotcloud-client-0.0.8/robotcloud/endpoints/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1100 2023-03-27 10:21:54.000000 robotcloud-client-0.0.8/robotcloud/endpoints/applications.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2760 2022-04-21 07:37:05.000000 robotcloud-client-0.0.8/robotcloud/endpoints/configurationtypes.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2199 2023-03-16 07:43:25.000000 robotcloud-client-0.0.8/robotcloud/endpoints/devices.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1157 2023-03-20 11:23:25.000000 robotcloud-client-0.0.8/robotcloud/endpoints/locations.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      630 2023-03-16 08:34:00.000000 robotcloud-client-0.0.8/robotcloud/endpoints/login.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1935 2022-07-08 06:51:48.000000 robotcloud-client-0.0.8/robotcloud/endpoints/organizations.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3036 2023-03-31 05:38:34.000000 robotcloud-client-0.0.8/robotcloud/endpoints/projects.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     7562 2023-07-13 11:25:39.000000 robotcloud-client-0.0.8/robotcloud/endpoints/services.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1604 2023-06-30 11:41:21.000000 robotcloud-client-0.0.8/robotcloud/endpoints/services_classifiers.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3705 2022-06-06 05:41:10.000000 robotcloud-client-0.0.8/robotcloud/endpoints/services_data.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1167 2022-04-08 09:23:38.000000 robotcloud-client-0.0.8/robotcloud/endpoints/subsystems.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1141 2022-07-08 05:52:20.000000 robotcloud-client-0.0.8/robotcloud/endpoints/tags.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2347 2023-03-16 08:37:33.000000 robotcloud-client-0.0.8/robotcloud/endpoints/users.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1255 2022-07-08 08:22:31.000000 robotcloud-client-0.0.8/robotcloud/exceptions.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/robotcloud/utils/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      117 2022-07-08 08:22:45.000000 robotcloud-client-0.0.8/robotcloud/utils/__init__.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/robotcloud/utils/datatables/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2022-05-10 13:46:31.000000 robotcloud-client-0.0.8/robotcloud/utils/datatables/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      428 2022-07-08 06:17:40.000000 robotcloud-client-0.0.8/robotcloud/utils/datatables/request.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      551 2022-07-08 06:17:51.000000 robotcloud-client-0.0.8/robotcloud/utils/datatables/response.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      235 2022-05-10 13:46:31.000000 robotcloud-client-0.0.8/robotcloud/utils/paginated_response.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      286 2023-03-16 08:04:55.000000 robotcloud-client-0.0.8/robotcloud/utils/pagination.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/robotcloud_client.egg-info/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-08-03 13:16:06.000000 robotcloud-client-0.0.8/robotcloud_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1058 2023-08-03 13:16:06.000000 robotcloud-client-0.0.8/robotcloud_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        1 2023-08-03 13:16:06.000000 robotcloud-client-0.0.8/robotcloud_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       15 2023-08-03 13:16:06.000000 robotcloud-client-0.0.8/robotcloud_client.egg-info/requires.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       11 2023-08-03 13:16:06.000000 robotcloud-client-0.0.8/robotcloud_client.egg-info/top_level.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      157 2023-08-03 13:16:06.352526 robotcloud-client-0.0.8/setup.cfg
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1408 2023-07-13 11:45:39.000000 robotcloud-client-0.0.8/setup.py
```

### Comparing `robotcloud-client-0.0.7/PKG-INFO` & `robotcloud-client-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcloud-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client to interact with robotcloud API from a python project.
 Home-page: https://github.com/robotmallorca/sw.module.python.robotcloud.client
 Author: Bernat Galmés Rubert
 Author-email: bernat.galmes@robotbas.com
 Keywords: client,robotcloud
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `robotcloud-client-0.0.7/README.md` & `robotcloud-client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/api.py` & `robotcloud-client-0.0.8/robotcloud/api.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/authenticator.py` & `robotcloud-client-0.0.8/robotcloud/authenticator.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/applications.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/applications.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/configurationtypes.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/configurationtypes.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/devices.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/devices.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/locations.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/locations.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/login.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/organizations.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/organizations.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/projects.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/services.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,43 +107,47 @@
         super().__init__(token)
 
     def get_endpoint(self):
         return f'projects/{self.project_id}/services/{self.service_type}/instances/{self.instance_id}/deviceconf'
 
 
 SERVICES_TYPES = [
-    {'code': 'AirHandlingUnit_1', 'description': 'Air Handling Unit v1'},  # Nou!
-    {'code': 'AirQuality_1', 'description': 'Air Quality v1'},  # Nou!
-    {'code': 'ChillerHeatingPump_1', 'description': 'Chiller Heating Pump v1'},  # Nou!
+    {'code': 'AirHandlingUnit_1', 'description': 'Air Handling Unit v1'},
+    {'code': 'AirQuality_1', 'description': 'Air Quality v1', 'groups': ['rooms']},
+    {'code': 'ChillerHeatingPump_1', 'description': 'Chiller Heating Pump v1'},
 
     {'code': 'CoolHeatProd_1', 'description': 'Cool & Heat Producer v1'},
     {'code': 'CoolHeatCons_1', 'description': 'Cool & Heat Consumer v1'},
     {'code': 'EnergyCounter_1', 'description': 'Energy Counter v1'},
     {'code': 'EnergyProduction_1', 'description': 'Energy Production v1'},
 
-    {'code': 'GasCounter_1', 'description': 'Gas Counter v1'},  # Nou!
+    {'code': 'GasCounter_1', 'description': 'Gas Counter v1'},
 
     {'code': 'HeatMeter_1', 'description': 'Heat Meter v1'},
     {'code': 'HeatProd_1', 'description': 'Heat Producer v1'},
     {'code': 'OutdoorClime_1', 'description': 'OutdoorClime_1'},
     {'code': 'PowerMeter_1', 'description': 'Power Meter v1'},
-    {'code': 'RoomClime_1', 'description': 'Room Clime v1'},
-    {'code': 'RoomConsumes_1', 'description': 'Room Consumes v1'},
+    {'code': 'RoomClime_1', 'description': 'Room Clime v1', 'groups': ['rooms']},
+    {'code': 'RoomConsumes_1', 'description': 'Room Consumes v1', 'groups': ['rooms']},
 
-    {'code': 'RoomDiagnostics_1', 'description': 'Room Diagnostics v1'},  # Nou!
-    {'code': 'RoomGuestStatus_1', 'description': 'Room Guest Status v1'},
+    {'code': 'RoomDiagnostics_1', 'description': 'Room Diagnostics v1', 'groups': ['rooms']},
+    {'code': 'RoomGuestStatus_1', 'description': 'Room Guest Status v1', 'groups': ['rooms']},
     {'code': 'TemporizedOutput_1', 'description': 'Temporized Output v1'},
     {'code': 'WaterCounter_1', 'description': 'Water Counter v1'},
 ]
 
 
 def get_services_types(token):
     return SERVICES_TYPES
 
 
+def get_services_types_by_group(token, group: str):
+    return [svc_type for svc_type in SERVICES_TYPES if 'groups' in svc_type and group in svc_type['groups']]
+
+
 def get_location_services(token, project_id, location_id):
     return APICallLocationServices(token, project_id, location_id).get()
 
 
 def get_location_services_instances(token, project_id, location_id, service_type):
     return APICallLocationServicesInstances(token, project_id, location_id, service_type).get()
```

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/services_classifiers.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/services_classifiers.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/services_data.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/services_data.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/subsystems.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/subsystems.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/tags.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/endpoints/users.py` & `robotcloud-client-0.0.8/robotcloud/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/exceptions.py` & `robotcloud-client-0.0.8/robotcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud/utils/datatables/response.py` & `robotcloud-client-0.0.8/robotcloud/utils/datatables/response.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/robotcloud_client.egg-info/PKG-INFO` & `robotcloud-client-0.0.8/robotcloud_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcloud-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client to interact with robotcloud API from a python project.
 Home-page: https://github.com/robotmallorca/sw.module.python.robotcloud.client
 Author: Bernat Galmés Rubert
 Author-email: bernat.galmes@robotbas.com
 Keywords: client,robotcloud
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `robotcloud-client-0.0.7/robotcloud_client.egg-info/SOURCES.txt` & `robotcloud-client-0.0.8/robotcloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.7/setup.py` & `robotcloud-client-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='robotcloud-client',
-    version='0.0.7',
+    version='0.0.8',
     author="Bernat Galmés Rubert",
     author_email="bernat.galmes@robotbas.com",
     description="Client to interact with robotcloud API from a python project.",
     url='https://github.com/robotmallorca/sw.module.python.robotcloud.client',
     keywords="client,robotcloud",
     packages=find_packages(include=['robotcloud', 'robotcloud.endpoints', 'robotcloud.utils', 'robotcloud.utils.datatables']),
     long_description=read('README.md'),
```

