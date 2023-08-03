# Comparing `tmp/django-forestadmin-1.6.3.tar.gz` & `tmp/django-forestadmin-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forestadmin-1.6.3.tar", last modified: Fri Jul 28 08:04:38 2023, max compression
+gzip compressed data, was "django-forestadmin-1.6.4.tar", last modified: Thu Aug  3 15:03:56 2023, max compression
```

## Comparing `django-forestadmin-1.6.3.tar` & `django-forestadmin-1.6.4.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.569388 django-forestadmin-1.6.3/django_forest/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/actions/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/actions/hooks/views/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/views/change.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/views/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/hooks/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/actions/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/actions/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/authentication/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/oidc/client_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/oidc/configuration_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/oidc/dynamic_client_registrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/authentication/views/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/views/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/views/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/authentication/views/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/middleware/deactivate_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/middleware/ip_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/middleware/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/resources/associations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.573389 django-forestadmin-1.6.3/django_forest/resources/associations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/utils/association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/associations/views/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/views/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/views/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/associations/views/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/in_search_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/json_api_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/query_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/limit_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/queryset/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/utils/smart_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/resources/views/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/views/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/views/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/views/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/resources/views/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.577389 django-forestadmin-1.6.3/django_forest/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/stats/views/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/stats/views/live_queries/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/views/live_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/views/live_queries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/stats/views/stats_with_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/views/stats_with_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/stats/views/stats_with_parameters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/test_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/actions/views/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/views/generate_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/views/mark_as_live.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/views/not_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/actions/views/send_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_client_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_configuration_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_dynamic_client_registrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.581389 django-forestadmin-1.6.3/django_forest/tests/authentication/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/views/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/views/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/authentication/views/test_logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92340 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/fixtures/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/forest/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/forest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/forest/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/forest/question.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/middleware/test_ip_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/middleware/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0002_auto_20210615_0942.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0003_auto_20210701_1508.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0004_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0005_alter_serial_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/0006_auto_20210806_2254.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/associations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/associations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.585389 django-forestadmin-1.6.3/django_forest/tests/resources/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.589390 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_filters_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/test_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/resources/views/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.589390 django-forestadmin-1.6.3/django_forest/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.589390 django-forestadmin-1.6.3/django_forest/tests/stats/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/stats/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/stats/views/test_live_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/stats/views/test_stats_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.589390 django-forestadmin-1.6.3/django_forest/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_forest_api_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_get_forest_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_json_api_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/utils/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.589390 django-forestadmin-1.6.3/django_forest/tests/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/views/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/tests/views/test_scope_cache_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/forest_api_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/forest_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/ip_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forest/utils/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/permissions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forest/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/apimap_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/json_api_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/schema/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/type_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forest/utils/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/views/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/utils/views/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forest/views/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/views/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/django_forest/views/scope_cache_invalidation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:38.593390 django-forestadmin-1.6.3/django_forestadmin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-28 08:04:38.000000 django-forestadmin-1.6.3/django_forestadmin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-28 08:04:38.000000 django-forestadmin-1.6.3/django_forestadmin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:04:38.000000 django-forestadmin-1.6.3/django_forestadmin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 08:04:38.000000 django-forestadmin-1.6.3/django_forestadmin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 08:04:38.000000 django-forestadmin-1.6.3/django_forestadmin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-28 08:04:38.597390 django-forestadmin-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:03:58.000000 django-forestadmin-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.503738 django-forestadmin-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-08-03 15:03:56.503738 django-forestadmin-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/actions/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/actions/hooks/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/views/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/views/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/hooks/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/actions/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/actions/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.463738 django-forestadmin-1.6.4/django_forest/authentication/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/oidc/client_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/oidc/configuration_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/oidc/dynamic_client_registrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/authentication/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/views/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/authentication/views/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/middleware/deactivate_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/middleware/ip_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/middleware/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/resources/associations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/resources/associations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/utils/association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.467738 django-forestadmin-1.6.4/django_forest/resources/associations/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/views/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/views/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/associations/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.471738 django-forestadmin-1.6.4/django_forest/resources/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/in_search_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/json_api_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/query_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.471738 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.471738 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.471738 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/limit_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/queryset/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/utils/smart_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/resources/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/views/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/views/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/views/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/resources/views/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/stats/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/stats/views/live_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/views/live_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/views/live_queries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/stats/views/stats_with_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/views/stats_with_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/stats/views/stats_with_parameters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.475738 django-forestadmin-1.6.4/django_forest/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/test_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/actions/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/views/generate_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/views/mark_as_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/views/not_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/actions/views/send_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.479738 django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_client_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_configuration_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_dynamic_client_registrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.483738 django-forestadmin-1.6.4/django_forest/tests/authentication/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/views/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/views/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/authentication/views/test_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.483738 django-forestadmin-1.6.4/django_forest/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92340 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/fixtures/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.483738 django-forestadmin-1.6.4/django_forest/tests/forest/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/forest/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/forest/question.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.483738 django-forestadmin-1.6.4/django_forest/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/middleware/test_ip_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/middleware/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0002_auto_20210615_0942.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0003_auto_20210701_1508.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0004_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0005_alter_serial_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/0006_auto_20210806_2254.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/associations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/associations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.487738 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.491738 django-forestadmin-1.6.4/django_forest/tests/resources/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.491738 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_filters_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/resources/views/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.491738 django-forestadmin-1.6.4/django_forest/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.491738 django-forestadmin-1.6.4/django_forest/tests/stats/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/stats/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/stats/views/test_live_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/stats/views/test_stats_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.495738 django-forestadmin-1.6.4/django_forest/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_forest_api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_get_forest_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_json_api_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/utils/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.495738 django-forestadmin-1.6.4/django_forest/tests/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/views/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/tests/views/test_scope_cache_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.499738 django-forestadmin-1.6.4/django_forest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/forest_api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/forest_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/ip_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.499738 django-forestadmin-1.6.4/django_forest/utils/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/permissions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.499738 django-forestadmin-1.6.4/django_forest/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/apimap_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/json_api_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/schema/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/type_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.499738 django-forestadmin-1.6.4/django_forest/utils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/views/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/utils/views/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.499738 django-forestadmin-1.6.4/django_forest/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/django_forest/views/scope_cache_invalidation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:03:56.503738 django-forestadmin-1.6.4/django_forestadmin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-08-03 15:03:56.000000 django-forestadmin-1.6.4/django_forestadmin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-08-03 15:03:56.000000 django-forestadmin-1.6.4/django_forestadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:03:56.000000 django-forestadmin-1.6.4/django_forestadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 15:03:56.000000 django-forestadmin-1.6.4/django_forestadmin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 15:03:56.000000 django-forestadmin-1.6.4/django_forestadmin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-03 15:03:56.503738 django-forestadmin-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:03:01.000000 django-forestadmin-1.6.4/setup.py
```

### Comparing `django-forestadmin-1.6.3/LICENCE` & `django-forestadmin-1.6.4/LICENCE`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/PKG-INFO` & `django-forestadmin-1.6.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forestadmin
-Version: 1.6.3
+Version: 1.6.4
 Summary: The Django Liana for Forest Admin.
 Home-page: https://forestadmin.com/
 Author: Guillaume Cisco
 Author-email: guillaumec@forestadmin.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-forestadmin-1.6.3/README.md` & `django-forestadmin-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/actions/hooks/views/change.py` & `django-forestadmin-1.6.4/django_forest/actions/hooks/views/change.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/actions/hooks/views/utils.py` & `django-forestadmin-1.6.4/django_forest/actions/hooks/views/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import logging
+
 from django.http import JsonResponse, HttpResponse
 
 from django_forest.utils import get_token
 from django_forest.utils.collection import Collection
 from django_forest.utils.views.base import BaseView
 
+logger = logging.getLogger(__name__)
+
 
 class HookView(BaseView):
 
     def action_name_from_endpoint(self, action):
         return str(action['endpoint'].split('/')[-1])
 
     def hook_exists(self, action, action_name, hook):
@@ -47,10 +51,11 @@
             get_token(request)
         except Exception:
             return HttpResponse(status=403)
         else:
             try:
                 data = self.get_hook_result(action_name, request)
             except Exception as e:
+                logger.exception(e)
                 return self.error_response(e)
             else:
                 return JsonResponse({'fields': data}, safe=False)
```

