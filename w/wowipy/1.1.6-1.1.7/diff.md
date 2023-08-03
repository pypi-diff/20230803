# Comparing `tmp/wowipy-1.1.6.tar.gz` & `tmp/wowipy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.6.tar", last modified: Wed Jul  5 08:29:36 2023, max compression
+gzip compressed data, was "wowipy-1.1.7.tar", last modified: Thu Aug  3 09:20:42 2023, max compression
```

## Comparing `wowipy-1.1.6.tar` & `wowipy-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.580701 wowipy-1.1.6/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.6/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-07-05 08:29:36.579707 wowipy-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-05 08:29:36.580701 wowipy-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-05 08:29:34.000000 wowipy-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.563746 wowipy-1.1.6/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.6/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.6/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    50382 2023-07-05 08:28:56.000000 wowipy-1.1.6/wowipy/models.py
--rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.6/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    43536 2023-07-05 08:07:06.000000 wowipy-1.1.6/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.578709 wowipy-1.1.6/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.048510 wowipy-1.1.7/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.7/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-08-03 09:20:42.047513 wowipy-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 09:20:42.048510 wowipy-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-08-03 09:20:23.000000 wowipy-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.032552 wowipy-1.1.7/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.7/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.7/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    56035 2023-08-03 09:04:47.000000 wowipy-1.1.7/wowipy/models.py
+-rw-rw-rw-   0        0        0     4577 2023-08-03 08:04:52.000000 wowipy-1.1.7/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    48072 2023-08-03 08:25:40.000000 wowipy-1.1.7/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.046540 wowipy-1.1.7/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.6/COPYING` & `wowipy-1.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.6/LICENSE` & `wowipy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.6/PKG-INFO` & `wowipy-1.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.6
+Version: 1.1.7
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.6/setup.py` & `wowipy-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.6',
+    version='1.1.7',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.6/wowipy/models.py` & `wowipy-1.1.7/wowipy/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1449,7 +1449,159 @@
         contract_position_type["id_"] = contract_position_type.pop("id")
         self.contract_position_type = ContractPositionType(**contract_position_type)
         if contract_position_type_slim is not None:
             contract_position_type_slim["id_"] = contract_position_type_slim.pop("id")
             self.contract_position_type_slim = ContractPositionTypeSlim(**contract_position_type_slim)
         else:
             self.contract_position_type_slim = None
