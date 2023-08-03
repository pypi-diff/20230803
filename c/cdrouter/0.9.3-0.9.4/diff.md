# Comparing `tmp/cdrouter-0.9.3.tar.gz` & `tmp/cdrouter-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdrouter-0.9.3.tar", last modified: Fri May  5 14:24:24 2023, max compression
+gzip compressed data, was "dist/cdrouter-0.9.4.tar", last modified: Thu Aug  3 19:34:22 2023, max compression
```

## Comparing `cdrouter-0.9.3.tar` & `cdrouter-0.9.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter/
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13566 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/alerts.py
--rw-r--r--   0 root         (0) root         (0)     4747 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/annotations.py
--rw-r--r--   0 root         (0) root         (0)     7330 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/attachments.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/captures.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.3/cdrouter/cdr_datetime.py
--rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.3/cdrouter/cdr_error.py
--rw-r--r--   0 root         (0) root         (0)    18456 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/cdrouter.py
--rw-r--r--   0 root         (0) root         (0)    22555 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/configs.py
--rw-r--r--   0 root         (0) root         (0)    17803 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/devices.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.3/cdrouter/exports.py
--rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.3/cdrouter/filters.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/highlights.py
--rw-r--r--   0 root         (0) root         (0)     3481 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/history.py
--rw-r--r--   0 root         (0) root         (0)     9626 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/imports.py
--rw-r--r--   0 root         (0) root         (0)    11399 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/jobs.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/metrics.py
--rw-r--r--   0 root         (0) root         (0)    17223 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/packages.py
--rw-r--r--   0 root         (0) root         (0)    40582 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/results.py
--rw-r--r--   0 root         (0) root         (0)    21568 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/system.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/tags.py
--rw-r--r--   0 root         (0) root         (0)    20275 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/testresults.py
--rw-r--r--   0 root         (0) root         (0)    24462 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/testsuites.py
--rw-r--r--   0 root         (0) root         (0)     9961 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7138 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 13:04:57.000000 cdrouter-0.9.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-05 14:24:24.000000 cdrouter-0.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-05 13:04:57.000000 cdrouter-0.9.3/setup.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-05-05 14:24:24.000000 cdrouter-0.9.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:34:22.000000 cdrouter-0.9.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-08-03 19:34:21.000000 cdrouter-0.9.4/cdrouter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/alerts.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/annotations.py
+-rw-r--r--   0 root         (0) root         (0)     7330 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/attachments.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/captures.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.4/cdrouter/cdr_datetime.py
+-rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.4/cdrouter/cdr_error.py
+-rw-r--r--   0 root         (0) root         (0)    18456 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/cdrouter.py
+-rw-r--r--   0 root         (0) root         (0)    22555 2023-05-05 14:23:20.000000 cdrouter-0.9.4/cdrouter/configs.py
+-rw-r--r--   0 root         (0) root         (0)    17803 2023-05-05 14:23:20.000000 cdrouter-0.9.4/cdrouter/devices.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.4/cdrouter/exports.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.4/cdrouter/filters.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/highlights.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/history.py
+-rw-r--r--   0 root         (0) root         (0)     9626 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/imports.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2023-08-03 19:17:58.000000 cdrouter-0.9.4/cdrouter/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    17995 2023-08-03 19:17:58.000000 cdrouter-0.9.4/cdrouter/packages.py
+-rw-r--r--   0 root         (0) root         (0)    40582 2023-05-05 14:23:20.000000 cdrouter-0.9.4/cdrouter/results.py
+-rw-r--r--   0 root         (0) root         (0)    21573 2023-08-03 19:17:58.000000 cdrouter-0.9.4/cdrouter/system.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20275 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/testresults.py
+-rw-r--r--   0 root         (0) root         (0)    24462 2023-05-05 13:02:04.000000 cdrouter-0.9.4/cdrouter/testsuites.py
+-rw-r--r--   0 root         (0) root         (0)     9961 2023-05-05 14:23:20.000000 cdrouter-0.9.4/cdrouter/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-03 19:34:22.000000 cdrouter-0.9.4/cdrouter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 13:04:57.000000 cdrouter-0.9.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-08-03 19:34:22.000000 cdrouter-0.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-05 13:04:57.000000 cdrouter-0.9.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-08-03 19:34:22.000000 cdrouter-0.9.4/PKG-INFO
```

### Comparing `cdrouter-0.9.3/cdrouter/alerts.py` & `cdrouter-0.9.4/cdrouter/alerts.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/annotations.py` & `cdrouter-0.9.4/cdrouter/annotations.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/attachments.py` & `cdrouter-0.9.4/cdrouter/attachments.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/captures.py` & `cdrouter-0.9.4/cdrouter/captures.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/cdr_datetime.py` & `cdrouter-0.9.4/cdrouter/cdr_datetime.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/cdrouter.py` & `cdrouter-0.9.4/cdrouter/cdrouter.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/configs.py` & `cdrouter-0.9.4/cdrouter/configs.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/devices.py` & `cdrouter-0.9.4/cdrouter/devices.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/exports.py` & `cdrouter-0.9.4/cdrouter/exports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/filters.py` & `cdrouter-0.9.4/cdrouter/filters.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/highlights.py` & `cdrouter-0.9.4/cdrouter/highlights.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/history.py` & `cdrouter-0.9.4/cdrouter/history.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/imports.py` & `cdrouter-0.9.4/cdrouter/imports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/jobs.py` & `cdrouter-0.9.4/cdrouter/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     :param updated: (optional) Job last-updated time as `DateTime`.
     :param automatic: (optional) Bool `True` if job scheduled automatically `DateTime`.
     :param run_at: (optional) Job scheduled run-time `DateTime`.
     :param interfaces: (optional) :class:`configs.Interfaces <configs.Interfaces>` list
     :param interface_names: (optional) Job interface names as string list.
     :param uses_wireless: (optional) Bool `True` if job uses any wireless interfaces.
     :param uses_ics: (optional) Bool `True` if job uses any ICS interfaces.