### Comparing `django-forestadmin-1.6.3/django_forest/authentication/oidc/client_manager.py` & `django-forestadmin-1.6.4/django_forest/authentication/oidc/client_manager.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/authentication/oidc/configuration_retriever.py` & `django-forestadmin-1.6.4/django_forest/authentication/oidc/configuration_retriever.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/authentication/oidc/dynamic_client_registrator.py` & `django-forestadmin-1.6.4/django_forest/authentication/oidc/dynamic_client_registrator.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/authentication/views/callback.py` & `django-forestadmin-1.6.4/django_forest/authentication/views/callback.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/authentication/views/index.py` & `django-forestadmin-1.6.4/django_forest/authentication/views/index.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/middleware/deactivate_count.py` & `django-forestadmin-1.6.4/django_forest/middleware/deactivate_count.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/middleware/ip_whitelist.py` & `django-forestadmin-1.6.4/django_forest/middleware/ip_whitelist.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/middleware/permissions.py` & `django-forestadmin-1.6.4/django_forest/middleware/permissions.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/associations/utils/association.py` & `django-forestadmin-1.6.4/django_forest/resources/associations/utils/association.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/associations/views/count.py` & `django-forestadmin-1.6.4/django_forest/resources/associations/views/count.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import logging
+
 from django_forest.resources.associations.utils import AssociationView
 from django_forest.utils import get_association_field
 
