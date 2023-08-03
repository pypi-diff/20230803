# Comparing `tmp/stigg_api_client_v2-0.517.0.tar.gz` & `tmp/stigg_api_client_v2-0.522.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.517.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.522.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.517.0.tar` & `stigg_api_client_v2-0.522.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1644 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/README.md
--rw-r--r--   0        0        0      452 2023-08-01 07:11:23.019905 stigg_api_client_v2-0.517.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/__init__.py
--rw-r--r--   0        0        0     4711 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/client.py
--rw-r--r--   0        0        0      932 2023-08-01 07:10:17.899443 stigg_api_client_v2-0.517.0/stigg/edge_utils.py
--rw-r--r--   0        0        0    41050 2023-08-01 07:11:20.699898 stigg_api_client_v2-0.517.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-08-01 07:11:18.759895 stigg_api_client_v2-0.517.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-08-01 07:11:20.339897 stigg_api_client_v2-0.517.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-08-01 07:11:12.779851 stigg_api_client_v2-0.517.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-08-01 07:11:18.679895 stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-08-01 07:11:18.707895 stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-08-01 07:11:13.095853 stigg_api_client_v2-0.517.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-08-01 07:11:18.743895 stigg_api_client_v2-0.517.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24306 2023-08-01 07:11:15.315870 stigg_api_client_v2-0.517.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-08-01 07:11:18.691895 stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-08-01 07:11:18.703895 stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-08-01 07:11:20.019897 stigg_api_client_v2-0.517.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-08-01 07:11:20.015897 stigg_api_client_v2-0.517.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-08-01 07:11:18.783895 stigg_api_client_v2-0.517.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-08-01 07:11:18.791895 stigg_api_client_v2-0.517.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-08-01 07:11:18.771895 stigg_api_client_v2-0.517.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-08-01 07:11:18.851896 stigg_api_client_v2-0.517.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-08-01 07:11:18.815895 stigg_api_client_v2-0.517.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-08-01 07:11:18.807895 stigg_api_client_v2-0.517.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-08-01 07:11:18.863896 stigg_api_client_v2-0.517.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-08-01 07:11:18.799895 stigg_api_client_v2-0.517.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-08-01 07:11:18.827895 stigg_api_client_v2-0.517.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-08-01 07:11:18.843896 stigg_api_client_v2-0.517.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-08-01 07:11:18.627894 stigg_api_client_v2-0.517.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-08-01 07:11:18.619894 stigg_api_client_v2-0.517.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-08-01 07:11:18.659894 stigg_api_client_v2-0.517.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   127287 2023-08-01 07:11:18.599894 stigg_api_client_v2-0.517.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-08-01 07:11:18.751895 stigg_api_client_v2-0.517.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-08-01 07:11:18.615894 stigg_api_client_v2-0.517.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-08-01 07:11:18.655894 stigg_api_client_v2-0.517.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-08-01 07:11:18.735895 stigg_api_client_v2-0.517.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-08-01 07:11:18.727895 stigg_api_client_v2-0.517.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-08-01 07:11:18.719895 stigg_api_client_v2-0.517.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-08-01 07:11:20.027897 stigg_api_client_v2-0.517.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-08-01 07:11:18.639894 stigg_api_client_v2-0.517.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-08-01 07:11:18.671894 stigg_api_client_v2-0.517.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-08-01 07:11:18.875896 stigg_api_client_v2-0.517.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.517.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/README.md
+-rw-r--r--   0        0        0      452 2023-08-03 12:59:36.334378 stigg_api_client_v2-0.522.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/__init__.py
+-rw-r--r--   0        0        0     4711 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/client.py
+-rw-r--r--   0        0        0      932 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/edge_utils.py
+-rw-r--r--   0        0        0    41178 2023-08-03 12:59:34.242369 stigg_api_client_v2-0.522.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-08-03 12:59:32.490362 stigg_api_client_v2-0.522.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-08-03 12:59:34.038368 stigg_api_client_v2-0.522.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-08-03 12:59:27.218340 stigg_api_client_v2-0.522.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-08-03 12:59:32.418362 stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-08-03 12:59:32.442362 stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-08-03 12:59:27.478341 stigg_api_client_v2-0.522.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-08-03 12:59:32.474362 stigg_api_client_v2-0.522.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24514 2023-08-03 12:59:29.422349 stigg_api_client_v2-0.522.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-08-03 12:59:32.430362 stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-08-03 12:59:32.438362 stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-08-03 12:59:32.506362 stigg_api_client_v2-0.522.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-08-03 12:59:32.518362 stigg_api_client_v2-0.522.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-08-03 12:59:32.498362 stigg_api_client_v2-0.522.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-08-03 12:59:32.562362 stigg_api_client_v2-0.522.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-08-03 12:59:32.534362 stigg_api_client_v2-0.522.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-08-03 12:59:32.530362 stigg_api_client_v2-0.522.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-08-03 12:59:32.574362 stigg_api_client_v2-0.522.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-08-03 12:59:32.522362 stigg_api_client_v2-0.522.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-08-03 12:59:32.546362 stigg_api_client_v2-0.522.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-08-03 12:59:32.558362 stigg_api_client_v2-0.522.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-08-03 12:59:32.382361 stigg_api_client_v2-0.522.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-08-03 12:59:32.374361 stigg_api_client_v2-0.522.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-08-03 12:59:32.406361 stigg_api_client_v2-0.522.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   128817 2023-08-03 12:59:32.350361 stigg_api_client_v2-0.522.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-08-03 12:59:32.482362 stigg_api_client_v2-0.522.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-08-03 12:59:32.366361 stigg_api_client_v2-0.522.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-08-03 12:59:32.402361 stigg_api_client_v2-0.522.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-08-03 12:59:32.466362 stigg_api_client_v2-0.522.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-08-03 12:59:32.458362 stigg_api_client_v2-0.522.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-08-03 12:59:32.450362 stigg_api_client_v2-0.522.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-08-03 12:59:33.646366 stigg_api_client_v2-0.522.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-08-03 12:59:32.390361 stigg_api_client_v2-0.522.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-08-03 12:59:32.414362 stigg_api_client_v2-0.522.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-08-03 12:59:32.582362 stigg_api_client_v2-0.522.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.522.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.517.0/README.md` & `stigg_api_client_v2-0.522.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.517.0/stigg/client.py` & `stigg_api_client_v2-0.522.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.517.0/stigg/edge_utils.py` & `stigg_api_client_v2-0.522.0/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.522.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
@@ -55,14 +55,15 @@
     MemberSortFields,
     MemberStatus,
     MeterType,
     MonthlyAccordingTo,
     PackageDTOSortFields,
     PackageEntitlementSortFields,
     PackageStatus,
