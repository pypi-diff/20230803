# Comparing `tmp/lendsmart_reva-1.6.tar.gz` & `tmp/lendsmart_reva-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_reva-1.6.tar", last modified: Tue Aug  1 06:40:20 2023, max compression
+gzip compressed data, was "lendsmart_reva-1.7.tar", last modified: Thu Aug  3 06:07:59 2023, max compression
```

## Comparing `lendsmart_reva-1.6.tar` & `lendsmart_reva-1.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/lendsmart_reva.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2109 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      531 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      158 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-08-01 06:40:20.000000 lendsmart_reva-1.6/lendsmart_reva.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      907 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/advisor_profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/autotest.py
--rw-rw-r--   0 user      (1000) user      (1000)      839 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/branch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/conf/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/conf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/conf/reva.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)      954 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/info.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/advisor_profile/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9937 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/create.py
--rw-rw-r--   0 user      (1000) user      (1000)      483 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/advisor_profile/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/auto/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/auto/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/auto/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1840 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      950 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/base/run_query.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/branch/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3452 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/create.py
--rw-rw-r--   0 user      (1000) user      (1000)      439 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/branch/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/client/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      684 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/builder.py
--rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/client/graphql_client.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.058670 lendsmart_reva-1.6/reva/lib/document_access_control/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      728 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/document_access_control/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/graphql_queries/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1954 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/advisor_profiles.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/branch.py
--rw-rw-r--   0 user      (1000) user      (1000)      806 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)      641 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)      386 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/namespace.py
--rw-rw-r--   0 user      (1000) user      (1000)      944 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      590 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      802 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/graphql_queries/workflow.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/loan_productus/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      642 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/loan_productus/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/roles_and_permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      687 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/roles_and_permissions/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/site_settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/site_settings/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      507 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/address.py
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/filter_data_with_id.py
--rw-rw-r--   0 user      (1000) user      (1000)     2634 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_json_files.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/get_paths.py
--rw-rw-r--   0 user      (1000) user      (1000)      236 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/utils/list_files.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/reva/lib/workflow/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      608 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/lib/workflow/update.py
--rw-rw-r--   0 user      (1000) user      (1000)      878 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)      933 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      853 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      820 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/reva/workflow.py
--rw-rw-r--   0 user      (1000) user      (1000)       86 2023-08-01 06:40:20.062670 lendsmart_reva-1.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2257 2023-08-01 06:38:53.000000 lendsmart_reva-1.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/lendsmart_reva.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2109 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      531 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      158 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-08-03 06:07:59.000000 lendsmart_reva-1.7/lendsmart_reva.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      907 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/advisor_profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/autotest.py
+-rw-rw-r--   0 user      (1000) user      (1000)      839 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/conf/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/conf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/conf/reva.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/info.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/advisor_profile/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/advisor_profile/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10215 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/advisor_profile/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      483 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/advisor_profile/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/auto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/auto/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1840 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/base/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      950 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/base/run_query.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/branch/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/branch/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3452 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/branch/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/branch/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      684 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/client/builder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/client/graphql_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.529999 lendsmart_reva-1.7/reva/lib/document_access_control/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/document_access_control/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/document_access_control/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/document_access_control/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/graphql_queries/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1954 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/advisor_profiles.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)      806 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)      641 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/namespace.py
+-rw-rw-r--   0 user      (1000) user      (1000)      944 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      590 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/graphql_queries/workflow.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/loan_productus/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/loan_productus/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/loan_productus/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/loan_productus/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/roles_and_permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/roles_and_permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      687 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/roles_and_permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/roles_and_permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/site_settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/site_settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/site_settings/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/site_settings/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      507 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/address.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/filter_data_with_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2634 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/get_json_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/get_namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/get_paths.py
+-rw-rw-r--   0 user      (1000) user      (1000)      236 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/utils/list_files.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/reva/lib/workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      608 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/workflow/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/lib/workflow/update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      878 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      933 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/reva/workflow.py
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2023-08-03 06:07:59.533999 lendsmart_reva-1.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2257 2023-08-03 06:06:20.000000 lendsmart_reva-1.7/setup.py
```

### Comparing `lendsmart_reva-1.6/PKG-INFO` & `lendsmart_reva-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart_reva
-Version: 1.6
+Version: 1.7
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.6/README.md` & `lendsmart_reva-1.7/README.md`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/lendsmart_reva.egg-info/PKG-INFO` & `lendsmart_reva-1.7/lendsmart_reva.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart-reva
-Version: 1.6
+Version: 1.7
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.6/lendsmart_reva.egg-info/SOURCES.txt` & `lendsmart_reva-1.7/lendsmart_reva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/lendsmart_reva.egg-info/entry_points.txt` & `lendsmart_reva-1.7/lendsmart_reva.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/advisor_profile.py` & `lendsmart_reva-1.7/reva/advisor_profile.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/autotest.py` & `lendsmart_reva-1.7/reva/autotest.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/branch.py` & `lendsmart_reva-1.7/reva/branch.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/cli.py` & `lendsmart_reva-1.7/reva/cli.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/conf/reva.py` & `lendsmart_reva-1.7/reva/conf/reva.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/document_access_control.py` & `lendsmart_reva-1.7/reva/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/exception.py` & `lendsmart_reva-1.7/reva/exception.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/info.py` & `lendsmart_reva-1.7/reva/info.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/advisor_profile/create.py` & `lendsmart_reva-1.7/reva/lib/advisor_profile/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,22 @@
             "last_name": path_or("", [1], user_name.split(" ")),
             "home_phone": path_or("", ["phone"], advisor_profile_data),
             "is_admin": False,
             "status": "Active",
             "avatar": path_or("", ["avatar"], advisor_profile_data),
             "roles_id": roles_id if roles_id else [],
             "metadata": {
-                "role": path_or("loan_officers", ["persona"], advisor_profile_data),
+                "role": path_or("loan_officers", ["persona"], advisor_profile_data) or "loan_officers",
                 "lendsmart_sh/nmls": path_or("", ["nmls"], advisor_profile_data),
                 "title": path_or("", ["title"], advisor_profile_data),
                 "profile_url": path_or("", ["my_site"], advisor_profile_data),
                 "company_address": path_or("", ["address"], advisor_profile_data),
                 "branch_nmls": path_or("", ["branch_nmls"], advisor_profile_data),
+                "lendsmart_sh/enable_login_timeout": path_or("false", ["enable_login_timeout"], advisor_profile_data) or "false",
+                "lendsmart_sh/enable_mfa": path_or("false", ["enable_mfa"], advisor_profile_data) or "false",
             },
             "password": path_or("", ["password"], advisor_profile_data) or "Speed#123",
             "sso": {"is_enable_sso": False},
         }
         return data
 
     def get_branch_by_code(self, branch_code: str) -> dict:
@@ -129,15 +131,15 @@
                 "lendsmart_sh/title": path_or("", ["title"], advisor_profile_data),
                 "lendsmart_sh/profile_url": path_or(
                     "", ["my_site"], advisor_profile_data
                 ),
                 "lendsmart_sh/display_location": company_address,
                 "lendsmart_sh/business_location": company_address,
             },
-            "persona": path_or("loan_officers", ["persona"], advisor_profile_data),
+            "persona": path_or("loan_officers", ["persona"], advisor_profile_data) or "loan_officers",
             "description": path_or("", ["description"], advisor_profile_data),
             "avatar": path_or("", ["avatar"], advisor_profile_data),
             "user_name": email_prefix.replace(".", "-"),
             "status": {
                 "phase": "Pending",
                 "reason": "initalize new advisor profile",
                 "conditions": [
```