+logger = logging.getLogger(__name__)
+
 
 class CountView(AssociationView):
 
     def get(self, request, pk, association_resource):
         try:
             get_association_field(self.Model, association_resource)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             queryset = getattr(self.Model.objects.get(pk=pk), association_resource).all()
             params = request.GET.dict()
             return self.get_count(queryset, params, request)
```

### Comparing `django-forestadmin-1.6.3/django_forest/resources/associations/views/csv.py` & `django-forestadmin-1.6.4/django_forest/resources/associations/views/csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 import csv
 
 from django_forest.resources.associations.utils import AssociationView
 from django_forest.resources.utils.csv import CsvMixin
 from django_forest.resources.utils.json_api_serializer import JsonApiSerializerMixin
 from django_forest.resources.utils.query_parameters import parse_qs
 from django_forest.resources.utils.smart_field import SmartFieldMixin
 from django_forest.utils import get_association_field
 
+logger = logging.getLogger(__name__)
+
 
 class CsvView(SmartFieldMixin, JsonApiSerializerMixin, CsvMixin, AssociationView):
     def get(self, request, pk, association_resource):
         try:
             association_field = get_association_field(self.Model, association_resource)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             RelatedModel = association_field.related_model
 
             # default
             queryset = getattr(self.Model.objects.get(pk=pk), association_resource).all()
```

### Comparing `django-forestadmin-1.6.3/django_forest/resources/associations/views/list.py` & `django-forestadmin-1.6.4/django_forest/resources/associations/views/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from distutils.util import strtobool
+import logging
 
 from django.http import JsonResponse, HttpResponse
 
 from django_forest.resources.associations.utils import AssociationView
 from django_forest.resources.utils.json_api_serializer import JsonApiSerializerMixin
 from django_forest.resources.utils.query_parameters import parse_qs
 from django_forest.resources.utils.smart_field import SmartFieldMixin
 from django_forest.utils import get_association_field
 
+logger = logging.getLogger(__name__)
+
 
 class ListView(SmartFieldMixin, JsonApiSerializerMixin, AssociationView):
 
     def get(self, request, pk, association_resource):
         try:
             association_field = get_association_field(self.Model, association_resource)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             RelatedModel = association_field.related_model
 
             # default
             queryset = getattr(self.Model.objects.get(pk=pk), association_resource).all()
 