+    PaymentCollection,
     PaymentMethodType,
     PlanSortFields,
     PriceSortFields,
     PricingType,
     ProductSortFields,
     PromotionalEntitlementPeriod,
     PromotionalEntitlementSortFields,
@@ -473,14 +474,15 @@
     PackageEntitlementFilterPackageDTOFilter,
     PackageEntitlementInput,
     PackageEntitlementSort,
     PackageEntitlementUpdateInput,
     PackagePricingInput,
     PackagePublishInput,
     PackageStatusFilterComparison,
+    PaymentCollectionFilterComparison,
     PaywallColorsPaletteInput,
     PaywallConfigurationInput,
     PaywallLayoutConfigurationInput,
     PlanCreateInput,
     PlanFilter,
     PlanFilterAddonFilter,
     PlanFilterProductFilter,
@@ -931,14 +933,16 @@
     "PackageEntitlementSort",
     "PackageEntitlementSortFields",
     "PackageEntitlementUpdateInput",
     "PackagePricingInput",
     "PackagePublishInput",
     "PackageStatus",
     "PackageStatusFilterComparison",
+    "PaymentCollection",
+    "PaymentCollectionFilterComparison",
     "PaymentMethodType",
     "PaywallAddonFragment",
     "PaywallAddonFragmentEntitlements",
     "PaywallAddonFragmentPrices",
     "PaywallCalculatedPricePointsFragment",
     "PaywallCalculatedPricePointsFragmentFeature",
     "PaywallColorsPaletteInput",
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.522.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.522.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.522.0/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.522.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/client.py` & `stigg_api_client_v2-0.522.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.522.0/stigg/generated/update_subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.522.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -265,14 +265,15 @@
     crmId = "crmId"
     crmLinkUrl = "crmLinkUrl"
     effectiveEndDate = "effectiveEndDate"
     endDate = "endDate"
     environmentId = "environmentId"
     id = "id"
     oldBillingId = "oldBillingId"
