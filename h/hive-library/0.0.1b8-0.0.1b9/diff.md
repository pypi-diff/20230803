# Comparing `tmp/hive_library-0.0.1b8.tar.gz` & `tmp/hive_library-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive_library-0.0.1b8.tar", last modified: Wed Mar 16 13:12:44 2022, max compression
+gzip compressed data, was "hive_library-0.0.1b9.tar", last modified: Wed Jul 27 13:50:33 2022, max compression
```

## Comparing `hive_library-0.0.1b8.tar` & `hive_library-0.0.1b9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-03-16 13:12:44.880068 hive_library-0.0.1b8/
--rw-r--r--   0 chipik     (501) staff       (20)     1063 2021-09-01 15:45:03.000000 hive_library-0.0.1b8/LICENSE
--rw-r--r--   0 chipik     (501) staff       (20)    19705 2022-03-16 13:12:44.879417 hive_library-0.0.1b8/PKG-INFO
--rw-r--r--   0 chipik     (501) staff       (20)    18700 2021-09-01 15:45:03.000000 hive_library-0.0.1b8/README.md
-drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-03-16 13:12:44.874228 hive_library-0.0.1b8/hive_library/
--rw-r--r--   0 chipik     (501) staff       (20)    47761 2022-03-05 11:26:26.000000 hive_library-0.0.1b8/hive_library/__init__.py
--rw-r--r--   0 chipik     (501) staff       (20)    19754 2022-03-05 11:26:26.000000 hive_library-0.0.1b8/hive_library/cli.py
--rw-r--r--   0 chipik     (501) staff       (20)     1252 2022-03-05 11:26:26.000000 hive_library-0.0.1b8/hive_library/enum.py
--rw-r--r--   0 chipik     (501) staff       (20)    89906 2022-03-16 13:06:35.000000 hive_library-0.0.1b8/hive_library/rest.py
-drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-03-16 13:12:44.878620 hive_library-0.0.1b8/hive_library.egg-info/
--rw-r--r--   0 chipik     (501) staff       (20)    19705 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/PKG-INFO
--rw-r--r--   0 chipik     (501) staff       (20)      331 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/SOURCES.txt
--rw-r--r--   0 chipik     (501) staff       (20)        1 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/dependency_links.txt
--rw-r--r--   0 chipik     (501) staff       (20)       52 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/entry_points.txt
--rw-r--r--   0 chipik     (501) staff       (20)       60 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/requires.txt
--rw-r--r--   0 chipik     (501) staff       (20)       13 2022-03-16 13:12:44.000000 hive_library-0.0.1b8/hive_library.egg-info/top_level.txt
--rw-r--r--   0 chipik     (501) staff       (20)       38 2022-03-16 13:12:44.880229 hive_library-0.0.1b8/setup.cfg
--rw-r--r--   0 chipik     (501) staff       (20)     1817 2022-03-05 11:26:26.000000 hive_library-0.0.1b8/setup.py
+drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-07-27 13:50:33.497569 hive_library-0.0.1b9/
+-rw-r--r--   0 chipik     (501) staff       (20)     1063 2021-09-01 15:45:03.000000 hive_library-0.0.1b9/LICENSE
+-rw-r--r--   0 chipik     (501) staff       (20)    19705 2022-07-27 13:50:33.496977 hive_library-0.0.1b9/PKG-INFO
+-rw-r--r--   0 chipik     (501) staff       (20)    18700 2021-09-01 15:45:03.000000 hive_library-0.0.1b9/README.md
+drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-07-27 13:50:33.493616 hive_library-0.0.1b9/hive_library/
+-rw-r--r--   0 chipik     (501) staff       (20)    55509 2022-07-27 13:46:32.000000 hive_library-0.0.1b9/hive_library/__init__.py
+-rw-r--r--   0 chipik     (501) staff       (20)    19754 2022-07-27 13:46:34.000000 hive_library-0.0.1b9/hive_library/cli.py
+-rw-r--r--   0 chipik     (501) staff       (20)     1636 2022-07-27 13:46:35.000000 hive_library-0.0.1b9/hive_library/enum.py
+-rw-r--r--   0 chipik     (501) staff       (20)   108810 2022-07-27 13:46:31.000000 hive_library-0.0.1b9/hive_library/rest.py
+drwxr-xr-x   0 chipik     (501) staff       (20)        0 2022-07-27 13:50:33.496290 hive_library-0.0.1b9/hive_library.egg-info/
+-rw-r--r--   0 chipik     (501) staff       (20)    19705 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/PKG-INFO
+-rw-r--r--   0 chipik     (501) staff       (20)      331 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/SOURCES.txt
+-rw-r--r--   0 chipik     (501) staff       (20)        1 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/dependency_links.txt
+-rw-r--r--   0 chipik     (501) staff       (20)       52 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/entry_points.txt
+-rw-r--r--   0 chipik     (501) staff       (20)       60 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/requires.txt
+-rw-r--r--   0 chipik     (501) staff       (20)       13 2022-07-27 13:50:32.000000 hive_library-0.0.1b9/hive_library.egg-info/top_level.txt
+-rw-r--r--   0 chipik     (501) staff       (20)       38 2022-07-27 13:50:33.497725 hive_library-0.0.1b9/setup.cfg
+-rw-r--r--   0 chipik     (501) staff       (20)     1817 2022-07-27 13:46:32.000000 hive_library-0.0.1b9/setup.py
```

### Comparing `hive_library-0.0.1b8/LICENSE` & `hive_library-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `hive_library-0.0.1b8/PKG-INFO` & `hive_library-0.0.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive_library
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Python Hive Library
 Home-page: https://hexway.io/
 Author: HexWay
 Author-email: contact@hexway.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hive_library-0.0.1b8/README.md` & `hive_library-0.0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `hive_library-0.0.1b8/hive_library/__init__.py` & `hive_library-0.0.1b9/hive_library/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 Hive dataclasses
 Author: HexWay
 License: MIT
 Copyright 2021, HexWay
 """
 
 # Import
-from hive_library.enum import RecordTypes, PermissionTypes, TaskStates, RowTypes
+from hive_library.enum import (
+    RecordTypes,
+    PermissionTypes,
+    TaskStates,
+    RowTypes,
+    CriticalityScores,
+    ProbabilityScores,
+    IssueStatuses,
+)
 from typing import List, Dict, Optional, Union
 from uuid import UUID
 from dataclasses import dataclass, field
 from marshmallow import (
     fields,
     pre_load,
     post_load,
@@ -32,15 +40,15 @@
 
 
 # Authorship information
 __author__ = "HexWay"
 __copyright__ = "Copyright 2021, HexWay"
 __credits__ = [""]
 __license__ = "MIT"
-__version__ = "0.0.1b8"
+__version__ = "0.0.1b9"
 __maintainer__ = "HexWay"
 __email__ = "contact@hexway.io"
 __status__ = "Development"
 
 
 class HiveLibrary:
     @dataclass
@@ -1240,14 +1248,225 @@
                     del clean_data[key]
                 return clean_data
 
             @post_load
             def make_snapshot(self, data, **kwargs):
                 return HiveLibrary.Snapshot(**data)
 
+    @dataclass
+    class Issue:
+        uuid: Optional[UUID] = None
+        status: Optional[str] = None
+        name: Optional[str] = None
+        ips: Optional[List[str]] = field(default_factory=lambda: [])
+        hostnames: Optional[List[str]] = field(default_factory=lambda: [])
+        criticality_score: Optional[int] = None
+        probability_score: Optional[int] = None
+        weakness_type: Optional[str] = None
+        additional_fields: Optional["HiveLibrary.Issue.AdditionalFields"] = None
+        files: Optional[List["HiveLibrary.File"]] = field(default_factory=lambda: [])
+        requests: Optional[List["HiveLibrary.Issue.Request"]] = field(
+            default_factory=lambda: []
+        )
+        checkmark_count: Optional[int] = None
+        creator_uuid: Optional[UUID] = None
+        edit_time: Optional[datetime] = None
+        post_time: Optional[datetime] = None
+        id: Optional[int] = None
+
+        @dataclass
+        class AdditionalFields:
+            general_description: Optional[str] = None
+            risks_description: Optional[str] = None
+            technical_description: Optional[str] = None
+            reproduce_description: Optional[str] = None
+            recommendations: Optional[str] = None
+
+            class Schema(MarshmallowSchema):
+                general_description = fields.String(
+                    missing=None, default=None, data_key="generalDescription"
+                )
+                risks_description = fields.String(
+                    missing=None, default=None, data_key="risksDescription"
+                )
+                technical_description = fields.String(
+                    missing=None, default=None, data_key="technicalDescription"
+                )
+                reproduce_description = fields.String(
+                    missing=None, default=None, data_key="reproduceDescription"
+                )
+                recommendations = fields.String(missing=None, default=None)
+
+                class Meta:
+                    unknown = EXCLUDE
+
+                @post_load
+                def make_issue_additional_fields(self, data, **kwargs):
+                    return HiveLibrary.Issue.AdditionalFields(**data)
+
+        @dataclass
+        class Request:
+            request: Optional[str] = None
+            response: Optional[str] = None
+            id: Optional[int] = None
+            node_id: Optional[int] = None
+            parent_id: Optional[int] = None
+            base_node_id: Optional[int] = None
+            uuid: Optional[UUID] = None
+            creator_uuid: Optional[UUID] = None
+            create_time: Optional[datetime] = None
+
+            class Schema(MarshmallowSchema):
+                request = fields.String(missing=None, default=None)
+                response = fields.String(missing=None, default=None)
+                id = fields.Integer(
+                    missing=None,
+                    default=None,
+                    load_only=True,
+                )
+                node_id = fields.Integer(
+                    missing=None,
+                    default=None,
+                    data_key="nodeId",
+                )
+                parent_id = fields.Integer(
+                    missing=None,
+                    default=None,
+                    load_only=True,
+                    data_key="parentId",
+                )
+                base_node_id = fields.Integer(
+                    missing=None,
+                    default=None,
+                    load_only=True,
+                    data_key="baseNodeId",
+                )
+                uuid = fields.UUID(missing=None, default=None, load_only=True)
+                creator_uuid = fields.UUID(
+                    missing=None,
+                    default=None,
+                    data_key="creatorUuid",
+                    load_only=True,
+                )
+                create_time = fields.DateTime(
+                    "%Y-%m-%dT%H:%M:%S.%fZ",
+                    missing=None,
+                    default=None,
+                    data_key="createTime",
+                    load_only=True,
+                )
+
+                class Meta:
+                    unknown = EXCLUDE
+
+                @post_load
+                def make_issue_request(self, data, **kwargs):
+                    return HiveLibrary.Issue.Request(**data)
+
+        class Schema(MarshmallowSchema):
+            uuid = fields.UUID(missing=None, default=None, load_only=True)
+            status = fields.String(
+                missing=None,
+                default=None,
+                validate=validate.OneOf(IssueStatuses.list(), None),
+            )
+            name = fields.String(required=True)
+            ips = fields.List(
+                fields.String,
+                many=True,
+                missing=[],
+                default=[],
+                allow_none=False,
+                data_key="ips",
+            )
+            hostnames = fields.List(
+                fields.String,
+                many=True,
+                missing=[],
+                default=[],
+                allow_none=False,
+                data_key="hostnames",
+            )
+            criticality_score = fields.Integer(
+                missing=None,
+                default=None,
+                data_key="criticalityScore",
+                validate=validate.OneOf(CriticalityScores.list(), None),
+            )
+            probability_score = fields.Integer(
+                missing=None,
+                default=None,
+                data_key="probabilityScore",
+                validate=validate.OneOf(ProbabilityScores.list(), None),
+            )
+            weakness_type = fields.String(
+                missing=None, default=None, data_key="weaknessType"
+            )
+            additional_fields = fields.Nested(
+                lambda: HiveLibrary.Issue.AdditionalFields.Schema,
+                data_key="additionalFields",
+                missing={},
+                default={},
+                allow_none=True,
+            )
+            files = fields.Nested(
+                lambda: HiveLibrary.File.Schema,
+                many=True,
+                missing=[],
+                default=[],
+                allow_none=True,
+                load_only=True,
+            )
+            requests = fields.Nested(
+                lambda: HiveLibrary.Issue.Request.Schema,
+                many=True,
+                missing=[],
+                default=[],
+                allow_none=True,
+                load_only=True,
+            )
+            checkmark_count = fields.Integer(
+                missing=None,
+                default=None,
+                data_key="checkmarkCount",
+                load_only=True,
+            )
+            creator_uuid = fields.UUID(
+                missing=None,
+                default=None,
+                data_key="creatorUuid",
+                load_only=True,
+            )
+            edit_time = fields.DateTime(
+                "%Y-%m-%dT%H:%M:%S.%fZ",
+                missing=None,
+                default=None,
+                data_key="editTime",
+                load_only=True,
+            )
+            post_time = fields.DateTime(
+                "%Y-%m-%dT%H:%M:%S.%fZ",
+                missing=None,
+                default=None,
+                data_key="postTime",
+                load_only=True,
+            )
+            id = fields.Integer(
+                missing=None,
+                default=None,
+                load_only=True,
+            )
+
+            class Meta:
+                unknown = EXCLUDE
+
+            @post_load
+            def make_issue(self, data, **kwargs):
+                return HiveLibrary.Issue(**data)
+
     @staticmethod
     def load_config() -> Config:
         config: HiveLibrary.Config = HiveLibrary.Config()
         if path.isfile(config.file) and path.getsize(config.file) > 0:
             with open(config.file, "r") as config_file:
                 config_dict: Dict[str, str] = safe_load(config_file)
                 config = HiveLibrary.Config.Schema().load(config_dict)
```

### Comparing `hive_library-0.0.1b8/hive_library/cli.py` & `hive_library-0.0.1b9/hive_library/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from prettytable import PrettyTable
 
 # Authorship information
 __author__ = "HexWay"
 __copyright__ = "Copyright 2021, HexWay"
 __credits__ = [""]
 __license__ = "MIT"
-__version__ = "0.0.1b8"
+__version__ = "0.0.1b9"
 __maintainer__ = "HexWay"
 __email__ = "contact@hexway.io"
 __status__ = "Development"
 
 
 # Pretty print hosts
 def pretty_print_hosts(hosts: List[HiveLibrary.Host]) -> None:
```

### Comparing `hive_library-0.0.1b8/hive_library/enum.py` & `hive_library-0.0.1b9/hive_library/enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # Authorship information
 __author__ = "HexWay"
 __copyright__ = "Copyright 2021, HexWay"
 __credits__ = [""]
 __license__ = "MIT"
-__version__ = "0.0.1b8"
+__version__ = "0.0.1b9"
 __maintainer__ = "HexWay"
 __email__ = "contact@hexway.io"
 __status__ = "Development"
 
 
 class ListEnum(Enum):
     @classmethod
@@ -62,7 +62,28 @@
     PORT = "port"
     PRODUCT = "product"
     SERVICE = "service"
     STATE = "state"
     TAG = "tag"
     VERSION = "version"
     DUMMY = "dummy"
+
+
+class CriticalityScores(int, ListEnum):
+    LOW = 1
+    MEDIUM = 2
+    HIGH = 3
+
+
+class ProbabilityScores(int, ListEnum):
+    LOW = 1
+    MEDIUM = 2
+    HIGH = 3
+
+
+class IssueStatuses(str, ListEnum):
+    DRAFT = "draft"
+    VERIFIED = "verified"
+    READY = "ready"
+    FIX_CONFIRMED = "fix_confirmed"
+    FIX_UNCONFIRMED = "fix_unconfirmed"
+    RETEST_REQUIRED = "retest_required"
```

### Comparing `hive_library-0.0.1b8/hive_library/rest.py` & `hive_library-0.0.1b9/hive_library/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from os import path
 
 # Authorship information
 __author__ = "HexWay"
 __copyright__ = "Copyright 2021, HexWay"
 __credits__ = [""]
 __license__ = "MIT"
-__version__ = "0.0.1b8"
+__version__ = "0.0.1b9"
 __maintainer__ = "HexWay"
 __email__ = "contact@hexway.io"
 __status__ = "Development"
 
 
 # Class AuthenticationError
 class AuthenticationError(Exception):
@@ -105,15 +105,15 @@
 
         # Set internal class variables
         self._server = server
         self._debug = debug
         self._session: Session = Session()
         self._session.headers.update(
             {
-                "User-Agent": "Hive Client/" + "0.0.1b8",
+                "User-Agent": "Hive Client/" + "0.0.1b9",
                 "Accept": "application/json",
                 "Connection": "close",
             }
         )
 
         # Set proxy
         if proxy is None:
@@ -493,14 +493,119 @@
             print(f"Assertion error: {error.args[0]}")
             return None
 
         except JSONDecodeError as error:
             print(f"JSON Decode error: {error.args[0]}")
             return None
 
+    def get_issues(self, project_id: UUID) -> Optional[List[HiveLibrary.Issue]]:
+        """
+        Get Issues
+        @param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        @return: None if error or List of issues, example:
+        [HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                           ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                           criticality_score=1, probability_score=1,
+                           weakness_type='cwe-123',
+                           additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                           files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                           checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                           edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                           post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                           id=1231350)]
+        """
+        try:
+            response = self._session.get(
+                self._server + self._endpoints.project + f"/{project_id}/graph/issues"
+            )
+            error_string: str = ""
+            if self._debug:
+                error_string = self._make_error_string(response)
+            assert (
+                response.status_code == 200
+            ), f"Bad status code in get issues {error_string}"
+            assert isinstance(
+                response.json(), List
+            ), f"Bad response in get issues {error_string}"
+            issues_schema: HiveLibrary.Issue.Schema = HiveLibrary.Issue.Schema(
+                many=True
+            )
+            issues: List[HiveLibrary.Issue] = issues_schema.load(response.json())
+            return issues
+
+        except AssertionError as error:
+            print(f"Assertion error: {error.args[0]}")
+            return None
+
+        except JSONDecodeError as error:
+            print(f"JSON Decode error: {error.args[0]}")
+            return None
+
+    def get_issue(
+        self, project_id: UUID, issue_uuid: UUID
+    ) -> Optional[HiveLibrary.Issue]:
+        """
+        Get Issue by UUID
+        @param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        @param issue_uuid: Issue UUID string, example: '66717b2e-9046-4a17-9928-590393a823d4'
+        @return: None if error or Issue, example:
+        HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                          ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                          criticality_score=1, probability_score=1,
+                          weakness_type='cwe-123',
+                          additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                          files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                          checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                          edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                          post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                          id=1231350)
+        """
+        try:
+            response = self._session.get(
+                self._server
+                + self._endpoints.project
+                + f"/{project_id}/graph/issues/{issue_uuid}"
+            )
+            error_string: str = ""
+            if self._debug:
+                error_string = self._make_error_string(response)
+            assert (
+                response.status_code == 200
+            ), f"Bad status code in get issue by UUID {error_string}"
+            assert isinstance(
+                response.json(), Dict
+            ), f"Bad response in get issue by UUID {error_string}"
+            issue_schema: HiveLibrary.Issue.Schema = HiveLibrary.Issue.Schema(
+                many=False
+            )
+            issue: HiveLibrary.Issue = issue_schema.load(response.json())
+            return issue
+
+        except AssertionError as error:
+            print(f"Assertion error: {error.args[0]}")
+            return None
+
+        except JSONDecodeError as error:
+            print(f"JSON Decode error: {error.args[0]}")
+            return None
+
     def get_credentials(
         self, project_id: UUID
     ) -> Optional[List[HiveLibrary.Credential]]:
         """
         Get credentials
         @param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
         @return: None if error or List of credentials, example:
@@ -1375,14 +1480,198 @@
         except AssertionError as error:
             print(f"Assertion error: {error.args[0]}")
             return None
         except JSONDecodeError as error:
             print(f"JSON Decode error: {error.args[0]}")
             return None
 
+    def create_issues(
+        self, project_id: UUID, issues: List[HiveLibrary.Issue]
+    ) -> Optional[List[HiveLibrary.Issue]]:
+        """
+        Create Issues
+        :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        :param issues: List of issues
+        :return: None if error or List of issues, example:
+        [HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                           ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                           criticality_score=1, probability_score=1,
+                           weakness_type='cwe-123',
+                           additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                           files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                           checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                           edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                           post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                           id=1231350)]
+
+        """
+        try:
+            response: Response = self._session.post(
+                self._server + self._endpoints.project + f"/{project_id}/graph/issues",
+                json=HiveLibrary.Issue.Schema(many=True).dump(issues),
+            )
+            error_string: str = ""
+            if self._debug:
+                error_string = self._make_error_string(response)
+            assert (
+                response.status_code == 200
+            ), f"Bad status code in create issues {error_string}"
+            assert isinstance(
+                response.json(), List
+            ), f"Bad response in create issues {error_string}"
+            assert (
+                len(response.json()) >= 1
+            ), f"Bad response in create issues {error_string}"
+            issues_schema: HiveLibrary.Issue.Schema = HiveLibrary.Issue.Schema(
+                many=True
+            )
+            created_issues: List[HiveLibrary.Issue] = issues_schema.load(
+                response.json()
+            )
+
+            # Add requests to created issues
+            for issue in issues:
+                for created_issue in created_issues:
+                    if len(issue.requests) > 0:
+                        if issue.name == created_issue.name:
+                            for request in issue.requests:
+                                request.node_id = created_issue.id
+                            response: Response = self._session.post(
+                                self._server
+                                + self._endpoints.project
+                                + f"/{project_id}/graph/nodes",
+                                json=HiveLibrary.Issue.Request.Schema(many=True).dump(
+                                    issue.requests
+                                ),
+                            )
+                            assert (
+                                response.status_code == 200
+                            ), f"Bad status code to add request to issues {error_string}"
+                            assert isinstance(
+                                response.json(), List
+                            ), f"Bad response to add request to issues {error_string}"
+                            assert (
+                                len(response.json()) >= 1
+                            ), f"Bad response to add request to issues {error_string}"
+                            requests_schema: HiveLibrary.Issue.Schema = (
+                                HiveLibrary.Issue.Request.Schema(many=True)
+                            )
+                            created_requests: List[
+                                HiveLibrary.Issue.Request
+                            ] = requests_schema.load(response.json())
+                            created_issue.requests = created_requests
+
+            return created_issues
+        except AssertionError as error:
+            print(f"Assertion error: {error.args[0]}")
+            return None
+        except JSONDecodeError as error:
+            print(f"JSON Decode error: {error.args[0]}")
+            return None
+
+    def create_issue(
+        self, project_id: UUID, issue: HiveLibrary.Issue
+    ) -> Optional[HiveLibrary.Issue]:
+        """
+        Create Issue
+        :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        :param issue: Issue
+        :return: None if error or Issue, example:
+        HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                          ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                          criticality_score=1, probability_score=1,
+                          weakness_type='cwe-123',
+                          additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                          files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                          checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                          edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                          post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                          id=1231350)
+
+        """
+        created_issues = self.create_issues(project_id=project_id, issues=[issue])
+        if isinstance(created_issues, List):
+            return created_issues[0]
+        else:
+            return None
+
+    def change_issue(
+        self, project_id: UUID, issue: HiveLibrary.Issue
+    ) -> Optional[HiveLibrary.Issue]:
+        """
+        Change Issue
+        :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        :param issue: Issue
+        :return: None if error or Issue, example:
+        HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                          ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                          criticality_score=1, probability_score=1,
+                          weakness_type='cwe-123',
+                          additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                          files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                          checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                          edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                          post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                          id=1231350)
+
+        """
+        try:
+            assert isinstance(
+                issue.uuid, UUID
+            ), f"Issue UUID is empty, please set issue uuid!"
+            issue_json = HiveLibrary.Issue.Schema(many=False).dump(issue)
+            issue_json["uuid"] = str(issue.uuid)
+            response: Response = self._session.patch(
+                self._server
+                + self._endpoints.project
+                + f"/{project_id}/graph/issues/{issue.uuid}",
+                json=issue_json,
+            )
+            error_string: str = ""
+            if self._debug:
+                error_string = self._make_error_string(response)
+            assert (
+                response.status_code == 200
+            ), f"Bad status code in change issue {error_string}"
+            assert isinstance(
+                response.json(), Dict
+            ), f"Bad response in change issue {error_string}"
+            issue_schema: HiveLibrary.Issue.Schema = HiveLibrary.Issue.Schema(
+                many=False
+            )
+            changed_issue: HiveLibrary.Issue = issue_schema.load(response.json())
+            return changed_issue
+        except AssertionError as error:
+            print(f"Assertion error: {error.args[0]}")
+            return None
+        except JSONDecodeError as error:
+            print(f"JSON Decode error: {error.args[0]}")
+            return None
+
     def upload_file(
         self,
         file_name: str,
         file_content: bytes,
         project_id: UUID,
         node_id: int,
         file_caption: Optional[str] = None,
@@ -1587,20 +1876,20 @@
             print(f"Assertion error: {error.args[0]}")
             return None
         except JSONDecodeError as error:
             print(f"JSON Decode error: {error.args[0]}")
             return None
 
     def custom_import_string(
-            self,
-            project_id: UUID,
-            data: str,
-            columns: List[str],
-            column_separator: str = ",",
-            row_separator: str = "\n"
+        self,
+        project_id: UUID,
+        data: str,
+        columns: List[str],
+        column_separator: str = ",",
+        row_separator: str = "\n",
     ) -> Optional[HiveLibrary.Task]:
         """
         Custom import data from string
         :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
         :param data: Data string, example: 'test1.com,1.1.1.1'
         :param columns: Columns for import, example: ['hostname', 'ip']
         :param column_separator: Column separator, example: ','
@@ -1617,23 +1906,19 @@
             rows: Optional[List[HiveLibrary.Row]] = self.parse_custom_import(
                 project_id=project_id,
                 data=data,
                 columns=columns,
                 column_separator=column_separator,
                 row_separator=row_separator,
             )
-            assert (
-                rows is not None
-            ), f"Failed to parse custom data: {data}"
+            assert rows is not None, f"Failed to parse custom data: {data}"
             task: Optional[HiveLibrary.Task] = self.upload_custom_import(
                 project_id=project_id, rows=rows
             )
-            assert (
-                task is not None
-            ), f"Failed to upload custom data: {data}"
+            assert task is not None, f"Failed to upload custom data: {data}"
             return task
         except AssertionError as error:
             print(f"Assertion error: {error.args[0]}")
             return None
         except JSONDecodeError as error:
             print(f"JSON Decode error: {error.args[0]}")
             return None
@@ -1678,14 +1963,69 @@
             print(f"Assertion error: {error.args[0]}")
             return None
         except JSONDecodeError as error:
             print(f"JSON Decode error: {error.args[0]}")
             return None
 
     # Delete methods
+    def delete_issue_by_id(
+        self, project_id: UUID, issue_id: int
+    ) -> Optional[HiveLibrary.Issue]:
+        """
+        Delete issue by identifier
+        :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
+        :param issue_id: Issue id integer, example: 123
+        :return: None if error or Project object, example:
+        HiveLibrary.Issue(uuid=UUID('2557c338-8b2b-483c-8884-16055b371566'), name='test',
+                          ips=['1.1.1.1', '2.2.2.2'], hostnames=['test.com'],
+                          criticality_score=1, probability_score=1,
+                          weakness_type='cwe-123',
+                          additional_fields=HiveLibrary.Issue.AdditionalFields(general_description='desc',
+                                                                                risks_description='risk',
+                                                                                technical_description='tech',
+                                                                                reproduce_description='steps',
+                                                                                recommendations='recommendations'),
+                          files=[], requests=[HiveLibrary.Issue.Request(request='123',
+                                                                         response='345',
+                                                                         id=1231392,
+                                                                         parent_id=1231350)],
+                          checkmark_count=0, creator_uuid=UUID('bc33859d-9ef9-44f6-a75e-2db032108c08'),
+                          edit_time=datetime.datetime(2022, 7, 15, 10, 36, 49, 252167),
+                          post_time=datetime.datetime(2022, 7, 13, 10, 50, 23, 822338),
+                          id=1231350)
+        """
+        try:
+            response = self._session.delete(
+                self._server
+                + self._endpoints.project
+                + f"/{project_id}/graph/nodes/{issue_id}"
+            )
+            error_string: str = ""
+            if self._debug:
+                error_string = self._make_error_string(response)
+            assert (
+                response.status_code == 200
+            ), f"Bad status code in get issue by UUID {error_string}"
+            assert isinstance(
+                response.json(), Dict
+            ), f"Bad response in get issue by UUID {error_string}"
+            issue_schema: HiveLibrary.Issue.Schema = HiveLibrary.Issue.Schema(
+                many=False
+            )
+            issue: HiveLibrary.Issue = issue_schema.load(response.json())
+            return issue
+
+        except AssertionError as error:
+            print(f"Assertion error: {error.args[0]}")
+            return None
+
+        except JSONDecodeError as error:
+            print(f"JSON Decode error: {error.args[0]}")
+            return None
+
     def delete_project_by_id(self, project_id: UUID) -> Optional[HiveLibrary.Project]:
         """
         Delete project by identifier
         :param project_id: Project identifier string, example: 'be282469-5615-493b-842b-733e6f0b015a'
         :return: None if error or Project object, example:
         HiveLibrary.Project(projectArchiveDate=None, projectConnectionId=None, projectCreateDate='2021-05-20T16:30:03.120592Z',
                      projectDescription='Unit test project', projectEndDate='2021-01-21T00:00:00.000000Z',
```

### Comparing `hive_library-0.0.1b8/hive_library.egg-info/PKG-INFO` & `hive_library-0.0.1b9/hive_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-library
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Python Hive Library
 Home-page: https://hexway.io/
 Author: HexWay
 Author-email: contact@hexway.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hive_library-0.0.1b8/setup.py` & `hive_library-0.0.1b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 # Authorship information
 __author__ = "HexWay"
 __copyright__ = "Copyright 2021, HexWay"
 __credits__ = [""]
 __license__ = "MIT"
-__version__ = "0.0.1b8"
+__version__ = "0.0.1b9"
 __maintainer__ = "HexWay"
 __email__ = "contact@hexway.io"
 __status__ = "Development"
 
 # Setup
 with open("README.md", "r") as readme:
     long_description = readme.read()
```