@@ -34,14 +38,15 @@
 
             return JsonResponse(data, safe=False)
 
     def post(self, request, pk, association_resource):
         try:
             association_field = get_association_field(self.Model, association_resource)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             RelatedModel = association_field.related_model
             body = self.get_body(request.body)
             ids = [x['id'] for x in body['data']]
 
             instance = self.Model.objects.get(pk=pk)
@@ -61,14 +66,15 @@
         self.handle_association(instance, objects, fields_to_update, 'remove')
 
     def delete(self, request, pk, association_resource):
         try:
             association_field = get_association_field(self.Model, association_resource)
             ids = self.get_ids_from_request(request, self.Model)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             RelatedModel = association_field.related_model
             params = request.GET.dict()
 
             # Notice: Delete
             if 'delete' in params and strtobool(params['delete']):
```

### Comparing `django-forestadmin-1.6.3/django_forest/resources/urls.py` & `django-forestadmin-1.6.4/django_forest/resources/urls.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/csv.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/csv.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/decorators.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/format.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/format.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/json_api_serializer.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/json_api_serializer.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/query_parameters.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/query_parameters.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/__init__.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/__init__.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/conditions.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/conditions.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/factory.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/factory.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/date/utils.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/date/utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/filters/utils.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/filters/utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/limit_fields.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/limit_fields.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/scope.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/scope.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/queryset/search.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/queryset/search.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/utils/smart_field.py` & `django-forestadmin-1.6.4/django_forest/resources/utils/smart_field.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/resources/views/csv.py` & `django-forestadmin-1.6.4/django_forest/resources/views/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 import csv
 
 from django_forest.resources.utils.csv import CsvMixin
 from django_forest.resources.utils.format import FormatFieldMixin
 from django_forest.resources.utils.json_api_serializer import JsonApiSerializerMixin
 from django_forest.resources.utils.query_parameters import parse_qs
 from django_forest.resources.utils.resource import ResourceView
 from django_forest.resources.utils.smart_field import SmartFieldMixin
 
+logger = logging.getLogger(__name__)
+
 
 class CsvView(FormatFieldMixin, SmartFieldMixin, JsonApiSerializerMixin, CsvMixin, ResourceView):
     def get(self, request):
         # default
         queryset = self.Model.objects.all()
 
         params = request.GET.dict()
@@ -21,14 +24,15 @@
 
             # handle smart fields
             self.handle_smart_fields(queryset, self.Model._meta.db_table, parse_qs(params), many=True)
 
             # json api serializer
             data = self.serialize(queryset, self.Model, params)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             response = self.csv_response(params['filename'])
 
             field_names_requested = [x for x in params[f'fields[{self.Model._meta.db_table}]'].split(',')]
             csv_header = params['header'].split(',')
```

### Comparing `django-forestadmin-1.6.3/django_forest/resources/views/detail.py` & `django-forestadmin-1.6.4/django_forest/resources/views/detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
+
 from django.http import JsonResponse, HttpResponse
 
 from django_forest.resources.utils.format import FormatFieldMixin
 from django_forest.utils.schema import Schema
 from django_forest.resources.utils.json_api_serializer import JsonApiSerializerMixin
 from django_forest.resources.utils.resource import ResourceView
 from django_forest.resources.utils.smart_field import SmartFieldMixin
 
 from django_forest.utils.schema.json_api_schema import JsonApiSchema
 
+logger = logging.getLogger(__name__)
+
 
 class DetailView(SmartFieldMixin, FormatFieldMixin, JsonApiSerializerMixin, ResourceView):
 
     def get_instance(self, request, pk):
         # Notice: filter by scopes first
         queryset = self.Model.objects.all()
         scope_filters = self.get_scope(request, self.Model)
