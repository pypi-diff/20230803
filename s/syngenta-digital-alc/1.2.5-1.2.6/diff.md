# Comparing `tmp/syngenta_digital_alc-1.2.5.tar.gz` & `tmp/syngenta_digital_alc-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngenta_digital_alc-1.2.5.tar", last modified: Wed Jun 21 17:45:33 2023, max compression
+gzip compressed data, was "syngenta_digital_alc-1.2.6.tar", last modified: Thu Aug  3 16:57:20 2023, max compression
```

## Comparing `syngenta_digital_alc-1.2.5.tar` & `syngenta_digital_alc-1.2.6.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.298652 syngenta_digital_alc-1.2.5/
--rw-r--r--   0 dbankhead   (501) staff       (20)    11357 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/LICENSE
--rw-r--r--   0 dbankhead   (501) staff       (20)    14528 2023-06-21 17:45:33.298760 syngenta_digital_alc-1.2.5/PKG-INFO
--rw-r--r--   0 dbankhead   (501) staff       (20)    13661 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/README.md
--rw-r--r--   0 dbankhead   (501) staff       (20)       68 2023-06-21 17:45:33.299204 syngenta_digital_alc-1.2.5/setup.cfg
--rw-r--r--   0 dbankhead   (501) staff       (20)     1239 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/setup.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.289495 syngenta_digital_alc-1.2.5/syngenta_digital_alc/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.291239 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      283 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/custom_exceptions.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      729 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/handler_requirements.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2146 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3716 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_validator.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3056 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/response_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3509 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/router.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.291766 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      339 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/json_helper.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2194 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/logger.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      724 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/troubleshoot_decorator.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.292300 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      480 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      294 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/handler_requirements.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2161 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.292697 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/
--rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      329 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      293 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/handler_requirements.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.293303 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/
--rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      478 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      288 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/handler_requirements.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1797 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.293818 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/
--rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      479 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      288 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/handler_requirements.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2026 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294398 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/
--rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      479 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      289 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/handler_requirements.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2395 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.290037 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/
--rw-r--r--   0 dbankhead   (501) staff       (20)    14528 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/PKG-INFO
--rw-r--r--   0 dbankhead   (501) staff       (20)     3181 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/SOURCES.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)        1 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/dependency_links.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)       51 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/requires.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)       27 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/top_level.txt
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294528 syngenta_digital_alc-1.2.5/tests/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/__init__.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294605 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.295812 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      464 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_before_all.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     5161 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      192 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_handler.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2665 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3478 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3923 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_validator.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1682 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_response.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1956 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_router.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296047 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1913 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/test_logger.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296391 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     5188 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1371 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/test_event_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296739 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)       82 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      551 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/test_event_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.297224 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1591 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2942 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1993 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.297819 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1175 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1773 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     1970 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_record_client.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.298518 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/
--rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     3279 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/mock_data.py
--rw-r--r--   0 dbankhead   (501) staff       (20)      570 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_event_client.py
--rw-r--r--   0 dbankhead   (501) staff       (20)     2430 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14528 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13661 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-08-03 16:57:20.644906 syngenta_digital_alc-1.2.6/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.624906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/custom_exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/error_handling/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/error_handling/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/error_handling/timeout.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2146 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/request_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3716 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/request_validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/response_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3509 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/router.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/json_helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/troubleshoot_decorator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/generic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/generic/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/generic/handler_requirements.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2395 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.628906 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14528 2023-08-03 16:57:20.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3361 2023-08-03 16:57:20.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-03 16:57:20.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2023-08-03 16:57:20.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-08-03 16:57:20.000000 syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/mock_before_all.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5161 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/mock_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2665 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_request_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_request_validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1956 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_router.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_timeout_handling.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1913 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/common/test_logger.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.632906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5188 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1371 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/test_event_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/generic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/generic/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/generic/test_event_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1591 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2942 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1970 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:20.636906 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3279 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-08-03 16:57:08.000000 syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/test_record_client.py
```

### Comparing `syngenta_digital_alc-1.2.5/LICENSE` & `syngenta_digital_alc-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/PKG-INFO` & `syngenta_digital_alc-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_alc
-Version: 1.2.5
+Version: 1.2.6
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_alc-1.2.5/README.md` & `syngenta_digital_alc-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/setup.py` & `syngenta_digital_alc-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_validator.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/request_validator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/response_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/response_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/router.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/apigateway/router.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/logger.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/troubleshoot_decorator.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/common/troubleshoot_decorator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/record_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/dynamodb/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/record_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/s3/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/record_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/sns/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/record_client.py` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc/sqs/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/PKG-INFO` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-alc
-Version: 1.2.5
+Version: 1.2.6
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/SOURCES.txt` & `syngenta_digital_alc-1.2.6/syngenta_digital_alc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 syngenta_digital_alc/apigateway/__init__.py
 syngenta_digital_alc/apigateway/custom_exceptions.py
 syngenta_digital_alc/apigateway/handler_requirements.py
 syngenta_digital_alc/apigateway/request_client.py
 syngenta_digital_alc/apigateway/request_validator.py
 syngenta_digital_alc/apigateway/response_client.py
 syngenta_digital_alc/apigateway/router.py
+syngenta_digital_alc/apigateway/error_handling/__init__.py
+syngenta_digital_alc/apigateway/error_handling/timeout.py
 syngenta_digital_alc/common/__init__.py
 syngenta_digital_alc/common/json_helper.py
 syngenta_digital_alc/common/logger.py
 syngenta_digital_alc/common/troubleshoot_decorator.py
 syngenta_digital_alc/dynamodb/__init__.py
 syngenta_digital_alc/dynamodb/event_client.py
 syngenta_digital_alc/dynamodb/handler_requirements.py
@@ -45,14 +47,15 @@
 tests/syngenta_digital_alc/apigateway/mock_data.py
 tests/syngenta_digital_alc/apigateway/mock_handler.py
 tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
 tests/syngenta_digital_alc/apigateway/test_request_client.py
 tests/syngenta_digital_alc/apigateway/test_request_validator.py
 tests/syngenta_digital_alc/apigateway/test_response.py
 tests/syngenta_digital_alc/apigateway/test_router.py
+tests/syngenta_digital_alc/apigateway/test_timeout_handling.py
 tests/syngenta_digital_alc/common/__init__.py
 tests/syngenta_digital_alc/common/test_logger.py
 tests/syngenta_digital_alc/dynamodb/__init__.py
 tests/syngenta_digital_alc/dynamodb/mock_data.py
 tests/syngenta_digital_alc/dynamodb/test_event_client.py
 tests/syngenta_digital_alc/generic/__init__.py
 tests/syngenta_digital_alc/generic/mock_data.py
```

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_data.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_validator.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_request_validator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_response.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_response.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_router.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/apigateway/test_router.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/test_logger.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/mock_data.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/test_event_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/dynamodb/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/test_event_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/generic/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/mock_data.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_event_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_record_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/s3/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/mock_data.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_event_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_record_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sns/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/mock_data.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_event_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_record_client.py` & `syngenta_digital_alc-1.2.6/tests/syngenta_digital_alc/sqs/test_record_client.py`

 * *Files identical despite different names*

