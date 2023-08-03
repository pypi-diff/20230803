# Comparing `tmp/oda_wd_client-0.0.3a0.tar.gz` & `tmp/oda_wd_client-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_wd_client-0.0.3a0.tar", max compression
+gzip compressed data, was "oda_wd_client-0.0.3a1.tar", max compression
```

## Comparing `oda_wd_client-0.0.3a0.tar` & `oda_wd_client-0.0.3a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/__init__.py
--rw-r--r--   0        0        0      368 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/api.py
--rw-r--r--   0        0        0        0 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/base/__init__.py
--rw-r--r--   0        0        0     6120 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/api.py
--rw-r--r--   0        0        0      623 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/logging.py
--rw-r--r--   0        0        0      741 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/tools.py
--rw-r--r--   0        0        0     1381 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/types.py
--rw-r--r--   0        0        0      830 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/utils.py
--rw-r--r--   0        0        0       19 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/__init__.py
--rw-r--r--   0        0        0     3796 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/api.py
--rw-r--r--   0        0        0     3708 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/types.py
--rw-r--r--   0        0        0     7865 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/__init__.py
--rw-r--r--   0        0        0     3062 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/api.py
--rw-r--r--   0        0        0      321 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/types.py
--rw-r--r--   0        0        0     2703 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/__init__.py
--rw-r--r--   0        0        0     1665 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/api.py
--rw-r--r--   0        0        0     3652 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/types.py
--rw-r--r--   0        0        0     6985 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/__init__.py
--rw-r--r--   0        0        0     1407 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/api.py
--rw-r--r--   0        0        0     3422 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/types.py
--rw-r--r--   0        0        0      983 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/utils.py
--rw-r--r--   0        0        0      350 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/__init__.py
--rw-r--r--   0        0        0      528 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/financial_management.py
--rw-r--r--   0        0        0       85 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/human_resources.py
--rw-r--r--   0        0        0      511 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/resource_management.py
--rw-r--r--   0        0        0       82 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/staffing.py
--rw-r--r--   0        0        0      838 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 oda_wd_client-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/__init__.py
+-rw-r--r--   0        0        0      368 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/api.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/__init__.py
+-rw-r--r--   0        0        0     7239 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/api.py
+-rw-r--r--   0        0        0      623 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/logging.py
+-rw-r--r--   0        0        0      741 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/tools.py
+-rw-r--r--   0        0        0     3774 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/types.py
+-rw-r--r--   0        0        0      830 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/base/utils.py
+-rw-r--r--   0        0        0       19 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/__init__.py
+-rw-r--r--   0        0        0     3796 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/api.py
+-rw-r--r--   0        0        0     6052 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/types.py
+-rw-r--r--   0        0        0     7865 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/__init__.py
+-rw-r--r--   0        0        0     3062 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/api.py
+-rw-r--r--   0        0        0      494 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/types.py
+-rw-r--r--   0        0        0     2703 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/resource_management/__init__.py
+-rw-r--r--   0        0        0     2257 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/resource_management/api.py
+-rw-r--r--   0        0        0     6174 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/resource_management/types.py
+-rw-r--r--   0        0        0    10809 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/resource_management/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/__init__.py
+-rw-r--r--   0        0        0     1407 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/api.py
+-rw-r--r--   0        0        0     3604 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/types.py
+-rw-r--r--   0        0        0      983 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/utils.py
+-rw-r--r--   0        0        0      350 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/types/__init__.py
+-rw-r--r--   0        0        0      528 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/types/financial_management.py
+-rw-r--r--   0        0        0       85 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/types/human_resources.py
+-rw-r--r--   0        0        0      511 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/types/resource_management.py
+-rw-r--r--   0        0        0       82 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/oda_wd_client/types/staffing.py
+-rw-r--r--   0        0        0      999 2023-08-03 12:17:38.641884 oda_wd_client-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 oda_wd_client-0.0.3a1/PKG-INFO
```

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/base/api.py` & `oda_wd_client-0.0.3a1/oda_wd_client/base/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+from datetime import datetime
 from typing import Any, Iterator
 from urllib.parse import urljoin
 
 from suds import client as suds_client
 from suds import sudsobject, wsse
 from suds.plugin import MessagePlugin
 
@@ -20,14 +22,43 @@
             if obj.children:
                 for child in obj.children:
                     recurse(child)
 
         recurse(root)
 
 
+class SudsLog(MessagePlugin):
+    """
+    Write all responses and requests to files during development
+
+    Inspired by https://www.guguweb.com/2019/12/11/how-to-log-raw-xml-requests-and-responses-in-suds/
+    """
+
+    def __init__(self, location):
+        self.location = location
+        if not os.path.exists(location):
+            os.makedirs(location)
+
+    def pretty_log(self, xml_content, direction):
+        try:
+            file_path = os.path.join(
+                self.location, f"suds-log-{datetime.now()}-{direction}.xml"
+            )
+            with open(file_path, "wb") as f:
+                f.write(xml_content)
+        except Exception as e:
+            log("warning", f"Cannot log XML ({e})")
+
+    def sending(self, context):
+        self.pretty_log(context.envelope, "send")
+
+    def received(self, context):
+        self.pretty_log(context.reply, "receive")
+
+
 # Using a singleton to hold all of our client instances to avoid re-initiation during app lifecycle. Changing the
 # credentials requires us to reload the app anyway.
 _workday_clients: dict[str, suds_client.Client] = {}
 
 
 class WorkdayClient:
     """
@@ -50,19 +81,21 @@
     def __init__(
         self,
         base_url: str,
         tenant_name: str,
         username: str,
         password: str,
         lazy_init: bool = True,
+        log_location: str | None = None,
     ) -> None:
         self._auth_base_url = base_url
         self._auth_tenant_name = tenant_name
         self._auth_username = username
         self._auth_password = password
+        self._log_location = log_location
         # If we do lazy init, we only initialize each service when they're first needed, since there's an overhead
         # with the init process
         if not lazy_init:
             for service in self._services:
                 self._init_service_client(service)
         assert (
             self.service
@@ -79,15 +112,18 @@
             f"/ccx/service/{self._auth_tenant_name}/{service}/v38.1?wsdl",
         )
 
     def _setup_client(self, url: str) -> suds_client.Client:
         """
         Create client instance with secrets and config
         """
-        client = suds_client.Client(url, plugins=[SudsHax()])
+        plugins = [SudsHax()]
+        if self._log_location:
+            plugins.append(SudsLog(self._log_location))
+        client = suds_client.Client(url, plugins=plugins)
         security = wsse.Security()
         token = wsse.UsernameToken(
             f"{self._auth_username}@{self._auth_tenant_name}",
             self._auth_password,
         )
         token.setnonce()
         token.setcreated()
```

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/base/logging.py` & `oda_wd_client-0.0.3a1/oda_wd_client/base/logging.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/base/tools.py` & `oda_wd_client-0.0.3a1/oda_wd_client/base/tools.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/base/utils.py` & `oda_wd_client-0.0.3a1/oda_wd_client/base/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/api.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/utils.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/financial_management/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/api.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/utils.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/human_resources/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/api.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/resource_management/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from suds import sudsobject
 
 from oda_wd_client.base.api import WorkdayClient
 from oda_wd_client.base.tools import suds_to_dict
 from oda_wd_client.service.resource_management.types import Supplier, SupplierInvoice
 from oda_wd_client.service.resource_management.utils import (
     pydantic_supplier_invoice_to_workday,
+    workday_supplier_invoice_to_pydantic,
     workday_supplier_to_pydantic,
 )
 
 
 class ResourceManagement(WorkdayClient):
     service = "Resource_Management"
 
