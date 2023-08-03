# Comparing `tmp/stigg_api_client-0.517.0.tar.gz` & `tmp/stigg_api_client-0.522.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.517.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.522.0.tar", max compression
```

## Comparing `stigg_api_client-0.517.0.tar` & `stigg_api_client-0.522.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/README.md
--rw-r--r--   0        0        0      480 2023-08-01 07:10:51.584442 stigg_api_client-0.517.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-08-01 07:10:16.828104 stigg_api_client-0.517.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-08-01 07:10:49.652430 stigg_api_client-0.517.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-08-01 07:10:50.068433 stigg_api_client-0.517.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   468257 2023-08-01 07:10:49.916432 stigg_api_client-0.517.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.517.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/README.md
+-rw-r--r--   0        0        0      480 2023-08-03 12:59:09.115447 stigg_api_client-0.522.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:59:07.115406 stigg_api_client-0.522.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-08-03 12:59:07.607416 stigg_api_client-0.522.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   471091 2023-08-03 12:59:07.379412 stigg_api_client-0.522.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.522.0/PKG-INFO
```

### Comparing `stigg_api_client-0.517.0/README.md` & `stigg_api_client-0.522.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.517.0/stigg/client.py` & `stigg_api_client-0.522.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.517.0/stigg/generated/operations.py` & `stigg_api_client-0.522.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.517.0/stigg/generated/schema.py` & `stigg_api_client-0.522.0/stigg/generated/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 class CustomerSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'crmHubspotCompanyId', 'crmHubspotCompanyUrl', 'crmId', 'customerId', 'deletedAt', 'email', 'environmentId', 'id', 'name', 'refId', 'updatedAt')
 
 
 class CustomerSubscriptionSortFields(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('billingId', 'cancelReason', 'cancellationDate', 'createdAt', 'crmId', 'crmLinkUrl', 'effectiveEndDate', 'endDate', 'environmentId', 'id', 'oldBillingId', 'pricingType', 'refId', 'resourceId', 'startDate', 'status', 'subscriptionId', 'trialEndDate')
+    __choices__ = ('billingId', 'cancelReason', 'cancellationDate', 'createdAt', 'crmId', 'crmLinkUrl', 'effectiveEndDate', 'endDate', 'environmentId', 'id', 'oldBillingId', 'paymentCollection', 'pricingType', 'refId', 'resourceId', 'startDate', 'status', 'subscriptionId', 'trialEndDate')
 
 
 DateTime = sgqlc.types.datetime.DateTime
 
 class Department(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('CEO_OR_FOUNDER', 'ENGINEERING', 'GROWTH', 'MARKETING', 'MONETIZATION', 'OTHER', 'PRODUCT')
@@ -254,14 +254,19 @@
 
 
 class PackageStatus(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('ARCHIVED', 'DRAFT', 'PUBLISHED')
 
 
+class PaymentCollection(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('ACTION_REQUIRED', 'FAILED', 'NOT_REQUIRED', 'PROCESSING')
+
+
 class PaymentMethodType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('BANK', 'CARD')
 
 
 class PlanSortFields(sgqlc.types.Enum):
     __schema__ = schema
@@ -900,28 +905,29 @@
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     subscriptions = sgqlc.types.Field('CustomerFilterCustomerSubscriptionFilter', graphql_name='subscriptions')
     updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
 
 
 class CustomerFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
     crm_link_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerFilterCustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field('PaymentCollectionFilterComparison', graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
@@ -1014,28 +1020,29 @@
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerFilter')), graphql_name='or')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
 
 
 class CustomerResourceFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
     crm_link_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field('PaymentCollectionFilterComparison', graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
@@ -1055,15 +1062,15 @@
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(CustomerSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
 class CustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('addons', 'and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'customer', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('addons', 'and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'customer', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'trial_end_date')
     addons = sgqlc.types.Field('CustomerSubscriptionFilterSubscriptionAddonFilter', graphql_name='addons')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
@@ -1071,14 +1078,15 @@
     customer = sgqlc.types.Field('CustomerSubscriptionFilterCustomerFilter', graphql_name='customer')
     effective_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field('PaymentCollectionFilterComparison', graphql_name='paymentCollection')
     plan = sgqlc.types.Field('CustomerSubscriptionFilterPlanFilter', graphql_name='plan')
     prices = sgqlc.types.Field('CustomerSubscriptionFilterSubscriptionPriceFilter', graphql_name='prices')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     resource = sgqlc.types.Field('CustomerSubscriptionFilterCustomerResourceFilter', graphql_name='resource')
     resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
@@ -2017,14 +2025,33 @@
     lte = sgqlc.types.Field(PackageStatus, graphql_name='lte')
     neq = sgqlc.types.Field(PackageStatus, graphql_name='neq')
     not_ilike = sgqlc.types.Field(PackageStatus, graphql_name='notILike')
     not_in = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PackageStatus)), graphql_name='notIn')
     not_like = sgqlc.types.Field(PackageStatus, graphql_name='notLike')
 
 
+class PaymentCollectionFilterComparison(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
+    eq = sgqlc.types.Field(PaymentCollection, graphql_name='eq')
+    gt = sgqlc.types.Field(PaymentCollection, graphql_name='gt')
+    gte = sgqlc.types.Field(PaymentCollection, graphql_name='gte')
+    i_like = sgqlc.types.Field(PaymentCollection, graphql_name='iLike')
+    in_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaymentCollection)), graphql_name='in')
+    is_ = sgqlc.types.Field(Boolean, graphql_name='is')
+    is_not = sgqlc.types.Field(Boolean, graphql_name='isNot')
+    like = sgqlc.types.Field(PaymentCollection, graphql_name='like')
+    lt = sgqlc.types.Field(PaymentCollection, graphql_name='lt')
+    lte = sgqlc.types.Field(PaymentCollection, graphql_name='lte')
+    neq = sgqlc.types.Field(PaymentCollection, graphql_name='neq')
+    not_ilike = sgqlc.types.Field(PaymentCollection, graphql_name='notILike')
+    not_in = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaymentCollection)), graphql_name='notIn')
+    not_like = sgqlc.types.Field(PaymentCollection, graphql_name='notLike')
+
+
 class PaywallColorsPaletteInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('background_color', 'border_color', 'current_plan_background', 'primary', 'text_color')
     background_color = sgqlc.types.Field(String, graphql_name='backgroundColor')
     border_color = sgqlc.types.Field(String, graphql_name='borderColor')
     current_plan_background = sgqlc.types.Field(String, graphql_name='currentPlanBackground')
     primary = sgqlc.types.Field(String, graphql_name='primary')