@@ -28,14 +32,15 @@
 
         return instance
 
     def get(self, request, pk):
         try:
             instance = self.get_instance(request, pk)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             # handle smart fields
             self.handle_smart_fields(instance, self.Model._meta.db_table)
 
             # json api serializer
             include_data = self.get_include_data(Schema.get_collection(self.Model._meta.db_table)['fields'])
@@ -51,14 +56,15 @@
             attributes = self.populate_attribute(body)
             instance = self.get_instance(request, pk)
             for k, v in attributes.items():
                 setattr(instance, k, v)
             instance = self.update_smart_fields(instance, body, self.Model._meta.db_table)
             instance.save()
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             # Notice: one to one case, where a new object is created with a new pk
             # It needs to be deleted, as django orm will create a new object
             if str(instance.pk) != pk:
                 self.Model.objects.filter(pk=pk).delete()
 
@@ -67,11 +73,12 @@
             data = Schema().dump(instance)
             return JsonResponse(data, safe=False)
 
     def delete(self, request, pk):
         try:
             instance = self.get_instance(request, pk)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             instance.delete()
             return HttpResponse(status=204)
```

### Comparing `django-forestadmin-1.6.3/django_forest/resources/views/list.py` & `django-forestadmin-1.6.4/django_forest/resources/views/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import logging
+
 from django.http import JsonResponse, HttpResponse
 
 from django_forest.resources.utils.format import FormatFieldMixin
 from django_forest.resources.utils.json_api_serializer import JsonApiSerializerMixin
 from django_forest.resources.utils.query_parameters import parse_qs
 from django_forest.resources.utils.resource import ResourceView
 from django_forest.resources.utils.smart_field import SmartFieldMixin
 from django_forest.utils.schema.json_api_schema import JsonApiSchema
 
+logger = logging.getLogger(__name__)
+
 
 class ListView(FormatFieldMixin, SmartFieldMixin, JsonApiSerializerMixin, ResourceView):
     def get(self, request):
         # default
         queryset = self.Model.objects.all()
 
         params = request.GET.dict()
@@ -24,25 +28,27 @@
 
             # json api serializer
             data = self.serialize(queryset, self.Model, params)
 
             # search decorator
             data = self.decorators(data, self.Model, params)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             return JsonResponse(data, safe=False)
 
     def post(self, request):
         body = self.get_body(request.body)
 
         try:
             attributes = self.populate_attribute(body)
             instance = self.Model.objects.create(**attributes)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             # json api serializer
             Schema = JsonApiSchema._registry[f'{self.Model._meta.db_table}Schema']
             data = Schema().dump(instance)
             return JsonResponse(data, safe=False)
```

### Comparing `django-forestadmin-1.6.3/django_forest/stats/utils/stats.py` & `django-forestadmin-1.6.4/django_forest/stats/utils/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import uuid
 from datetime import datetime
+import logging
 
 from django.http import JsonResponse
 
+logger = logging.getLogger(__name__)
+
 
 class StatsMixin:
     def serialize(self, value):
         if isinstance(value, datetime):
             return value.strftime('%d/%m/%Y')
         return value
 
@@ -45,10 +48,11 @@
             }
         return res
 
     def chart(self, params, request, queryset=None):
         try:
             res = self.handle_chart(params, request, queryset)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             return JsonResponse(res, safe=False)
