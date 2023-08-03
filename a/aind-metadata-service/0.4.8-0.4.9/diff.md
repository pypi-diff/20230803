# Comparing `tmp/aind_metadata_service-0.4.8.tar.gz` & `tmp/aind_metadata_service-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.8.tar", last modified: Sat Jun  3 00:35:56 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.9.tar", last modified: Mon Jun 12 18:57:15 2023, max compression
```

## Comparing `aind_metadata_service-0.4.8.tar` & `aind_metadata_service-0.4.9.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 00:35:37.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113301 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_sp_procedure.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item19.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item18.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 18:56:57.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113301 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-12 18:57:15.000000 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-12 18:57:15.000000 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:57:15.000000 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-12 18:57:15.000000 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 18:57:15.000000 aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.089430 aind_metadata_service-0.4.9/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.093430 aind_metadata_service-0.4.9/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.093430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.093430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.085430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.093430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:15.097430 aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-12 18:56:56.000000 aind_metadata_service-0.4.9/tests/test_response_handler.py
```

### Comparing `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.9/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/.github/workflows/ci.yml` & `aind_metadata_service-0.4.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/.github/workflows/publish.yml` & `aind_metadata_service-0.4.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/.gitignore` & `aind_metadata_service-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/Dockerfile` & `aind_metadata_service-0.4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/LICENSE` & `aind_metadata_service-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/PKG-INFO` & `aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aind_metadata_service
-Version: 0.4.8
+Name: aind-metadata-service
+Version: 0.4.9
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.8/README.md` & `aind_metadata_service-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/doc_template/Makefile` & `aind_metadata_service-0.4.9/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/doc_template/make.bat` & `aind_metadata_service-0.4.9/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.9/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/doc_template/source/conf.py` & `aind_metadata_service-0.4.9/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/pyproject.toml` & `aind_metadata_service-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'flake8',
     'interrogate',
     'isort',
     'Sphinx'
 ]
 
 server = [
-    'aind-data-schema==0.13.43',
+    'aind-data-schema==0.13.50',
     'pyodbc',
     'office365-rest-python-client',
     'fastapi',
     'uvicorn[standard]',
     'python-dateutil'
 ]
```

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/procedures.py` & `aind_metadata_service-0.4.9/src/aind_metadata_service/sharepoint/nsb2023/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aind-metadata-service
-Version: 0.4.8
+Name: aind_metadata_service
+Version: 0.4.9
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.9/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.9/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.9/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.9/tests/labtracks/test_response_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             "group_name": "C57BL6J_OLD",
             "group_description": "C57BL/6J",
         }
     ]
 
     expected_subject = Subject.parse_obj(
         {
-            "schema_version": "0.3.2",
+            "schema_version": "0.4.1",
             "species": Species.MUS_MUSCULUS,
             "subject_id": "115977",
             "sex": "Male",
             "date_of_birth": "2012-05-13",
             "genotype": "Adora2a-Cre/wt",
             "maternal_id": "107392",
             "maternal_genotype": "wt/wt",
@@ -126,15 +126,15 @@
             notes=None,
             procedure_type="Retro-orbital injection",
         ),
     ]
 
     expected_procedures = Procedures.parse_obj(
         {
-            "schema_version": "0.7.8",
+            "schema_version": "0.8.1",
             "subject_id": "115977",
             "subject_procedures": expected_subject_procedures,
         }
     )
 
 
 class TestLabTracksResponseHandler(unittest.TestCase):
```

### Comparing `aind_metadata_service-0.4.8/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.4.9/tests/resources/json_responses/combined.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'data'": "{'schema_version': '0.8.1'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "data": {
         "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/procedures.py",
         "notes": null,
-        "schema_version": "0.7.8",
+        "schema_version": "0.8.1",
         "specimen_procedures": [],
         "subject_id": "115977",
         "subject_procedures": [
             {
                 "anaesthesia": null,
                 "animal_weight_post": null,
                 "animal_weight_prior": null,
```

### Comparing `aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.4.9/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'data'": "{'schema_version': '0.8.1'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "data": {
         "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/procedures.py",
         "notes": null,
-        "schema_version": "0.7.8",
+        "schema_version": "0.8.1",
         "specimen_procedures": [],
         "subject_id": "115977",
         "subject_procedures": [
             {
                 "anaesthesia": null,
                 "animal_weight_post": null,
                 "animal_weight_prior": null,
```

### Comparing `aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.4.9/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'data'": "{'schema_version': '0.8.1'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "data": {
         "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/procedures.py",
         "notes": null,
-        "schema_version": "0.7.8",
+        "schema_version": "0.8.1",
         "specimen_procedures": [],
         "subject_id": "115977",
         "subject_procedures": [
             {
                 "anaesthesia": null,
                 "animal_weight_post": null,
                 "animal_weight_prior": null,
```

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item19.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item19.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item18.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item18.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.9/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.9/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.9/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.9/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/test_client.py` & `aind_metadata_service-0.4.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.8/tests/test_response_handler.py` & `aind_metadata_service-0.4.9/tests/test_response_handler.py`

 * *Files identical despite different names*