@@ -25,21 +26,36 @@
             )
 
     def get_supplier_invoices(
         self, return_suds_object=False
     ) -> Iterator[sudsobject.Object | SupplierInvoice]:
         method = "Get_Supplier_Invoices"
         results = self._get_paginated(method, "Supplier_Invoice")
-        for supplier in results:
-            yield supplier if return_suds_object else workday_supplier_to_pydantic(
-                suds_to_dict(supplier)
+        for invoice in results:
+            yield invoice if return_suds_object else workday_supplier_invoice_to_pydantic(
+                suds_to_dict(invoice)
             )
 
     def submit_supplier_invoice(self, invoice: SupplierInvoice) -> sudsobject.Object:
         method = "Submit_Supplier_Invoice"
         request = self.factory("ns0:Submit_Supplier_Invoice_Request")
         request.Supplier_Invoice_Data = pydantic_supplier_invoice_to_workday(
             invoice, self
         )
         return self._request(
             method, Supplier_Invoice_Data=request.Supplier_Invoice_Data
         )
+
+    def cancel_supplier_invoice(self, invoice_ref_id: str):
+        """
+        Cancel an invoice in Workday
+
+        :param invoice_ref_id:
+        :return:
+        """
+        method = "Cancel_Supplier_Invoice"
+        ref_obj = self.factory("ns0:Supplier_InvoiceObjectType")
+        id_obj = self.factory("ns0:Supplier_InvoiceObjectIDType")
+        id_obj._type = "Supplier_Invoice_Reference_ID"
+        id_obj.value = invoice_ref_id
+        ref_obj.ID.append(id_obj)
+        return self._request(method, Supplier_Invoice_Reference=ref_obj)
```

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/api.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/types.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from pydantic import BaseModel
 
 # All public imports should be done through oda_wd_client.types.staffing
 __all__: list = []
 
 
 class Document(BaseModel):
+    """
+    Reference: https://community.workday.com/sites/default/files/file-hosting/productionapi/Staffing/v40.2/Put_Worker_Document.html#Worker_Document_DataType  # noqa
+    """
+
     class WorkdayCategory(str, Enum):
         employee_contract = "EMPLOYEE_CONTRACT"
         student_collections = "STUDENT_COLLECTIONS"
         prospect_resume_cover_letter = "PROSPECT_RESUME_AND_COVER_LETTER"
         candidate_resume_cover_letter = "CANDIDATE_RESUME_AND_COVER_LETTER"
         residency_determination = "RESIDENCY_DETERMINATION"
         education = "EDUCATION"
```

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/utils.py` & `oda_wd_client-0.0.3a1/oda_wd_client/service/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/oda_wd_client/types/financial_management.py` & `oda_wd_client-0.0.3a1/oda_wd_client/types/financial_management.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.3a0/pyproject.toml` & `oda_wd_client-0.0.3a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "oda-wd-client"
-version = "0.0.3a0"
+version = "0.0.3a1"
 description = "A library for interacting with Workday from Python"
 authors = [
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pydantic = ">=1.10.0,<2.0"
 suds-py3 = "^1.4.5.0"
 pre-commit = "^3.3.3"
 yamllint = "^1.32.0"
+python-magic = "^0.4.27"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.30.1"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 flake8 = "^6.0.0"
 black = "^23.7.0"
@@ -38,7 +39,15 @@
 include_trailing_comma = true
 use_parentheses = true
 group_by_package = true
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
 [tool.mypy]
 ignore_missing_imports = true
+plugins = [
+    "pydantic.mypy"
+]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
```