+
+
+class TicketComment:
+    id_: int
+    created_at: datetime
+    content: str
+    user_name: str
+
+    def __init__(self, id_: int, created_at: str, content: str, user_name: str) -> None:
+        self.id_ = id_
+        self.created_at = datetime.strptime(created_at, "%Y-%m-%dT%H:%M:%S.%f%z")
+        self.content = content
+        self.user_name = user_name
+
+
+class TicketAssignment:
+    id_: int
+    assignment_entity_id: int
+    assignment_entity_code: str
+    entity_id: int
+
+    def __init__(self,  assignment_entity_id: int, entity_id: int, id_: int = 0,
+                 assignment_entity_code: str = "") -> None:
+        self.id_ = id_
+        self.assignment_entity_id = assignment_entity_id
+        self.assignment_entity_code = assignment_entity_code
+        self.entity_id = entity_id
+
+
+class Ticket:
+    id_: int
+    id_num: str
+    time_received: datetime
+    subject: str
+    content: str
+    department_id: int
+    user_id: int
+    priority_id: int
+    priority_code: str
+    status_id: int
+    status_code: str
+    source_id: int
+    source_code: str
+    comments: Optional[List[TicketComment]]
+    main_assignment: Optional[TicketAssignment]
+    assignments: Optional[List[TicketAssignment]]
+
+    def __init__(self,
+                 id_: int,
+                 id_num: str,
+                 time_received: str,
+                 subject: str,
+                 content: str,
+                 department_id: int,
+                 user_id: int,
+                 priority: Dict,
+                 status: Dict,
+                 source: Dict,
+                 comments: List[Dict],
+                 main_assignment: Dict,
+                 assignment: List[Dict]
+                 ) -> None:
+        self.id_ = id_
+        self.id_num = id_num
+        try:
+            self.time_received = datetime.strptime(time_received, "%Y-%m-%dT%H:%M:%S.%f%z")
+        except ValueError:
+            self.time_received = datetime.strptime(time_received, "%Y-%m-%dT%H:%M:%S%z")
+        self.subject = subject
+        self.content = content
+        self.department_id = department_id
+        self.user_id = user_id
+        self.priority_id = priority["id"]
+        self.priority_code = priority["code"]
+        self.status_id = status["id"]
+        self.status_code = status["code"]
+        self.source_id = source["id"]
+        self.source_code = source["code"]
+
+        self.comments = []
+        if comments is not None and len(comments) > 0:
+            for tentry in comments:
+                try:
+                    tcomment = TicketComment(id_=tentry["id"],
+                                             created_at=tentry["created_at"],
+                                             content=tentry["content"],
+                                             user_name=tentry["user_name"])
+                    self.comments.append(tcomment)
+                except KeyError as e:
+                    print(f"Key error: {e.args}")
+                    continue
+
+        if main_assignment is not None:
+            try:
+                tassignment = TicketAssignment(id_=main_assignment["id"],
+                                               assignment_entity_id=main_assignment["assignment_entity"]["id"],
+                                               assignment_entity_code=main_assignment["assignment_entity"]["code"],
+                                               entity_id=main_assignment["entity_id"])
+                self.main_assignment = tassignment
+            except KeyError as e:
+                print(f"Key error: {e.args}")
+        else:
+            self.main_assignment = None
+
+        # Hinweis: Im JSON lautet dieser Wert "assignment", wir verwenden in der Klasse jedoch "assignments", weil
+        # ich das passender finde
+        self.assignments = []
+        if assignment is not None and len(assignment) > 0:
+            for tentry in assignment:
+                try:
+                    tassignment = TicketAssignment(id_=tentry["id"],
+                                                   assignment_entity_id=tentry["assignment_entity"]["id"],
+                                                   assignment_entity_code=tentry["assignment_entity"]["code"],
+                                                   entity_id=tentry["entity_id"])
+                    self.assignments.append(tassignment)
+                except KeyError as e:
+                    print(f"Key error: {e.args}")
+
+
+class CommunicationCatalog:
+    ticket_assignment_entity_name: Dict
+    ticket_priority_name: Dict
+    ticket_source_name: Dict
+    ticket_status_name: Dict
+    ticket_assignment_entity_id: Dict
+    ticket_priority_id: Dict
+    ticket_source_id: Dict
+    ticket_status_id: Dict
+
+    def __init__(self,
+                 source_catalogues: List[Dict]
+                 ) -> None:
+        dicts = []
+        dicts_rev = []
+        for tcat in source_catalogues:
+            tdict = {}
+            tdict_rev = {}
+            for tentry in tcat:
+                tdict[tentry["Id"]] = tentry["Code"]
+                tdict_rev[tentry["Code"]] = tentry["Id"]
+            dicts.append(tdict)
+            dicts_rev.append(tdict_rev)
+
+        self.ticket_assignment_entity_name = dicts[0]
+        self.ticket_priority_name = dicts[1]
+        self.ticket_source_name = dicts[2]
+        self.ticket_status_name = dicts[3]
+
+        self.ticket_assignment_entity_id = dicts_rev[0]
+        self.ticket_priority_id = dicts_rev[1]
+        self.ticket_source_id = dicts_rev[2]
+        self.ticket_status_id = dicts_rev[3]
```

### Comparing `wowipy-1.1.6/wowipy/rest_adapter.py` & `wowipy-1.1.7/wowipy/rest_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         if ep_params is None:
             ep_params = {}
 
         if http_method.upper() == "GET":
             if "limit" not in ep_params.keys():
                 ep_params["limit"] = 100
 
-        if ep_params.get("limit") > 100 or ep_params.get("limit") < 1:
-            raise WowiPyException("Wert für limit muss zwischen 1 und 100 liegen")
+            if ep_params.get("limit") > 100 or ep_params.get("limit") < 1:
+                raise WowiPyException("Wert für limit muss zwischen 1 und 100 liegen")
         ep_params["apiKey"] = self.api_key
 
         full_url = self.url + endpoint
         headers = {
             'Accept': 'text/plain',
             'Authorization': f'Bearer {self.token}'
         }
@@ -99,8 +99,8 @@
 
         is_success = 200 <= response.status_code <= 299
         log_line = log_line_post.format(is_success, response.status_code, response.reason)
         if is_success:
             self._logger.debug(msg=log_line)
             return Result(response.status_code, message=response.reason, data=data_out)
         self._logger.error(msg=log_line)
-        raise WowiPyException(f"{response.status_code}: {response.reason}")
+        raise WowiPyException(f"{response.status_code}: {response.reason} -> {response.text}")
```

### Comparing `wowipy-1.1.6/wowipy/wowipy.py` & `wowipy-1.1.7/wowipy/wowipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -903,7 +903,123 @@
         for entry in result.data:
             data = dict(humps.decamelize(entry))
             data['id_'] = data.pop('id')
             ret_la = ContractPosition(**data)
             retlist.append(ret_la)
 
         return retlist