@@ -2650,28 +2677,29 @@
     status = sgqlc.types.Field(PackageStatusFilterComparison, graphql_name='status')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     version_number = sgqlc.types.Field(IntFieldComparison, graphql_name='versionNumber')
 
 
 class SubscriptionAddonFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterCustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field(PaymentCollectionFilterComparison, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
     resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
@@ -2751,28 +2779,29 @@
     subscription = sgqlc.types.Field('SubscriptionEntitlementFilterCustomerSubscriptionFilter', graphql_name='subscription')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
 
 
 class SubscriptionEntitlementFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionEntitlementFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReasonFilterComparison, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionEntitlementFilterCustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field(PaymentCollectionFilterComparison, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
     resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
@@ -2885,28 +2914,29 @@
     subscription = sgqlc.types.Field('SubscriptionPriceFilterCustomerSubscriptionFilter', graphql_name='subscription')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     usage_limit = sgqlc.types.Field(NumberFieldComparison, graphql_name='usageLimit')
 
 
 class SubscriptionPriceFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReasonFilterComparison, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterCustomerSubscriptionFilter')), graphql_name='or')
+    payment_collection = sgqlc.types.Field(PaymentCollectionFilterComparison, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
     resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
@@ -4083,15 +4113,15 @@
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class CustomerSubscription(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'future_updates', 'id', 'is_custom_price_subscription', 'latest_invoice', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
+    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'future_updates', 'id', 'is_custom_price_subscription', 'latest_invoice', 'old_billing_id', 'outdated_price_packages', 'payment_collection', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddon')), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionAddonFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
@@ -4112,14 +4142,15 @@
     experiment_info = sgqlc.types.Field('experimentInfo', graphql_name='experimentInfo')
     future_updates = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionFutureUpdate'))), graphql_name='futureUpdates')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     is_custom_price_subscription = sgqlc.types.Field(Boolean, graphql_name='isCustomPriceSubscription')
     latest_invoice = sgqlc.types.Field('SubscriptionInvoice', graphql_name='latestInvoice')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     outdated_price_packages = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='outdatedPricePackages')
+    payment_collection = sgqlc.types.Field(sgqlc.types.non_null(PaymentCollection), graphql_name='paymentCollection')
     plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='plan')
     prices = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPrice')), graphql_name='prices', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionPriceFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionPriceSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     pricing_type = sgqlc.types.Field(sgqlc.types.non_null(PricingType), graphql_name='pricingType')
@@ -4139,26 +4170,27 @@
     total_price = sgqlc.types.Field('CustomerSubscriptionTotalPrice', graphql_name='totalPrice')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
     was_in_trial = sgqlc.types.Field(Boolean, graphql_name='wasInTrial')
 
 
 class CustomerSubscriptionAggregateGroupBy(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
+    payment_collection = sgqlc.types.Field(PaymentCollection, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
@@ -4170,26 +4202,27 @@
     edges = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionEdge'))), graphql_name='edges')
     page_info = sgqlc.types.Field(sgqlc.types.non_null('PageInfo'), graphql_name='pageInfo')
     total_count = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalCount')
 
 
 class CustomerSubscriptionCountAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(Int, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(Int, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(Int, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(Int, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(Int, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(Int, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(Int, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(Int, graphql_name='endDate')
     environment_id = sgqlc.types.Field(Int, graphql_name='environmentId')
     id = sgqlc.types.Field(Int, graphql_name='id')
     old_billing_id = sgqlc.types.Field(Int, graphql_name='oldBillingId')
+    payment_collection = sgqlc.types.Field(Int, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(Int, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(Int, graphql_name='refId')
     resource_id = sgqlc.types.Field(Int, graphql_name='resourceId')
     start_date = sgqlc.types.Field(Int, graphql_name='startDate')
     status = sgqlc.types.Field(Int, graphql_name='status')
     subscription_id = sgqlc.types.Field(Int, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(Int, graphql_name='trialEndDate')
@@ -4200,49 +4233,51 @@
     __field_names__ = ('cursor', 'node')
     cursor = sgqlc.types.Field(sgqlc.types.non_null(ConnectionCursor), graphql_name='cursor')
     node = sgqlc.types.Field(sgqlc.types.non_null(CustomerSubscription), graphql_name='node')
 
 
 class CustomerSubscriptionMaxAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
+    payment_collection = sgqlc.types.Field(PaymentCollection, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
 
 
 class CustomerSubscriptionMinAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'payment_collection', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
+    payment_collection = sgqlc.types.Field(PaymentCollection, graphql_name='paymentCollection')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
```

### Comparing `stigg_api_client-0.517.0/PKG-INFO` & `stigg_api_client-0.522.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.517.0
+Version: 0.522.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

