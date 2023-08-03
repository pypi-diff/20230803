# Comparing `tmp/razorpay-1.3.1.tar.gz` & `tmp/razorpay-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "razorpay-1.3.1.tar", last modified: Thu Aug  3 07:03:28 2023, max compression
+gzip compressed data, was "razorpay-1.4.1.tar", last modified: Thu Aug  3 08:29:54 2023, max compression
```

## Comparing `razorpay-1.3.1.tar` & `razorpay-1.4.1.tar`

### file list

```diff
@@ -1,156 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.160666 razorpay-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 07:03:14.000000 razorpay-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 07:03:14.000000 razorpay-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 07:03:28.160666 razorpay-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 07:03:14.000000 razorpay-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.140666 razorpay-1.3.1/razorpay/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   258424 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/ca-bundle.crt
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.144666 razorpay-1.3.1/razorpay/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/constants/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/constants/http_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/constants/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.144666 razorpay-1.3.1/razorpay/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/fund_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/qrcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/registration_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/resources/virtual_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.144666 razorpay-1.3.1/razorpay/utility/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-03 07:03:14.000000 razorpay-1.3.1/razorpay/utility/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.140666 razorpay-1.3.1/razorpay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 07:03:28.000000 razorpay-1.3.1/razorpay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-03 07:03:28.000000 razorpay-1.3.1/razorpay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:03:28.000000 razorpay-1.3.1/razorpay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 07:03:28.000000 razorpay-1.3.1/razorpay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 07:03:28.000000 razorpay-1.3.1/razorpay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:03:28.160666 razorpay-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-03 07:03:14.000000 razorpay-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.148666 razorpay-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:03:28.160666 razorpay-1.3.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/addon_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/bad_request_error.json
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/cancel_payment_link.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/customer_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/edit_customer.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/edit_order.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/edit_payment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/edit_payment_link.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_addon.json
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_app_details.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_bank_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_captured_payment.json
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_card.json
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_card_detail_payment.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_create_recurring.json
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_customer.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_delete_allowed_payer.json
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_invoice.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_invoice_cancel.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_invoice_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_invoice_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_invoice_notify_by.json
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_item.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_order.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_otp_generate.json
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_otp_resend.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_otp_submit.json
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_payment.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_payment_authorized_webhook.json
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_payment_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_payment_link.json
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_plan.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_qrcode.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_refund.json
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_registration_link.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_reversal.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_settlement.json
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_subscription.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_subscription_addon.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_subscription_cancelled.json
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_subscription_paused.json
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_subscription_resumed.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_token.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_upi_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_virtual_accounts.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_virtual_accounts_closed.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fake_virtual_accounts_receiver.json
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/fund_account_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_create_recurring.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_customer.json
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_invoice.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_invoice_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_order.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_payment_link.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_plan.json
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_registration_link.json
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_settlement.json
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_subscription.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/init_virtual_accounts.json
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/invoice_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/invoice_collection_with_one_invoice.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/item_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/order_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/order_collection_with_one_order.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/payment_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/payment_collection_with_one_payment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/payment_link_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/plan_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/qrcode_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/qrcode_payments_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/refund_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/reversal_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/settlement_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/settlement_collection_with_one_settlement.json
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/subscription_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/token_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/token_collection_with_one_token.json
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/transfers_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/transfers_collection_with_payment_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/virtual_accounts_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/mocks/virtual_accounts_collection_with_one_item.json
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_fund_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_qrcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_registration_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_client_virtual_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_multiple_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-03 07:03:14.000000 razorpay-1.3.1/tests/test_user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.249341 razorpay-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 08:29:41.000000 razorpay-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 08:29:41.000000 razorpay-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-03 08:29:54.249341 razorpay-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-03 08:29:41.000000 razorpay-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.221341 razorpay-1.4.1/razorpay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   258424 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/ca-bundle.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.225341 razorpay-1.4.1/razorpay/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/constants/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/constants/http_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/constants/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.229341 razorpay-1.4.1/razorpay/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/fund_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/iin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/registration_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/stakeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/virtual_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/resources/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.229341 razorpay-1.4.1/razorpay/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-03 08:29:41.000000 razorpay-1.4.1/razorpay/utility/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.225341 razorpay-1.4.1/razorpay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-03 08:29:54.000000 razorpay-1.4.1/razorpay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-03 08:29:54.000000 razorpay-1.4.1/razorpay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:29:54.000000 razorpay-1.4.1/razorpay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 08:29:54.000000 razorpay-1.4.1/razorpay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 08:29:54.000000 razorpay-1.4.1/razorpay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:29:54.249341 razorpay-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-03 08:29:41.000000 razorpay-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.233341 razorpay-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:54.249341 razorpay-1.4.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/addon_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/bad_request_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/cancel_payment_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/customer_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/edit_customer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/edit_order.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/edit_payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/edit_payment_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_addon.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_app_details.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_bank_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_captured_payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_card.json
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_card_detail_payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_create_recurring.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_customer.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_delete_allowed_payer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_iin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_invoice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_invoice_cancel.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_invoice_delete.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_invoice_edit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_invoice_notify_by.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_merchant_token.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_order.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_otp_generate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_otp_resend.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_otp_submit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_payment_authorized_webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_payment_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_payment_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_product.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_qrcode.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_reference_card.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_refund.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_registration_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_reversal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_settlement.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_stakeholder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_subscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_subscription_addon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_subscription_cancelled.json
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_subscription_paused.json
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_subscription_resumed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_token.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_upi_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_virtual_accounts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_virtual_accounts_closed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_virtual_accounts_receiver.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fake_webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/fund_account_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_create_recurring.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_customer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_invoice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_invoice_edit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_order.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_payment_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_registration_link.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_settlement.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_stakeholder.json
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_subscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_virtual_accounts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/init_webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/invoice_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/invoice_collection_with_one_invoice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/item_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/order_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/order_collection_with_one_order.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/payment_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/payment_collection_with_one_payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/payment_link_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/plan_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/qrcode_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/qrcode_payments_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/refund_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/reversal_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/settlement_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/settlement_collection_with_one_settlement.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/stakeholder_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/subscription_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/token_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/token_collection_with_one_token.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/transfers_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/transfers_collection_with_payment_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/virtual_accounts_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/virtual_accounts_collection_with_one_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/mocks/webhook_collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_fund_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_iin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_registration_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_stakeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_virtual_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_client_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_multiple_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-03 08:29:41.000000 razorpay-1.4.1/tests/test_user_agent.py
```

### Comparing `razorpay-1.3.1/LICENSE` & `razorpay-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/PKG-INFO` & `razorpay-1.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: razorpay
-Version: 1.3.1
+Version: 1.4.1
 Summary: Razorpay Python Client
 Home-page: https://github.com/razorpay/razorpay-python
 Author: Team Razorpay
 License: MIT
 Keywords: razorpay payment gateway india
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Razorpay Python Client
 
