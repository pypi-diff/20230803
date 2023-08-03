# Comparing `tmp/fern_merge-0.2.1.tar.gz` & `tmp/fern_merge-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_merge-0.2.1.tar", max compression
+gzip compressed data, was "fern_merge-0.2.2.tar", max compression
```

## Comparing `fern_merge-0.2.1.tar` & `fern_merge-0.2.2.tar`

### file list

```diff
@@ -1,1222 +1,1222 @@
--rw-r--r--   0        0        0     4149 2023-07-26 02:55:46.682442 fern_merge-0.2.1/README.md
--rw-r--r--   0        0        0      388 2023-07-26 02:55:46.682442 fern_merge-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      277 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/__init__.py
--rw-r--r--   0        0        0     2830 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/client.py
--rw-r--r--   0        0        0      519 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1482 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      201 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/py.typed
--rw-r--r--   0        0        0      206 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/__init__.py
--rw-r--r--   0        0        0    12630 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/__init__.py
--rw-r--r--   0        0        0    12026 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/client.py
--rw-r--r--   0        0        0     1410 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2430 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2670 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/accounts/__init__.py
--rw-r--r--   0        0        0    18250 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/addresses/__init__.py
--rw-r--r--   0        0        0     4508 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/addresses/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/attachments/__init__.py
--rw-r--r--   0        0        0    14669 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2508 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/balance_sheets/__init__.py
--rw-r--r--   0        0        0    10935 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/balance_sheets/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
--rw-r--r--   0        0        0    11063 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/company_info/__init__.py
--rw-r--r--   0        0        0    10594 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/company_info/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/contacts/__init__.py
--rw-r--r--   0        0        0    17956 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/credit_notes/__init__.py
--rw-r--r--   0        0        0    14854 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/credit_notes/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2173 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/expenses/__init__.py
--rw-r--r--   0        0        0    16615 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/expenses/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3086 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/income_statements/__init__.py
--rw-r--r--   0        0        0    11009 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/income_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/invoices/__init__.py
--rw-r--r--   0        0        0    20202 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/invoices/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/issues/__init__.py
--rw-r--r--   0        0        0    10594 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/items/__init__.py
--rw-r--r--   0        0        0    13155 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/items/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/journal_entries/__init__.py
--rw-r--r--   0        0        0    16931 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/journal_entries/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8934 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10699 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7392 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/payments/__init__.py
--rw-r--r--   0        0        0    17415 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/payments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/phone_numbers/__init__.py
--rw-r--r--   0        0        0     3317 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/phone_numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/purchase_orders/__init__.py
--rw-r--r--   0        0        0    19258 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/purchase_orders/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2865 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8336 2023-07-26 02:55:46.682442 fern_merge-0.2.1/src/merge/resources/accounting/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3408 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/tax_rates/__init__.py
--rw-r--r--   0        0        0    10815 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/tax_rates/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/tracking_categories/__init__.py
--rw-r--r--   0        0        0    13405 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/tracking_categories/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/transactions/__init__.py
--rw-r--r--   0        0        0    12082 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/transactions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/vendor_credits/__init__.py
--rw-r--r--   0        0        0    12106 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/vendor_credits/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5271 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    17717 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/__init__.py
--rw-r--r--   0        0        0    17393 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account.py
--rw-r--r--   0        0        0      195 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_classification.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_currency.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_integration.py
--rw-r--r--   0        0        0    16986 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_request.py
--rw-r--r--   0        0        0      202 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_request_classification.py
--rw-r--r--   0        0        0      178 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_request_currency.py
--rw-r--r--   0        0        0      192 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_response.py
--rw-r--r--   0        0        0      185 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_status.py
--rw-r--r--   0        0        0      758 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_status_enum.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/account_token.py
--rw-r--r--   0        0        0     1935 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment.py
--rw-r--r--   0        0        0     1462 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment_request.py
--rw-r--r--   0        0        0     1158 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment_response.py
--rw-r--r--   0        0        0     1344 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_phone_number.py
--rw-r--r--   0        0        0     1346 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_phone_number_request.py
--rw-r--r--   0        0        0      819 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
--rw-r--r--   0        0        0      831 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      847 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    11090 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/address.py
--rw-r--r--   0        0        0      167 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/address_country.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/address_type.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/address_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/available_actions.py
--rw-r--r--   0        0        0    16903 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/balance_sheet.py
--rw-r--r--   0        0        0      176 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/balance_sheet_currency.py
--rw-r--r--   0        0        0    17216 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/cash_flow_statement.py
--rw-r--r--   0        0        0      181 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/cash_flow_statement_currency.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/category_enum.py
--rw-r--r--   0        0        0      560 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/category_type_enum.py
--rw-r--r--   0        0        0     1103 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/classification_enum.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0    16863 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/company_info.py
--rw-r--r--   0        0        0      175 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/company_info_currency.py
--rw-r--r--   0        0        0      827 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/company_info_list_request_expand.py
--rw-r--r--   0        0        0      843 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/condition_type_enum.py
--rw-r--r--   0        0        0     3027 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contact.py
--rw-r--r--   0        0        0     2478 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contact_request.py
--rw-r--r--   0        0        0      182 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contact_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contact_response.py
--rw-r--r--   0        0        0      175 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contact_status.py
--rw-r--r--   0        0        0     1675 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contacts_list_request_expand.py
--rw-r--r--   0        0        0     1707 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
--rw-r--r--   0        0        0    35178 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/country_enum.py
--rw-r--r--   0        0        0    17747 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note.py
--rw-r--r--   0        0        0      174 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_currency.py
--rw-r--r--   0        0        0     2275 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_line_item.py
--rw-r--r--   0        0        0      198 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_status.py
--rw-r--r--   0        0        0      784 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_status_enum.py
--rw-r--r--   0        0        0     1859 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
--rw-r--r--   0        0        0      731 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
--rw-r--r--   0        0        0      743 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1891 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      747 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      759 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    47961 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/currency_enum.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/error_validation_problem.py
--rw-r--r--   0        0        0    16980 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_currency.py
--rw-r--r--   0        0        0     2074 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_line.py
--rw-r--r--   0        0        0     2076 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_line_request.py
--rw-r--r--   0        0        0    16445 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_request.py
--rw-r--r--   0        0        0      178 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.686442 fern_merge-0.2.1/src/merge/resources/accounting/types/expense_response.py
--rw-r--r--   0        0        0     3715 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/expenses_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
--rw-r--r--   0        0        0    17240 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/income_statement.py
--rw-r--r--   0        0        0      179 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/income_statement_currency.py
--rw-r--r--   0        0        0    18003 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_currency.py
--rw-r--r--   0        0        0    16460 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item.py
--rw-r--r--   0        0        0      179 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item_currency.py
--rw-r--r--   0        0        0    16389 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item_request.py
--rw-r--r--   0        0        0      186 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
--rw-r--r--   0        0        0    17620 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_request.py
--rw-r--r--   0        0        0      178 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_request_currency.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_request_type.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_response.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_type.py
--rw-r--r--   0        0        0      709 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_type_enum.py
--rw-r--r--   0        0        0     8275 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_list_request_expand.py
--rw-r--r--   0        0        0      622 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_list_request_type.py
--rw-r--r--   0        0        0     8403 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/issues_list_request_status.py
--rw-r--r--   0        0        0     2624 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/item.py
--rw-r--r--   0        0        0      172 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/item_status.py
--rw-r--r--   0        0        0     1791 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/items_list_request_expand.py
--rw-r--r--   0        0        0     1823 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py
--rw-r--r--   0        0        0     3771 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
--rw-r--r--   0        0        0     3835 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
--rw-r--r--   0        0        0    17164 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry.py
--rw-r--r--   0        0        0      176 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_currency.py
--rw-r--r--   0        0        0      197 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_posting_status.py
--rw-r--r--   0        0        0    16526 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_request.py
--rw-r--r--   0        0        0      183 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_request_currency.py
--rw-r--r--   0        0        0      204 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
--rw-r--r--   0        0        0     1126 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_response.py
--rw-r--r--   0        0        0     1790 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_line.py
--rw-r--r--   0        0        0     1792 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/journal_line_request.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_account_list.py
--rw-r--r--   0        0        0      941 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
--rw-r--r--   0        0        0      909 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
--rw-r--r--   0        0        0      930 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
--rw-r--r--   0        0        0      905 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_company_info_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_contact_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_credit_note_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_expense_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_income_statement_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_invoice_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_item_list.py
--rw-r--r--   0        0        0      909 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_payment_list.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      889 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py
--rw-r--r--   0        0        0      925 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py
--rw-r--r--   0        0        0      904 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_transaction_list.py
--rw-r--r--   0        0        0      909 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
--rw-r--r--   0        0        0    16832 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payment.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payment_currency.py
--rw-r--r--   0        0        0    16241 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payment_request.py
--rw-r--r--   0        0        0      178 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payment_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payment_response.py
--rw-r--r--   0        0        0     3715 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payments_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
--rw-r--r--   0        0        0      554 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/posting_status_enum.py
--rw-r--r--   0        0        0    17816 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_currency.py
--rw-r--r--   0        0        0    16830 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item.py
--rw-r--r--   0        0        0      185 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
--rw-r--r--   0        0        0    16854 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py
--rw-r--r--   0        0        0      192 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
--rw-r--r--   0        0        0    17041 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_request.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_request_currency.py
--rw-r--r--   0        0        0      217 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_request_status.py
--rw-r--r--   0        0        0     1130 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_response.py
--rw-r--r--   0        0        0      210 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_status.py
--rw-r--r--   0        0        0     1154 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_status_enum.py
--rw-r--r--   0        0        0     9043 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
--rw-r--r--   0        0        0     9171 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/remote_response.py
--rw-r--r--   0        0        0     1649 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/report_item.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0      542 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/status_7_d_1_enum.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2002 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/tax_rate.py
--rw-r--r--   0        0        0     2481 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/tracking_category.py
--rw-r--r--   0        0        0      197 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/tracking_category_category_type.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/tracking_category_status.py
--rw-r--r--   0        0        0    17229 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transaction.py
--rw-r--r--   0        0        0      175 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transaction_currency.py
--rw-r--r--   0        0        0    16685 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transaction_line_item.py
--rw-r--r--   0        0        0      183 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transaction_line_item_currency.py
--rw-r--r--   0        0        0     3899 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transactions_list_request_expand.py
--rw-r--r--   0        0        0     3963 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/validation_problem_source.py
--rw-r--r--   0        0        0    16901 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credit.py
--rw-r--r--   0        0        0      176 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credit_currency.py
--rw-r--r--   0        0        0     1999 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credit_line.py
--rw-r--r--   0        0        0     3675 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
--rw-r--r--   0        0        0     3739 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/accounting/types/webhook_receiver.py
--rw-r--r--   0        0        0     9656 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-26 02:55:46.690442 fern_merge-0.2.1/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2656 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    18450 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    22753 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    18326 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    25052 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     9128 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0    13425 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3072 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2841 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    19472 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0    10566 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0    10955 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0    14939 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8920 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10685 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0    13609 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     9042 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2851 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     9178 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0    14473 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3394 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     6731 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0    11995 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5243 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13447 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2705 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2155 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0      187 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_request_visibility.py
--rw-r--r--   0        0        0     1109 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/activity_visibility.py
--rw-r--r--   0        0        0     2473 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0      201 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/eeoc_disability_status.py
--rw-r--r--   0        0        0      160 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/eeoc_gender.py
--rw-r--r--   0        0        0      152 2023-07-26 02:55:46.694442 fern_merge-0.2.1/src/merge/resources/ats/types/eeoc_race.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/eeoc_veteran_status.py
--rw-r--r--   0        0        0     3803 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3428 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0      169 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/job_status.py
--rw-r--r--   0        0        0     1045 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2786 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/offer_status.py
--rw-r--r--   0        0        0     1832 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2562 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      183 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/remote_user_access_role.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3187 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2464 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0      237 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_request_status.py
--rw-r--r--   0        0        0     1150 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      230 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_status.py
--rw-r--r--   0        0        0      893 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2692 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0      226 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scorecard_overall_recommendation.py
--rw-r--r--   0        0        0     1731 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0     9538 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/__init__.py
--rw-r--r--   0        0        0     9931 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/client.py
--rw-r--r--   0        0        0     1144 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2656 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/accounts/__init__.py
--rw-r--r--   0        0        0    25993 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/association_types/__init__.py
--rw-r--r--   0        0        0    17340 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/association_types/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/associations/__init__.py
--rw-r--r--   0        0        0    12477 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/associations/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/contacts/__init__.py
--rw-r--r--   0        0        0    28327 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/custom_object_classes/__init__.py
--rw-r--r--   0        0        0    13387 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/custom_object_classes/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/custom_objects/__init__.py
--rw-r--r--   0        0        0    22608 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/custom_objects/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.698442 fern_merge-0.2.1/src/merge/resources/crm/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/engagement_types/__init__.py
--rw-r--r--   0        0        0    15005 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/engagement_types/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/engagements/__init__.py
--rw-r--r--   0        0        0    25867 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/engagements/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3072 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2841 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/issues/__init__.py
--rw-r--r--   0        0        0    10566 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/leads/__init__.py
--rw-r--r--   0        0        0    22118 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/leads/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8920 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10685 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/notes/__init__.py
--rw-r--r--   0        0        0    22396 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/notes/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/opportunities/__init__.py
--rw-r--r--   0        0        0    30544 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/opportunities/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2851 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/stages/__init__.py
--rw-r--r--   0        0        0    14779 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/stages/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3394 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/tasks/__init__.py
--rw-r--r--   0        0        0    25417 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/tasks/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/users/__init__.py
--rw-r--r--   0        0        0    17206 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5243 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13264 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/__init__.py
--rw-r--r--   0        0        0     2708 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_integration.py
--rw-r--r--   0        0        0     1916 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_request.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/account_token.py
--rw-r--r--   0        0        0      719 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/activity_type_enum.py
--rw-r--r--   0        0        0    10978 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_address_type.py
--rw-r--r--   0        0        0      167 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_country.py
--rw-r--r--   0        0        0    11024 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_request.py
--rw-r--r--   0        0        0      191 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_request_address_type.py
--rw-r--r--   0        0        0      174 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_request_country.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/address_type_enum.py
--rw-r--r--   0        0        0     1226 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/association.py
--rw-r--r--   0        0        0      955 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/association_sub_type.py
--rw-r--r--   0        0        0     1663 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/association_type.py
--rw-r--r--   0        0        0      191 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/association_type_cardinality.py
--rw-r--r--   0        0        0     1335 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/association_type_request_request.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/available_actions.py
--rw-r--r--   0        0        0     1033 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/cardinality_enum.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/condition_type_enum.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/contact.py
--rw-r--r--   0        0        0     1944 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/contact_request.py
--rw-r--r--   0        0        0    35178 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/country_enum.py
--rw-r--r--   0        0        0     1108 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/crm_account_response.py
--rw-r--r--   0        0        0     1141 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/crm_association_type_response.py
--rw-r--r--   0        0        0     1108 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/crm_contact_response.py
--rw-r--r--   0        0        0     1129 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/crm_custom_object_response.py
--rw-r--r--   0        0        0     1399 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/custom_object.py
--rw-r--r--   0        0        0     1520 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/custom_object_class.py
--rw-r--r--   0        0        0      782 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/custom_object_request.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      549 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/direction_enum.py
--rw-r--r--   0        0        0     1317 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/email_address.py
--rw-r--r--   0        0        0     1319 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/email_address_request.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/encoding_enum.py
--rw-r--r--   0        0        0     2645 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement.py
--rw-r--r--   0        0        0      178 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_direction.py
--rw-r--r--   0        0        0     2216 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_request.py
--rw-r--r--   0        0        0      185 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_request_direction.py
--rw-r--r--   0        0        0     1117 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_response.py
--rw-r--r--   0        0        0     1866 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_type.py
--rw-r--r--   0        0        0      195 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagement_type_activity_type.py
--rw-r--r--   0        0        0     3563 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagements_list_request_expand.py
--rw-r--r--   0        0        0     3627 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/field_type_enum.py
--rw-r--r--   0        0        0      999 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/ignore_common_model_request.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/item_type_enum.py
--rw-r--r--   0        0        0     2863 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/lead.py
--rw-r--r--   0        0        0     2369 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/lead_request.py
--rw-r--r--   0        0        0     1093 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/lead_response.py
--rw-r--r--   0        0        0     1851 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/leads_list_request_expand.py
--rw-r--r--   0        0        0     1883 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2150 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/note.py
--rw-r--r--   0        0        0     1590 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/note_request.py
--rw-r--r--   0        0        0     1093 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/note_response.py
--rw-r--r--   0        0        0     3267 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/notes_list_request_expand.py
--rw-r--r--   0        0        0     3331 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      925 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/object_class_description_request.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/operator_schema.py
--rw-r--r--   0        0        0     1475 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_list_request_expand.py
--rw-r--r--   0        0        0      665 2023-07-26 02:55:46.702442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_list_request_status.py
--rw-r--r--   0        0        0     1507 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
--rw-r--r--   0        0        0     2685 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity.py
--rw-r--r--   0        0        0     2243 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_request.py
--rw-r--r--   0        0        0      208 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_request_status.py
--rw-r--r--   0        0        0     1121 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_response.py
--rw-r--r--   0        0        0      201 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_status.py
--rw-r--r--   0        0        0      704 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_status_enum.py
--rw-r--r--   0        0        0      893 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/origin_type_enum.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_account_list.py
--rw-r--r--   0        0        0      904 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_association_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_association_type_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_contact_list.py
--rw-r--r--   0        0        0      930 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py
--rw-r--r--   0        0        0      909 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_custom_object_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_engagement_list.py
--rw-r--r--   0        0        0      917 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_engagement_type_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_lead_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_note_list.py
--rw-r--r--   0        0        0      904 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_opportunity_list.py
--rw-r--r--   0        0        0      926 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_stage_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_task_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/paginated_user_list.py
--rw-r--r--   0        0        0     1923 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_account_request.py
--rw-r--r--   0        0        0     1951 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_contact_request.py
--rw-r--r--   0        0        0     2245 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_engagement_request.py
--rw-r--r--   0        0        0      192 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_engagement_request_direction.py
--rw-r--r--   0        0        0     2272 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_opportunity_request.py
--rw-r--r--   0        0        0      215 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_opportunity_request_status.py
--rw-r--r--   0        0        0     2029 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_task_request.py
--rw-r--r--   0        0        0      187 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/patched_task_request_status.py
--rw-r--r--   0        0        0     1307 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/phone_number.py
--rw-r--r--   0        0        0     1309 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/phone_number_request.py
--rw-r--r--   0        0        0      814 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class.py
--rw-r--r--   0        0        0     1722 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
--rw-r--r--   0        0        0      213 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
--rw-r--r--   0        0        0      205 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
--rw-r--r--   0        0        0      911 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
--rw-r--r--   0        0        0      825 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1694 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/stage.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2429 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task.py
--rw-r--r--   0        0        0     2000 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task_request.py
--rw-r--r--   0        0        0      180 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task_request_status.py
--rw-r--r--   0        0        0     1093 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task_response.py
--rw-r--r--   0        0        0      173 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task_status.py
--rw-r--r--   0        0        0      517 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/task_status_enum.py
--rw-r--r--   0        0        0     1531 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/tasks_list_request_expand.py
--rw-r--r--   0        0        0     1563 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
--rw-r--r--   0        0        0     1894 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/user.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/crm/types/webhook_receiver.py
--rw-r--r--   0        0        0     4324 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/__init__.py
--rw-r--r--   0        0        0     6830 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/client.py
--rw-r--r--   0        0        0      784 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2672 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2510 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/drives/__init__.py
--rw-r--r--   0        0        0     9456 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/drives/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/files/__init__.py
--rw-r--r--   0        0        0    18009 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/files/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/folders/__init__.py
--rw-r--r--   0        0        0    16547 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/folders/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3088 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2857 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/groups/__init__.py
--rw-r--r--   0        0        0     9050 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/issues/__init__.py
--rw-r--r--   0        0        0    10598 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8936 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10701 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7394 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2867 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8342 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3410 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/users/__init__.py
--rw-r--r--   0        0        0     9402 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5275 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0     5614 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/account_token.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/available_actions.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1912 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/drive.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/error_validation_problem.py
--rw-r--r--   0        0        0     2988 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/file.py
--rw-r--r--   0        0        0     2282 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/file_request.py
--rw-r--r--   0        0        0     1104 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/file_storage_file_response.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/file_storage_folder_response.py
--rw-r--r--   0        0        0     1511 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/files_list_request_expand.py
--rw-r--r--   0        0        0     1543 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/files_retrieve_request_expand.py
--rw-r--r--   0        0        0     2771 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/folder.py
--rw-r--r--   0        0        0     2061 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/folder_request.py
--rw-r--r--   0        0        0     1667 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/folders_list_request_expand.py
--rw-r--r--   0        0        0     1699 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/folders_retrieve_request_expand.py
--rw-r--r--   0        0        0     1931 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/group.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.706442 fern_merge-0.2.1/src/merge/resources/filestorage/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_drive_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_file_list.py
--rw-r--r--   0        0        0      884 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_folder_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_issue_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_user_list.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1970 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/user.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/filestorage/types/webhook_receiver.py
--rw-r--r--   0        0        0    10290 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2418 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2658 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2496 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0    15339 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0    10821 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     9072 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2161 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0    13612 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    30137 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0    14343 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2843 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0    11861 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0    10570 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8922 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10687 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0    11629 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7380 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     9094 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0    15544 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3396 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0    10785 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    22208 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0    15538 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5247 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    14549 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6788 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0      205 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_employment_status.py
--rw-r--r--   0        0        0      176 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_ethnicity.py
--rw-r--r--   0        0        0      164 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_gender.py
--rw-r--r--   0        0        0      193 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_marital_status.py
--rw-r--r--   0        0        0     2796 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6252 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0      212 2023-07-26 02:55:46.710442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_request_employment_status.py
--rw-r--r--   0        0        0      183 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_request_ethnicity.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_request_gender.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_request_marital_status.py
--rw-r--r--   0        0        0     1109 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18682 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      183 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_flsa_status.py
--rw-r--r--   0        0        0      187 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_pay_currency.py
--rw-r--r--   0        0        0      191 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_pay_frequency.py
--rw-r--r--   0        0        0      179 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_pay_period.py
--rw-r--r--   0        0        0      770 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/ignore_common_model_request_reason.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11870 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      168 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/location_country.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2811 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      175 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_run_run_state.py
--rw-r--r--   0        0        0      171 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3481 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3199 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      193 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request_status.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0      166 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request_units.py
--rw-r--r--   0        0        0     1106 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      186 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_status.py
--rw-r--r--   0        0        0     1146 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      159 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/time_off_units.py
--rw-r--r--   0        0        0      495 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     7030 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/__init__.py
--rw-r--r--   0        0        0     8338 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/client.py
--rw-r--r--   0        0        0      946 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2428 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.714442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2668 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/accounts/__init__.py
--rw-r--r--   0        0        0     9088 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/attachments/__init__.py
--rw-r--r--   0        0        0    17255 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2506 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/collections/__init__.py
--rw-r--r--   0        0        0    19212 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/collections/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/comments/__init__.py
--rw-r--r--   0        0        0    15547 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/comments/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/contacts/__init__.py
--rw-r--r--   0        0        0    10401 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2171 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3084 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/issues/__init__.py
--rw-r--r--   0        0        0    10590 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8932 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10697 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7390 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/projects/__init__.py
--rw-r--r--   0        0        0    13572 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/projects/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2863 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8330 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3406 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/tags/__init__.py
--rw-r--r--   0        0        0     8998 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/teams/__init__.py
--rw-r--r--   0        0        0     9020 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/tickets/__init__.py
--rw-r--r--   0        0        0    42221 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/tickets/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/users/__init__.py
--rw-r--r--   0        0        0    10850 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5267 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0     9623 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/__init__.py
--rw-r--r--   0        0        0      743 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/access_level_enum.py
--rw-r--r--   0        0        0     1879 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/account_token.py
--rw-r--r--   0        0        0     2201 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/attachment.py
--rw-r--r--   0        0        0     1716 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/attachment_request.py
--rw-r--r--   0        0        0     1245 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/available_actions.py
--rw-r--r--   0        0        0     1391 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/category_enum.py
--rw-r--r--   0        0        0     2535 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collection.py
--rw-r--r--   0        0        0      187 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collection_access_level.py
--rw-r--r--   0        0        0      199 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collection_collection_type.py
--rw-r--r--   0        0        0      536 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collection_type_enum.py
--rw-r--r--   0        0        0      527 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
--rw-r--r--   0        0        0      727 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
--rw-r--r--   0        0        0     2161 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/comment.py
--rw-r--r--   0        0        0     1693 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/comment_request.py
--rw-r--r--   0        0        0     1105 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/comment_response.py
--rw-r--r--   0        0        0     1435 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/comments_list_request_expand.py
--rw-r--r--   0        0        0     1467 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
--rw-r--r--   0        0        0      997 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/condition_type_enum.py
--rw-r--r--   0        0        0     2024 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/contact.py
--rw-r--r--   0        0        0      870 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/field_type_enum.py
--rw-r--r--   0        0        0     1323 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/item_type_enum.py
--rw-r--r--   0        0        0      835 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_account_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      900 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_collection_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_comment_list.py
--rw-r--r--   0        0        0      921 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_contact_list.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_issue_list.py
--rw-r--r--   0        0        0      888 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_project_list.py
--rw-r--r--   0        0        0      926 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      901 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_tag_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_team_list.py
--rw-r--r--   0        0        0      884 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_ticket_list.py
--rw-r--r--   0        0        0      876 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_user_list.py
--rw-r--r--   0        0        0     3241 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/patched_ticket_request.py
--rw-r--r--   0        0        0      184 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
--rw-r--r--   0        0        0      195 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/patched_ticket_request_status.py
--rw-r--r--   0        0        0      843 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/priority_enum.py
--rw-r--r--   0        0        0     1704 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/project.py
--rw-r--r--   0        0        0      715 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field_class.py
--rw-r--r--   0        0        0      825 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1559 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tag.py
--rw-r--r--   0        0        0     1705 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/team.py
--rw-r--r--   0        0        0     3778 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket.py
--rw-r--r--   0        0        0      170 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_priority.py
--rw-r--r--   0        0        0     3258 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_request.py
--rw-r--r--   0        0        0      177 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_request_priority.py
--rw-r--r--   0        0        0      188 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_request_status.py
--rw-r--r--   0        0        0     1101 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_response.py
--rw-r--r--   0        0        0      181 2023-07-26 02:55:46.718442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_status.py
--rw-r--r--   0        0        0      926 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_status_enum.py
--rw-r--r--   0        0        0     1126 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py
--rw-r--r--   0        0        0      743 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
--rw-r--r--   0        0        0    37875 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py
--rw-r--r--   0        0        0      810 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py
--rw-r--r--   0        0        0     1635 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
--rw-r--r--   0        0        0     1659 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      845 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_status.py
--rw-r--r--   0        0        0    38387 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
--rw-r--r--   0        0        0     1667 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1691 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1949 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/user.py
--rw-r--r--   0        0        0      683 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/users_list_request_expand.py
--rw-r--r--   0        0        0      699 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-26 02:55:46.722442 fern_merge-0.2.1/src/merge/resources/ticketing/types/webhook_receiver.py
--rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 fern_merge-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4149 2023-07-26 16:23:52.293848 fern_merge-0.2.2/README.md
+-rw-r--r--   0        0        0      388 2023-07-26 16:23:52.293848 fern_merge-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/__init__.py
+-rw-r--r--   0        0        0     2830 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/client.py
+-rw-r--r--   0        0        0      519 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1482 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      201 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/py.typed
+-rw-r--r--   0        0        0      206 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0    12630 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/__init__.py
+-rw-r--r--   0        0        0    12026 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/client.py
+-rw-r--r--   0        0        0     1410 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2430 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2670 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    18250 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/addresses/__init__.py
+-rw-r--r--   0        0        0     4508 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/addresses/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    14669 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2508 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/balance_sheets/__init__.py
+-rw-r--r--   0        0        0    10935 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/balance_sheets/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
+-rw-r--r--   0        0        0    11063 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/cash_flow_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/company_info/__init__.py
+-rw-r--r--   0        0        0    10594 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/company_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    17956 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/credit_notes/__init__.py
+-rw-r--r--   0        0        0    14854 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/credit_notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2173 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/expenses/__init__.py
+-rw-r--r--   0        0        0    16615 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/expenses/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3086 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/income_statements/__init__.py
+-rw-r--r--   0        0        0    11009 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/income_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/invoices/__init__.py
+-rw-r--r--   0        0        0    20202 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/invoices/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10594 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/items/__init__.py
+-rw-r--r--   0        0        0    13155 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/items/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/journal_entries/__init__.py
+-rw-r--r--   0        0        0    16931 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/journal_entries/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8934 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10699 2023-07-26 16:23:52.293848 fern_merge-0.2.2/src/merge/resources/accounting/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7392 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/payments/__init__.py
+-rw-r--r--   0        0        0    17415 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/payments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/phone_numbers/__init__.py
+-rw-r--r--   0        0        0     3317 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/phone_numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/purchase_orders/__init__.py
+-rw-r--r--   0        0        0    19258 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/purchase_orders/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2865 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8336 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3408 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/tax_rates/__init__.py
+-rw-r--r--   0        0        0    10815 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/tax_rates/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/tracking_categories/__init__.py
+-rw-r--r--   0        0        0    13405 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/tracking_categories/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    12082 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/transactions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/vendor_credits/__init__.py
+-rw-r--r--   0        0        0    12106 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/vendor_credits/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5271 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    17717 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/__init__.py
+-rw-r--r--   0        0        0    17393 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account.py
+-rw-r--r--   0        0        0      195 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_classification.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_currency.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_integration.py
+-rw-r--r--   0        0        0    16986 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_request.py
+-rw-r--r--   0        0        0      202 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_request_classification.py
+-rw-r--r--   0        0        0      178 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_request_currency.py
+-rw-r--r--   0        0        0      192 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_response.py
+-rw-r--r--   0        0        0      185 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_status.py
+-rw-r--r--   0        0        0      758 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_status_enum.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/account_token.py
+-rw-r--r--   0        0        0     1935 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment.py
+-rw-r--r--   0        0        0     1462 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment_request.py
+-rw-r--r--   0        0        0     1158 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment_response.py
+-rw-r--r--   0        0        0     1344 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_phone_number.py
+-rw-r--r--   0        0        0     1346 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_phone_number_request.py
+-rw-r--r--   0        0        0      819 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
+-rw-r--r--   0        0        0      831 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      847 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    11090 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/address.py
+-rw-r--r--   0        0        0      167 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/address_country.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/address_type.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/address_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/available_actions.py
+-rw-r--r--   0        0        0    16903 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/balance_sheet.py
+-rw-r--r--   0        0        0      176 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/balance_sheet_currency.py
+-rw-r--r--   0        0        0    17216 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/cash_flow_statement.py
+-rw-r--r--   0        0        0      181 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/cash_flow_statement_currency.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/category_enum.py
+-rw-r--r--   0        0        0      560 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/category_type_enum.py
+-rw-r--r--   0        0        0     1103 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/classification_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0    16863 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/company_info.py
+-rw-r--r--   0        0        0      175 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/company_info_currency.py
+-rw-r--r--   0        0        0      827 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/company_info_list_request_expand.py
+-rw-r--r--   0        0        0      843 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/condition_type_enum.py
+-rw-r--r--   0        0        0     3027 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contact.py
+-rw-r--r--   0        0        0     2478 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contact_request.py
+-rw-r--r--   0        0        0      182 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contact_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contact_response.py
+-rw-r--r--   0        0        0      175 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contact_status.py
+-rw-r--r--   0        0        0     1675 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contacts_list_request_expand.py
+-rw-r--r--   0        0        0     1707 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
+-rw-r--r--   0        0        0    35178 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/country_enum.py
+-rw-r--r--   0        0        0    17747 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note.py
+-rw-r--r--   0        0        0      174 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_currency.py
+-rw-r--r--   0        0        0     2275 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_line_item.py
+-rw-r--r--   0        0        0      198 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_status.py
+-rw-r--r--   0        0        0      784 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_status_enum.py
+-rw-r--r--   0        0        0     1859 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
+-rw-r--r--   0        0        0      731 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
+-rw-r--r--   0        0        0      743 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1891 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      747 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      759 2023-07-26 16:23:52.297849 fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    47961 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/currency_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/error_validation_problem.py
+-rw-r--r--   0        0        0    16980 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_currency.py
+-rw-r--r--   0        0        0     2074 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_line.py
+-rw-r--r--   0        0        0     2076 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_line_request.py
+-rw-r--r--   0        0        0    16445 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expense_response.py
+-rw-r--r--   0        0        0     3715 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expenses_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17240 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/income_statement.py
+-rw-r--r--   0        0        0      179 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/income_statement_currency.py
+-rw-r--r--   0        0        0    18003 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_currency.py
+-rw-r--r--   0        0        0    16460 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item.py
+-rw-r--r--   0        0        0      179 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item_currency.py
+-rw-r--r--   0        0        0    16389 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0      186 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
+-rw-r--r--   0        0        0    17620 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_request_currency.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_request_type.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_response.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_type.py
+-rw-r--r--   0        0        0      709 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_type_enum.py
+-rw-r--r--   0        0        0     8275 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_list_request_expand.py
+-rw-r--r--   0        0        0      622 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_list_request_type.py
+-rw-r--r--   0        0        0     8403 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     2624 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/item.py
+-rw-r--r--   0        0        0      172 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/item_status.py
+-rw-r--r--   0        0        0     1791 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/items_list_request_expand.py
+-rw-r--r--   0        0        0     1823 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/items_retrieve_request_expand.py
+-rw-r--r--   0        0        0     3771 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
+-rw-r--r--   0        0        0     3835 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17164 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry.py
+-rw-r--r--   0        0        0      176 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_currency.py
+-rw-r--r--   0        0        0      197 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_posting_status.py
+-rw-r--r--   0        0        0    16526 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_request.py
+-rw-r--r--   0        0        0      183 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_request_currency.py
+-rw-r--r--   0        0        0      204 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
+-rw-r--r--   0        0        0     1126 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_response.py
+-rw-r--r--   0        0        0     1790 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_line.py
+-rw-r--r--   0        0        0     1792 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/journal_line_request.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_account_list.py
+-rw-r--r--   0        0        0      941 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
+-rw-r--r--   0        0        0      905 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_company_info_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_credit_note_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_expense_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_income_statement_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_invoice_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_item_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_journal_entry_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_payment_list.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_purchase_order_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      889 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_tax_rate_list.py
+-rw-r--r--   0        0        0      925 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_tracking_category_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_transaction_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
+-rw-r--r--   0        0        0    16832 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payment.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payment_currency.py
+-rw-r--r--   0        0        0    16241 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payment_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payment_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payment_response.py
+-rw-r--r--   0        0        0     3715 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payments_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      554 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/posting_status_enum.py
+-rw-r--r--   0        0        0    17816 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_currency.py
+-rw-r--r--   0        0        0    16830 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item.py
+-rw-r--r--   0        0        0      185 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
+-rw-r--r--   0        0        0    16854 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item_request.py
+-rw-r--r--   0        0        0      192 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
+-rw-r--r--   0        0        0    17041 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_request.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_request_currency.py
+-rw-r--r--   0        0        0      217 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_request_status.py
+-rw-r--r--   0        0        0     1130 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_response.py
+-rw-r--r--   0        0        0      210 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_status.py
+-rw-r--r--   0        0        0     1154 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_status_enum.py
+-rw-r--r--   0        0        0     9043 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
+-rw-r--r--   0        0        0     9171 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/remote_response.py
+-rw-r--r--   0        0        0     1649 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/report_item.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0      542 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/status_7_d_1_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2002 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/tax_rate.py
+-rw-r--r--   0        0        0     2481 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/tracking_category.py
+-rw-r--r--   0        0        0      197 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/tracking_category_category_type.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/tracking_category_status.py
+-rw-r--r--   0        0        0    17229 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transaction.py
+-rw-r--r--   0        0        0      175 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transaction_currency.py
+-rw-r--r--   0        0        0    16685 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transaction_line_item.py
+-rw-r--r--   0        0        0      183 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transaction_line_item_currency.py
+-rw-r--r--   0        0        0     3899 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transactions_list_request_expand.py
+-rw-r--r--   0        0        0     3963 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.301849 fern_merge-0.2.2/src/merge/resources/accounting/types/validation_problem_source.py
+-rw-r--r--   0        0        0    16901 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credit.py
+-rw-r--r--   0        0        0      176 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credit_currency.py
+-rw-r--r--   0        0        0     1999 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credit_line.py
+-rw-r--r--   0        0        0     3675 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
+-rw-r--r--   0        0        0     3739 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/accounting/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9656 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2656 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    18450 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    22753 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    18326 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    25052 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     9128 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0    13425 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3072 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    19472 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10566 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0    10955 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0    14939 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8920 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10685 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0    13609 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     9042 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2851 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     9178 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0    14473 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3394 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     6731 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0    11995 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5243 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-26 16:23:52.305848 fern_merge-0.2.2/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9538 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/__init__.py
+-rw-r--r--   0        0        0     9931 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/client.py
+-rw-r--r--   0        0        0     1144 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2656 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    25993 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/association_types/__init__.py
+-rw-r--r--   0        0        0    17340 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/association_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/associations/__init__.py
+-rw-r--r--   0        0        0    12477 2023-07-26 16:23:52.309848 fern_merge-0.2.2/src/merge/resources/crm/resources/associations/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    28327 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/custom_object_classes/__init__.py
+-rw-r--r--   0        0        0    13387 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/custom_object_classes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/custom_objects/__init__.py
+-rw-r--r--   0        0        0    22608 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/custom_objects/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/engagement_types/__init__.py
+-rw-r--r--   0        0        0    15005 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/engagement_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/engagements/__init__.py
+-rw-r--r--   0        0        0    25867 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/engagements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3072 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10566 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/leads/__init__.py
+-rw-r--r--   0        0        0    22118 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/leads/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8920 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10685 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/notes/__init__.py
+-rw-r--r--   0        0        0    22396 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/opportunities/__init__.py
+-rw-r--r--   0        0        0    30544 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/opportunities/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2851 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/stages/__init__.py
+-rw-r--r--   0        0        0    14779 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3394 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/tasks/__init__.py
+-rw-r--r--   0        0        0    25417 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/tasks/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/users/__init__.py
+-rw-r--r--   0        0        0    17206 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5243 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13264 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/__init__.py
+-rw-r--r--   0        0        0     2708 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_integration.py
+-rw-r--r--   0        0        0     1916 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_request.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/account_token.py
+-rw-r--r--   0        0        0      719 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/activity_type_enum.py
+-rw-r--r--   0        0        0    10978 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_address_type.py
+-rw-r--r--   0        0        0      167 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_country.py
+-rw-r--r--   0        0        0    11024 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_request.py
+-rw-r--r--   0        0        0      191 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_request_address_type.py
+-rw-r--r--   0        0        0      174 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_request_country.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/address_type_enum.py
+-rw-r--r--   0        0        0     1226 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/association.py
+-rw-r--r--   0        0        0      955 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/association_sub_type.py
+-rw-r--r--   0        0        0     1663 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/association_type.py
+-rw-r--r--   0        0        0      191 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/association_type_cardinality.py
+-rw-r--r--   0        0        0     1335 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/association_type_request_request.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/available_actions.py
+-rw-r--r--   0        0        0     1033 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/cardinality_enum.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/contact.py
+-rw-r--r--   0        0        0     1944 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/contact_request.py
+-rw-r--r--   0        0        0    35178 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/country_enum.py
+-rw-r--r--   0        0        0     1108 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/crm_account_response.py
+-rw-r--r--   0        0        0     1141 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/crm_association_type_response.py
+-rw-r--r--   0        0        0     1108 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/crm_contact_response.py
+-rw-r--r--   0        0        0     1129 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/crm_custom_object_response.py
+-rw-r--r--   0        0        0     1399 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/custom_object.py
+-rw-r--r--   0        0        0     1520 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/custom_object_class.py
+-rw-r--r--   0        0        0      782 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/custom_object_request.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      549 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/direction_enum.py
+-rw-r--r--   0        0        0     1317 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/email_address.py
+-rw-r--r--   0        0        0     1319 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/email_address_request.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/encoding_enum.py
+-rw-r--r--   0        0        0     2645 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement.py
+-rw-r--r--   0        0        0      178 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_direction.py
+-rw-r--r--   0        0        0     2216 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_request.py
+-rw-r--r--   0        0        0      185 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_request_direction.py
+-rw-r--r--   0        0        0     1117 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_response.py
+-rw-r--r--   0        0        0     1866 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_type.py
+-rw-r--r--   0        0        0      195 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagement_type_activity_type.py
+-rw-r--r--   0        0        0     3563 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagements_list_request_expand.py
+-rw-r--r--   0        0        0     3627 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/field_type_enum.py
+-rw-r--r--   0        0        0      999 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/ignore_common_model_request.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/item_type_enum.py
+-rw-r--r--   0        0        0     2863 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/lead.py
+-rw-r--r--   0        0        0     2369 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/lead_request.py
+-rw-r--r--   0        0        0     1093 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/lead_response.py
+-rw-r--r--   0        0        0     1851 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/leads_list_request_expand.py
+-rw-r--r--   0        0        0     1883 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/leads_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.313849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2150 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/note.py
+-rw-r--r--   0        0        0     1590 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/note_request.py
+-rw-r--r--   0        0        0     1093 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/note_response.py
+-rw-r--r--   0        0        0     3267 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/notes_list_request_expand.py
+-rw-r--r--   0        0        0     3331 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      925 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/object_class_description_request.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/operator_schema.py
+-rw-r--r--   0        0        0     1475 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_list_request_expand.py
+-rw-r--r--   0        0        0      665 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_list_request_status.py
+-rw-r--r--   0        0        0     1507 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2685 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity.py
+-rw-r--r--   0        0        0     2243 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_request.py
+-rw-r--r--   0        0        0      208 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_request_status.py
+-rw-r--r--   0        0        0     1121 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_response.py
+-rw-r--r--   0        0        0      201 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_status.py
+-rw-r--r--   0        0        0      704 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_status_enum.py
+-rw-r--r--   0        0        0      893 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/origin_type_enum.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_account_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_association_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_association_type_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_custom_object_class_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_custom_object_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_engagement_list.py
+-rw-r--r--   0        0        0      917 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_engagement_type_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_lead_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_note_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_opportunity_list.py
+-rw-r--r--   0        0        0      926 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_stage_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_task_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/paginated_user_list.py
+-rw-r--r--   0        0        0     1923 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_account_request.py
+-rw-r--r--   0        0        0     1951 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_contact_request.py
+-rw-r--r--   0        0        0     2245 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_engagement_request.py
+-rw-r--r--   0        0        0      192 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_engagement_request_direction.py
+-rw-r--r--   0        0        0     2272 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_opportunity_request.py
+-rw-r--r--   0        0        0      215 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_opportunity_request_status.py
+-rw-r--r--   0        0        0     2029 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_task_request.py
+-rw-r--r--   0        0        0      187 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/patched_task_request_status.py
+-rw-r--r--   0        0        0     1307 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/phone_number.py
+-rw-r--r--   0        0        0     1309 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/phone_number_request.py
+-rw-r--r--   0        0        0      814 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class.py
+-rw-r--r--   0        0        0     1722 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
+-rw-r--r--   0        0        0      213 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
+-rw-r--r--   0        0        0      205 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
+-rw-r--r--   0        0        0      911 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
+-rw-r--r--   0        0        0      825 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1694 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/stage.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2429 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task.py
+-rw-r--r--   0        0        0     2000 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task_request.py
+-rw-r--r--   0        0        0      180 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task_request_status.py
+-rw-r--r--   0        0        0     1093 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task_response.py
+-rw-r--r--   0        0        0      173 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task_status.py
+-rw-r--r--   0        0        0      517 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/task_status_enum.py
+-rw-r--r--   0        0        0     1531 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/tasks_list_request_expand.py
+-rw-r--r--   0        0        0     1563 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1894 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/user.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/crm/types/webhook_receiver.py
+-rw-r--r--   0        0        0     4324 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/__init__.py
+-rw-r--r--   0        0        0     6830 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/client.py
+-rw-r--r--   0        0        0      784 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2672 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2510 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/drives/__init__.py
+-rw-r--r--   0        0        0     9456 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/drives/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/files/__init__.py
+-rw-r--r--   0        0        0    18009 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/files/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/folders/__init__.py
+-rw-r--r--   0        0        0    16547 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/folders/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3088 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/groups/__init__.py
+-rw-r--r--   0        0        0     9050 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10598 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8936 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10701 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7394 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2867 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8342 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3410 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/users/__init__.py
+-rw-r--r--   0        0        0     9402 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5275 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0     5614 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/account_token.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/available_actions.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1912 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/drive.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.317849 fern_merge-0.2.2/src/merge/resources/filestorage/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2988 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/file.py
+-rw-r--r--   0        0        0     2282 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/file_request.py
+-rw-r--r--   0        0        0     1104 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/file_storage_file_response.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/file_storage_folder_response.py
+-rw-r--r--   0        0        0     1511 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/files_list_request_expand.py
+-rw-r--r--   0        0        0     1543 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/files_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2771 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/folder.py
+-rw-r--r--   0        0        0     2061 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/folder_request.py
+-rw-r--r--   0        0        0     1667 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/folders_list_request_expand.py
+-rw-r--r--   0        0        0     1699 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/folders_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1931 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/group.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_drive_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_file_list.py
+-rw-r--r--   0        0        0      884 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_folder_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_user_list.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1970 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/user.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/filestorage/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10290 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2418 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2658 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2496 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0    15339 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0    10821 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     9072 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2161 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0    13612 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    30137 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0    14343 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0    11861 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10570 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8922 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10687 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0    11629 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7380 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     9094 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0    15544 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3396 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0    10785 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    22208 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0    15538 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5247 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14549 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.321848 fern_merge-0.2.2/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/ignore_common_model_request_reason.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-26 16:23:52.325848 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     7030 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/__init__.py
+-rw-r--r--   0        0        0     8338 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/client.py
+-rw-r--r--   0        0        0      946 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2428 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2668 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/accounts/__init__.py
+-rw-r--r--   0        0        0     9088 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    17255 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2506 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/collections/__init__.py
+-rw-r--r--   0        0        0    19212 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/collections/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/comments/__init__.py
+-rw-r--r--   0        0        0    15547 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/comments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    10401 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3084 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10590 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8932 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10697 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7390 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/projects/__init__.py
+-rw-r--r--   0        0        0    13572 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/projects/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2863 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8330 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3406 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/tags/__init__.py
+-rw-r--r--   0        0        0     8998 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/teams/__init__.py
+-rw-r--r--   0        0        0     9020 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/tickets/__init__.py
+-rw-r--r--   0        0        0    42221 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/tickets/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/users/__init__.py
+-rw-r--r--   0        0        0    10850 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5267 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0     9623 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/access_level_enum.py
+-rw-r--r--   0        0        0     1879 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/account_token.py
+-rw-r--r--   0        0        0     2201 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/attachment.py
+-rw-r--r--   0        0        0     1716 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/attachment_request.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/available_actions.py
+-rw-r--r--   0        0        0     1391 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/category_enum.py
+-rw-r--r--   0        0        0     2535 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collection.py
+-rw-r--r--   0        0        0      187 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collection_access_level.py
+-rw-r--r--   0        0        0      199 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collection_collection_type.py
+-rw-r--r--   0        0        0      536 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collection_type_enum.py
+-rw-r--r--   0        0        0      527 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
+-rw-r--r--   0        0        0      727 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
+-rw-r--r--   0        0        0     2161 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/comment.py
+-rw-r--r--   0        0        0     1693 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/comment_request.py
+-rw-r--r--   0        0        0     1105 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/comment_response.py
+-rw-r--r--   0        0        0     1435 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/comments_list_request_expand.py
+-rw-r--r--   0        0        0     1467 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      997 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2024 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/contact.py
+-rw-r--r--   0        0        0      870 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/field_type_enum.py
+-rw-r--r--   0        0        0     1323 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/item_type_enum.py
+-rw-r--r--   0        0        0      835 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_account_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_collection_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_comment_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_project_list.py
+-rw-r--r--   0        0        0      926 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_tag_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_team_list.py
+-rw-r--r--   0        0        0      884 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_ticket_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_user_list.py
+-rw-r--r--   0        0        0     3241 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/patched_ticket_request.py
+-rw-r--r--   0        0        0      184 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
+-rw-r--r--   0        0        0      195 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/patched_ticket_request_status.py
+-rw-r--r--   0        0        0      843 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/priority_enum.py
+-rw-r--r--   0        0        0     1704 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/project.py
+-rw-r--r--   0        0        0      715 2023-07-26 16:23:52.329849 fern_merge-0.2.2/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field_class.py
+-rw-r--r--   0        0        0      825 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1559 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tag.py
+-rw-r--r--   0        0        0     1705 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/team.py
+-rw-r--r--   0        0        0     3778 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket.py
+-rw-r--r--   0        0        0      170 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_priority.py
+-rw-r--r--   0        0        0     3258 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_request.py
+-rw-r--r--   0        0        0      177 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_request_priority.py
+-rw-r--r--   0        0        0      188 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_request_status.py
+-rw-r--r--   0        0        0     1101 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_response.py
+-rw-r--r--   0        0        0      181 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_status.py
+-rw-r--r--   0        0        0      926 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_status_enum.py
+-rw-r--r--   0        0        0     1126 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/ticketing_attachment_response.py
+-rw-r--r--   0        0        0      743 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
+-rw-r--r--   0        0        0    37875 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_expand.py
+-rw-r--r--   0        0        0      810 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_priority.py
+-rw-r--r--   0        0        0     1635 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1659 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      845 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_status.py
+-rw-r--r--   0        0        0    38387 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1667 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1691 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1949 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/user.py
+-rw-r--r--   0        0        0      683 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/users_list_request_expand.py
+-rw-r--r--   0        0        0      699 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 16:23:52.333849 fern_merge-0.2.2/src/merge/resources/ticketing/types/webhook_receiver.py
+-rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 fern_merge-0.2.2/PKG-INFO
```

### Comparing `fern_merge-0.2.1/README.md` & `fern_merge-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/client.py` & `fern_merge-0.2.2/src/merge/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         timeout: typing.Optional[float] = 60
     ):
         self._environment = environment
         self._client_wrapper = SyncClientWrapper(
             account_token=account_token, token=token, httpx_client=httpx.Client(timeout=timeout)
         )
         self.filestorage = FilestorageClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.crm = CrmClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.hris = HrisClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ats = AtsClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.crm = CrmClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ticketing = TicketingClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.hris = HrisClient(environment=environment, client_wrapper=self._client_wrapper)
         self.accounting = AccountingClient(environment=environment, client_wrapper=self._client_wrapper)
 
 
 class AsyncMerge:
     def __init__(
         self,
         *,
@@ -45,12 +45,12 @@
         timeout: typing.Optional[float] = 60
     ):
         self._environment = environment
         self._client_wrapper = AsyncClientWrapper(
             account_token=account_token, token=token, httpx_client=httpx.AsyncClient(timeout=timeout)
         )
         self.filestorage = AsyncFilestorageClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.crm = AsyncCrmClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.hris = AsyncHrisClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ats = AsyncAtsClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.crm = AsyncCrmClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ticketing = AsyncTicketingClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.hris = AsyncHrisClient(environment=environment, client_wrapper=self._client_wrapper)
         self.accounting = AsyncAccountingClient(environment=environment, client_wrapper=self._client_wrapper)