+    :param ics_interface_name: (optional) If uses_ics is `True`, ICS interface name as string.
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.active = kwargs.get('active', None)
         self.status = kwargs.get('status', None)
         self.options = kwargs.get('options', None)
         self.package_id = kwargs.get('package_id', None)
@@ -85,14 +86,15 @@
         self.updated = kwargs.get('updated', None)
         self.automatic = kwargs.get('automatic', None)
         self.run_at = kwargs.get('run_at', None)
         self.interfaces = kwargs.get('interfaces', None)
         self.interface_names = kwargs.get('interface_names', None)
         self.uses_wireless = kwargs.get('uses_wireless', None)
         self.uses_ics = kwargs.get('uses_ics', None)
+        self.ics_interface_name = kwargs.get('ics_interface_name', None)
 
 class JobSchema(Schema):
     id = fields.Int(as_string=True)
     active = fields.Bool()
     status = fields.Str()
     options = fields.Nested(OptionsSchema, unknown=EXCLUDE)
     package_id = fields.Int(as_string=True)
@@ -107,14 +109,15 @@
     updated = DateTime()
     automatic = fields.Bool()
     run_at = DateTime()
     interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
     interface_names = fields.List(fields.Str())
     uses_wireless = fields.Bool()
     uses_ics = fields.Bool()
+    ics_interface_name = fields.Str(load_default=None)
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Job(**data)
@@ -180,29 +183,29 @@
     def edit(self, resource):
         """Edit a job.
 
         :param resource: :class:`jobs.Job <jobs.Job>` object
         :return: :class:`jobs.Job <jobs.Job>` object
         :rtype: jobs.Job
         """