+    paymentCollection = "paymentCollection"
     pricingType = "pricingType"
     refId = "refId"
     resourceId = "resourceId"
     startDate = "startDate"
     status = "status"
     subscriptionId = "subscriptionId"
     trialEndDate = "trialEndDate"
@@ -609,14 +610,21 @@
 
 class PackageStatus(str, Enum):
     ARCHIVED = "ARCHIVED"
     DRAFT = "DRAFT"
     PUBLISHED = "PUBLISHED"
 
 
+class PaymentCollection(str, Enum):
+    ACTION_REQUIRED = "ACTION_REQUIRED"
+    FAILED = "FAILED"
+    NOT_REQUIRED = "NOT_REQUIRED"
+    PROCESSING = "PROCESSING"
+
+
 class PaymentMethodType(str, Enum):
     BANK = "BANK"
     CARD = "CARD"
 
 
 class PlanSortFields(str, Enum):
     billingId = "billingId"
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.522.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.522.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -329,14 +329,27 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -381,14 +394,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -401,21 +421,14 @@
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -493,27 +506,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,61 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class SubscriptionFutureUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -668,60 +621,56 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
+class SubscriptionFutureUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
         alias="targetPackage"
     )
     schedule_variables: Optional[
         Annotated[
             Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="scheduleVariables")
 
 
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
     BaseModel
 ):
     typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
+class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
     typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
     addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
+class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
@@ -734,14 +683,65 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1431,68 +1431,68 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-SubscriptionFutureUpdateData.update_forward_refs()
-SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+SubscriptionFutureUpdateData.update_forward_refs()
+SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.522.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.522.0/stigg/generated/get_coupons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.522.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.522.0/stigg/generated/get_mock_paywall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.522.0/stigg/generated/get_sdk_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.522.0/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -41,14 +41,15 @@
     IntegrationSortFields,
     MemberSortFields,
     MeterType,
     MonthlyAccordingTo,
     PackageDTOSortFields,
     PackageEntitlementSortFields,
     PackageStatus,
+    PaymentCollection,
     PlanSortFields,
     PriceSortFields,
     PricingType,
     ProductSortFields,
     PromotionalEntitlementPeriod,
     PromotionalEntitlementSortFields,
     PromotionalEntitlementStatus,
@@ -490,14 +491,17 @@
         alias="effectiveEndDate"
     )
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[List["CustomerFilterCustomerSubscriptionFilter"]] = Field(alias="or")
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
     status: Optional["SubscriptionStatusFilterComparison"]
     subscription_id: Optional["StringFieldComparison"] = Field(alias="subscriptionId")
     trial_end_date: Optional["DateFieldComparison"] = Field(alias="trialEndDate")
@@ -606,14 +610,17 @@
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[List["CustomerResourceFilterCustomerSubscriptionFilter"]] = Field(
         alias="or"
     )
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
     status: Optional["SubscriptionStatusFilterComparison"]
     subscription_id: Optional["StringFieldComparison"] = Field(alias="subscriptionId")
     trial_end_date: Optional["DateFieldComparison"] = Field(alias="trialEndDate")
@@ -647,14 +654,17 @@
         alias="effectiveEndDate"
     )
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[List["CustomerSubscriptionFilter"]] = Field(alias="or")
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     plan: Optional["CustomerSubscriptionFilterPlanFilter"]
     prices: Optional["CustomerSubscriptionFilterSubscriptionPriceFilter"]
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource: Optional["CustomerSubscriptionFilterCustomerResourceFilter"]
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
@@ -1501,14 +1511,31 @@
     lte: Optional[PackageStatus]
     neq: Optional[PackageStatus]
     not_i_like: Optional[PackageStatus] = Field(alias="notILike")
     not_in: Optional[List[PackageStatus]] = Field(alias="notIn")
     not_like: Optional[PackageStatus] = Field(alias="notLike")
 
 