```

### Comparing `fern_merge-0.2.1/src/merge/core/__init__.py` & `fern_merge-0.2.2/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/core/client_wrapper.py` & `fern_merge-0.2.2/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/core/datetime_utils.py` & `fern_merge-0.2.2/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/core/jsonable_encoder.py` & `fern_merge-0.2.2/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/__init__.py` & `fern_merge-0.2.2/src/merge/resources/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/addresses/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/addresses/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/attachments/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/balance_sheets/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/balance_sheets/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/cash_flow_statements/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/company_info/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/company_info/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/contacts/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/credit_notes/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/credit_notes/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/expenses/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/expenses/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/income_statements/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/income_statements/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/invoices/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/invoices/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/items/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/items/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/journal_entries/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/journal_entries/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/payments/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/payments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/phone_numbers/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/phone_numbers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/purchase_orders/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/purchase_orders/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/tax_rates/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/tax_rates/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/tracking_categories/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/tracking_categories/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/transactions/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/vendor_credits/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/vendor_credits/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/accounting/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_attachment_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_phone_number.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounting_phone_number_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounting_phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/address.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/address_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/balance_sheet.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/cash_flow_statement.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/category_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/category_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/classification_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/classification_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/company_info.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/company_info.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/company_info_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/company_info_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/contact.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/contact.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/contact_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/contact_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/contact_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/contacts_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/contacts_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/country_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_line_item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_line_item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_note_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_note_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/currency_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expense.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expense.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expense_line.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expense_line.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expense_line_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expense_line_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expense_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expense_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expense_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expense_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expenses_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expenses_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/income_statement.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/income_statement.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_line_item_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoice_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoice_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_list_request_type.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_list_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/items_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/items_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/items_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entries_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_entry_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_entry_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_line.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_line.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/journal_line_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/journal_line_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_account_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_balance_sheet_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_company_info_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_company_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_contact_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_credit_note_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_credit_note_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_expense_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_expense_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_income_statement_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_income_statement_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_invoice_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_invoice_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_item_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_item_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_journal_entry_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_payment_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_payment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_purchase_order_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_tax_rate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_tracking_category_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_transaction_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_transaction_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/paginated_vendor_credit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/payment.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/payment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/payment_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/payment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/payment_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/payment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/payments_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/payments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/payments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/posting_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/posting_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_line_item_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_request.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_order_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_order_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/remote_data.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/report_item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/report_item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/status_7_d_1_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/status_7_d_1_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/tax_rate.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/tax_rate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/tracking_category.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/tracking_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/transaction.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/transaction_line_item.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/transaction_line_item.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/transactions_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/transactions_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credit.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credit_line.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credit_line.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/accounting/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/accounting/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/activities/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/applications/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/attachments/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/candidates/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/departments/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/eeocs/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/interviews/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/job_interview_stages/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/jobs/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/offers/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/offices/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/reject_reasons/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/scorecards/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/tags/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/users/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/access_role_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activity.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activity.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activity_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activity_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activity_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/activity_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/application.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/application_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/application_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/applications_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/attachment.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/attachment_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/attachment_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/attachment_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/candidate.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/candidate_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/candidate_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/candidates_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/department.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/disability_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/eeoc.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/email_address.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/email_address_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/email_address_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/gender_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/interviews_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/job.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/job_interview_stage.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/job_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/jobs_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/jobs_list_request_status.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/offer.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/offer_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/offers_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/office.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/overall_recommendation_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_activity_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_application_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_attachment_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_candidate_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_department_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_eeoc_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_job_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_offer_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_office_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_remote_user_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_scorecard_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/paginated_tag_list.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/patched_candidate_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/phone_number.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/phone_number_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/race_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/reason_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/reject_reason.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/remote_data.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/remote_user.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_response.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scorecard.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/tag.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/url.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/url_request.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/url_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/veteran_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/visibility_enum.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ats/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/__init__.py` & `fern_merge-0.2.2/src/merge/resources/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/association_types/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/association_types/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/associations/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/associations/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/contacts/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/custom_object_classes/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/custom_object_classes/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/custom_objects/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/custom_objects/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/engagement_types/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/engagement_types/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/engagements/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/engagements/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/leads/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/leads/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/notes/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/notes/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/opportunities/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/opportunities/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/stages/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/stages/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/tasks/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/tasks/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/users/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/crm/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/activity_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/address.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/address_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/address_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/association.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/association.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/association_sub_type.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/association_sub_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/association_type.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/association_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/association_type_request_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/association_type_request_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/cardinality_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/cardinality_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/contact.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/contact.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/contact_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/country_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/crm_account_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/crm_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/crm_association_type_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/crm_association_type_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/crm_contact_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/crm_contact_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/crm_custom_object_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/crm_custom_object_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/custom_object.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/custom_object.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/custom_object_class.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/custom_object_class.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/custom_object_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/custom_object_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/direction_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/direction_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/email_address.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/email_address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/email_address_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagement.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagement.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagement_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagement_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagement_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagement_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagement_type.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagement_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagements_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagements_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/engagements_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/field_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/field_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/ignore_common_model_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/ignore_common_model_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/item_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/item_schema.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/item_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/lead.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/lead.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/lead_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/lead_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/lead_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/lead_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/leads_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/leads_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/leads_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/note.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/note.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/note_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/note_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/note_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/note_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/notes_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/object_class_description_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/object_class_description_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_list_request_status.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunity.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunity.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/opportunity_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/opportunity_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/origin_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/origin_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_account_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_association_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_association_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_association_type_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_association_type_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_contact_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_custom_object_class_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_custom_object_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_custom_object_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_engagement_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_engagement_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_engagement_type_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_engagement_type_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_lead_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_lead_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_note_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_note_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_opportunity_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_opportunity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_stage_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_task_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/paginated_user_list.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/patched_account_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/patched_account_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/patched_contact_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/patched_contact_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/patched_engagement_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/patched_engagement_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/patched_opportunity_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/patched_opportunity_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/patched_task_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/phone_number.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/phone_number_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/reason_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_data.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_field.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_field_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/stage.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/task.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/task.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/task_request.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/task_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/task_response.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/task_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/task_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/task_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/tasks_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/tasks_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/tasks_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/user.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/crm/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/crm/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/__init__.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/drives/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/drives/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/files/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/files/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/folders/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/folders/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/groups/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/users/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/drive.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/drive.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/file.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/file.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/file_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/file_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/file_storage_file_response.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/file_storage_file_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/file_storage_folder_response.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/file_storage_folder_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/files_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/files_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/files_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/files_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/folder.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/folder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/folder_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/folder_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/folders_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/folders_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/folders_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/folders_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/group.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_drive_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_drive_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_file_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_file_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_folder_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_folder_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_group_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/paginated_user_list.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/user.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/filestorage/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/filestorage/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/__init__.py` & `fern_merge-0.2.2/src/merge/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/bank_info/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/benefits/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/companies/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/employees/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/employments/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/groups/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/locations/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/pay_groups/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/payroll_runs/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/teams/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/time_off/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/time_off_balances/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/account_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/bank_info.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/benefit.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/company.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/country_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/deduction.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/earning.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/earning_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_run.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employee_response.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employment.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employment_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employment_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_order_by.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/ethnicity_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/flsa_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/gender_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/group.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/group_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/location.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/location.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/marital_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_bank_info_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_benefit_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_company_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employee_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_employment_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_group_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_location_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_pay_group_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_team_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/paginated_time_off_list.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/pay_currency_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/pay_frequency_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/pay_group.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/pay_period_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_run.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/policy_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/reason_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/remote_data.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/request_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/run_state_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/run_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/tax.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/team.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_balance.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_list_request_status.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_request.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_response.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/time_off_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/hris/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_details/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/account_token/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/attachments/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/available_actions/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/collections/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/collections/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/comments/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/comments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/contacts/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/delete_account/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/force_resync/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/generate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/issues/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/link_token/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/linked_accounts/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/passthrough/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/projects/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/projects/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/regenerate_key/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/selective_sync/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/sync_status/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/tags/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/teams/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/tickets/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/tickets/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/users/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/__init__.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/access_level_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/access_level_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_integration.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/account_token.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/attachment.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/attachment_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/available_actions.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/categories_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/category_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/collection.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/collection.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/collection_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/collection_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/collections_list_request_collection_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/collections_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/comment.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/comment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/comment_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/comment_response.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/comments_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/comments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/condition_schema.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/condition_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/contact.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/contact.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/debug_mode_log.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/debug_model_log_summary.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/enabled_actions_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/encoding_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/error_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/field_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/field_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/issue.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/issue_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/item_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/item_schema.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/item_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/link_token.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_condition.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_condition_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_account_status.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/meta_response.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/method_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/model_operation.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/multipart_form_field_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/operator_schema.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_account_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_attachment_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_collection_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_collection_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_comment_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_comment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_contact_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_issue_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_project_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_project_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_tag_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_team_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_ticket_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_ticket_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/paginated_user_list.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/patched_ticket_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/patched_ticket_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/priority_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/priority_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/project.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/project.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/projects_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_data.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field_class.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_field_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_key.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/remote_response.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/request_format_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/response_type_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/sync_status.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/sync_status_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tag.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/team.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_request.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_response.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/ticket_status_enum.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/ticket_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/ticketing_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_priority.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_list_request_status.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/user.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/users_list_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/users_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/validation_problem_source.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/warning_validation_problem.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/src/merge/resources/ticketing/types/webhook_receiver.py` & `fern_merge-0.2.2/src/merge/resources/ticketing/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.2.1/PKG-INFO` & `fern_merge-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-merge
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