-[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/pypi/pyversions/razorpay.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/badge/python-3%20%7C%203.4%20%7C%203.5%20%7C%203.6-blue.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
 
 Python bindings for interacting with the Razorpay API
 
 This is primarily meant for merchants who wish to perform interactions with the Razorpay API programatically.
 
 ## Installation
 
@@ -53,14 +51,16 @@
 client.set_app_details({"title" : "<YOUR_APP_TITLE>", "version" : "<YOUR_APP_VERSION>"})
 ```
 
 For example, you can set the title to `Django` and version to `1.8.17`. Please ensure
 that both app title and version are strings.
 
 ## Supported Resources
+- [Account](documents/account.md)
+
 - [Addon](documents/addon.md)
 
 - [Item](documents/items.md)
 
 - [Customer](documents/customer.md)
 
 - [Token](documents/token.md)
@@ -96,14 +96,20 @@
 - [UPI](documents/upi.md)
 
 - [Register Emandate and Charge First Payment Together](documents/registerEmandate.md)
 
 - [Register NACH and Charge First Payment Together](documents/registerNach.md)
 
 - [Payment Verification](documents/paymentVerfication.md)
+
+- [Product Configuration](documents/productConfiguration.md)
+
+- [Stakeholder](documents/stakeholder.md)
+
+- [Webhook](documents/webhook.md)
 ---
 
 ## Bugs? Feature requests? Pull requests?
 
 All of those are welcome. You can [file issues][issues] or [submit pull requests][pulls] in this repository.
 
 [issues]: https://github.com/razorpay/razorpay-python/issues
```

### Comparing `razorpay-1.3.1/README.md` & `razorpay-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Razorpay Python Client
 
-[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/pypi/pyversions/razorpay.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/badge/python-3%20%7C%203.4%20%7C%203.5%20%7C%203.6-blue.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
 
 Python bindings for interacting with the Razorpay API
 
 This is primarily meant for merchants who wish to perform interactions with the Razorpay API programatically.
 
 ## Installation
 
@@ -31,14 +31,16 @@
 client.set_app_details({"title" : "<YOUR_APP_TITLE>", "version" : "<YOUR_APP_VERSION>"})
 ```
 
 For example, you can set the title to `Django` and version to `1.8.17`. Please ensure
 that both app title and version are strings.
 
 ## Supported Resources
+- [Account](documents/account.md)
+
 - [Addon](documents/addon.md)
 
 - [Item](documents/items.md)
 
 - [Customer](documents/customer.md)
 
 - [Token](documents/token.md)
@@ -74,14 +76,20 @@
 - [UPI](documents/upi.md)
 
 - [Register Emandate and Charge First Payment Together](documents/registerEmandate.md)
 
 - [Register NACH and Charge First Payment Together](documents/registerNach.md)
 
 - [Payment Verification](documents/paymentVerfication.md)
+
+- [Product Configuration](documents/productConfiguration.md)
+
+- [Stakeholder](documents/stakeholder.md)
+
+- [Webhook](documents/webhook.md)
 ---
 
 ## Bugs? Feature requests? Pull requests?
 
 All of those are welcome. You can [file issues][issues] or [submit pull requests][pulls] in this repository.
 
 [issues]: https://github.com/razorpay/razorpay-python/issues
```

### Comparing `razorpay-1.3.1/razorpay/__init__.py` & `razorpay-1.4.1/razorpay/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 from .resources import Settlement
 from .resources import Item
 from .resources import Qrcode
 from .resources import FundAccount
 from .utility import Utility
 from .constants import ERROR_CODE
 from .constants import HTTP_STATUS_CODE
+from .resources import Account
+from .resources import Stakeholder
+from .resources import Product
+from .resources import Iin
+from .resources import Webhook
 
 __all__ = [
         'Payment',
         'Refund',
         'Order',
         'Client',
         'Invoice',
@@ -40,8 +45,13 @@
         'Plan',
         'FundAccount',
         'Settlement',
         'Item',
         'Qrcode',
         'HTTP_STATUS_CODE',
         'ERROR_CODE',
+        'Account',
+        'Stakeholder',
+        'Product',
+        'Iin',
+        'Webhook'
 ]
```

### Comparing `razorpay-1.3.1/razorpay/ca-bundle.crt` & `razorpay-1.4.1/razorpay/ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/razorpay/client.py` & `razorpay-1.4.1/razorpay/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,14 +172,31 @@
     def put(self, path, data, **options):
         """
         Parses PUT request options and dispatches a request
         """
         data, options = self._update_request(data, options)
         return self.request('put', path, data=data, **options)
 
+    def file(self, path, data, **options):     
+        fileDict = {}
+        fieldDict = {}
+        
+        if('file' not in data):
+            # if file is not exists in the dictionary
+            data['file'] = ""
+
+        fileDict['file'] = data['file'] 
+        
+        # Create a dict of form fields 
+        for fields in data:
+          if(fields != 'file'):
+            fieldDict[str(fields)] = data[fields] 
+
+        return self.request('post', path, files=fileDict, data=fieldDict, **options)
+
     def _update_request(self, data, options):
         """
         Updates The resource data and header options
         """
         data = json.dumps(data)
 
         if 'headers' not in options:
```

### Comparing `razorpay-1.3.1/razorpay/constants/url.py` & `razorpay-1.4.1/razorpay/constants/url.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 class URL(object):
-    BASE_URL = 'https://api.razorpay.com/v1'
+    BASE_URL = 'https://api.razorpay.com'
+    V1 = '/v1'
+    V2 = '/v2'
     ORDER_URL = "/orders"
     INVOICE_URL = "/invoices"
     PAYMENT_LINK_URL = "/payment_links"
     PAYMENTS_URL = "/payments"
     REFUNDS_URL = "/refunds"
     CARD_URL = "/cards"
     CUSTOMER_URL = "/customers"
@@ -13,7 +15,14 @@
     ADDON_URL = "/addons"
     PLAN_URL = "/plans"
     SETTLEMENT_URL = "/settlements"
     ITEM_URL = "/items"
     QRCODE_URL = "/payments/qr_codes"
     REGISTRATION_LINK_URL = "/subscription_registration"
     FUND_ACCOUNT_URL = "/fund_accounts"
+    ACCOUNT = "/accounts"
+    STAKEHOLDER = "/stakeholders"
+    PRODUCT = "/products"
+    TNC = "/tnc"
+    TOKEN = "/tokens"
+    IIN = "/iins"
+    WEBHOOK = "/webhooks"
```

### Comparing `razorpay-1.3.1/razorpay/errors.py` & `razorpay-1.4.1/razorpay/errors.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/razorpay/resources/__init__.py` & `razorpay-1.4.1/razorpay/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from .plan import Plan
 from .subscription import Subscription
 from .qrcode import Qrcode
 from .registration_link import RegistrationLink
 from .settlement import Settlement
 from .item import Item
 from .fund_account import FundAccount
+from .account import Account
+from .stakeholder import Stakeholder
+from .product import Product
+from .iin import Iin
+from .webhook import Webhook
 
 __all__ = [
     'Payment',
     'Refund',
     'Order',
     'Invoice',
     'PaymentLink',
@@ -31,9 +36,14 @@
     'Addon',
     'Plan',
     'Subscription',
     'RegistrationLink',
     'Settlement',
     'Item',
     'QrCode',
-    'FundAccount'
+    'FundAccount',
+    'Account',
+    'Stakeholder',
+    'Product',
+    'Iin',
+    'Webhook'
 ]
```

### Comparing `razorpay-1.3.1/razorpay/resources/addon.py` & `razorpay-1.4.1/razorpay/resources/addon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Addon(Resource):
     def __init__(self, client=None):
         super(Addon, self).__init__(client)
-        self.base_url = URL.ADDON_URL
+        self.base_url = URL.V1 + URL.ADDON_URL
 
     def fetch(self, addon_id, data={}, **kwargs):
-        """"
+        """
         Fetch addon for given Id
 
         Args:
             addon_id : Id for which addon object has to be retrieved
 
         Returns:
             addon dict for given subscription Id
@@ -27,13 +27,13 @@
             addon_id : Id for which addon object has to be deleted
         """
         url = '{}/{}'.format(self.base_url, addon_id)
 
         return self.delete_url(url, data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Add-ons
         Returns:
             Dictionary of Add-ons
         """
         return super(Addon, self).all(data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/base.py` & `razorpay-1.4.1/razorpay/resources/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 
     def delete_url(self, url, data, **kwargs):
         return self.client.delete(url, data, **kwargs)
 
     def delete(self, id, data, **kwargs):
         url = "{}/{}/delete".format(self.base_url, id)
         return self.delete_url(url, data, **kwargs)
+
+    def file_url(self, url, data, **kwargs):
+        return self.client.file(url, data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/customer.py` & `razorpay-1.4.1/razorpay/resources/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Customer(Resource):
     def __init__(self, client=None):
         super(Customer, self).__init__(client)
-        self.base_url = URL.CUSTOMER_URL
+        self.base_url = URL.V1 + URL.CUSTOMER_URL
 
     def fetch(self, customer_id, data={}, **kwargs):
-        """"
+        """
         Fetch Customer for given Id
 
         Args:
             customer_id : Id for which customer object has to be retrieved
 
         Returns:
             Order dict for given customer Id
         """
         return super(Customer, self).fetch(customer_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Customer from given dict
 
         Returns:
             Customer Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def edit(self, customer_id, data={}, **kwargs):
-        """"
+        """
         Edit Customer information from given dict
 
         Returns:
             Customer Dict which was edited
         """
         url = '{}/{}'.format(self.base_url, customer_id)
 
         return self.put_url(url, data, **kwargs)
     
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all customer
 
         Returns:
             Dictionary of Customers data
         """
         return super(Customer, self).all(data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/fund_account.py` & `razorpay-1.4.1/razorpay/resources/fund_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class FundAccount(Resource):
     def __init__(self, client=None):
         super(FundAccount, self).__init__(client)
-        self.base_url = URL.FUND_ACCOUNT_URL
+        self.base_url = URL.V1 + URL.FUND_ACCOUNT_URL
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Fund Account entities
 
         Returns:
             Dictionary of Fund Account
         """
         return super(FundAccount, self).all(data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create a fund account
 
         Args:
             data : Dictionary having keys using which order have to be created
                 'customerId' :  Customer Id for the customer
                 'account_type' : The bank_account to be linked to the customer ID
                 'bank_account' : key value pair
```

### Comparing `razorpay-1.3.1/razorpay/resources/invoice.py` & `razorpay-1.4.1/razorpay/resources/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,108 +2,108 @@
 from ..constants.url import URL
 import warnings
 
 
 class Invoice(Resource):
     def __init__(self, client=None):
         super(Invoice, self).__init__(client)
-        self.base_url = URL.INVOICE_URL
+        self.base_url = URL.V1 + URL.INVOICE_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release", DeprecationWarning)
         return self.all(data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Invoice entities
 
         Returns:
             Dictionary of Invoice data
         """
         return super(Invoice, self).all(data, **kwargs)
 
     def fetch(self, invoice_id, data={}, **kwargs):
-        """"
+        """
         Fetch Invoice for given Id
 
         Args:
             invoice_id : Id for which invoice object has to be retrieved
 
         Returns:
             Invoice dict for given invoice Id
         """
         return super(Invoice, self).fetch(invoice_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Invoice from given dict
 
         Args:
             data : Dictionary having keys using which invoice have to be created
 
         Returns:
             Invoice Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def notify_by(self, invoice_id, medium, **kwargs):
-        """"
+        """
         Send/Resend notifications to customer via email/sms
 
         Args:
             invoice_id : Id for trigger notify
             medium : Medium for triggering notification via email or sms
 
         Returns:
             {"success": true}
         """
         url = "{}/{}/notify_by/{}".format(self.base_url, invoice_id, medium)
         return self.post_url(url, {}, **kwargs)
 
     def cancel(self, invoice_id, **kwargs):
-        """"
+        """
         Cancel an unpaid Invoice with given ID via API
         It can only be called on an invoice that is not in the paid state.
 
         Args:
             invoice_id : Id for cancel the invoice
         Returns:
             The response for the API will be the invoice entity, similar to create/update API response, with status attribute's value as cancelled
         """
         url = "{}/{}/cancel".format(self.base_url, invoice_id)
         return self.post_url(url, {}, **kwargs)
 
     def delete(self, invoice_id, **kwargs):
-        """"
+        """
         Delete an invoice
         You can delete an invoice which is in the draft state.
 
         Args:
             invoice_id : Id for delete the invoice
         Returns:
             The response is always be an empty array like this - []
         """
         url = "{}/{}".format(self.base_url, invoice_id)
         return self.delete_url(url, {}, **kwargs)
 
     def issue(self, invoice_id, **kwargs):
-        """"
+        """
         Issues an invoice in draft state
 
         Args:
             invoice_id : Id for delete the invoice
         Returns:
             Its response is the invoice entity, similar to create/update API response. Its status now would be issued.
         """
         url = "{}/{}/issue".format(self.base_url, invoice_id)
         return self.post_url(url, {}, **kwargs)
 
     def edit(self, invoice_id, data={}, **kwargs):
-        """"
+        """
         Update an invoice
         In draft state all the attributes are allowed.
 
         Args:
             invoice_id : Id for delete the invoice
             data : Dictionary having keys using which invoice have to be updated
         Returns:
```

### Comparing `razorpay-1.3.1/razorpay/resources/item.py` & `razorpay-1.4.1/razorpay/resources/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Item(Resource):
     def __init__(self, client=None):
         super(Item, self).__init__(client)
-        self.base_url = URL.ITEM_URL
+        self.base_url = URL.V1 + URL.ITEM_URL
     
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create item
 
         Returns:
             Item Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def fetch(self, item_id, data={}, **kwargs):
-        """"
+        """
         Fetch an Item
 
         Args:
             item_id : The id of the item to be fetched
 
         Returns:
             Item dict for given card Id
         """
         return super(Item, self).fetch(item_id, data, **kwargs)
     
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all items
 
         Returns:
             Dictionary of Items data
         """
         return super(Item, self).all(data, **kwargs)
 
     def edit(self, item_id, data={}, **kwargs):
-        """"
+        """
         Update an Item
 
         Returns:
             Item Dict which was edited
         """
         url = '{}/{}'.format(self.base_url, item_id)
 
         return self.patch_url(url, data, **kwargs)    
     
     def delete(self, item_id, **kwargs):
-        """"
+        """
         Delete an Item
 
         Args:
             item_id : The id of the item to be deleted
 
         Returns:
             The response is always be an empty array like this - []
```

### Comparing `razorpay-1.3.1/razorpay/resources/order.py` & `razorpay-1.4.1/razorpay/resources/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from ..constants.url import URL
 import warnings
 
 
 class Order(Resource):
     def __init__(self, client=None):
         super(Order, self).__init__(client)
-        self.base_url = URL.ORDER_URL
+        self.base_url = URL.V1 + URL.ORDER_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release, use all",
                       DeprecationWarning)
         return self.all(data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Order entities
 
         Returns:
             Dictionary of Order data
         """
         return super(Order, self).all(data, **kwargs)
 
     def fetch(self, order_id, data={}, **kwargs):
-        """"
+        """
         Fetch Order for given Id
 
         Args:
             order_id : Id for which order object has to be retrieved
 
         Returns:
             Order dict for given order Id
@@ -36,28 +36,28 @@
 
     def fetch_all_payments(self, order_id, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release, use payments",
                       DeprecationWarning)
         return self.payments(order_id, data, **kwargs)
 
     def payments(self, order_id, data={}, **kwargs):
-        """"
+        """
         Fetch Payment for Order Id
 
         Args:
             order_id : Id for which payment objects has to be retrieved
 
         Returns:
             Payment dict for given Order Id
         """
         url = "{}/{}/payments".format(self.base_url, order_id)
         return self.get_url(url, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Order from given dict
 
         Args:
             data : Dictionary having keys using which order have to be created
                 'amount' :  Amount of Order
                 'currency' : Currency used in Order
                 'receipt' : Receipt Id for the order
@@ -67,15 +67,15 @@
         Returns:
             Order Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
     
     def edit(self, order_id, data={}, **kwargs):
-        """"
+        """
          Update order
 
         Args:
             data : Dictionary having keys using which order have to be edited
                 'notes' : key value pair as notes
             
             Returns:
```

### Comparing `razorpay-1.3.1/razorpay/resources/payment.py` & `razorpay-1.4.1/razorpay/resources/payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,287 +2,287 @@
 from ..constants.url import URL
 import warnings
 
 
 class Payment(Resource):
     def __init__(self, client=None):
         super(Payment, self).__init__(client)
-        self.base_url = URL.PAYMENTS_URL
+        self.base_url = URL.V1 + URL.PAYMENTS_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release, use all",
                       DeprecationWarning)
         return self.all(data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Payment entities
 
         Returns:
             Dictionary of Payment data
         """
         return super(Payment, self).all(data, **kwargs)
 
     def fetch(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Fetch Payment for given Id
 
         Args:
             payment_id : Id for which payment object has to be retrieved
 
         Returns:
             Payment dict for given payment Id
         """
         return super(Payment, self).fetch(payment_id, data, **kwargs)
 
     def capture(self, payment_id, amount, data={}, **kwargs): # nosemgrep : python.lang.correctness.common-mistakes.default-mutable-dict.default-mutable-dict
-        """"
+        """
         Capture Payment for given Id
 
         Args:
             payment_id : Id for which payment object has to be retrieved
             amount : Amount for which the payment has to be retrieved
 
         Returns:
             Payment dict after getting captured
         """
         url = "{}/{}/capture".format(self.base_url, payment_id)
         data['amount'] = amount
         return self.post_url(url, data, **kwargs)
 
     def refund(self, payment_id, amount, data={}, **kwargs):  # pragma: no cover # nosemgrep : python.lang.correctness.common-mistakes.default-mutable-dict.default-mutable-dict
-        """"
+        """
         Refund Payment for given Id
 
         Args:
             payment_id : Id for which payment object has to be refunded
             amount : Amount for which the payment has to be refunded
 
         Returns:
             Payment dict after getting refunded
         """
         url = "{}/{}/refund".format(self.base_url, payment_id)
         data['amount'] = amount
         return self.post_url(url, data, **kwargs)
 
     def transfer(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Create Transfer for given Payment Id
 
         Args:
             payment_id : Id for which payment object has to be transferred
 
         Returns:
             Payment dict after getting transferred
         """
         url = "{}/{}/transfers".format(self.base_url, payment_id)
         return self.post_url(url, data, **kwargs)
 
     def transfers(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Fetches all transfer for given Payment Id
 
         Args:
             payment_id : Id for which all the transfers has to be fetched
 
         Returns:
             A collection (dict) of transfers
             items : The key containing a list of 'transfer' entities
         """
         url = "{}/{}/transfers".format(self.base_url, payment_id)
         return self.get_url(url, data, **kwargs)
 
     def bank_transfer(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Bank Transfer Entity for given Payment
 
         Args:
             payment_id : Id for which bank transfer entity has to be fetched
 
         Returns:
             Bank Transfer dict
         """
         url = "{}/{}/bank_transfer".format(self.base_url, payment_id)
         return self.get_url(url, data, **kwargs)
 
     def upi_transfer(self, payment_id, data={}, **kwargs):
-        """"
+        """
         UPI Transfer Entity for given Payment
 
         Args:
             payment_id : Id for which upi transfer entity has to be fetched
 
         Returns:
             UPI Transfer dict
         """
         url = "{}/{}/upi_transfer".format(self.base_url, payment_id)
         return self.get_url(url, data, **kwargs)
     
     def refund(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Create a normal refund
 
         Returns:
             Payment dict after getting refund
         """
         url = "{}/{}/refund".format(self.base_url, payment_id)
         return self.post_url(url, data, **kwargs)
 
     def fetch_multiple_refund(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Fetch multiple refunds for a payment
 
         Returns:
             refunds dict
         """
         url = "{}/{}/refunds".format(self.base_url, payment_id)
         return self.get_url(url, data, **kwargs) 
 
     def fetch_refund_id(self, payment_id, refund_id, **kwargs):
-        """"
+        """
         Fetch multiple refunds for a payment
 
         Returns:
             Refund dict
         """
         url = "{}/{}/refunds/{}".format(self.base_url, payment_id, refund_id)
         return self.get_url(url, {}, **kwargs)  
   
     def edit(self, payment_id, data={}, **kwargs):
-        """"
+        """
          Update the Payment
         Args:
             data : Dictionary having keys using which order have to be edited
                 'notes' : key value pair as notes
             
             Returns:
             Payment Dict which was edited
         """
         url = '{}/{}'.format(self.base_url, payment_id)
 
         return self.patch_url(url, data, **kwargs) 
     
     def fetchCardDetails(self, payment_id, **kwargs):
-        """"
+        """
         Fetch Card Details of a Payment
 
         Args:
             payment_id : Id for which payment objects has to be retrieved
 
         Returns:
             Payment dict for given Order Id
         """
         url = "{}/{}/card".format(self.base_url, payment_id)
         return self.get_url(url, {}, **kwargs)
 
     def fetchDownTime(self, **kwargs):
-        """"
+        """
         Fetch Card Details of a Payment
 
         Args:
             payment_id : Id for which payment objects has to be retrieved
 
         Returns:
             Payment dict for given Order Id
         """
         url = "{}/{}".format(self.base_url,'downtimes')
         return self.get_url(url, {}, **kwargs)        
     
     def fetchDownTimeById(self, downtime_id, **kwargs):
-        """"
+        """
         Fetch Payment Downtime Details by ID
 
         Args:
             payment_id : Id for which payment objects has to be retrieved
 
         Returns:
             Payment dict for given Order Id
         """
         url = "{}/downtimes/{}".format(self.base_url, downtime_id)
         return self.get_url(url, {}, **kwargs)
     
     def createPaymentJson(self ,data={}, **kwargs):
-        """"
+        """
         Create a Payment
 
         Args:
             payment_id : Id for which payment object has to be refunded
             amount : Amount for which the payment has to be refunded
 
         Returns:
             Payment Dict which was created
         """
         url = "{}/create/{}".format(self.base_url, 'json')
 
         return self.post_url(url, data, **kwargs)  
 
     def createRecurring(self, data={}, **kwargs):
-        """"
+        """
         Create Recurring Payments
         Return:
             Recurring Payments dict
         """
         url = "{}/{}/recurring".format(self.base_url,'create')
         return self.post_url(url, data, **kwargs)
 
     def createUpi(self, data={}, **kwargs):
-        """"
+        """
         Initiate a payment
         Return:
           Payments dict
         """
         url = "{}/create/{}".format(self.base_url,'upi')
         return self.post_url(url, data, **kwargs)
 
     def validateVpa(self, data={}, **kwargs):
-        """"
+        """
         Validate the VPA
         Return:
           Payments dict
         """
         url = "{}/validate/{}".format(self.base_url,'vpa')
         return self.post_url(url, data, **kwargs)            
 
     def fetchPaymentMethods(self, **kwargs):
-        """"
+        """
         Fetch payment methods
         Return:
           Payments dict
         """
         url = "/{}".format('methods')
         return self.get_url(url, {}, **kwargs)
     
     def otpGenerate(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Otp Generate
 
         Args:
             payment_id : Id for which upi transfer entity has to be fetched
 
         Returns:
             Otp Dict which was created
         """
         url = "{}/{}/otp_generate".format(self.base_url, payment_id)
         return self.post_url(url, data, **kwargs)
 
     def otpSubmit(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Otp Submit
 
         Args:
             payment_id : Id for which upi transfer entity has to be fetched
 
         Returns:
             Otp Dict which was created
         """
         url = "{}/{}/otp/submit".format(self.base_url, payment_id)
         return self.post_url(url, data, **kwargs)
 
     def otpResend(self, payment_id, data={}, **kwargs):
-        """"
+        """
         Otp Resend
 
         Args:
             payment_id : Id for which upi transfer entity has to be fetched
 
         Returns:
             Otp Dict which was created
```

### Comparing `razorpay-1.3.1/razorpay/resources/payment_link.py` & `razorpay-1.4.1/razorpay/resources/payment_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,69 +2,69 @@
 from ..constants.url import URL
 import warnings
 
 
 class PaymentLink(Resource):
     def __init__(self, client=None):
         super(PaymentLink, self).__init__(client)
-        self.base_url = URL.PAYMENT_LINK_URL
+        self.base_url = URL.V1 + URL.PAYMENT_LINK_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release", DeprecationWarning)
         return self.all(data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Payment link entities
 
         Returns:
             Dictionary of Payment link data
         """
         return super(PaymentLink, self).all(data, **kwargs)
 
     def fetch(self, payment_link_id, data={}, **kwargs):
-        """"
+        """
         Fetch Payment link for given Id
 
         Args:
             payment_link_id : Id for which Payment link object has to be retrieved
 
         Returns:
             Payment link dict for given payment_link_id Id
         """
         return super(PaymentLink, self).fetch(payment_link_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Payment link from given dict
 
         Args:
             data : Dictionary having keys using which Payment link have to be created
 
         Returns:
             Payment link Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def cancel(self, payment_link_id, **kwargs):
-        """"
+        """
         Cancel an unpaid Payment link with given ID via API
         It can only be called on an Payment link that is not in the paid state.
 
         Args:
             payment_link_id : Id for cancel the Payment link
         Returns:
             The response for the API will be the Payment link entity, similar to create/update API response, with status attribute's value as cancelled
         """
         url = "{}/{}/cancel".format(self.base_url, payment_link_id)
         return self.post_url(url, {}, **kwargs)
    
     def edit(self, payment_link_id, data={}, **kwargs):
-        """"
+        """
         Edit the Payment link
         Args:
             data : Dictionary having keys using which order have to be edited
                 reference_id : Adds a unique reference number to an existing link.
 
                 expire_by : Timestamp, in Unix format, when the payment links should expire.
 
@@ -73,15 +73,15 @@
             Returns:
             Payment Link Dict which was edited
         """
         url = '{}/{}'.format(self.base_url, payment_link_id)
         return self.patch_url(url, data, **kwargs)
 
     def notifyBy(self, payment_link_id, medium, **kwargs):
-        """"
+        """
         Send notification
 
         Args:
             payment_link_id : Unique identifier of the Payment Link that should be resent.
             
             medium : sms/email
         """
```

### Comparing `razorpay-1.3.1/razorpay/resources/plan.py` & `razorpay-1.4.1/razorpay/resources/plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Plan(Resource):
     def __init__(self, client=None):
         super(Plan, self).__init__(client)
-        self.base_url = URL.PLAN_URL
+        self.base_url = URL.V1 + URL.PLAN_URL
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Plan from given dict
 
         Args:
             data : Dictionary having keys using which Plan has to be created
 
         Returns:
             Plan Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def fetch(self, plan_id, data={}, **kwargs):
-        """"
+        """
         Fetch Plan for given Id
 
         Args:
             plan_id : Id for which Plan object has to be retrieved
 
         Returns:
             Plan dict for given subscription Id
         """
         return super(Plan, self).fetch(plan_id, data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all plan entities
 
         Returns:
             Dictionary of plan data
         """
         return super(Plan, self).all(data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/qrcode.py` & `razorpay-1.4.1/razorpay/resources/qrcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Qrcode(Resource):
     def __init__(self, client=None):
         super(Qrcode, self).__init__(client)
-        self.base_url = URL.QRCODE_URL
+        self.base_url = URL.V1 + URL.QRCODE_URL
 
     def fetch(self, qrcode_id, data={}, **kwargs):
-        """"
+        """
         Fetch a Qr code
 
         Args:
             customer_id : Id for which customer object has to be retrieved
 
         Returns:
             Qrcode dict for given qrcode id
         """
         return super(Qrcode, self).fetch(qrcode_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create a QR Code
 
         Returns:
             QrCode Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
     
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch All Qr Code
 
         Returns:
             Qrcode dict
         """
         return super(Qrcode, self).all(data, **kwargs)
 
     def fetch_all_payments(self, qrcode_id,  data={}, **kwargs):
-        """"
+        """
         Fetch Payments for a QR Code
 
         Returns:
             Qrcode payment dict
         """
         url = "{}/{}/payments".format(self.base_url, qrcode_id)
         return self.get_url(url, data, **kwargs)   
 
     def close(self, qrcode_id, **kwargs):
-        """"
+        """
         Close a QR Code
 
         Returns:
             Qrcode Dict which was closed
         """
         url = '{}/{}/close'.format(self.base_url, qrcode_id)
```

### Comparing `razorpay-1.3.1/razorpay/resources/refund.py` & `razorpay-1.4.1/razorpay/resources/refund.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 from ..constants.url import URL
 import warnings
 
 
 class Refund(Resource):
     def __init__(self, client=None):
         super(Refund, self).__init__(client)
-        self.base_url = URL.REFUNDS_URL
+        self.base_url = URL.V1 + URL.REFUNDS_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release, use all",
                       DeprecationWarning)
         return self.all(data, **kwargs)
 
     def create(self, data={}, **kwargs):
         """
         Create refund for given payment id
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch All Refund
 
         Returns:
             Refund dict
         """
         return super(Refund, self).all(data, **kwargs)
 
     def fetch(self, refund_id, data={}, **kwargs):
-        """"
+        """
         Refund object for given paymnet Id
 
         Args:
             refund_id : Refund Id for which refund has to be retrieved
 
         Returns:
             Refund dict for given refund Id
         """
         return super(Refund, self).fetch(refund_id, data, **kwargs)
 
     def edit(self, refund_id, data={}, **kwargs):
-        """"
+        """
         Update Refund
 
         Returns:
             Refund Dict which was edited
         """
         url = "{}/{}".format(self.base_url, refund_id)
         return self.patch_url(url, data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/registration_link.py` & `razorpay-1.4.1/razorpay/resources/registration_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class RegistrationLink(Resource):
     def __init__(self, client=None):
         super(RegistrationLink, self).__init__(client)
-        self.base_url = URL.REGISTRATION_LINK_URL
+        self.base_url = URL.V1 + URL.REGISTRATION_LINK_URL
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create a Registration Link
         Args:
             customer : Details of the customer to whom the registration link will be sent.
             type* : In this case the value is link.
             currency* : Currency used in Order
             amount* : Amount of Order
             description : The count may not be greater than 100.
```

### Comparing `razorpay-1.3.1/razorpay/resources/settlement.py` & `razorpay-1.4.1/razorpay/resources/settlement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Settlement(Resource):
     def __init__(self, client=None):
         super(Settlement, self).__init__(client)
-        self.base_url = URL.SETTLEMENT_URL
+        self.base_url = URL.V1 + URL.SETTLEMENT_URL
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Settlement entities
 
         Returns:
             Dictionary of Settlement data
         """
         return super(Settlement, self).all(data, **kwargs)
 
     def fetch(self, settlement_id, data={}, **kwargs):
-        """"
+        """
         Fetch Settlement data for given Id
 
         Args:
             settlement_id : Id for which settlement object has to be retrieved
 
         Returns:
             settlement dict for given settlement id
         """
         return super(Settlement, self).fetch(settlement_id, data, **kwargs)
 
     def report(self, data={}, **kwargs):
-        """"
+        """
         Settlement report for a month
 
         Returns:
             settlement dict
         """
         url = "{}/recon/{}".format(self.base_url, 'combined')
         return self.get_url(url, data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/subscription.py` & `razorpay-1.4.1/razorpay/resources/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Subscription(Resource):
     def __init__(self, client=None):
         super(Subscription, self).__init__(client)
-        self.base_url = URL.SUBSCRIPTION_URL
+        self.base_url = URL.V1 + URL.SUBSCRIPTION_URL
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Subscription entities
 
         Returns:
             Dictionary of Subscription data
         """
         return super(Subscription, self).all(data, **kwargs)
 
     def fetch(self, subscription_id, data={}, **kwargs):
-        """"
+        """
         Fetch Subscription for given Id
 
         Args:
             subscription_id : Id for which subscription object is retrieved
 
         Returns:
             Subscription dict for given subscription Id
         """
         return super(Subscription, self).fetch(subscription_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Subscription from given dict
 
         Args:
             data : Dictionary using which Subscription has to be created
 
         Returns:
             Subscription Dict which was created
@@ -77,27 +77,27 @@
         Return:
             Subscription dict for given subscription id
         """
         url = "{}/{}/addons".format(self.base_url, subscription_id)
         return self.post_url(url, data, **kwargs) 
 
     def edit(self, subscription_id, data={}, **kwargs):
-        """"
+        """
          Update particular subscription
 
         Args:
             subscription_id : Id for which subscription has to be edited         
         Returns:
             Subscription dict for given subscription id
         """
         url = '{}/{}'.format(self.base_url, subscription_id)   
         return self.patch_url(url, data, **kwargs) 
 
     def pending_update(self, subscription_id, **kwargs):
-        """"
+        """
         Fetch Subscription for given Id
 
         Args:
             subscription_id : Id for which subscription object is retrieved
 
         Returns:
             Subscription dict for given subscription Id
```

### Comparing `razorpay-1.3.1/razorpay/resources/token.py` & `razorpay-1.4.1/razorpay/resources/token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,89 @@
 from .base import Resource
 from ..constants.url import URL
 
 
 class Token(Resource):
     def __init__(self, client=None):
         super(Token, self).__init__(client)
-        self.base_url = URL.CUSTOMER_URL
+        self.base_url = URL.V1 + URL.CUSTOMER_URL
+
+    def create(self, data={}, **kwargs):
+        """
+        Create token from given dict
+
+        Returns:
+            token Dict which was created
+        """
+        url = '{}{}'.format(URL.V1, URL.TOKEN)
+
+        return self.post_url(url, data, **kwargs)
 
     def fetch(self, customer_id, token_id, data={}, **kwargs):
-        """"
+        """
         Fetch Token for given Id and given customer Id
 
         Args:
             customer_id : Customer Id for which tokens have to be fetched
             token_id    : Id for which TOken object has to be fetched
 
         Returns:
             Token dict for given token Id
         """
         url = "{}/{}/tokens/{}".format(self.base_url, customer_id, token_id)
         return self.get_url(url, data, **kwargs)
 
     def all(self, customer_id, data={}, **kwargs):
-        """"
+        """
         Get all tokens for given customer Id
 
         Args:
             customer_id : Customer Id for which tokens have to be fetched
 
         Returns:
             Token dicts for given cutomer Id
         """
         url = "{}/{}/tokens".format(self.base_url, customer_id)
         return self.get_url(url, data, **kwargs)
 
     def delete(self, customer_id, token_id, data={}, **kwargs):
-        """"
+        """
         Delete Given Token For a Customer
 
         Args:
             customer_id : Customer Id for which tokens have to be deleted
             token_id    : Id for which TOken object has to be deleted
         Returns:
             Dict for deleted token
         """
         url = "{}/{}/tokens/{}".format(self.base_url, customer_id, token_id)
         return self.delete_url(url, data, **kwargs)
+
+    def fetchToken(self, data={}, **kwargs):
+        """
+        fetch Given Token For a Customer
+
+        Returns:
+            Dict for fetch token
+        """
+        url = '{}{}/{}'.format(URL.V1, URL.TOKEN, "fetch")
+        return self.post_url(url, data, **kwargs) 
+
+    def deleteToken(self, data={}, **kwargs):
+        """
+        Delete Given Token
+
+        Returns:
+            Dict for deleted token
+        """
+        url = '{}{}/{}'.format(URL.V1, URL.TOKEN, "delete")
+        return self.post_url(url, data, **kwargs) 
+
+    def processPaymentOnAlternatePAorPG(self, data={}, **kwargs):
+        """
+        Process a Payment on another PA/PG with Token Created on Razorpay
+
+        Returns:
+            
+        """
+        url = '{}{}/{}'.format(URL.V1, URL.TOKEN, "service_provider_tokens/token_transactional_data")
+        return self.post_url(url, data, **kwargs)
```

### Comparing `razorpay-1.3.1/razorpay/resources/transfer.py` & `razorpay-1.4.1/razorpay/resources/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,88 +2,88 @@
 from ..constants.url import URL
 import warnings
 
 
 class Transfer(Resource):
     def __init__(self, client=None):
         super(Transfer, self).__init__(client)
-        self.base_url = URL.TRANSFER_URL
+        self.base_url = URL.V1 + URL.TRANSFER_URL
 
     def fetch_all(self, data={}, **kwargs):  # pragma: no cover
         warnings.warn("Will be Deprecated in next release, use all",
                       DeprecationWarning)
         return self.all(data, **kwargs)
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Transfer entities
 
         Returns:
             Dictionary of Transfer data
         """
         if 'payment_id' in data:
-            url = "/payments/{}/transfers".format(data['payment_id'])
+            url = URL.V1 + "/payments/{}/transfers".format(data['payment_id'])
 
             del data['payment_id']
             return self.get_url(url, data, **kwargs)
 
         return super(Transfer, self).all(data, **kwargs)
 
     def fetch(self, transfer_id, data={}, **kwargs):
-        """"
+        """
         Fetch Transfer for given Id
 
         Args:
             transfer_id : Id for which transfer object has to be retrieved
 
         Returns:
             Transfer dict for given transfer Id
         """
         return super(Transfer, self).fetch(transfer_id, data, **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Transfer from given dict
 
         Args:
 
         Returns:
             Transfer Dict which was created
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def edit(self, transfer_id, data={}, **kwargs):
-        """"
+        """
         Edit Transfer from given id
 
         Args:
             transfer_id : Id for which transfer object has to be edited
 
         Returns:
             Transfer Dict which was edited
         """
         url = "{}/{}".format(self.base_url, transfer_id)
         return self.patch_url(url, data, **kwargs)
 
     def reverse(self, transfer_id, data={}, **kwargs):
-        """"
+        """
         Reverse Transfer from given id
 
         Args:
             transfer_id : Id for which transfer object has to be reversed
 
         Returns:
             Transfer Dict which was reversed
         """
         url = "{}/{}/reversals".format(self.base_url, transfer_id)
         return self.post_url(url, data, **kwargs)
 
     def reversals(self, transfer_id, data={}, **kwargs):
-        """"
+        """
         Get all Reversal Transfer from given id
 
         Args:
             transfer_id :
                 Id for which reversal transfer object has to be fetched
 
         Returns:
```

### Comparing `razorpay-1.3.1/razorpay/resources/virtual_account.py` & `razorpay-1.4.1/razorpay/resources/virtual_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from ..constants.url import URL
 import json
 
 
 class VirtualAccount(Resource):
     def __init__(self, client=None):
         super(VirtualAccount, self).__init__(client)
-        self.base_url = URL.VIRTUAL_ACCOUNT_URL
+        self.base_url = URL.V1 + URL.VIRTUAL_ACCOUNT_URL
 
     def all(self, data={}, **kwargs):
-        """"
+        """
         Fetch all Virtual Account entities
 
         Returns:
             Dictionary of Virtual Account data
         """
         return super(VirtualAccount, self).all(data, **kwargs)
 
     def fetch(self, virtual_account_id, data={}, **kwargs):
-        """"
+        """
         Fetch Virtual Account for given Id
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account object has to be retrieved
 
         Returns:
@@ -30,75 +30,75 @@
         """
         return super(VirtualAccount, self).fetch(
             virtual_account_id,
             data,
             **kwargs)
 
     def create(self, data={}, **kwargs):
-        """"
+        """
         Create Virtual Account from given dict
 
         Args:
             Param for Creating Virtual Account
 
         Returns:
             Virtual Account dict
         """
         url = self.base_url
         return self.post_url(url, data, **kwargs)
 
     def close(self, virtual_account_id, data={}, **kwargs):
-        """"
+        """
         Close Virtual Account from given Id
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account objects has to be Closed
         """
         url = "{}/{}/close".format(self.base_url, virtual_account_id)
         return self.post_url(url, data, **kwargs)
 
     def payments(self, virtual_account_id, data={}, **kwargs):
-        """"
+        """
         Fetch Payment for Virtual Account Id
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account objects has to be retrieved
 
         Returns:
             Payment dict for given Virtual Account Id
         """
         url = "{}/{}/payments".format(self.base_url, virtual_account_id)
         return self.get_url(url, data, **kwargs)
 
     def add_receiver(self, virtual_account_id, data={}, **kwargs):
-        """"
+        """
         Add receiver to an existing virtual account
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account objects has to be Closed
         """
         url = "{}/{}/receivers".format(self.base_url, virtual_account_id)
         return self.post_url(url, data, **kwargs)
 
     def add_allowed_player(self, virtual_account_id, data={}, **kwargs):
-        """"
+        """
         Add an Allowed Payer Account
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account objects has to be Closed
         """
         url = "{}/{}/allowed_payers".format(self.base_url, virtual_account_id)
         return self.post_url(url, data, **kwargs) 
 
     def delete_allowed_player(self, virtual_account_id, allowed_player_id, data={}, **kwargs):
-        """"
+        """
         Delete an Allowed Payer Account
 
         Args:
             virtual_account_id :
                 Id for which Virtual Account objects has to be Closed
         Returns:
             204
```

### Comparing `razorpay-1.3.1/razorpay/utility/utility.py` & `razorpay-1.4.1/razorpay/utility/utility.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/razorpay.egg-info/PKG-INFO` & `razorpay-1.4.1/razorpay.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: razorpay
-Version: 1.3.1
+Version: 1.4.1
 Summary: Razorpay Python Client
 Home-page: https://github.com/razorpay/razorpay-python
 Author: Team Razorpay
 License: MIT
 Keywords: razorpay payment gateway india
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Razorpay Python Client
 
-[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/pypi/pyversions/razorpay.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI Version](https://img.shields.io/pypi/v/razorpay.svg)](https://pypi.python.org/pypi/razorpay) [![Coverage Status](https://coveralls.io/repos/github/razorpay/razorpay-python/badge.svg?branch=master)](https://coveralls.io/github/razorpay/razorpay-python?branch=master) [![PyPI](https://img.shields.io/badge/python-3%20%7C%203.4%20%7C%203.5%20%7C%203.6-blue.svg)]() [![License](https://img.shields.io/:license-mit-blue.svg)](https://opensource.org/licenses/MIT)
 
 Python bindings for interacting with the Razorpay API
 
 This is primarily meant for merchants who wish to perform interactions with the Razorpay API programatically.
 
 ## Installation
 
@@ -53,14 +51,16 @@
 client.set_app_details({"title" : "<YOUR_APP_TITLE>", "version" : "<YOUR_APP_VERSION>"})
 ```
 
 For example, you can set the title to `Django` and version to `1.8.17`. Please ensure
 that both app title and version are strings.
 
 ## Supported Resources
+- [Account](documents/account.md)
+
 - [Addon](documents/addon.md)
 
 - [Item](documents/items.md)
 
 - [Customer](documents/customer.md)
 
 - [Token](documents/token.md)
@@ -96,14 +96,20 @@
 - [UPI](documents/upi.md)
 
 - [Register Emandate and Charge First Payment Together](documents/registerEmandate.md)
 
 - [Register NACH and Charge First Payment Together](documents/registerNach.md)
 
 - [Payment Verification](documents/paymentVerfication.md)
+
+- [Product Configuration](documents/productConfiguration.md)
+
+- [Stakeholder](documents/stakeholder.md)
+
+- [Webhook](documents/webhook.md)
 ---
 
 ## Bugs? Feature requests? Pull requests?
 
 All of those are welcome. You can [file issues][issues] or [submit pull requests][pulls] in this repository.
 
 [issues]: https://github.com/razorpay/razorpay-python/issues
```

### Comparing `razorpay-1.3.1/razorpay.egg-info/SOURCES.txt` & `razorpay-1.4.1/razorpay.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,120 +12,140 @@
 razorpay.egg-info/requires.txt
 razorpay.egg-info/top_level.txt
 razorpay/constants/__init__.py
 razorpay/constants/error_code.py
 razorpay/constants/http_status_code.py
 razorpay/constants/url.py
 razorpay/resources/__init__.py
+razorpay/resources/account.py
 razorpay/resources/addon.py
 razorpay/resources/base.py
 razorpay/resources/card.py
 razorpay/resources/customer.py
 razorpay/resources/fund_account.py
+razorpay/resources/iin.py
 razorpay/resources/invoice.py
 razorpay/resources/item.py
 razorpay/resources/order.py
 razorpay/resources/payment.py
 razorpay/resources/payment_link.py
 razorpay/resources/plan.py
+razorpay/resources/product.py
 razorpay/resources/qrcode.py
 razorpay/resources/refund.py
 razorpay/resources/registration_link.py
 razorpay/resources/settlement.py
+razorpay/resources/stakeholder.py
 razorpay/resources/subscription.py
 razorpay/resources/token.py
 razorpay/resources/transfer.py
 razorpay/resources/virtual_account.py
+razorpay/resources/webhook.py
 razorpay/utility/__init__.py
 razorpay/utility/utility.py
 tests/__init__.py
 tests/helpers.py
+tests/test_client_account.py
 tests/test_client_addon.py
 tests/test_client_card.py
 tests/test_client_customer.py
 tests/test_client_error.py
 tests/test_client_fund_account.py
+tests/test_client_iin.py
 tests/test_client_invoice.py
 tests/test_client_item.py
 tests/test_client_order.py
 tests/test_client_payment.py
 tests/test_client_payment_link.py
 tests/test_client_plan.py
+tests/test_client_product.py
 tests/test_client_qrcode.py
 tests/test_client_refund.py
 tests/test_client_registration_link.py
 tests/test_client_settlement.py
+tests/test_client_stakeholder.py
 tests/test_client_subscription.py
 tests/test_client_token.py
 tests/test_client_transfer.py
 tests/test_client_utility.py
 tests/test_client_virtual_account.py
+tests/test_client_webhook.py
 tests/test_multiple_client.py
 tests/test_user_agent.py
 tests/mocks/addon_collection.json
 tests/mocks/bad_request_error.json
 tests/mocks/cancel_payment_link.json
 tests/mocks/customer_collection.json
 tests/mocks/edit_customer.json
 tests/mocks/edit_order.json
 tests/mocks/edit_payment.json
 tests/mocks/edit_payment_link.json
+tests/mocks/fake_account.json
 tests/mocks/fake_addon.json
 tests/mocks/fake_app_details.json
 tests/mocks/fake_bank_transfer.json
 tests/mocks/fake_captured_payment.json
 tests/mocks/fake_card.json
 tests/mocks/fake_card_detail_payment.json
 tests/mocks/fake_create_recurring.json
 tests/mocks/fake_customer.json
 tests/mocks/fake_delete_allowed_payer.json
+tests/mocks/fake_iin.json
 tests/mocks/fake_invoice.json
 tests/mocks/fake_invoice_cancel.json
 tests/mocks/fake_invoice_delete.json
 tests/mocks/fake_invoice_edit.json
 tests/mocks/fake_invoice_notify_by.json
 tests/mocks/fake_item.json
+tests/mocks/fake_merchant_token.json
 tests/mocks/fake_order.json
 tests/mocks/fake_otp_generate.json
 tests/mocks/fake_otp_resend.json
 tests/mocks/fake_otp_submit.json
 tests/mocks/fake_payment.json
 tests/mocks/fake_payment_authorized_webhook.json
 tests/mocks/fake_payment_json.json
 tests/mocks/fake_payment_link.json
 tests/mocks/fake_plan.json
+tests/mocks/fake_product.json
 tests/mocks/fake_qrcode.json
+tests/mocks/fake_reference_card.json
 tests/mocks/fake_refund.json
 tests/mocks/fake_registration_link.json
 tests/mocks/fake_reversal.json
 tests/mocks/fake_settlement.json
+tests/mocks/fake_stakeholder.json
 tests/mocks/fake_subscription.json
 tests/mocks/fake_subscription_addon.json
 tests/mocks/fake_subscription_cancelled.json
 tests/mocks/fake_subscription_paused.json
 tests/mocks/fake_subscription_resumed.json
 tests/mocks/fake_token.json
 tests/mocks/fake_transfer.json
 tests/mocks/fake_upi_transfer.json
 tests/mocks/fake_virtual_accounts.json
 tests/mocks/fake_virtual_accounts_closed.json
 tests/mocks/fake_virtual_accounts_receiver.json
+tests/mocks/fake_webhook.json
 tests/mocks/fund_account_collection.json
+tests/mocks/init_account.json
 tests/mocks/init_create_recurring.json
 tests/mocks/init_customer.json
 tests/mocks/init_invoice.json
 tests/mocks/init_invoice_edit.json
 tests/mocks/init_order.json
 tests/mocks/init_payment_link.json
 tests/mocks/init_plan.json
 tests/mocks/init_registration_link.json
 tests/mocks/init_settlement.json
+tests/mocks/init_stakeholder.json
 tests/mocks/init_subscription.json
 tests/mocks/init_transfer.json
 tests/mocks/init_virtual_accounts.json
+tests/mocks/init_webhook.json
 tests/mocks/invoice_collection.json
 tests/mocks/invoice_collection_with_one_invoice.json
 tests/mocks/item_collection.json
 tests/mocks/order_collection.json
 tests/mocks/order_collection_with_one_order.json
 tests/mocks/payment_collection.json
 tests/mocks/payment_collection_with_one_payment.json
@@ -133,14 +153,16 @@
 tests/mocks/plan_collection.json
 tests/mocks/qrcode_collection.json
 tests/mocks/qrcode_payments_collection.json
 tests/mocks/refund_collection.json
 tests/mocks/reversal_collection.json
 tests/mocks/settlement_collection.json
 tests/mocks/settlement_collection_with_one_settlement.json
+tests/mocks/stakeholder_collection.json
 tests/mocks/subscription_collection.json
 tests/mocks/token_collection.json
 tests/mocks/token_collection_with_one_token.json
 tests/mocks/transfers_collection.json
 tests/mocks/transfers_collection_with_payment_id.json
 tests/mocks/virtual_accounts_collection.json
-tests/mocks/virtual_accounts_collection_with_one_item.json
+tests/mocks/virtual_accounts_collection_with_one_item.json
+tests/mocks/webhook_collection.json
```

### Comparing `razorpay-1.3.1/setup.py` & `razorpay-1.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme:
     readme_content = readme.read()
 
 setup(
     name="razorpay",
-    version="1.3.1",
+    version="1.4.1",
     description="Razorpay Python Client",
     long_description=readme_content,
     long_description_content_type='text/markdown',
     url="https://github.com/razorpay/razorpay-python",
     author="Team Razorpay",
     license="MIT",
     install_requires=["requests"],
@@ -21,16 +21,14 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
 
         # List of supported Python versions
         # Make sure that this is reflected in .github/workflows/python.yml as well
         "Programming Language :: Python",
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
 
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
```

### Comparing `razorpay-1.3.1/tests/helpers.py` & `razorpay-1.4.1/tests/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,18 @@
         mock_file_data = f.read()
     return mock_file_data
 
 
 class ClientTestCase(unittest.TestCase):
     def setUp(self):
         self.base_url = 'https://api.razorpay.com/v1'
-        self.secondary_url = 'https://test-api.razorpay.com/v1'
+        self.base_url_v2 = 'https://api.razorpay.com/v2'
+        self.secondary_url = 'https://test-api.razorpay.com'
+        self.v1 = 'v1'
+        self.v2 = 'v2'
         self.payment_id = 'fake_payment_id'
         self.refund_id = 'fake_refund_id'
         self.card_id = 'fake_card_id'
         self.customer_id = 'fake_customer_id'
         self.token_id = 'fake_token_id'
         self.addon_id = 'fake_addon_id'
         self.subscription_id = 'fake_subscription_id'
```

### Comparing `razorpay-1.3.1/tests/mocks/addon_collection.json` & `razorpay-1.4.1/tests/mocks/addon_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/cancel_payment_link.json` & `razorpay-1.4.1/tests/mocks/cancel_payment_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/edit_payment.json` & `razorpay-1.4.1/tests/mocks/edit_payment.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/edit_payment_link.json` & `razorpay-1.4.1/tests/mocks/edit_payment_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_addon.json` & `razorpay-1.4.1/tests/mocks/fake_addon.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_invoice.json` & `razorpay-1.4.1/tests/mocks/fake_invoice.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_invoice_cancel.json` & `razorpay-1.4.1/tests/mocks/fake_invoice_cancel.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_invoice_edit.json` & `razorpay-1.4.1/tests/mocks/fake_invoice_edit.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_otp_generate.json` & `razorpay-1.4.1/tests/mocks/fake_otp_generate.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_payment_authorized_webhook.json` & `razorpay-1.4.1/tests/mocks/fake_payment_authorized_webhook.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_payment_json.json` & `razorpay-1.4.1/tests/mocks/fake_payment_json.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_payment_link.json` & `razorpay-1.4.1/tests/mocks/fake_payment_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_qrcode.json` & `razorpay-1.4.1/tests/mocks/fake_qrcode.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_registration_link.json` & `razorpay-1.4.1/tests/mocks/fake_registration_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_subscription_addon.json` & `razorpay-1.4.1/tests/mocks/fake_subscription_addon.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_subscription_paused.json` & `razorpay-1.4.1/tests/mocks/fake_subscription_paused.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_subscription_resumed.json` & `razorpay-1.4.1/tests/mocks/fake_subscription_resumed.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fake_virtual_accounts_receiver.json` & `razorpay-1.4.1/tests/mocks/fake_virtual_accounts_receiver.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/fund_account_collection.json` & `razorpay-1.4.1/tests/mocks/fund_account_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/init_payment_link.json` & `razorpay-1.4.1/tests/mocks/init_payment_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/init_registration_link.json` & `razorpay-1.4.1/tests/mocks/init_registration_link.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/init_settlement.json` & `razorpay-1.4.1/tests/mocks/init_settlement.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/invoice_collection.json` & `razorpay-1.4.1/tests/mocks/invoice_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/invoice_collection_with_one_invoice.json` & `razorpay-1.4.1/tests/mocks/invoice_collection_with_one_invoice.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/item_collection.json` & `razorpay-1.4.1/tests/mocks/item_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/order_collection.json` & `razorpay-1.4.1/tests/mocks/order_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/payment_collection.json` & `razorpay-1.4.1/tests/mocks/payment_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/payment_link_collection.json` & `razorpay-1.4.1/tests/mocks/payment_link_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/plan_collection.json` & `razorpay-1.4.1/tests/mocks/plan_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/qrcode_collection.json` & `razorpay-1.4.1/tests/mocks/qrcode_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/qrcode_payments_collection.json` & `razorpay-1.4.1/tests/mocks/qrcode_payments_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/settlement_collection.json` & `razorpay-1.4.1/tests/mocks/settlement_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/subscription_collection.json` & `razorpay-1.4.1/tests/mocks/subscription_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/token_collection.json` & `razorpay-1.4.1/tests/mocks/token_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/transfers_collection.json` & `razorpay-1.4.1/tests/mocks/transfers_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/virtual_accounts_collection.json` & `razorpay-1.4.1/tests/mocks/virtual_accounts_collection.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/mocks/virtual_accounts_collection_with_one_item.json` & `razorpay-1.4.1/tests/mocks/virtual_accounts_collection_with_one_item.json`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_addon.py` & `razorpay-1.4.1/tests/test_client_addon.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_card.py` & `razorpay-1.4.1/tests/test_client_iin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import responses
 import json
 
 from .helpers import mock_file, ClientTestCase
 
 
-class TestClientRefund(ClientTestCase):
+class TestClientIin(ClientTestCase):
 
     def setUp(self):
-        super(TestClientRefund, self).setUp()
-        self.base_url = '{}/cards'.format(self.base_url)
+        super(TestClientIin, self).setUp()
+        self.base_url = '{}/iins'.format(self.base_url)
+        self.token_iin = '412345'
 
     @responses.activate
-    def test_card_fetch(self):
-        result = mock_file('fake_card')
-        url = '{}/{}'.format(self.base_url, self.card_id)
+    def test_addon_fetch(self):
+        result = mock_file('fake_iin')
+        url = '{}/{}'.format(self.base_url, self.token_iin)
         responses.add(responses.GET, url, status=200, body=json.dumps(result),
                       match_querystring=True)
-        self.assertEqual(self.client.card.fetch(self.card_id), result)
+        self.assertEqual(self.client.iin.fetch(self.token_iin), result)
```

### Comparing `razorpay-1.3.1/tests/test_client_customer.py` & `razorpay-1.4.1/tests/test_client_customer.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_error.py` & `razorpay-1.4.1/tests/test_client_error.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_fund_account.py` & `razorpay-1.4.1/tests/test_client_fund_account.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_invoice.py` & `razorpay-1.4.1/tests/test_client_invoice.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_item.py` & `razorpay-1.4.1/tests/test_client_item.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_order.py` & `razorpay-1.4.1/tests/test_client_order.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_payment.py` & `razorpay-1.4.1/tests/test_client_payment.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_payment_link.py` & `razorpay-1.4.1/tests/test_client_payment_link.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_plan.py` & `razorpay-1.4.1/tests/test_client_plan.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_qrcode.py` & `razorpay-1.4.1/tests/test_client_qrcode.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_refund.py` & `razorpay-1.4.1/tests/test_client_refund.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_registration_link.py` & `razorpay-1.4.1/tests/test_client_registration_link.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_settlement.py` & `razorpay-1.4.1/tests/test_client_settlement.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_subscription.py` & `razorpay-1.4.1/tests/test_client_subscription.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_token.py` & `razorpay-1.4.1/tests/test_client_account.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import responses
 import json
 
 from .helpers import mock_file, ClientTestCase
 
 
-class TestClientCustomer(ClientTestCase):
+class TestClientAccount(ClientTestCase):
 
     def setUp(self):
-        super(TestClientCustomer, self).setUp()
-        self.base_url = '{}/customers'.format(self.base_url)
+        super(TestClientAccount, self).setUp()
+        self.base_url = '{}/accounts'.format(self.base_url_v2)
+        self.account_id = 'acc_GRWKk7qQsLnDjX'
 
     @responses.activate
-    def test_tokens_all(self):
-        result = mock_file('token_collection')
-        url = '{}/{}/tokens'.format(self.base_url, self.customer_id)
-        responses.add(responses.GET, url, status=200, body=json.dumps(result),
+    def test_account_create(self):
+        init = mock_file('init_account')
+        result = mock_file('fake_account')
+        url = self.base_url
+        responses.add(responses.POST,
+                      url,
+                      status=200,
+                      body=json.dumps(result),
                       match_querystring=True)
-        self.assertEqual(self.client.token.all(self.customer_id),
-                         result)
 
+        self.assertEqual(self.client.account.create(init), result)
+    
     @responses.activate
-    def test_token_fetch(self):
-        result = mock_file('token_collection')
-        url = '{}/{}/tokens/{}'.format(self.base_url,
-                                       self.customer_id,
-                                       self.token_id)
+    def test_account_fetch(self):
+        result = mock_file('fake_account')
+        url = '{}/{}'.format(self.base_url, self.account_id)
         responses.add(responses.GET, url, status=200, body=json.dumps(result),
                       match_querystring=True)
-        self.assertEqual(
-            self.client.token.fetch(self.customer_id, self.token_id),
-            result)
+        self.assertEqual(self.client.account.fetch(self.account_id), result)
 
     @responses.activate
-    def test_token_delete(self):
-        url = '{}/{}/tokens/{}'.format(self.base_url,
-                                       self.customer_id,
-                                       self.token_id)
-        responses.add(responses.DELETE,
-                      url,
-                      status=200,
-                      body=json.dumps({'deleted': True}),
+    def test_account_edit(self):
+        init = { "customer_facing_business_name": "ABCD Ltd" }
+        result = mock_file('fake_account')
+        url = '{}/{}'.format(self.base_url, self.account_id)
+        responses.add(responses.PATCH, url, status=200, body=json.dumps(result),
+                      match_querystring=True)
+        self.assertEqual(self.client.account.edit(self.account_id, init), result)        
+        
+    @responses.activate
+    def test_account_delete(self):
+        result = mock_file('fake_account')
+        url = '{}/{}'.format(self.base_url, self.account_id)
+        responses.add(responses.DELETE, url, status=200, body=json.dumps(result),
                       match_querystring=True)
-        self.assertEqual(
-            self.client.token.delete(self.customer_id, self.token_id),
-            {'deleted': True})
+        self.assertEqual(self.client.account.delete(self.account_id), result)
```

### Comparing `razorpay-1.3.1/tests/test_client_transfer.py` & `razorpay-1.4.1/tests/test_client_transfer.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_utility.py` & `razorpay-1.4.1/tests/test_client_utility.py`

 * *Files identical despite different names*

### Comparing `razorpay-1.3.1/tests/test_client_virtual_account.py` & `razorpay-1.4.1/tests/test_client_virtual_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,19 +148,18 @@
             self.fake_virtual_account_id, init)   
         self.assertEqual(response['id'], self.fake_virtual_account_id)
         self.assertEqual(response['entity'], 'virtual_account')
 
    
     @unittest.skip
     def test_virtual_delete_allowed_player(self):
-        result = mock_file('fake_delete_allowed_payer')
+        result = None
         url = "{}/{}/allowed_payers/{}".format(self.base_url, self.fake_virtual_account_id, 'fake_allowed_player_id')
         responses.add(responses.DELETE,
                       url,
                       status=204,
                       body=result,
                       match_querystring=True)
         response = self.client.virtual_account.delete_allowed_player(
         self.fake_virtual_account_id, 'fake_allowed_player_id');   
         self.assertEqual(response, result)
           
-
```

### Comparing `razorpay-1.3.1/tests/test_multiple_client.py` & `razorpay-1.4.1/tests/test_multiple_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import unittest
 import responses
 import json
 
 from .helpers import mock_file, ClientTestCase
 
 
 class TestClientPayment(ClientTestCase):
@@ -15,15 +16,15 @@
     def test_payment_primary_url(self):
         result = mock_file('payment_collection')
         url = self.base_url
         responses.add(responses.GET, url, status=200,
                       body=json.dumps(result), match_querystring=True)
         self.assertEqual(self.client.payment.all(), result)
 
-    @responses.activate
+    @unittest.skip
     def test_payment_secondary_url(self):
         result = mock_file('payment_collection')
         url = self.secondary_base_url
         responses.add(responses.GET, url, status=200,
                       body=json.dumps(result), match_querystring=True)
         self.assertEqual(self.secondary_client.payment.all(), result)
```

### Comparing `razorpay-1.3.1/tests/test_user_agent.py` & `razorpay-1.4.1/tests/test_user_agent.py`

 * *Files identical despite different names*