+class PaymentCollectionFilterComparison(BaseModel):
+    eq: Optional[PaymentCollection]
+    gt: Optional[PaymentCollection]
+    gte: Optional[PaymentCollection]
+    i_like: Optional[PaymentCollection] = Field(alias="iLike")
+    in_: Optional[List[PaymentCollection]] = Field(alias="in")
+    is_: Optional[bool] = Field(alias="is")
+    is_not: Optional[bool] = Field(alias="isNot")
+    like: Optional[PaymentCollection]
+    lt: Optional[PaymentCollection]
+    lte: Optional[PaymentCollection]
+    neq: Optional[PaymentCollection]
+    not_i_like: Optional[PaymentCollection] = Field(alias="notILike")
+    not_in: Optional[List[PaymentCollection]] = Field(alias="notIn")
+    not_like: Optional[PaymentCollection] = Field(alias="notLike")
+
+
 class PaywallColorsPaletteInput(BaseModel):
     background_color: Optional[str] = Field(alias="backgroundColor")
     border_color: Optional[str] = Field(alias="borderColor")
     current_plan_background: Optional[str] = Field(alias="currentPlanBackground")
     primary: Optional[str]
     text_color: Optional[str] = Field(alias="textColor")
 
@@ -2100,14 +2127,17 @@
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[List["SubscriptionAddonFilterCustomerSubscriptionFilter"]] = Field(
         alias="or"
     )
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
     status: Optional["SubscriptionStatusFilterComparison"]
     subscription_id: Optional["StringFieldComparison"] = Field(alias="subscriptionId")
     trial_end_date: Optional["DateFieldComparison"] = Field(alias="trialEndDate")
@@ -2199,14 +2229,17 @@
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[
         List["SubscriptionEntitlementFilterCustomerSubscriptionFilter"]
     ] = Field(alias="or")
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
     status: Optional["SubscriptionStatusFilterComparison"]
     subscription_id: Optional["StringFieldComparison"] = Field(alias="subscriptionId")
     trial_end_date: Optional["DateFieldComparison"] = Field(alias="trialEndDate")
@@ -2349,14 +2382,17 @@
     end_date: Optional["DateFieldComparison"] = Field(alias="endDate")
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     old_billing_id: Optional["StringFieldComparison"] = Field(alias="oldBillingId")
     or_: Optional[List["SubscriptionPriceFilterCustomerSubscriptionFilter"]] = Field(
         alias="or"
     )
+    payment_collection: Optional["PaymentCollectionFilterComparison"] = Field(
+        alias="paymentCollection"
+    )
     pricing_type: Optional["PricingTypeFilterComparison"] = Field(alias="pricingType")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     resource_id: Optional["StringFieldComparison"] = Field(alias="resourceId")
     start_date: Optional["DateFieldComparison"] = Field(alias="startDate")
     status: Optional["SubscriptionStatusFilterComparison"]
     subscription_id: Optional["StringFieldComparison"] = Field(alias="subscriptionId")
     trial_end_date: Optional["DateFieldComparison"] = Field(alias="trialEndDate")
@@ -2915,14 +2951,15 @@
 PackageEntitlementFilterPackageDTOFilter.update_forward_refs()
 PackageEntitlementInput.update_forward_refs()
 PackageEntitlementSort.update_forward_refs()
 PackageEntitlementUpdateInput.update_forward_refs()
 PackagePricingInput.update_forward_refs()
 PackagePublishInput.update_forward_refs()
 PackageStatusFilterComparison.update_forward_refs()
+PaymentCollectionFilterComparison.update_forward_refs()
 PaywallColorsPaletteInput.update_forward_refs()
 PaywallConfigurationInput.update_forward_refs()
 PaywallLayoutConfigurationInput.update_forward_refs()
 PlanCreateInput.update_forward_refs()
 PlanFilter.update_forward_refs()
 PlanFilterAddonFilter.update_forward_refs()
 PlanFilterProductFilter.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.522.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.522.0/stigg/generated/provision_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.522.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.522.0/stigg/generated/report_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.517.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.522.0/stigg/generated/create_subscription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-08-01 07:11
+# Generated by ariadne-codegen on 2023-08-03 12:59
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class UpdateSubscription(BaseModel):
-    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
-        alias="updateSubscription"
+class CreateSubscription(BaseModel):
+    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
+        alias="createSubscription"
     )
 
 
-class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
+class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
     pass
 
 
-UpdateSubscription.update_forward_refs()
-UpdateSubscriptionUpdateSubscription.update_forward_refs()
+CreateSubscription.update_forward_refs()
+CreateSubscriptionCreateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.517.0/PKG-INFO` & `stigg_api_client_v2-0.522.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.517.0
+Version: 0.522.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

