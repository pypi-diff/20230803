# Comparing `tmp/sqlalchemy-declarative-extensions-0.6.3.tar.gz` & `tmp/sqlalchemy-declarative-extensions-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-declarative-extensions-0.6.3.tar", max compression
+gzip compressed data, was "sqlalchemy-declarative-extensions-0.6.4.tar", max compression
```

## Comparing `sqlalchemy-declarative-extensions-0.6.3.tar` & `sqlalchemy-declarative-extensions-0.6.4.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0    11357 2023-06-06 21:03:29.912185 sqlalchemy-declarative-extensions-0.6.3/LICENSE
--rw-r--r--   0        0        0    11293 2023-06-06 21:03:29.912185 sqlalchemy-declarative-extensions-0.6.3/README.md
--rw-r--r--   0        0        0     3056 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1350 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/__init__.py
--rw-r--r--   0        0        0      129 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/__init__.py
--rw-r--r--   0        0        0     1054 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/base.py
--rw-r--r--   0        0        0     1338 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/function.py
--rw-r--r--   0        0        0     1916 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/grant.py
--rw-r--r--   0        0        0     1894 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/role.py
--rw-r--r--   0        0        0     2153 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/row.py
--rw-r--r--   0        0        0     1465 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/schema.py
--rw-r--r--   0        0        0     1480 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/trigger.py
--rw-r--r--   0        0        0     1510 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/view.py
--rw-r--r--   0        0        0     8396 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/api.py
--rw-r--r--   0        0        0     7790 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/audit.py
--rw-r--r--   0        0        0      720 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/__init__.py
--rw-r--r--   0        0        0      775 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/from_string.py
--rw-r--r--   0        0        0        0 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
--rw-r--r--   0        0        0      958 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
--rw-r--r--   0        0        0     1008 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
--rw-r--r--   0        0        0     1104 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     4503 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
--rw-r--r--   0        0        0     1288 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
--rw-r--r--   0        0        0    11796 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
--rw-r--r--   0        0        0     5557 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
--rw-r--r--   0        0        0     5978 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
--rw-r--r--   0        0        0     8152 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
--rw-r--r--   0        0        0     7540 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
--rw-r--r--   0        0        0     4941 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
--rw-r--r--   0        0        0     2139 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/query.py
--rw-r--r--   0        0        0        0 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
--rw-r--r--   0        0        0     1014 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
--rw-r--r--   0        0        0      189 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/__init__.py
--rw-r--r--   0        0        0     2700 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/base.py
--rw-r--r--   0        0        0     2743 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/compare.py
--rw-r--r--   0        0        0      529 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/ddl.py
--rw-r--r--   0        0        0       93 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/__init__.py
--rw-r--r--   0        0        0     2308 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/base.py
--rw-r--r--   0        0        0     4462 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/compare.py
--rw-r--r--   0        0        0      643 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/ddl.py
--rw-r--r--   0        0        0        0 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/py.typed
--rw-r--r--   0        0        0       91 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/__init__.py
--rw-r--r--   0        0        0     1092 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/base.py
--rw-r--r--   0        0        0     3861 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/compare.py
--rw-r--r--   0        0        0      707 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/ddl.py
--rw-r--r--   0        0        0     1088 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/generic.py
--rw-r--r--   0        0        0     2615 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/topological_sort.py
--rw-r--r--   0        0        0      176 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/base.py
--rw-r--r--   0        0        0     5633 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/compare.py
--rw-r--r--   0        0        0      516 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/query.py
--rw-r--r--   0        0        0      118 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/__init__.py
--rw-r--r--   0        0        0     1691 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/base.py
--rw-r--r--   0        0        0     1457 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/compare.py
--rw-r--r--   0        0        0      446 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/ddl.py
--rw-r--r--   0        0        0      299 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/sql.py
--rw-r--r--   0        0        0     1926 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/sqlalchemy.py
--rw-r--r--   0        0        0      182 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/__init__.py
--rw-r--r--   0        0        0     2148 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/base.py
--rw-r--r--   0        0        0     2334 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/compare.py
--rw-r--r--   0        0        0      541 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/ddl.py
--rw-r--r--   0        0        0      215 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/__init__.py
--rw-r--r--   0        0        0    16516 2023-06-06 21:03:29.916187 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/base.py
--rw-r--r--   0        0        0     3017 2023-06-06 21:03:29.920189 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/compare.py
--rw-r--r--   0        0        0      580 2023-06-06 21:03:29.920189 sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/ddl.py
--rw-r--r--   0        0        0    13149 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.6.3/setup.py
--rw-r--r--   0        0        0    12478 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      191 2023-08-03 14:18:41.519716 sqlalchemy-declarative-extensions-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-08-03 14:18:41.519716 sqlalchemy-declarative-extensions-0.6.4/LICENSE
+-rw-r--r--   0        0        0    11293 2023-08-03 14:18:41.519716 sqlalchemy-declarative-extensions-0.6.4/README.md
+-rw-r--r--   0        0        0     3056 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1350 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/__init__.py
+-rw-r--r--   0        0        0      129 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/__init__.py
+-rw-r--r--   0        0        0     1054 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/base.py
+-rw-r--r--   0        0        0     1338 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/function.py
+-rw-r--r--   0        0        0     1916 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/grant.py
+-rw-r--r--   0        0        0     1894 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/role.py
+-rw-r--r--   0        0        0     2153 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/row.py
+-rw-r--r--   0        0        0     1465 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/schema.py
+-rw-r--r--   0        0        0     1480 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/trigger.py
+-rw-r--r--   0        0        0     1510 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/view.py
+-rw-r--r--   0        0        0     8415 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/api.py
+-rw-r--r--   0        0        0     8108 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/audit.py
+-rw-r--r--   0        0        0      720 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/__init__.py
+-rw-r--r--   0        0        0      775 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/from_string.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
+-rw-r--r--   0        0        0      958 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
+-rw-r--r--   0        0        0     1008 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
+-rw-r--r--   0        0        0     1104 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
+-rw-r--r--   0        0        0     4503 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
+-rw-r--r--   0        0        0     1288 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
+-rw-r--r--   0        0        0    11796 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
+-rw-r--r--   0        0        0     5557 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
+-rw-r--r--   0        0        0     5989 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
+-rw-r--r--   0        0        0     8152 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
+-rw-r--r--   0        0        0     7540 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
+-rw-r--r--   0        0        0     4941 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
+-rw-r--r--   0        0        0     2139 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/query.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
+-rw-r--r--   0        0        0     1213 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
+-rw-r--r--   0        0        0     1014 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
+-rw-r--r--   0        0        0      189 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/__init__.py
+-rw-r--r--   0        0        0     2723 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/base.py
+-rw-r--r--   0        0        0     2743 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/compare.py
+-rw-r--r--   0        0        0      529 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/ddl.py
+-rw-r--r--   0        0        0       93 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/__init__.py
+-rw-r--r--   0        0        0     2308 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/base.py
+-rw-r--r--   0        0        0     4488 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/compare.py
+-rw-r--r--   0        0        0      643 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/ddl.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/py.typed
+-rw-r--r--   0        0        0       91 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/__init__.py
+-rw-r--r--   0        0        0     1092 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/base.py
+-rw-r--r--   0        0        0     3861 2023-08-03 14:18:41.523716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/compare.py
+-rw-r--r--   0        0        0      707 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/ddl.py
+-rw-r--r--   0        0        0     1088 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/generic.py
+-rw-r--r--   0        0        0     2615 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/topological_sort.py
+-rw-r--r--   0        0        0      176 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/base.py
+-rw-r--r--   0        0        0     5633 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/compare.py
+-rw-r--r--   0        0        0      516 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/query.py
+-rw-r--r--   0        0        0      118 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/__init__.py
+-rw-r--r--   0        0        0     1691 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/base.py
+-rw-r--r--   0        0        0     1457 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/compare.py
+-rw-r--r--   0        0        0      430 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/ddl.py
+-rw-r--r--   0        0        0      299 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/sql.py
+-rw-r--r--   0        0        0     2158 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/sqlalchemy.py
+-rw-r--r--   0        0        0      182 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/__init__.py
+-rw-r--r--   0        0        0     2170 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/base.py
+-rw-r--r--   0        0        0     2334 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/compare.py
+-rw-r--r--   0        0        0      541 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/ddl.py
+-rw-r--r--   0        0        0      215 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/__init__.py
+-rw-r--r--   0        0        0    16641 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/base.py
+-rw-r--r--   0        0        0     3017 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/compare.py
+-rw-r--r--   0        0        0      580 2023-08-03 14:18:41.527716 sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/ddl.py
+-rw-r--r--   0        0        0    13149 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.6.4/setup.py
+-rw-r--r--   0        0        0    12478 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.6.4/PKG-INFO
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/LICENSE` & `sqlalchemy-declarative-extensions-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/README.md` & `sqlalchemy-declarative-extensions-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/pyproject.toml` & `sqlalchemy-declarative-extensions-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sqlalchemy-declarative-extensions"
-version = "0.6.3"
-description = "Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic."
-
+version = "0.6.4"
 authors = ["Dan Cardin <ddcardin@gmail.com>"]