+
+    def get_tickets(self,
+                    ticket_id: int = None,
+                    ticket_id_num: str = None,
+                    ticket_priority_id: int = None,
+                    ticket_status_id: int = None,
+                    ticket_source_id: int = None,
+                    limit: int = None,
+                    offset: int = 0,
+                    add_args: Dict = None
+                    ) -> List[Ticket]:
+
+        filter_params = {}
+        if ticket_id is not None:
+            filter_params['ticketId'] = ticket_id
+        if ticket_id_num is not None:
+            filter_params['ticketIdNum'] = ticket_id_num
+        if ticket_priority_id is not None:
+            filter_params['ticketPriorityId'] = ticket_priority_id
+        if ticket_status_id is not None:
+            filter_params['ticketStatusId'] = ticket_status_id
+        if ticket_source_id is not None:
+            filter_params['ticketSourceId'] = ticket_source_id
+
+        if limit is not None:
+            filter_params['limit'] = limit
+        filter_params['offset'] = offset
+
+        # Standardparameter, können via add_args überschrieben werden
+        filter_params['includeComments'] = 'true'
+        filter_params['includeAssignmentEntity'] = 'true'
+        filter_params['showNullValues'] = 'true'
+
+        if add_args is not None:
+            filter_params.update(add_args)
+
+        retlist = []
+
+        result = self._rest_adapter.get(endpoint='CommunicationRead/Ticket', ep_params=filter_params)
+        for entry in result.data:
+            data = dict(humps.decamelize(entry))
+            data['id_'] = data.pop('id')
+            ret_la = Ticket(**data)
+            retlist.append(ret_la)
+
+        return retlist
+
+    def get_communication_catalogs(self) -> CommunicationCatalog:
+        cat_ass = self._rest_adapter.get(endpoint='CommunicationCatalog/TicketAssignmentEntity').data
+        cat_prio = self._rest_adapter.get(endpoint='CommunicationCatalog/TicketPriority').data
+        cat_source = self._rest_adapter.get(endpoint='CommunicationCatalog/TicketSource').data
+        cat_status = self._rest_adapter.get(endpoint='CommunicationCatalog/TicketStatus').data
+
+        cat_list = [
+            cat_ass,
+            cat_prio,
+            cat_source,
+            cat_status
+        ]
+
+        return CommunicationCatalog(cat_list)
+
+    def create_ticket(self,
+                      subject: str,
+                      content: str,
+                      source_id: int,
+                      main_assignment: TicketAssignment = None,
+                      assignments: List[TicketAssignment] = None,
+                      department_id: int = None,
+                      user_id: int = None,
+                      priority_id: int = 1
+                      ) -> Result:
+        data_dict = {
+            "Subject": subject,
+            "Content": content,
+            "SourceId": source_id,
+            "PriorityId": priority_id,
+        }
+        if department_id is not None:
+            data_dict["DepartmentId"] = department_id
+        if user_id is not None:
+            data_dict["UserId"] = user_id
+
+        data_dict["MainEntityAssignment"] = None
+        if main_assignment is not None:
+            tmain_ass = {
+                "AssignmentEntityId": main_assignment.assignment_entity_id,
+                "EntityId": main_assignment.entity_id
+            }
+            data_dict["MainEntityAssignment"] = tmain_ass
+
+        if assignments is not None and len(assignments) > 0:
+            asslist = []
+            for tentry in assignments:
+                tass = {
+                    "AssignmentEntityId": tentry.assignment_entity_id,
+                    "EntityId": tentry.entity_id
+                }
+                asslist.append(tass)
+            if len(asslist) > 0:
+                data_dict["EntityAssignments"] = asslist
+        print(f"MAIN: {data_dict['MainEntityAssignment']}")
+        result = self._rest_adapter.post(endpoint='CommunicationEdit/Ticket', data=data_dict)
+        return result
+
+    def create_ticket_comment(self,
+                              ticket_id: int,
+                              content: str
+                              ) -> Result:
+        data_dict = {
+            "TicketId": ticket_id,
+            "Content": content
+        }
+
+        result = self._rest_adapter.post(endpoint='CommunicationEdit/Ticket/AddComment', data=data_dict)
+        return result
```

### Comparing `wowipy-1.1.6/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.7/wowipy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.6
+Version: 1.1.7
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