```

### Comparing `django-forestadmin-1.6.3/django_forest/stats/views/live_queries/__init__.py` & `django-forestadmin-1.6.4/django_forest/stats/views/live_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/stats/views/live_queries/utils.py` & `django-forestadmin-1.6.4/django_forest/stats/views/live_queries/utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/stats/views/stats_with_parameters/__init__.py` & `django-forestadmin-1.6.4/django_forest/stats/views/stats_with_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/stats/views/stats_with_parameters/utils.py` & `django-forestadmin-1.6.4/django_forest/stats/views/stats_with_parameters/utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/test_change.py` & `django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/test_change.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/actions/hooks/views/test_load.py` & `django-forestadmin-1.6.4/django_forest/tests/actions/hooks/views/test_load.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/actions/urls.py` & `django-forestadmin-1.6.4/django_forest/tests/actions/urls.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/actions/views/generate_invoice.py` & `django-forestadmin-1.6.4/django_forest/tests/actions/views/generate_invoice.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_client_manager.py` & `django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_client_manager.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_configuration_retriever.py` & `django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_configuration_retriever.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/authentication/oidc/test_dynamic_client_registrator.py` & `django-forestadmin-1.6.4/django_forest/tests/authentication/oidc/test_dynamic_client_registrator.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/authentication/views/test_callback.py` & `django-forestadmin-1.6.4/django_forest/tests/authentication/views/test_callback.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/authentication/views/test_index.py` & `django-forestadmin-1.6.4/django_forest/tests/authentication/views/test_index.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/fixtures/schema.py` & `django-forestadmin-1.6.4/django_forest/tests/fixtures/schema.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/forest/choice.py` & `django-forestadmin-1.6.4/django_forest/tests/forest/choice.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/forest/question.py` & `django-forestadmin-1.6.4/django_forest/tests/forest/question.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/middleware/__init__.py` & `django-forestadmin-1.6.4/django_forest/tests/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/middleware/test_ip_whitelist.py` & `django-forestadmin-1.6.4/django_forest/tests/middleware/test_ip_whitelist.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/middleware/test_permissions.py` & `django-forestadmin-1.6.4/django_forest/tests/middleware/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/migrations/0001_initial.py` & `django-forestadmin-1.6.4/django_forest/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/migrations/0002_auto_20210615_0942.py` & `django-forestadmin-1.6.4/django_forest/tests/migrations/0002_auto_20210615_0942.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/migrations/0003_auto_20210701_1508.py` & `django-forestadmin-1.6.4/django_forest/tests/migrations/0003_auto_20210701_1508.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/migrations/0006_auto_20210806_2254.py` & `django-forestadmin-1.6.4/django_forest/tests/migrations/0006_auto_20210806_2254.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/models.py` & `django-forestadmin-1.6.4/django_forest/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_count.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_count.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_csv.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_csv.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/associations/views/test_list.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/associations/views/test_list.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/test_factory.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/test_factory.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/utils/queryset/filters/date/test_utils.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/utils/queryset/filters/date/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_filters.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_filters.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_filters_date.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_filters_date.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_scope.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_scope.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_search.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_search.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_fields.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_fields.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_relationship.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_relationship.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_smart_segment.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_smart_segment.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/list/test_list_sort.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/list/test_list_sort.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/test_count.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/test_count.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/test_csv.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/test_csv.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/resources/views/test_detail.py` & `django-forestadmin-1.6.4/django_forest/tests/resources/views/test_detail.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/settings.py` & `django-forestadmin-1.6.4/django_forest/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/stats/views/test_live_queries.py` & `django-forestadmin-1.6.4/django_forest/tests/stats/views/test_live_queries.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/stats/views/test_stats_with_parameters.py` & `django-forestadmin-1.6.4/django_forest/tests/stats/views/test_stats_with_parameters.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_collection.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_collection.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_cors.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_cors.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_date.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_forest_api_requester.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_forest_api_requester.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_get_forest_setting.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_get_forest_setting.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_json_api_schema.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_json_api_schema.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_middlewares.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_middlewares.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/utils/test_schema.py` & `django-forestadmin-1.6.4/django_forest/tests/utils/test_schema.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/tests/views/test_scope_cache_invalidation.py` & `django-forestadmin-1.6.4/django_forest/tests/views/test_scope_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/urls.py` & `django-forestadmin-1.6.4/django_forest/urls.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/__init__.py` & `django-forestadmin-1.6.4/django_forest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/collection.py` & `django-forestadmin-1.6.4/django_forest/utils/collection.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/cors.py` & `django-forestadmin-1.6.4/django_forest/utils/cors.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/error_handler.py` & `django-forestadmin-1.6.4/django_forest/utils/error_handler.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/forest_api_requester.py` & `django-forestadmin-1.6.4/django_forest/utils/forest_api_requester.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/ip_whitelist.py` & `django-forestadmin-1.6.4/django_forest/utils/ip_whitelist.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/models.py` & `django-forestadmin-1.6.4/django_forest/utils/models.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/permissions/__init__.py` & `django-forestadmin-1.6.4/django_forest/utils/permissions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from datetime import datetime
 
 import pytz
 
 from django_forest.utils.forest_api_requester import ForestApiRequester
 from django_forest.utils.forest_setting import get_forest_setting