+
+description = "Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic."
 license = "Apache-2.0"
 repository = "https://github.com/dancardin/sqlalchemy-declarative-extensions"
 readme = 'README.md'
 
 keywords = [
   "alembic",
   "declarative",
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/__init__.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/function.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/function.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/grant.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/role.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/role.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/row.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/row.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/schema.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/trigger.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/alembic/view.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/alembic/view.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/api.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,49 +6,47 @@
 from sqlalchemy.sql.schema import MetaData
 
 from sqlalchemy_declarative_extensions.function.base import Function, Functions
 from sqlalchemy_declarative_extensions.grant.base import Grants
 from sqlalchemy_declarative_extensions.role.base import Roles
 from sqlalchemy_declarative_extensions.row.base import Row, Rows
 from sqlalchemy_declarative_extensions.schema.base import Schemas
-from sqlalchemy_declarative_extensions.sqlalchemy import DeclarativeMeta, HasMetaData
+from sqlalchemy_declarative_extensions.sqlalchemy import HasMetaData
 from sqlalchemy_declarative_extensions.trigger.base import Trigger, Triggers
 from sqlalchemy_declarative_extensions.view.base import View, Views
 
 if TYPE_CHECKING:
     from sqlalchemy_declarative_extensions.dialects import postgresql
     from sqlalchemy_declarative_extensions.grant.base import G
     from sqlalchemy_declarative_extensions.role import generic
     from sqlalchemy_declarative_extensions.schema.base import Schema
 
 
-T = TypeVar("T", bound=DeclarativeMeta)
+T = TypeVar("T")
 
 
 def declarative_database(base: T) -> T:
     """Decorate a SQLAlchemy declarative base object to register database objects.
 
     See also :func:`sqlalchemy_declarative_extensions.declare_database`, of which this decorator is syntactic sugar.
 
     By decorating your declarative base with this decorator, the attributes
     "schemas", "roles", and "grants" are read and will register with SQLAlchemy
     and/or Alembic to ensure they're created during a ``metadata.create_createall``
     call or ``alembic --autogenerate``.
 
     Examples:
-        >>> try:
-        ...     from sqlalchemy.orm import declarative_base
-        ... except ImportError:
-        ...     from sqlalchemy_declarative_extensions.sqlalchemy import declarative_base
-        >>> Base_ = declarative_base()
-        >>>
+        >>> from sqlalchemy_declarative_extensions.sqlalchemy import declarative_base
         >>> from sqlalchemy_declarative_extensions import declarative_database, Roles
         >>> from sqlalchemy_declarative_extensions.dialects.postgresql import Role
+        >>>
+        >>> _Base = declarative_base()
+
         >>> @declarative_database
-        ... class Base(Base_):
+        ... class Base(_Base):  # type: ignore
         ...     __abstract__ = True
         ...
         ...     schemas = Schemas().are('example')
         ...     roles = (
         ...         Roles(ignore_unspecified=True)
         ...         .are(
         ...             'read',
@@ -61,16 +59,20 @@
     raw_schemas = getattr(base, "schemas", None)
     raw_grants = getattr(base, "grants", None)
     raw_views = getattr(base, "views", None)
     raw_functions = getattr(base, "functions", None)
     raw_triggers = getattr(base, "triggers", None)
     raw_rows = getattr(base, "rows", None)
 
+    metadata = getattr(base, "metadata", None)
+    if metadata is None:  # pragma: no cover
+        raise ValueError("Base must have a 'metadata' attribute.")
+
     declare_database(
-        base.metadata,
+        metadata,
         schemas=raw_schemas,
         roles=raw_roles,
         grants=raw_grants,
         views=raw_views,
         functions=raw_functions,
         triggers=raw_triggers,
         rows=raw_rows,
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/audit.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/audit.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 
 from sqlalchemy_declarative_extensions import (
     Function,
     register_function,
     register_trigger,
 )
 from sqlalchemy_declarative_extensions.dialects.postgresql.trigger import Trigger
-from sqlalchemy_declarative_extensions.sqlalchemy import HasTable
 
 default_primary_key = Column(
     "audit_pk", types.Integer(), primary_key=True, autoincrement=True
 )
 
 
-T = TypeVar("T", bound=HasTable)
+T = TypeVar("T")
 AUDIT_PK = "audit_pk"
 AUDIT_OPERATION = "audit_operation"
 AUDIT_TIMESTAMP = "audit_timestamp"
 AUDIT_CURRENT_USER = "audit_current_user"
 
 
 def audit(
@@ -55,16 +54,20 @@
     schema: str | None = None,
     ignore_columns: set = set(),
     context_columns: list[Column] | None = None,
     insert: bool = True,
     update: bool = True,
     delete: bool = True,
 ) -> T:
+    table = getattr(model, "__table__", None)
+    if table is None:  # pragma: no cover
+        raise ValueError(f"{model} is not a valid model, lacks __table__ attribute.")
+
     table = audit_table(
-        model.__table__,
+        table,
         primary_key=primary_key,
         schema=schema,
         ignore_columns=ignore_columns,
         context_columns=context_columns,
         insert=insert,
         update=update,
         delete=delete,
@@ -79,24 +82,27 @@
     schema: str | None = None,
     ignore_columns: set = set(),
     context_columns: list[Column] | None = None,
     insert: bool = True,
     update: bool = True,
     delete: bool = True,
 ):
+    metadata = getattr(table, "metadata", None)
+    assert metadata
+
     audit_table = create_audit_table(
-        table.metadata,
+        metadata,
         table,
         primary_key=primary_key,
         schema=schema,
         ignore_columns=ignore_columns,
         context_columns=context_columns,
     )
     create_audit_functions(
-        table.metadata,
+        metadata,
         table,
         audit_table,
         insert=insert,
         update=update,
         delete=delete,
     )
     create_audit_triggers(
@@ -283,7 +289,18 @@
 
 
 def set_context_values(connectable, **values):
     """Set transaction-local context values, to be included on audit-tables."""
     for name, value in values.items():
         statement = f"SET LOCAL audit.{name} = '{value}'"
         connectable.execute(text(statement))
+
+
+__all__ = [
+    "audit",
+    "audit_model",
+    "audit_table",
+    "create_audit_functions",
+    "create_audit_table",
+    "create_audit_triggers",
+    "set_context_values",
+]
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/__init__.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/from_string.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/from_string.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,17 @@
 
 def get_default_grants_postgresql(
     connection: Connection,
     roles: Container[str] | None = None,
     expanded: bool = False,
 ):
     default_permissions = connection.execute(default_acl_query).fetchall()
-    current_role: str = connection.engine.url.username  # type: ignore
+
+    assert connection.engine.url.username
+    current_role: str = connection.engine.url.username
 
     result = []
     for permission in default_permissions:
         for acl_item in permission.acl:
             default_grants = parse_default_acl(
                 acl_item,
                 permission.object_type,
@@ -140,15 +142,15 @@
             for raw in connection.dialect.get_indexes(connection, v.name, schema=schema)
         ]
         view = View(
             v.name,
             v.definition,
             schema=schema,
             materialized=v.materialized,
-            constraints=indexes or None,  # type: ignore
+            constraints=indexes or None,
         )
         views.append(view)
     return views
 
 
 def get_view_postgresql(connection: Connection, name: str, schema: str = "public"):
     result = connection.execute(view_query, {"schema": schema, "name": name}).fetchone()
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/query.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field, replace
 from typing import Iterable
 
+from sqlalchemy import MetaData
+
 from sqlalchemy_declarative_extensions.sql import qualify_name
-from sqlalchemy_declarative_extensions.sqlalchemy import HasMetaData, MetaData
+from sqlalchemy_declarative_extensions.sqlalchemy import HasMetaData
 
 
 @dataclass
 class Function:
     """Describes a user defined function.
 
     Many function attributes are not currently supported. Support is **currently**
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/function/ddl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/function/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
 
 def compare_grants(
     connection: Connection, grants: Grants, roles: Roles | None = None
 ) -> list[Operation]:
     result: list[Operation] = []
 
-    current_role: str = connection.engine.url.username  # type: ignore
+    assert connection.engine.url.username
+    current_role: str = connection.engine.url.username
 
     filtered_roles: set[str] | None = None
     if grants.only_defined_roles:
         filtered_roles = {r.name for r in (roles or [])}
 
     default_grant_ops = compare_default_grants(connection, grants, roles=filtered_roles)
     result.extend(default_grant_ops)
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/grant/ddl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/grant/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/ddl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/generic.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/generic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/role/topological_sort.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/role/topological_sort.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/row/query.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/row/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/schema/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/schema/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/sqlalchemy.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/sqlalchemy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import sqlalchemy
-from sqlalchemy import MetaData, Table
+from sqlalchemy import MetaData
 from sqlalchemy.engine import Connection
 from typing_extensions import Protocol
 
 version = getattr(sqlalchemy, "__version__", "1.3")
 
 
 class HasMetaData(Protocol):
     metadata: MetaData
 
 
-class HasTable(Protocol):
-    __table__: Table
-
-
 def dialect_dispatch(postgresql=None, sqlite=None, mysql=None):
     dispatchers = {
         "postgresql": postgresql,
         "sqlite": sqlite,
         "mysql": mysql,
     }
 
@@ -38,28 +34,27 @@
 
 
 def escape_params(query: str) -> str:
     return query.replace(":", r"\:")
 
 
 if version.startswith("1.3"):
-    from sqlalchemy.ext.declarative import (  # type: ignore
+    from sqlalchemy.ext.declarative import (
         DeclarativeMeta,
-        declarative_base,
         instrument_declarative,
     )
 
     def select(*args):
         return sqlalchemy.select(list(args))
 
     def create_mapper(cls, metadata):
         return instrument_declarative(cls, {}, metadata)
 
 else:
-    from sqlalchemy.orm import DeclarativeMeta, declarative_base, registry
+    from sqlalchemy.orm import DeclarativeMeta, registry
 
     select = sqlalchemy.select
 
     def create_mapper(cls, metadata):
         reg = registry(metadata=metadata)
         return reg.mapped(cls)
 
@@ -71,14 +66,28 @@
 
 else:
 
     def row_to_dict(row):
         return dict(row)
 
 
+def declarative_base() -> HasMetaData:
+    if version.startswith("2"):
+        from sqlalchemy.orm import DeclarativeBase
+
+        return DeclarativeBase
+
+    if version.startswith("1.3"):
+        from sqlalchemy.ext.declarative import declarative_base
+    else:
+        from sqlalchemy.orm import declarative_base
+
+    return declarative_base()
+
+
 __all__ = [
     "create_mapper",
     "declarative_base",
     "DeclarativeMeta",
     "dialect_dispatch",
     "HasMetaData",
     "row_to_dict",
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field, replace
 from typing import Iterable
 
+from sqlalchemy import MetaData
 from sqlalchemy.engine import Connection
 
-from sqlalchemy_declarative_extensions.sqlalchemy import HasMetaData, MetaData
+from sqlalchemy_declarative_extensions.sqlalchemy import HasMetaData
 
 
 @dataclass
 class Trigger:
     """Describes a generic trigger."""
 
     name: str
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/trigger/ddl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/trigger/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/base.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sqlalchemy_declarative_extensions.sql import qualify_name
 from sqlalchemy_declarative_extensions.sqlalchemy import (
     HasMetaData,
     create_mapper,
     escape_params,
 )
 
-T = TypeVar("T", bound=HasMetaData)
+T = TypeVar("T")
 
 
 def view(
     base: T, materialized: bool = False, register_as_model=False
 ) -> Callable[[type], T]:
     """Decorate a class or declarative base model in order to register a View.
 
@@ -57,14 +57,17 @@
     >>> @view(Base)
     ... class Foo:
     ...     __tablename__ = "foo"
     ...     __view__ = "SELECT * from bar"
     ...
     ...     id = Column(types.Integer, primary_key=True)
     """
+    metadata = getattr(base, "metadata", None)
+    if metadata is None:  # pragma: no cover
+        raise ValueError("Model must have a 'metadata' attribute.")
 
     def decorator(cls):
         name = cls.__tablename__
         table_args = getattr(cls, "__table_args__", None)
         view_def = cls.__view__
 
         schema = find_schema(table_args)
@@ -83,15 +86,15 @@
             return instrument_sqlalchemy(base, cls)
         return cls
 
     return decorator
 
 
 def instrument_sqlalchemy(base: T, cls) -> T:
-    temp_metadata = MetaData(naming_convention=base.metadata.naming_convention)
+    temp_metadata = MetaData(naming_convention=base.metadata.naming_convention)  # type: ignore
     return create_mapper(cls, temp_metadata)
 
 
 def register_view(base_or_metadata: HasMetaData | MetaData, view: View):
     """Register a view onto the given declarative base or `Metadata`.
 
     This can be used instead of the [view](view) decorator, if you are constructing
@@ -273,15 +276,15 @@
         if (
             from_view.definition != self.definition
             or from_view.materialized != self.materialized
         ):
             result.extend(from_view.to_sql_drop(dialect))
             result.extend(self.to_sql_create(dialect))
         else:
-            removed, missing = ViewIndex.diff(from_view.constraints, self.constraints)  # type: ignore
+            removed, missing = ViewIndex.diff(from_view.constraints, self.constraints)
             result.extend([c.drop(from_view) for c in removed])
             result.extend([c.create(self) for c in missing])
 
         return result
 
     def to_sql_drop(self, dialect: Dialect) -> list[str]:
         components = ["DROP"]
@@ -391,15 +394,15 @@
                 name=index.name,
                 unique=index.unique,
             )
         elif isinstance(index, UniqueConstraint):
             convention = "uq"
             instance = ViewIndex(
                 columns=cast(List[str], list(index._pending_colargs)),
-                name=index.name,  # type: ignore
+                name=index.name,
                 unique=True,
             )
         else:  # pragma: no cover
             raise NotImplementedError()
 
         if instance.name:
             return instance
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/compare.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/src/sqlalchemy_declarative_extensions/view/ddl.py` & `sqlalchemy-declarative-extensions-0.6.4/src/sqlalchemy_declarative_extensions/view/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.6.3/setup.py` & `sqlalchemy-declarative-extensions-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 extras_require = \
 {':python_version < "3.11"': ['typing_extensions>=4.0'],
  'alembic': ['alembic>=1.0'],
  'parse': ['sqlglot']}
 
 setup_kwargs = {
     'name': 'sqlalchemy-declarative-extensions',
-    'version': '0.6.3',
+    'version': '0.6.4',
     'description': 'Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.',
     'long_description': '# SQLAlchemy Declarative Extensions\n\n[![Actions Status](https://github.com/dancardin/sqlalchemy-declarative-extensions/workflows/test/badge.svg)](https://github.com/dancardin/sqlalchemy-declarative-extensions/actions) [![Coverage Status](https://coveralls.io/repos/github/DanCardin/sqlalchemy-declarative-extensions/badge.svg?branch=main)](https://coveralls.io/github/DanCardin/sqlalchemy-declarative-extensions?branch=main) [![Documentation Status](https://readthedocs.org/projects/sqlalchemy-declarative-extensions/badge/?version=latest)](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/?badge=latest)\n\nSee the full documentation [here](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/).\n\nAdds extensions to SQLAlchemy (and/or Alembic) which allows declaratively\nstating the existence of additional kinds of objects about your database\nnot natively supported by SQLAlchemy/Alembic.\n\nThis includes:\n\n- Schemas\n- Views\n- Roles\n- Privileges (Grants/Default Grants)\n- Functions\n- Triggers\n- Rows (i.e. data)\n- "audit tables" (i.e. triggers which record data changes to some source table)\n\nThe primary function(s) of this library include:\n\n- Registering onto the SQLAlchemy event system such that `metadata.create_all`\n  creates these objects.\n- (Optionally) Registers into Alembic such that `alembic revision --autogenerate`\n  automatically creates/updates/deletes declared objects.\n\n## Kitchen Sink Example (using all available features)\n\n```python\nfrom sqlalchemy import Column, types, select\nfrom sqlalchemy.orm import as_declarative\nfrom sqlalchemy_declarative_extensions import (\n    declarative_database, Schemas, Roles, Row, View, view,\n)\nfrom sqlalchemy_declarative_extensions.dialects.postgresql import (\n    DefaultGrant, Function, Trigger, Role\n)\nfrom sqlalchemy_declarative_extensions.audit import audit\n\n\n@declarative_database\n@as_declarative\nclass Base:\n    # Note: each object type also has a plural version (i.e. Schemas/Roles/etc) where you can specify\n    # collection-level options like `ignore_unspecified`).\n    #\n    # If you dont set any collection-level options, you can instead use raw list/iterable as the collection.\n    schemas = Schemas().are("example")\n    roles = Roles(ignore_unspecified=True).are(\n        Role("read", login=False),\n        Role(\n            "app",\n            in_roles=[\'read\']\n        ),\n    )\n    grants = [\n        DefaultGrant.on_tables_in_schema("public", \'example\').grant("select", to="read"),\n        DefaultGrant.on_sequences_in_schema("public").grant("usage", to="read"),\n        Grant.new("usage", to="read").on_schemas("example")\n    ]\n    rows = [\n        Row(\'foo\', id=1),\n    ]\n    views = [\n        View("low_foo", "select * from foo where i < 10"),\n    ]\n    functions = [\n        Function(\n            "fancy_function",\n            """\n            BEGIN\n            INSERT INTO foo (id) select NEW.id + 1;\n            RETURN NULL;\n            END\n            """,\n            language="plpgsql",\n            returns="trigger",\n        ),\n    ]\n    triggers = [\n        Trigger.after("insert", on="foo", execute="fancy_function")\n        .named("on_insert_foo")\n        .when("pg_trigger_depth() < 1")\n        .for_each_row(),\n    ]\n\n\n@audit()\nclass Foo(Base):\n    __tablename__ = \'foo\'\n\n    id = Column(types.Integer(), primary_key=True)\n\n\naudit_table = Foo.__audit_table__\n\n\n@view(Base)\nclass HighFoo:\n    __tablename__ = "high_foo"\n    __view__ = select(Foo.__table__).where(Foo.__table__.c.id >= 10)\n```\n\nNote, there is also support for declaring objects directly through the `MetaData` for\nusers not using sqlalchemy\'s declarative API.\n\n## Event Registration\n\nBy default, the above example does not automatically do anything. Depending on the context,\nyou can use one of two registration hooks: `register_sqlalchemy_events` or `register_alembic_events`.\n\n### `register_sqlalchemy_events`\n\nThis registers events in SQLAlchemy\'s event system such that a `metadata.create_all(...)` call\nwill create the declared database objects.\n\n```python\nfrom sqlalchemy_declarative_extensions import register_sqlalchemy_events\n\nmetadata = Base.metadata  # Given the example above.\nregister_sqlalchemy_events(metadata)\n# Which is equivalent to...\nregister_sqlalchemy_events(metadata, schemas=False, roles=False, grants=False, rows=False)\n```\n\nAll object types are opt in, and should be explicitly included in order to get registered.\n\nPractically, this is to avoid issues with testing. In **most** cases the `metadata.create_all` call\nwill be run in tests, a context where it\'s more likely that you dont **need** grants or grants,\nand where parallel test execution could lead to issues with role or schema creation, depending\non your setup.\n\n### `register_alembic_events`\n\nThis registers comparators in Alembic\'s registration system such that an `alembic revision --autogenerate`\ncommand will diff the existing database state against the declared database objects, and issue\nstatements to create/update/delete objects in order to match the declared state.\n\n```python\n# alembic\'s `env.py`\nfrom sqlalchemy_declarative_extensions import register_alembic_events\n\nregister_alembic_events()\n# Which is equivalent to...\nregister_sqlalchemy_events(schemas=True, roles=True, grants=True, rows=True)\n```\n\nAll object types are opt out but can be excluded.\n\nIn contrast to `register_sqlalchemy_events`, it\'s much more likely that you\'re declaring most of these\nobject types in order to have alembic track them\n\n## Database support\n\nIn principle, this library **can** absolutely support any database supported by SQLAlchemy,\nand capable of being introspected enough to support detection of different kinds of objects.\n\nAs you can see below, in reality the existence of implementations are going to be purely driven by actual\nusage. The current maintainer(s) primarily use PostgreSQL and as such individual features for\nother databases will either suffer or lack implementation.\n\n|               | Postgres | MySQL | SQLite |\n|---------------|----------|-------|--------|\n| Schema        | ✓        |       | ✓      |\n| View          | ✓        | ✓     | ✓      |\n| Role          | ✓        |       | N/A    |\n| Grant         | ✓        |       | N/A    |\n| Default Grant | ✓        |       | N/A    |\n| Function      | ✓        | *     |        |\n| Trigger       | ✓        | *     |        |\n| Row (data)    | ✓        | ✓     | ✓      |\n| "Audit Table" | ✓        |       |        |\n\nThe astrisks above note pending or provisional support. The level of expertise in each dialects\'\nparticular behaviors is not uniform, and deciding on the correct behavior for those dialects\nwill require users to submit issues/fixes!\n\nSupporting a new dialect **can** be as simple as providing the dialect-dispatched implementations\nfor detecting existing objects of the given type. Very much the intent is that once a given object\ntype is supported at all, the comparison infrastructure for that type should make it straightforward\nto support other dialects. At the end of the day, this library is primarily producing SQL statements,\nso in theory any dialect supporting a given object type should be able to be supported.\n\nIn such cases (like Grants/Roles) that different dialects support wildly different\noptions/syntax, there are also patterns for defining dialect-specific objects, to mediate\nany additional differences.\n\n## Alembic-utils\n\n[Alembic Utils](https://github.com/olirice/alembic_utils) is the primary library against which\nthis library can be compared. At time of writing, **most** (but not all) object types supported\nby alembic-utils are supported by this library. One might begin to question when to use which library.\n\nBelow is a list of points on which the two libraries diverge. But note that you **can** certainly\nuse both in tandem! It doesn\'t need to be one or the other, and certainly for any object types\nwhich do not overlap, you might **need** to use both.\n\n- Database Support\n\n  - Alembic Utils seems to explicitly only support PostgreSQL.\n\n  - This library is designed to support any dialect (in theory). Certainly PostgreSQL\n    is **best** supported, but there does exist support for specific kinds of objects\n    to varying levels of support for SQLite and MySQL, so far.\n\n- Architecture\n\n  - Alembic Utils is directly tied to Alembic and does not support SQLAlchemy\'s `MetaData.create_all`.\n    It\'s also the responsibility of the user to discover/register objects in alembic.\n\n  - This library **depends** only on SQLAlchemy, although it also supports alembic. Support for\n    `MetaData.create_all` can be important for creating all object types in tests. It also\n    is designed such that objects are registered on the `MetaData` itself, so there is no need for\n    any specific discovery phase.\n\n- Scope\n\n  - Alembic Utils declares specific, individual objects. I.e. you instantiate one specific `PGGrantTable`\n    or `PGView` instance and Alembic know knows you want that object to be created. It cannot drop\n    objects it is not already aware of.\n\n  - This library declares ths objects the system as a whole expects to exist. Similar to Alembic\'s\n    behavior on tables, it will (by default) detect any **undeclared** objects that should not exist\n    and drop them. That means, you can rely on this object to ensure the state of your migrations\n    matches the state of your database exactly.\n\n- Migration history\n\n  - Alembic Utils imports and references its own objects in your migrations history. This can be\n    unfortunate, in that it deeply ties your migrations history to alembic-utils.\n\n    (In fact, this can be a sticking point, trying to convert **away** from `alembic_utils`, because it\n    will attempt to drop all the (e.g `PGView`) instances previously created when we replaced it with\n    this library.)\n\n  - This library, by contrast, prefers to emit the raw SQL of the operation into your migration.\n    That means you know the exact commands that will execute in your migration, which can be helpful\n    in debugging failure. It also means, if at any point you decide to stop use of the library\n    (or pause a given type of object, due to a bug), you can! This library\'s behaviors are primarily\n    very much `--autogenerate`-time only.\n\n- Abstraction Level\n\n  - Alembic Utils appears to define a very "literal" interface (for example, `PGView` accepts\n    the whole view definition as a raw literal string).\n\n  - This library tries to, as much as possible, provide a more abstracted interface that enables\n    more compatibility with SQLAlchemy (For example `View` accepts SQLAlchemy objects which can\n    be coerced into a `SELECT`). It also tends towards "builder" interfaces which progressively produce\n    a object (Take a look at the `DefaultGrant` above, for an example of where that\'s helpful).\n\nA separate note on conversion/compatibility. Where possible, this library tries to support alembic-utils\nnative objects as stand-ins for the objects defined in this library. For example, `alembic_utils.pg_view.PGView`\ncan be declared instead of a `sqlalchemy_declarative_extensions.View`, and we will internally\ncoerce it into the appropriate type. Hopefully this eases any transitional costs, or\nissues using one or the other library.\n',
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/sqlalchemy-declarative-extensions',
```

### Comparing `sqlalchemy-declarative-extensions-0.6.3/PKG-INFO` & `sqlalchemy-declarative-extensions-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-declarative-extensions
-Version: 0.6.3
+Version: 0.6.4
 Summary: Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.
 Home-page: https://github.com/dancardin/sqlalchemy-declarative-extensions
 License: Apache-2.0
 Keywords: alembic,declarative,grant,mysql,postgresql,role,schema,sqlalchemy,view
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.7,<4
```

