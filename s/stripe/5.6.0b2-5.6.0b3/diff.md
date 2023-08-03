# Comparing `tmp/stripe-5.6.0b2.tar.gz` & `tmp/stripe-5.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe-5.6.0b2.tar", last modified: Fri Jul 28 17:20:06 2023, max compression
+gzip compressed data, was "stripe-5.6.0b3.tar", last modified: Thu Aug  3 20:54:00 2023, max compression
```

## Comparing `stripe-5.6.0b2.tar` & `stripe-5.6.0b3.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.417542 stripe-5.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 17:19:44.000000 stripe-5.6.0b2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 17:19:44.000000 stripe-5.6.0b2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    50861 2023-07-28 17:19:44.000000 stripe-5.6.0b2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-28 17:19:44.000000 stripe-5.6.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-28 17:19:44.000000 stripe-5.6.0b2/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 17:19:44.000000 stripe-5.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-28 17:20:06.417542 stripe-5.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-28 17:19:44.000000 stripe-5.6.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 17:19:44.000000 stripe-5.6.0b2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.377541 stripe-5.6.0b2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 17:19:44.000000 stripe-5.6.0b2/examples/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-28 17:19:44.000000 stripe-5.6.0b2/examples/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 17:19:44.000000 stripe-5.6.0b2/examples/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-28 17:19:44.000000 stripe-5.6.0b2/examples/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 17:19:44.000000 stripe-5.6.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 17:20:06.417542 stripe-5.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-28 17:19:44.000000 stripe-5.6.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.381541 stripe-5.6.0b2/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.389541 stripe-5.6.0b2/stripe/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/abstract/verify_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/account_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/application_fee_refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/apps/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/bank_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/billing_portal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/billing_portal/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/capability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/capital/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/capital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/capital/financing_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/capital/financing_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/capital/financing_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/cash_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/charge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/checkout/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/credit_note_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/customer_cash_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/customer_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/error_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/file_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/financial_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/account_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/account_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/inferred_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/financial_connections/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/funding_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/gift_cards/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/gift_cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/gift_cards/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/gift_cards/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.393541 stripe-5.6.0b2/stripe/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/identity/verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/identity/verification_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/invoice_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/card_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/card_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/issuing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/login_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/payment_method_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/quote_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/radar/early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/radar/value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/radar/value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/recipient_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/reporting/report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/reporting/report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/shipping_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/sigma/scheduled_query_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/subscription_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/terminal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/terminal/connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/terminal/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/terminal/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.397541 stripe-5.6.0b2/stripe/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/test_helpers/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.401541 stripe-5.6.0b2/stripe/api_resources/treasury/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/credit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/debit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/financial_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/inbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/outbound_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/outbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/received_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/received_debit.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/treasury/transaction_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_resources/webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.401541 stripe-5.6.0b2/stripe/data/
--rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/data/ca-certificates.crt
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/request_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-28 17:19:44.000000 stripe-5.6.0b2/stripe/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.381541 stripe-5.6.0b2/stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 17:20:06.000000 stripe-5.6.0b2/stripe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.401541 stripe-5.6.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.409541 stripe-5.6.0b2/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_test_helpers_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/abstract/test_updateable_api_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/billing_portal/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/billing_portal/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/checkout/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/identity/test_verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/identity/test_verification_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/test_cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/issuing/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/radar/test_early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/radar/test_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/radar/test_value_list_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/reporting/test_report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/reporting/test_report_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/sigma/test_scheduled_query_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:20:06.413541 stripe-5.6.0b2/tests/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/terminal/test_connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/terminal/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/terminal/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_application_fee_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_file_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_subscription_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/api_resources/test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/stripe_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)   116823 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_generated_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-28 17:19:44.000000 stripe-5.6.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 20:53:38.000000 stripe-5.6.0b3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 20:53:38.000000 stripe-5.6.0b3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-08-03 20:53:38.000000 stripe-5.6.0b3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 20:53:38.000000 stripe-5.6.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-03 20:53:38.000000 stripe-5.6.0b3/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 20:53:38.000000 stripe-5.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-03 20:54:00.802182 stripe-5.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-08-03 20:53:38.000000 stripe-5.6.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 20:53:38.000000 stripe-5.6.0b3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.762182 stripe-5.6.0b3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 20:53:38.000000 stripe-5.6.0b3/examples/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-03 20:53:38.000000 stripe-5.6.0b3/examples/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-03 20:53:38.000000 stripe-5.6.0b3/examples/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 20:53:38.000000 stripe-5.6.0b3/examples/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 20:53:38.000000 stripe-5.6.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 20:54:00.802182 stripe-5.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-03 20:53:38.000000 stripe-5.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.766182 stripe-5.6.0b3/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.774182 stripe-5.6.0b3/stripe/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/abstract/verify_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/account_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/application_fee_refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/apps/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/bank_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/billing_portal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/billing_portal/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/capability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/capital/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/capital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/capital/financing_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/capital/financing_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/capital/financing_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/cash_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/charge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/checkout/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/credit_note_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/customer_cash_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/customer_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/error_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/file_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/financial_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/account_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/account_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/inferred_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/financial_connections/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/funding_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/gift_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/gift_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/gift_cards/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/gift_cards/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/identity/verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/identity/verification_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/invoice_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.778182 stripe-5.6.0b3/stripe/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/card_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/card_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/issuing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/login_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/payment_method_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/quote_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/radar/early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/radar/value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/radar/value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/recipient_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/reporting/report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/reporting/report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/shipping_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/sigma/scheduled_query_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/subscription_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/terminal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/terminal/connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/terminal/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/terminal/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.782182 stripe-5.6.0b3/stripe/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/test_helpers/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.786182 stripe-5.6.0b3/stripe/api_resources/treasury/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/credit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/debit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/financial_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/inbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/outbound_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/outbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/received_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/received_debit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/treasury/transaction_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_resources/webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/api_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.786182 stripe-5.6.0b3/stripe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/data/ca-certificates.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/request_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-03 20:53:38.000000 stripe-5.6.0b3/stripe/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.766182 stripe-5.6.0b3/stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 20:54:00.000000 stripe-5.6.0b3/stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.786182 stripe-5.6.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.798182 stripe-5.6.0b3/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.798182 stripe-5.6.0b3/tests/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/abstract/test_updateable_api_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.798182 stripe-5.6.0b3/tests/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/billing_portal/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/billing_portal/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.798182 stripe-5.6.0b3/tests/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/checkout/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.798182 stripe-5.6.0b3/tests/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/identity/test_verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/identity/test_verification_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/tests/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/test_cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/issuing/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/tests/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/radar/test_early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/radar/test_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/radar/test_value_list_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/tests/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/reporting/test_report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/reporting/test_report_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/tests/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/sigma/test_scheduled_query_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:54:00.802182 stripe-5.6.0b3/tests/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/terminal/test_connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/terminal/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/terminal/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_application_fee_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_file_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_subscription_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/api_resources/test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/stripe_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116823 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_generated_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 20:53:38.000000 stripe-5.6.0b3/tox.ini
```

### Comparing `stripe-5.6.0b2/CHANGELOG.md` & `stripe-5.6.0b3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 5.6.0b3 - 2023-08-03
+* [#1004](https://github.com/stripe/stripe-python/pull/1004) Update generated code for beta
+  * Add support for `submit_card` test helper method on resource `Issuing.Card`
+* [#999](https://github.com/stripe/stripe-python/pull/999) Update generated code for beta
+
+* [#997](https://github.com/stripe/stripe-python/pull/997) Remove developer_message support
+
 ## 5.6.0b2 - 2023-07-28
 * [#995](https://github.com/stripe/stripe-python/pull/995) Update generated code for beta
   * Add support for new resource `Tax.Form`
   * Add support for `list`, `pdf`, and `retrieve` methods on resource `Form`
 * [#992](https://github.com/stripe/stripe-python/pull/992) Update generated code for beta
```

### Comparing `stripe-5.6.0b2/LICENSE` & `stripe-5.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/LONG_DESCRIPTION.rst` & `stripe-5.6.0b3/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/PKG-INFO` & `stripe-5.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.6.0b2
+Version: 5.6.0b3
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.6.0b2/README.md` & `stripe-5.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/examples/oauth.py` & `stripe-5.6.0b3/examples/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/examples/proxy.py` & `stripe-5.6.0b3/examples/proxy.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/examples/webhooks.py` & `stripe-5.6.0b3/examples/webhooks.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/setup.py` & `stripe-5.6.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/__init__.py` & `stripe-5.6.0b3/stripe/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_requestor.py` & `stripe-5.6.0b3/stripe/api_requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,15 @@
             err = self.specific_api_error(
                 rbody, rcode, resp, rheaders, error_data
             )
 
         raise err
 
     def specific_api_error(self, rbody, rcode, resp, rheaders, error_data):
-        message = error_data.get("message") or error_data.get(
-            "developer_message"
-        )
+        message = error_data.get("message")
 
         util.log_info(
             "Stripe API error received",
             error_code=error_data.get("code"),
             error_type=error_data.get("type"),
             error_message=message,
             error_param=error_data.get("param"),
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/__init__.py` & `stripe-5.6.0b3/stripe/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/__init__.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/createable_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/custom_method.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/deletable_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/listable_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/nested_resource_class_methods.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/searchable_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/singleton_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/test_helpers.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/test_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,22 @@
       class TestHelpers(APIResourceTestHelpers):
     """
 
     def __init__(self, resource):
         self.resource = resource
 
     @classmethod
+    def _static_request(cls, *args, **kwargs):
+        return cls._resource_cls._static_request(*args, **kwargs)
+
+    @classmethod
+    def _static_request_stream(cls, *args, **kwargs):
+        return cls._resource_cls._static_request_stream(*args, **kwargs)
+
+    @classmethod
     def class_url(cls):
         if cls == APIResourceTestHelpers:
             raise NotImplementedError(
                 "APIResourceTestHelpers is an abstract class.  You should perform "
                 "actions on its subclasses (e.g. Charge, Customer)"
             )
         # Namespaces are separated in object names with periods (.) and in URLs
@@ -44,24 +52,19 @@
 
         id = util.utf8(id)
         base = self.class_url()
         extn = quote_plus(id)
         return "%s/%s" % (base, extn)
 
 
+# TODO (next major)
 def test_helpers(cls):
     """
-    test_helpers decorator adds a test_helpers property and
-    wires the parent resource class to the nested TestHelpers class.
-
-    Should only be used on types that inherit from APIResource.
-
-    @test_helpers
-    class Foo(APIResource):
-      class TestHelpers(APIResourceTestHelpers):
+    The test_helpers decorator is deprecated and will be removed in a future version
+    of the library.
     """
 
     def test_helpers_getter(self):
         return self.TestHelpers(self)
 
     if not issubclass(cls, APIResource):
         raise ValueError(
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/abstract/updateable_api_resource.py` & `stripe-5.6.0b3/stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/account.py` & `stripe-5.6.0b3/stripe/api_resources/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/account_link.py` & `stripe-5.6.0b3/stripe/api_resources/account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/account_session.py` & `stripe-5.6.0b3/stripe/api_resources/account_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/apple_pay_domain.py` & `stripe-5.6.0b3/stripe/api_resources/apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/application_fee.py` & `stripe-5.6.0b3/stripe/api_resources/application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/application_fee_refund.py` & `stripe-5.6.0b3/stripe/api_resources/application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/apps/secret.py` & `stripe-5.6.0b3/stripe/api_resources/apps/secret.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/balance.py` & `stripe-5.6.0b3/stripe/api_resources/balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/balance_transaction.py` & `stripe-5.6.0b3/stripe/api_resources/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/bank_account.py` & `stripe-5.6.0b3/stripe/api_resources/bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/billing_portal/configuration.py` & `stripe-5.6.0b3/stripe/api_resources/billing_portal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/billing_portal/session.py` & `stripe-5.6.0b3/stripe/api_resources/billing_portal/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/capability.py` & `stripe-5.6.0b3/stripe/api_resources/capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/capital/financing_offer.py` & `stripe-5.6.0b3/stripe/api_resources/capital/financing_offer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/capital/financing_summary.py` & `stripe-5.6.0b3/stripe/api_resources/capital/financing_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/card.py` & `stripe-5.6.0b3/stripe/api_resources/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/cash_balance.py` & `stripe-5.6.0b3/stripe/api_resources/cash_balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/charge.py` & `stripe-5.6.0b3/stripe/api_resources/charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/checkout/session.py` & `stripe-5.6.0b3/stripe/api_resources/checkout/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/country_spec.py` & `stripe-5.6.0b3/stripe/api_resources/country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/coupon.py` & `stripe-5.6.0b3/stripe/api_resources/coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/credit_note.py` & `stripe-5.6.0b3/stripe/api_resources/credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/customer.py` & `stripe-5.6.0b3/stripe/api_resources/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import DeletableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import SearchableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
 from stripe.api_resources.abstract import nested_resource_class_methods
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 @nested_resource_class_methods(
     "balance_transaction",
     operations=["create", "retrieve", "update", "list"],
 )
 @nested_resource_class_methods(
     "cash_balance_transaction",
     operations=["retrieve", "list"],
@@ -249,7 +247,14 @@
                 "post",
                 "/v1/test_helpers/customers/{customer}/fund_cash_balance".format(
                     customer=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+Customer.TestHelpers._resource_cls = Customer
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/customer_balance_transaction.py` & `stripe-5.6.0b3/stripe/api_resources/customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/customer_cash_balance_transaction.py` & `stripe-5.6.0b3/stripe/api_resources/customer_cash_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/dispute.py` & `stripe-5.6.0b3/stripe/api_resources/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/ephemeral_key.py` & `stripe-5.6.0b3/stripe/api_resources/ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/error_object.py` & `stripe-5.6.0b3/stripe/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/event.py` & `stripe-5.6.0b3/stripe/api_resources/event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/exchange_rate.py` & `stripe-5.6.0b3/stripe/api_resources/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/file.py` & `stripe-5.6.0b3/stripe/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/file_link.py` & `stripe-5.6.0b3/stripe/api_resources/file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/financial_connections/__init__.py` & `stripe-5.6.0b3/stripe/api_resources/financial_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/financial_connections/account.py` & `stripe-5.6.0b3/stripe/api_resources/financial_connections/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/funding_instructions.py` & `stripe-5.6.0b3/stripe/api_resources/funding_instructions.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/gift_cards/card.py` & `stripe-5.6.0b3/stripe/api_resources/gift_cards/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/gift_cards/transaction.py` & `stripe-5.6.0b3/stripe/api_resources/gift_cards/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/identity/verification_report.py` & `stripe-5.6.0b3/stripe/api_resources/identity/verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/identity/verification_session.py` & `stripe-5.6.0b3/stripe/api_resources/identity/verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/invoice.py` & `stripe-5.6.0b3/stripe/api_resources/invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/invoice_item.py` & `stripe-5.6.0b3/stripe/api_resources/invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/__init__.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/authorization.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/card.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/outbound_payment.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,143 +2,149 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import UpdateableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
-class Card(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
+class OutboundPayment(CreateableAPIResource, ListableAPIResource):
     """
-    You can [create physical or virtual cards](https://stripe.com/docs/issuing/cards) that are issued to cardholders.
+    Use OutboundPayments to send funds to another party's external bank account or [FinancialAccount](https://stripe.com/docs/api#financial_accounts). To send money to an account belonging to the same user, use an [OutboundTransfer](https://stripe.com/docs/api#outbound_transfers).
+
+    Simulate OutboundPayment state changes with the `/v1/test_helpers/treasury/outbound_payments` endpoints. These methods can only be called on test mode objects.
     """
 
-    OBJECT_NAME = "issuing.card"
+    OBJECT_NAME = "treasury.outbound_payment"
+
+    @classmethod
+    def _cls_cancel(
+        cls,
+        id,
+        api_key=None,
+        stripe_version=None,
+        stripe_account=None,
+        **params
+    ):
+        return cls._static_request(
+            "post",
+            "/v1/treasury/outbound_payments/{id}/cancel".format(
+                id=util.sanitize_id(id)
+            ),
+            api_key=api_key,
+            stripe_version=stripe_version,
+            stripe_account=stripe_account,
+            params=params,
+        )
+
+    @util.class_method_variant("_cls_cancel")
+    def cancel(self, idempotency_key=None, **params):
+        return self._request(
+            "post",
+            "/v1/treasury/outbound_payments/{id}/cancel".format(
+                id=util.sanitize_id(self.get("id"))
+            ),
+            idempotency_key=idempotency_key,
+            params=params,
+        )
 
     class TestHelpers(APIResourceTestHelpers):
         @classmethod
-        def _cls_deliver_card(
+        def _cls_fail(
             cls,
-            card,
+            id,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/deliver".format(
-                    card=util.sanitize_id(card)
+                "/v1/test_helpers/treasury/outbound_payments/{id}/fail".format(
+                    id=util.sanitize_id(id)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_deliver_card")
-        def deliver_card(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_fail")
+        def fail(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/deliver".format(
-                    card=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/treasury/outbound_payments/{id}/fail".format(
+                    id=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
 
         @classmethod
-        def _cls_fail_card(
+        def _cls_post(
             cls,
-            card,
+            id,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/fail".format(
-                    card=util.sanitize_id(card)
+                "/v1/test_helpers/treasury/outbound_payments/{id}/post".format(
+                    id=util.sanitize_id(id)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_fail_card")
-        def fail_card(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_post")
+        def post(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/fail".format(
-                    card=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/treasury/outbound_payments/{id}/post".format(
+                    id=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
 
         @classmethod
-        def _cls_return_card(
+        def _cls_return_outbound_payment(
             cls,
-            card,
+            id,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/return".format(
-                    card=util.sanitize_id(card)
+                "/v1/test_helpers/treasury/outbound_payments/{id}/return".format(
+                    id=util.sanitize_id(id)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_return_card")
-        def return_card(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_return_outbound_payment")
+        def return_outbound_payment(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/return".format(
-                    card=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/treasury/outbound_payments/{id}/return".format(
+                    id=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
 
-        @classmethod
-        def _cls_ship_card(
-            cls,
-            card,
-            api_key=None,
-            stripe_version=None,
-            stripe_account=None,
-            **params
-        ):
-            return cls._static_request(
-                "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/ship".format(
-                    card=util.sanitize_id(card)
-                ),
-                api_key=api_key,
-                stripe_version=stripe_version,
-                stripe_account=stripe_account,
-                params=params,
-            )
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
 
-        @util.class_method_variant("_cls_ship_card")
-        def ship_card(self, idempotency_key=None, **params):
-            return self.resource._request(
-                "post",
-                "/v1/test_helpers/issuing/cards/{card}/shipping/ship".format(
-                    card=util.sanitize_id(self.resource.get("id"))
-                ),
-                idempotency_key=idempotency_key,
-                params=params,
-            )
+
+OutboundPayment.TestHelpers._resource_cls = OutboundPayment
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/card_design.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/card_design.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 class CardDesign(ListableAPIResource, UpdateableAPIResource):
     """
     A Card Design is a logical grouping of a Card Bundle, card logo, and carrier text that represents a product line.
     """
 
     OBJECT_NAME = "issuing.card_design"
 
@@ -75,7 +73,14 @@
                 "post",
                 "/v1/test_helpers/issuing/card_designs/{card_design}/status/deactivate".format(
                     card_design=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+CardDesign.TestHelpers._resource_cls = CardDesign
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/cardholder.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/dispute.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/issuing/transaction.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/list_object.py` & `stripe-5.6.0b3/stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/order.py` & `stripe-5.6.0b3/stripe/api_resources/order.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/payment_intent.py` & `stripe-5.6.0b3/stripe/api_resources/payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/payment_link.py` & `stripe-5.6.0b3/stripe/api_resources/payment_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/payment_method.py` & `stripe-5.6.0b3/stripe/api_resources/payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/payment_method_configuration.py` & `stripe-5.6.0b3/stripe/api_resources/payment_method_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/payout.py` & `stripe-5.6.0b3/stripe/api_resources/payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/person.py` & `stripe-5.6.0b3/stripe/api_resources/person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/plan.py` & `stripe-5.6.0b3/stripe/api_resources/plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/price.py` & `stripe-5.6.0b3/stripe/api_resources/price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/product.py` & `stripe-5.6.0b3/stripe/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/promotion_code.py` & `stripe-5.6.0b3/stripe/api_resources/promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/quote.py` & `stripe-5.6.0b3/stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/quote_phase.py` & `stripe-5.6.0b3/stripe/api_resources/quote_phase.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/radar/early_fraud_warning.py` & `stripe-5.6.0b3/stripe/api_resources/radar/early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/radar/value_list.py` & `stripe-5.6.0b3/stripe/api_resources/radar/value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/radar/value_list_item.py` & `stripe-5.6.0b3/stripe/api_resources/radar/value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/refund.py` & `stripe-5.6.0b3/stripe/api_resources/refund.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 class Refund(
     CreateableAPIResource, ListableAPIResource, UpdateableAPIResource
 ):
     """
     `Refund` objects allow you to refund a charge that has previously been created
     but not yet refunded. Funds will be refunded to the credit or debit card that
     was originally charged.
@@ -82,7 +80,14 @@
                 "post",
                 "/v1/test_helpers/refunds/{refund}/expire".format(
                     refund=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+Refund.TestHelpers._resource_cls = Refund
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/reporting/report_run.py` & `stripe-5.6.0b3/stripe/api_resources/reporting/report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/reporting/report_type.py` & `stripe-5.6.0b3/stripe/api_resources/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/reversal.py` & `stripe-5.6.0b3/stripe/api_resources/reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/review.py` & `stripe-5.6.0b3/stripe/api_resources/review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/search_result_object.py` & `stripe-5.6.0b3/stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/setup_attempt.py` & `stripe-5.6.0b3/stripe/api_resources/setup_attempt.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/setup_intent.py` & `stripe-5.6.0b3/stripe/api_resources/setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/shipping_rate.py` & `stripe-5.6.0b3/stripe/api_resources/shipping_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/sigma/scheduled_query_run.py` & `stripe-5.6.0b3/stripe/api_resources/sigma/scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/source.py` & `stripe-5.6.0b3/stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/source_transaction.py` & `stripe-5.6.0b3/stripe/api_resources/source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/subscription.py` & `stripe-5.6.0b3/stripe/api_resources/subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/subscription_item.py` & `stripe-5.6.0b3/stripe/api_resources/subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/subscription_schedule.py` & `stripe-5.6.0b3/stripe/api_resources/subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax/calculation.py` & `stripe-5.6.0b3/stripe/api_resources/tax/calculation.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax/form.py` & `stripe-5.6.0b3/stripe/api_resources/tax/form.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax/registration.py` & `stripe-5.6.0b3/stripe/api_resources/tax/registration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax/settings.py` & `stripe-5.6.0b3/stripe/api_resources/tax/settings.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax/transaction.py` & `stripe-5.6.0b3/stripe/api_resources/tax/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax_id.py` & `stripe-5.6.0b3/stripe/api_resources/tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/tax_rate.py` & `stripe-5.6.0b3/stripe/api_resources/tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/terminal/configuration.py` & `stripe-5.6.0b3/stripe/api_resources/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/terminal/location.py` & `stripe-5.6.0b3/stripe/api_resources/terminal/location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/terminal/reader.py` & `stripe-5.6.0b3/stripe/api_resources/terminal/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import DeletableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 class Reader(
     CreateableAPIResource,
     DeletableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
@@ -301,7 +299,14 @@
                 "post",
                 "/v1/test_helpers/terminal/readers/{reader}/present_payment_method".format(
                     reader=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+Reader.TestHelpers._resource_cls = Reader
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/test_helpers/test_clock.py` & `stripe-5.6.0b3/stripe/api_resources/test_helpers/test_clock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/token.py` & `stripe-5.6.0b3/stripe/api_resources/token.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/topup.py` & `stripe-5.6.0b3/stripe/api_resources/topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/transfer.py` & `stripe-5.6.0b3/stripe/api_resources/transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/__init__.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/credit_reversal.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/credit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/debit_reversal.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/debit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/financial_account.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/financial_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/inbound_transfer.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/inbound_transfer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 class InboundTransfer(CreateableAPIResource, ListableAPIResource):
     """
     Use [InboundTransfers](https://stripe.com/docs/treasury/moving-money/financial-accounts/into/inbound-transfers) to add funds to your [FinancialAccount](https://stripe.com/docs/api#financial_accounts) via a PaymentMethod that is owned by you. The funds will be transferred via an ACH debit.
     """
 
     OBJECT_NAME = "treasury.inbound_transfer"
 
@@ -137,7 +135,14 @@
                 "post",
                 "/v1/test_helpers/treasury/inbound_transfers/{id}/succeed".format(
                     id=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+InboundTransfer.TestHelpers._resource_cls = InboundTransfer
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/outbound_payment.py` & `stripe-5.6.0b3/stripe/api_resources/issuing/card.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,144 +2,179 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import test_helpers
+from stripe.api_resources.abstract import UpdateableAPIResource
 
 
-@test_helpers
-class OutboundPayment(CreateableAPIResource, ListableAPIResource):
+class Card(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     """
-    Use OutboundPayments to send funds to another party's external bank account or [FinancialAccount](https://stripe.com/docs/api#financial_accounts). To send money to an account belonging to the same user, use an [OutboundTransfer](https://stripe.com/docs/api#outbound_transfers).
-
-    Simulate OutboundPayment state changes with the `/v1/test_helpers/treasury/outbound_payments` endpoints. These methods can only be called on test mode objects.
+    You can [create physical or virtual cards](https://stripe.com/docs/issuing/cards) that are issued to cardholders.
     """
 
-    OBJECT_NAME = "treasury.outbound_payment"
-
-    @classmethod
-    def _cls_cancel(
-        cls,
-        id,
-        api_key=None,
-        stripe_version=None,
-        stripe_account=None,
-        **params
-    ):
-        return cls._static_request(
-            "post",
-            "/v1/treasury/outbound_payments/{id}/cancel".format(
-                id=util.sanitize_id(id)
-            ),
-            api_key=api_key,
-            stripe_version=stripe_version,
-            stripe_account=stripe_account,
-            params=params,
-        )
-
-    @util.class_method_variant("_cls_cancel")
-    def cancel(self, idempotency_key=None, **params):
-        return self._request(
-            "post",
-            "/v1/treasury/outbound_payments/{id}/cancel".format(
-                id=util.sanitize_id(self.get("id"))
-            ),
-            idempotency_key=idempotency_key,
-            params=params,
-        )
+    OBJECT_NAME = "issuing.card"
 
     class TestHelpers(APIResourceTestHelpers):
         @classmethod
-        def _cls_fail(
+        def _cls_deliver_card(
+            cls,
+            card,
+            api_key=None,
+            stripe_version=None,
+            stripe_account=None,
+            **params
+        ):
+            return cls._static_request(
+                "post",
+                "/v1/test_helpers/issuing/cards/{card}/shipping/deliver".format(
+                    card=util.sanitize_id(card)
+                ),
+                api_key=api_key,
+                stripe_version=stripe_version,
+                stripe_account=stripe_account,
+                params=params,
+            )
+
+        @util.class_method_variant("_cls_deliver_card")
+        def deliver_card(self, idempotency_key=None, **params):
+            return self.resource._request(
+                "post",
+                "/v1/test_helpers/issuing/cards/{card}/shipping/deliver".format(
+                    card=util.sanitize_id(self.resource.get("id"))
+                ),
+                idempotency_key=idempotency_key,
+                params=params,
+            )
+
+        @classmethod
+        def _cls_fail_card(
             cls,
-            id,
+            card,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/fail".format(
-                    id=util.sanitize_id(id)
+                "/v1/test_helpers/issuing/cards/{card}/shipping/fail".format(
+                    card=util.sanitize_id(card)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_fail")
-        def fail(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_fail_card")
+        def fail_card(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/fail".format(
-                    id=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/issuing/cards/{card}/shipping/fail".format(
+                    card=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
 
         @classmethod
-        def _cls_post(
+        def _cls_return_card(
             cls,
-            id,
+            card,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/post".format(
-                    id=util.sanitize_id(id)
+                "/v1/test_helpers/issuing/cards/{card}/shipping/return".format(
+                    card=util.sanitize_id(card)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_post")
-        def post(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_return_card")
+        def return_card(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/post".format(
-                    id=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/issuing/cards/{card}/shipping/return".format(
+                    card=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
 
         @classmethod
-        def _cls_return_outbound_payment(
+        def _cls_ship_card(
             cls,
-            id,
+            card,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/return".format(
-                    id=util.sanitize_id(id)
+                "/v1/test_helpers/issuing/cards/{card}/shipping/ship".format(
+                    card=util.sanitize_id(card)
                 ),
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
 
-        @util.class_method_variant("_cls_return_outbound_payment")
-        def return_outbound_payment(self, idempotency_key=None, **params):
+        @util.class_method_variant("_cls_ship_card")
+        def ship_card(self, idempotency_key=None, **params):
             return self.resource._request(
                 "post",
-                "/v1/test_helpers/treasury/outbound_payments/{id}/return".format(
-                    id=util.sanitize_id(self.resource.get("id"))
+                "/v1/test_helpers/issuing/cards/{card}/shipping/ship".format(
+                    card=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+        @classmethod
+        def _cls_submit_card(
+            cls,
+            card,
+            api_key=None,
+            stripe_version=None,
+            stripe_account=None,
+            **params
+        ):
+            return cls._static_request(
+                "post",
+                "/v1/test_helpers/issuing/cards/{card}/shipping/submit".format(
+                    card=util.sanitize_id(card)
+                ),
+                api_key=api_key,
+                stripe_version=stripe_version,
+                stripe_account=stripe_account,
+                params=params,
+            )
+
+        @util.class_method_variant("_cls_submit_card")
+        def submit_card(self, idempotency_key=None, **params):
+            return self.resource._request(
+                "post",
+                "/v1/test_helpers/issuing/cards/{card}/shipping/submit".format(
+                    card=util.sanitize_id(self.resource.get("id"))
+                ),
+                idempotency_key=idempotency_key,
+                params=params,
+            )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+Card.TestHelpers._resource_cls = Card
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/outbound_transfer.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/outbound_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
 class OutboundTransfer(CreateableAPIResource, ListableAPIResource):
     """
     Use OutboundTransfers to transfer funds from a [FinancialAccount](https://stripe.com/docs/api#financial_accounts) to a PaymentMethod belonging to the same entity. To send funds to a different party, use [OutboundPayments](https://stripe.com/docs/api#outbound_payments) instead. You can send funds over ACH rails or through a domestic wire transfer to a user's own external bank account.
 
     Simulate OutboundTransfer state changes with the `/v1/test_helpers/treasury/outbound_transfers` endpoints. These methods can only be called on test mode objects.
     """
 
@@ -139,7 +137,14 @@
                 "post",
                 "/v1/test_helpers/treasury/outbound_transfers/{outbound_transfer}/return".format(
                     outbound_transfer=util.sanitize_id(self.resource.get("id"))
                 ),
                 idempotency_key=idempotency_key,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+OutboundTransfer.TestHelpers._resource_cls = OutboundTransfer
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/received_credit.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/received_debit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # -*- coding: utf-8 -*-
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
-class ReceivedCredit(ListableAPIResource):
+class ReceivedDebit(ListableAPIResource):
     """
-    ReceivedCredits represent funds sent to a [FinancialAccount](https://stripe.com/docs/api#financial_accounts) (for example, via ACH or wire). These money movements are not initiated from the FinancialAccount.
+    ReceivedDebits represent funds pulled from a [FinancialAccount](https://stripe.com/docs/api#financial_accounts). These are not initiated from the FinancialAccount.
     """
 
-    OBJECT_NAME = "treasury.received_credit"
+    OBJECT_NAME = "treasury.received_debit"
 
     class TestHelpers(APIResourceTestHelpers):
         @classmethod
         def create(
             cls,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/treasury/received_credits",
+                "/v1/test_helpers/treasury/received_debits",
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+ReceivedDebit.TestHelpers._resource_cls = ReceivedDebit
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/received_debit.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/received_credit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # -*- coding: utf-8 -*-
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe.api_resources.abstract import APIResourceTestHelpers
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import test_helpers
 
 
-@test_helpers
-class ReceivedDebit(ListableAPIResource):
+class ReceivedCredit(ListableAPIResource):
     """
-    ReceivedDebits represent funds pulled from a [FinancialAccount](https://stripe.com/docs/api#financial_accounts). These are not initiated from the FinancialAccount.
+    ReceivedCredits represent funds sent to a [FinancialAccount](https://stripe.com/docs/api#financial_accounts) (for example, via ACH or wire). These money movements are not initiated from the FinancialAccount.
     """
 
-    OBJECT_NAME = "treasury.received_debit"
+    OBJECT_NAME = "treasury.received_credit"
 
     class TestHelpers(APIResourceTestHelpers):
         @classmethod
         def create(
             cls,
             api_key=None,
             stripe_version=None,
             stripe_account=None,
             **params
         ):
             return cls._static_request(
                 "post",
-                "/v1/test_helpers/treasury/received_debits",
+                "/v1/test_helpers/treasury/received_credits",
                 api_key=api_key,
                 stripe_version=stripe_version,
                 stripe_account=stripe_account,
                 params=params,
             )
+
+    @property
+    def test_helpers(self):
+        return self.TestHelpers(self)
+
+
+ReceivedCredit.TestHelpers._resource_cls = ReceivedCredit
```

### Comparing `stripe-5.6.0b2/stripe/api_resources/treasury/transaction_entry.py` & `stripe-5.6.0b3/stripe/api_resources/treasury/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/usage_record.py` & `stripe-5.6.0b3/stripe/api_resources/usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/api_resources/webhook_endpoint.py` & `stripe-5.6.0b3/stripe/api_resources/webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/data/ca-certificates.crt` & `stripe-5.6.0b3/stripe/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/error.py` & `stripe-5.6.0b3/stripe/error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/http_client.py` & `stripe-5.6.0b3/stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/multipart_data_generator.py` & `stripe-5.6.0b3/stripe/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/oauth.py` & `stripe-5.6.0b3/stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/oauth_error.py` & `stripe-5.6.0b3/stripe/oauth_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/object_classes.py` & `stripe-5.6.0b3/stripe/object_classes.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/preview.py` & `stripe-5.6.0b3/stripe/preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/raw_request.py` & `stripe-5.6.0b3/stripe/raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/six.py` & `stripe-5.6.0b3/stripe/six.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/stripe_object.py` & `stripe-5.6.0b3/stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/stripe_response.py` & `stripe-5.6.0b3/stripe/stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/util.py` & `stripe-5.6.0b3/stripe/util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe/webhook.py` & `stripe-5.6.0b3/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/stripe.egg-info/PKG-INFO` & `stripe-5.6.0b3/stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.6.0b2
+Version: 5.6.0b3
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.6.0b2/stripe.egg-info/SOURCES.txt` & `stripe-5.6.0b3/stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_createable_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_custom_method.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_deletable_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_listable_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_nested_resource_class_methods.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_searchable_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_singleton_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_test_helpers_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import absolute_import, division, print_function
 
 import stripe
-import pytest
 from stripe import util
 from stripe.api_resources.abstract import APIResourceTestHelpers
 
 
 class TestTestHelperAPIResource(object):
-    @stripe.api_resources.abstract.test_helpers
     class MyTestHelpersResource(stripe.api_resources.abstract.APIResource):
         OBJECT_NAME = "myresource"
 
         @stripe.api_resources.abstract.custom_method(
             "do_stuff", http_verb="post", http_path="do_the_thing"
         )
         class TestHelpers(APIResourceTestHelpers):
@@ -22,14 +20,20 @@
                 url = self.instance_url() + "/do_the_thing"
                 headers = util.populate_headers(idempotency_key)
                 self.resource.refresh_from(
                     self.resource.request("post", url, params, headers)
                 )
                 return self.resource
 
+        @property
+        def test_helpers(self):
+            return self.TestHelpers(self)
+
+    MyTestHelpersResource.TestHelpers._resource_cls = MyTestHelpersResource
+
     def test_call_custom_method_class(self, request_mock):
         request_mock.stub_request(
             "post",
             "/v1/test_helpers/myresources/mid/do_the_thing",
             {"id": "mid", "thing_done": True},
             rheaders={"request-id": "req_id"},
         )
@@ -56,11 +60,7 @@
 
         request_mock.assert_requested(
             "post",
             "/v1/test_helpers/myresources/mid/do_the_thing",
             {"foo": "bar"},
         )
         assert obj.thing_done is True
-
-    def test_helper_decorator_raises_for_non_resource(self):
-        with pytest.raises(ValueError):
-            stripe.api_resources.abstract.test_helpers(str)
```

### Comparing `stripe-5.6.0b2/tests/api_resources/abstract/test_updateable_api_resource.py` & `stripe-5.6.0b3/tests/api_resources/abstract/test_updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/billing_portal/test_configuration.py` & `stripe-5.6.0b3/tests/api_resources/billing_portal/test_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/checkout/test_session.py` & `stripe-5.6.0b3/tests/api_resources/checkout/test_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/identity/test_verification_report.py` & `stripe-5.6.0b3/tests/api_resources/identity/test_verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/identity/test_verification_session.py` & `stripe-5.6.0b3/tests/api_resources/identity/test_verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/issuing/test_authorization.py` & `stripe-5.6.0b3/tests/api_resources/issuing/test_authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/issuing/test_card.py` & `stripe-5.6.0b3/tests/api_resources/issuing/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/issuing/test_cardholder.py` & `stripe-5.6.0b3/tests/api_resources/issuing/test_cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/issuing/test_dispute.py` & `stripe-5.6.0b3/tests/api_resources/issuing/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/issuing/test_transaction.py` & `stripe-5.6.0b3/tests/api_resources/issuing/test_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/radar/test_early_fraud_warning.py` & `stripe-5.6.0b3/tests/api_resources/radar/test_early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/radar/test_value_list.py` & `stripe-5.6.0b3/tests/api_resources/radar/test_value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/radar/test_value_list_item.py` & `stripe-5.6.0b3/tests/api_resources/radar/test_value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/reporting/test_report_run.py` & `stripe-5.6.0b3/tests/api_resources/reporting/test_report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/reporting/test_report_type.py` & `stripe-5.6.0b3/tests/api_resources/reporting/test_report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/sigma/test_scheduled_query_run.py` & `stripe-5.6.0b3/tests/api_resources/sigma/test_scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/terminal/test_location.py` & `stripe-5.6.0b3/tests/api_resources/terminal/test_location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/terminal/test_reader.py` & `stripe-5.6.0b3/tests/api_resources/terminal/test_reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_account.py` & `stripe-5.6.0b3/tests/api_resources/test_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_account_link.py` & `stripe-5.6.0b3/tests/api_resources/test_account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_apple_pay_domain.py` & `stripe-5.6.0b3/tests/api_resources/test_apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_application_fee.py` & `stripe-5.6.0b3/tests/api_resources/test_application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_application_fee_refund.py` & `stripe-5.6.0b3/tests/api_resources/test_application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_balance_transaction.py` & `stripe-5.6.0b3/tests/api_resources/test_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_bank_account.py` & `stripe-5.6.0b3/tests/api_resources/test_bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_capability.py` & `stripe-5.6.0b3/tests/api_resources/test_capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_card.py` & `stripe-5.6.0b3/tests/api_resources/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_charge.py` & `stripe-5.6.0b3/tests/api_resources/test_charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_country_spec.py` & `stripe-5.6.0b3/tests/api_resources/test_country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_coupon.py` & `stripe-5.6.0b3/tests/api_resources/test_coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_credit_note.py` & `stripe-5.6.0b3/tests/api_resources/test_credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_customer.py` & `stripe-5.6.0b3/tests/api_resources/test_customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_customer_balance_transaction.py` & `stripe-5.6.0b3/tests/api_resources/test_customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_dispute.py` & `stripe-5.6.0b3/tests/api_resources/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_ephemeral_key.py` & `stripe-5.6.0b3/tests/api_resources/test_ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_event.py` & `stripe-5.6.0b3/tests/api_resources/test_event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_exchange_rate.py` & `stripe-5.6.0b3/tests/api_resources/test_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_file.py` & `stripe-5.6.0b3/tests/api_resources/test_file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_file_link.py` & `stripe-5.6.0b3/tests/api_resources/test_file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_file_upload.py` & `stripe-5.6.0b3/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_invoice.py` & `stripe-5.6.0b3/tests/api_resources/test_invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_invoice_item.py` & `stripe-5.6.0b3/tests/api_resources/test_invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_list_object.py` & `stripe-5.6.0b3/tests/api_resources/test_list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_payment_intent.py` & `stripe-5.6.0b3/tests/api_resources/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_payment_method.py` & `stripe-5.6.0b3/tests/api_resources/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_payout.py` & `stripe-5.6.0b3/tests/api_resources/test_payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_person.py` & `stripe-5.6.0b3/tests/api_resources/test_person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_plan.py` & `stripe-5.6.0b3/tests/api_resources/test_plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_price.py` & `stripe-5.6.0b3/tests/api_resources/test_price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_product.py` & `stripe-5.6.0b3/tests/api_resources/test_product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_promotion_code.py` & `stripe-5.6.0b3/tests/api_resources/test_promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_quote.py` & `stripe-5.6.0b3/tests/api_resources/test_quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_refund.py` & `stripe-5.6.0b3/tests/api_resources/test_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_reversal.py` & `stripe-5.6.0b3/tests/api_resources/test_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_review.py` & `stripe-5.6.0b3/tests/api_resources/test_review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_search_result_object.py` & `stripe-5.6.0b3/tests/api_resources/test_search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_setup_intent.py` & `stripe-5.6.0b3/tests/api_resources/test_setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_source.py` & `stripe-5.6.0b3/tests/api_resources/test_source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_source_transaction.py` & `stripe-5.6.0b3/tests/api_resources/test_source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_subscription.py` & `stripe-5.6.0b3/tests/api_resources/test_subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_subscription_item.py` & `stripe-5.6.0b3/tests/api_resources/test_subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_subscription_schedule.py` & `stripe-5.6.0b3/tests/api_resources/test_subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_tax_code.py` & `stripe-5.6.0b3/tests/api_resources/test_tax_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_tax_id.py` & `stripe-5.6.0b3/tests/api_resources/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_tax_rate.py` & `stripe-5.6.0b3/tests/api_resources/test_tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_topup.py` & `stripe-5.6.0b3/tests/api_resources/test_topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_transfer.py` & `stripe-5.6.0b3/tests/api_resources/test_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_usage_record.py` & `stripe-5.6.0b3/tests/api_resources/test_usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_usage_record_summary.py` & `stripe-5.6.0b3/tests/api_resources/test_usage_record_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/api_resources/test_webhook_endpoint.py` & `stripe-5.6.0b3/tests/api_resources/test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/conftest.py` & `stripe-5.6.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/request_mock.py` & `stripe-5.6.0b3/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/stripe_mock.py` & `stripe-5.6.0b3/tests/stripe_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_api_requestor.py` & `stripe-5.6.0b3/tests/test_api_requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,21 +730,14 @@
             urllib3.response.HTTPResponse(
                 body=util.io.BytesIO(b'{"error": "invalid_grant"}'),
                 preload_content=False,
             ),
             400,
         )
 
-    def test_developer_message_in_error(self, requestor, mock_response):
-        mock_response('{"error": {"developer_message": "Unacceptable"}}', 400)
-
-        with pytest.raises(stripe.error.InvalidRequestError) as excinfo:
-            requestor.request("get", self.valid_path, {})
-        assert excinfo.value.user_message == "Unacceptable"
-
     def test_raw_request_with_file_param(self, requestor, mock_response):
         test_file = tempfile.NamedTemporaryFile()
         test_file.write("\u263A".encode("utf-16"))
         test_file.seek(0)
         params = {"file": test_file, "purpose": "dispute_evidence"}
         supplied_headers = {"Content-Type": "multipart/form-data"}
         mock_response("{}", 200)
```

### Comparing `stripe-5.6.0b2/tests/test_error.py` & `stripe-5.6.0b3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_generated_examples.py` & `stripe-5.6.0b3/tests/test_generated_examples.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_http_client.py` & `stripe-5.6.0b3/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_integration.py` & `stripe-5.6.0b3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_multipart_data_generator.py` & `stripe-5.6.0b3/tests/test_multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_oauth.py` & `stripe-5.6.0b3/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_preview.py` & `stripe-5.6.0b3/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_raw_request.py` & `stripe-5.6.0b3/tests/test_raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_stripe_object.py` & `stripe-5.6.0b3/tests/test_stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_stripe_response.py` & `stripe-5.6.0b3/tests/test_stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tests/test_util.py` & `stripe-5.6.0b3/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 }
             ],
             "livemode": False,
         }
 
         obj = util.convert_to_stripe_object(resp)
         assert isinstance(obj, stripe.Balance)
-        assert type(obj.available) == list
+        assert isinstance(obj.available, list)
         assert isinstance(obj.available[0], stripe.stripe_object.StripeObject)
 
         d = util.convert_to_dict(obj)
         assert isinstance(d, dict)
         assert isinstance(d["available"], list)
         assert isinstance(d["available"][0], dict)
```

### Comparing `stripe-5.6.0b2/tests/test_webhook.py` & `stripe-5.6.0b3/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.6.0b2/tox.ini` & `stripe-5.6.0b3/tox.ini`

 * *Files identical despite different names*