-from django_forest.utils.permissions.utils import date_difference_in_seconds, is_stat_allowed, is_user_allowed,\
-    is_smart_action_allowed
+from django_forest.utils.permissions.utils import (
+    date_difference_in_seconds,
+    is_stat_allowed,
+    is_user_allowed,
+    is_smart_action_allowed,
+)
 
 
 class Permission:
     renderings_cached = {}
     permissions_cached = {}
     expiration_in_seconds = get_forest_setting('FOREST_PERMISSIONS_EXPIRATION_IN_SECONDS', 3600)
```

### Comparing `django-forestadmin-1.6.3/django_forest/utils/permissions/utils.py` & `django-forestadmin-1.6.4/django_forest/utils/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/schema/__init__.py` & `django-forestadmin-1.6.4/django_forest/utils/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/schema/apimap_errors.py` & `django-forestadmin-1.6.4/django_forest/utils/schema/apimap_errors.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/schema/definitions.py` & `django-forestadmin-1.6.4/django_forest/utils/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/schema/json_api_schema.py` & `django-forestadmin-1.6.4/django_forest/utils/schema/json_api_schema.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/schema/validations.py` & `django-forestadmin-1.6.4/django_forest/utils/schema/validations.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/scope.py` & `django-forestadmin-1.6.4/django_forest/utils/scope.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/type_mapping.py` & `django-forestadmin-1.6.4/django_forest/utils/type_mapping.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/utils/views/action.py` & `django-forestadmin-1.6.4/django_forest/utils/views/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import logging
+
 from django.http import HttpResponse
 
 from django_forest.utils import get_token
 from django_forest.utils.permissions import Permission
 from django_forest.utils.views.base import BaseView
 
+logger = logging.getLogger(__name__)
+
 
 class ActionView(BaseView):
     def get_smart_action_request_info(self, request):
         return {
             'endpoint': request.path,
             'http_method': request.method
         }
@@ -25,14 +29,15 @@
     def dispatch(self, request, *args, **kwargs):
         body = self.get_body(request.body)
         resource = body['data']['attributes']['collection_name']
 
         try:
             self.Model = self.get_model(resource)
         except Exception as e:
+            logger.exception(e)
             return self.error_response(e)
         else:
             # check permissions
             try:
                 token = get_token(request)
                 self.is_authorized(request, token, resource)
             except Exception:
```

### Comparing `django-forestadmin-1.6.3/django_forest/utils/views/base.py` & `django-forestadmin-1.6.4/django_forest/utils/views/base.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forest/views/scope_cache_invalidation.py` & `django-forestadmin-1.6.4/django_forest/views/scope_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/django_forestadmin.egg-info/PKG-INFO` & `django-forestadmin-1.6.4/django_forestadmin.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forestadmin
-Version: 1.6.3
+Version: 1.6.4
 Summary: The Django Liana for Forest Admin.
 Home-page: https://forestadmin.com/
 Author: Guillaume Cisco
 Author-email: guillaumec@forestadmin.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-forestadmin-1.6.3/django_forestadmin.egg-info/SOURCES.txt` & `django-forestadmin-1.6.4/django_forestadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-forestadmin-1.6.3/setup.cfg` & `django-forestadmin-1.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-forestadmin
-version = 1.6.3
+version = 1.6.4
 description = The Django Liana for Forest Admin.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://forestadmin.com/
 author = Guillaume Cisco
 author_email = guillaumec@forestadmin.com
 license = GNU General Public License v3 or later (GPLv3+)
```