-        schema = JobSchema(exclude=('id', 'active', 'status', 'options', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'run_at', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics'))
+        schema = JobSchema(exclude=('id', 'active', 'status', 'options', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'run_at', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics', 'ics_interface_name'))
         json = self.service.encode(schema, resource)
 
         schema = JobSchema()
         resp = self.service.edit(self.base, resource.id, json)
         return self.service.decode(schema, resp)
 
     def launch(self, resource):
         """Launch a new job.
 
         :param resource: :class:`jobs.Job <jobs.Job>` object
         :return: :class:`jobs.Job <jobs.Job>` object
         :rtype: jobs.Job
         """
-        schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics'))
+        schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics', 'ics_interface_name'))
         json = self.service.encode(schema, resource)
 
         schema = JobSchema()
         resp = self.service.create(self.base, json)
         return self.service.decode(schema, resp)
 
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
@@ -214,15 +217,15 @@
 
     def get_interfaces(self, resource):
         """Process job with cdrouter-cli -print-interfaces.
 
         :param resource: :class:`jobs.Job <jobs.Job>` object
         :return: :class:`configs.Interfaces <configs.Interfaces>` list
         """
-        schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics'))
+        schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics', 'ics_interface_name'))
         json = self.service.encode(schema, resource)
 
         schema = InterfacesSchema()
         resp = self.service.post(self.base,
                                  params={'process': 'interfaces'}, json=json)
         return self.service.decode(schema, resp, many=True)
 
@@ -238,15 +241,15 @@
         """
         json = {}
         if jobs is not None:
             schema = JobSchema()
             jobs_json = self.service.encode(schema, jobs, many=True)
             json[self.RESOURCE] = jobs_json
         elif _fields is not None:
-            schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics'))
+            schema = JobSchema(exclude=('id', 'active', 'status', 'package_name', 'config_name', 'device_name', 'result_id', 'user_id', 'created', 'updated', 'automatic', 'interfaces', 'interface_names', 'uses_wireless', 'uses_ics', 'ics_interface_name'))
             jobs_json = self.service.encode(schema, _fields)
             json['fields'] = jobs_json
 
         schema = JobSchema()
         resp = self.service.post(self.base,
                                  params={'bulk': 'launch', 'filter': filter, 'type': type, 'all': all}, json=json)
         return self.service.decode(schema, resp, many=True)
```

### Comparing `cdrouter-0.9.3/cdrouter/metrics.py` & `cdrouter-0.9.4/cdrouter/metrics.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/packages.py` & `cdrouter-0.9.4/cdrouter/packages.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,41 +46,50 @@
     """Model for CDRouter Package Options.
 
     :param forever: (optional) Bool `True` if package looped forver.
     :param loop: (optional) Loop count as an int.
     :param repeat: (optional) Repeat count as an int.
     :param maxfail: (optional) Max fail count as an int.
     :param duration: (optional) Max testing time duration as an int.
+    :param duration_units: (optional) Units for max testing time duration as string.  Must be `seconds`, `minutes`, `hours` or `days`.
+    :param duration_interrupt: (optional) Bool `True` if max testing time duration elapsing should interrupt currently running test.
+    :param duration_no_error: (optional) Bool `True` if max testing time duration elapsing should not be considered an error.
     :param wait: (optional) Wait between tests duration as an int.
     :param pause: (optional) Bool `True` if pausing between tests.
     :param shuffle: (optional) Bool `True` if testlist is shuffled.
     :param seed: (optional) Shuffle seed as an int.
     :param retry: (optional) Retry count as an int.
     :param rdelay: (optional) Retry delay as an int.
     """
     def __init__(self, **kwargs):
         self.forever = kwargs.get('forever', None)
         self.loop = kwargs.get('loop', None)
         self.repeat = kwargs.get('repeat', None)
         self.maxfail = kwargs.get('maxfail', None)
         self.duration = kwargs.get('duration', None)
+        self.duration_units = kwargs.get('duration_units', None)
+        self.duration_interrupt = kwargs.get('duration_interrupt', None)
+        self.duration_no_error = kwargs.get('duration_no_error', None)
         self.wait = kwargs.get('wait', None)
         self.pause = kwargs.get('pause', None)
         self.shuffle = kwargs.get('shuffle', None)
         self.seed = kwargs.get('seed', None)
         self.retry = kwargs.get('retry', None)
         self.rdelay = kwargs.get('rdelay', None)
         self.sync = kwargs.get('sync', None)
 
 class OptionsSchema(Schema):
     forever = fields.Bool()
     loop = fields.Int(as_string=True)
     repeat = fields.Int(as_string=True)
     maxfail = fields.Int(as_string=True)
     duration = fields.Int(as_string=True)
+    duration_units = fields.Str(load_default='seconds')
+    duration_interrupt = fields.Bool(load_default=False)
+    duration_no_error = fields.Bool(load_default=False)
     wait = fields.Int(as_string=True)
     pause = fields.Bool()
     shuffle = fields.Bool()
     seed = fields.Int(as_string=True)
     retry = fields.Int(as_string=True)
     rdelay = fields.Int(as_string=True)
     sync = fields.Bool()
```

### Comparing `cdrouter-0.9.3/cdrouter/results.py` & `cdrouter-0.9.4/cdrouter/results.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/system.py` & `cdrouter-0.9.4/cdrouter/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Release(**data)
 
 class Upgrade(object):
     """Model for CDRouter Upgrades.
 
     :param success: (optional) Bool `True` if successful.
-    :param installer: (optional) Installer filename as string.
+    :param installer_path: (optional) Installer filename as string.
     :param output: (optional) Output as string.
     :param error: (optional) Error output as string.
     """
     def __init__(self, **kwargs):
         self.success = kwargs.get('success', None)
         self.installer_path = kwargs.get('installer_path', None)
         self.output = kwargs.get('output', None)
```

### Comparing `cdrouter-0.9.3/cdrouter/tags.py` & `cdrouter-0.9.4/cdrouter/tags.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/testresults.py` & `cdrouter-0.9.4/cdrouter/testresults.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/testsuites.py` & `cdrouter-0.9.4/cdrouter/testsuites.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter/users.py` & `cdrouter-0.9.4/cdrouter/users.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/cdrouter.egg-info/PKG-INFO` & `cdrouter-0.9.4/cdrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

### Comparing `cdrouter-0.9.3/cdrouter.egg-info/SOURCES.txt` & `cdrouter-0.9.4/cdrouter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/LICENSE.txt` & `cdrouter-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/README.rst` & `cdrouter-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/setup.py` & `cdrouter-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.3/PKG-INFO` & `cdrouter-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