### Comparing `lendsmart_reva-1.6/reva/lib/auto/main.py` & `lendsmart_reva-1.7/reva/lib/auto/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/base/base.py` & `lendsmart_reva-1.7/reva/lib/base/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/base/run_query.py` & `lendsmart_reva-1.7/reva/lib/base/run_query.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/branch/create.py` & `lendsmart_reva-1.7/reva/lib/branch/create.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/client/builder.py` & `lendsmart_reva-1.7/reva/lib/client/builder.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/client/graphql_client.py` & `lendsmart_reva-1.7/reva/lib/client/graphql_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/document_access_control/main.py` & `lendsmart_reva-1.7/reva/lib/document_access_control/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/document_access_control/update.py` & `lendsmart_reva-1.7/reva/lib/document_access_control/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/advisor_profiles.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/advisor_profiles.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/branch.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/branch.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/document_access_control.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/loan_products.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/roles_and_permissions.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/site_settings.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/graphql_queries/workflow.py` & `lendsmart_reva-1.7/reva/lib/graphql_queries/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/loan_productus/main.py` & `lendsmart_reva-1.7/reva/lib/loan_productus/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/loan_productus/update.py` & `lendsmart_reva-1.7/reva/lib/loan_productus/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/roles_and_permissions/main.py` & `lendsmart_reva-1.7/reva/lib/roles_and_permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/roles_and_permissions/update.py` & `lendsmart_reva-1.7/reva/lib/roles_and_permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/site_settings/main.py` & `lendsmart_reva-1.7/reva/lib/site_settings/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/site_settings/update.py` & `lendsmart_reva-1.7/reva/lib/site_settings/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/utils/get_json_files.py` & `lendsmart_reva-1.7/reva/lib/utils/get_json_files.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/utils/get_namespaces.py` & `lendsmart_reva-1.7/reva/lib/utils/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/utils/get_paths.py` & `lendsmart_reva-1.7/reva/lib/utils/get_paths.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/workflow/main.py` & `lendsmart_reva-1.7/reva/lib/workflow/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/lib/workflow/update.py` & `lendsmart_reva-1.7/reva/lib/workflow/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/loan_products.py` & `lendsmart_reva-1.7/reva/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/namespaces.py` & `lendsmart_reva-1.7/reva/namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/roles_and_permissions.py` & `lendsmart_reva-1.7/reva/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/site_settings.py` & `lendsmart_reva-1.7/reva/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/reva/workflow.py` & `lendsmart_reva-1.7/reva/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.6/setup.py` & `lendsmart_reva-1.7/setup.py`

 * *Files identical despite different names*

