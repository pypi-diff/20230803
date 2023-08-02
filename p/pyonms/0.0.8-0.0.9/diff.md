# Comparing `tmp/pyonms-0.0.8.tar.gz` & `tmp/pyonms-0.0.9.tar.gz`

## Comparing `pyonms-0.0.8.tar` & `pyonms-0.0.9.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/CHANGES.PY
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/MANIFEST.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyonms-0.0.8/antora-playbook-local.yml
--rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyonms-0.0.8/external-functionapp-openapi.yaml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyonms-0.0.8/old.env
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyonms-0.0.8/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/python-version.txt
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/antora.yml
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/introduction.adoc
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/alarms.adoc
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/business_services.adoc
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/events.adoc
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/nodes.adoc
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/requisitions.adoc
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/portal/introduction.adoc
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/connecting.adoc
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/introduction.adoc
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/support.adoc
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 pyonms-0.0.8/examples/example.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyonms-0.0.8/examples/portal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/MANIFEST.in
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/__init__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/__init__.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/alarms.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/business_services.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/events.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/foreign_sources.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/health.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/info.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/nodes.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/requisitions.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/__init__.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/alarm.py
--rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/business_service.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/event.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/exceptions.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/foreign_source.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/health.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/info.py
--rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/node.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/requisition.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/portal/__init__.py
--rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/portal/models.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/utils/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyonms-0.0.8/test-mock/docker-compose.yaml
--rw-r--r--   0        0        0    26775 2020-02-02 00:00:00.000000 pyonms-0.0.8/test-mock/mocks/node_all.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_alarms.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_events.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_nodes.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_requisitions.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_all.yaml
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_batch.yaml
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_one.yaml
--rw-r--r--   0        0        0    88993 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_all.yaml
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_batch.yaml
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_one.yaml
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_all.yaml
--rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_batch.yaml
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_ip.yaml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_ip_services.yaml
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_metadata.yaml
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_one.yaml
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_snmp.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_add_asset.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_add_metadata.yaml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_all.yaml
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_batch.yaml
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_count_active.yaml
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_count_deployed.yaml
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_import.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_one.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_update_asset.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_update_metadata.yaml
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyonms-0.0.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyonms-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyonms-0.0.8/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyonms-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.9/CHANGES.PY
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.9/MANIFEST.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyonms-0.0.9/antora-playbook-local.yml
+-rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyonms-0.0.9/external-functionapp-openapi.yaml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyonms-0.0.9/old.env
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyonms-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyonms-0.0.9/.github/python-version.txt
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pyonms-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pyonms-0.0.9/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyonms-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/antora.yml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/introduction.adoc
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/alarms.adoc
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/business_services.adoc
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/events.adoc
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/nodes.adoc
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/requisitions.adoc
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/portal/introduction.adoc
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/using/connecting.adoc
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/using/introduction.adoc
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyonms-0.0.9/docs/modules/ROOT/pages/using/support.adoc
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 pyonms-0.0.9/examples/example.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyonms-0.0.9/examples/portal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/MANIFEST.in
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/__init__.py
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/alarms.py
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/business_services.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/events.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/foreign_sources.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/health.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/nodes.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/requisitions.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/dao/udl.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/__init__.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/alarm.py
+-rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/business_service.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/event.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/exceptions.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/foreign_source.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/health.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/info.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/node.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/requisition.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/models/udl.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/portal/__init__.py
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/portal/models.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyonms/utils/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyonms-0.0.9/test-mock/docker-compose.yaml
+-rw-r--r--   0        0        0    26775 2020-02-02 00:00:00.000000 pyonms-0.0.9/test-mock/mocks/node_all.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/test_alarms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/test_events.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/test_nodes.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/test_requisitions.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_alarm_all.yaml
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_alarm_batch.yaml
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_alarm_one.yaml
+-rw-r--r--   0        0        0    88993 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_event_all.yaml
+-rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_event_batch.yaml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_event_one.yaml
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_all.yaml
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_batch.yaml
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_ip.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_ip_services.yaml
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_metadata.yaml
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_one.yaml
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_node_snmp.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_add_asset.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_add_metadata.yaml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_all.yaml
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_batch.yaml
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_count_active.yaml
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_count_deployed.yaml
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_import.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_one.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_update_asset.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.9/tests/cassettes/test_requisition_update_metadata.yaml
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyonms-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyonms-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pyonms-0.0.9/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyonms-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 pyonms-0.0.9/PKG-INFO
```

### Comparing `pyonms-0.0.8/antora-playbook-local.yml` & `pyonms-0.0.9/antora-playbook-local.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/external-functionapp-openapi.yaml` & `pyonms-0.0.9/external-functionapp-openapi.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `pyonms-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/.github/workflows/codeql.yml` & `pyonms-0.0.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/.github/workflows/publish.yml` & `pyonms-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/alarms.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/alarms.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/business_services.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/business_services.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/events.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/events.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/nodes.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/nodes.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/requisitions.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/endpoints/requisitions.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/portal/introduction.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/portal/introduction.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/using/connecting.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/using/connecting.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/docs/modules/ROOT/pages/using/introduction.adoc` & `pyonms-0.0.9/docs/modules/ROOT/pages/using/introduction.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/examples/example.py` & `pyonms-0.0.9/examples/example.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # cSpell:disable
 # pylama:ignore=W0611,E501
 
 import json
 import os
 
 from dotenv import load_dotenv
+from tqdm import tqdm
 
 from pyonms import PyONMS
 from pyonms.dao.nodes import NodeComponents
 from pyonms.models import foreign_source, requisition
 from pyonms.models.event import Event, EventParameter, Severity
 from pyonms.models.foreign_source import Parameter
+from pyonms.models.udl import UserDefinedLink
 from pyonms.utils import normalize_dict
 
 # try:
 #     import pyroscope
 
 #     pyroscope.configure(
 #         application_name="pyonms.test",  # replace this with some name for your application
@@ -40,110 +42,128 @@
 
 
 my_server = PyONMS(
     hostname=os.getenv("hostname"),
     username=os.getenv("user"),
     password=os.getenv("password"),
 )
-
+print(my_server.health.probe())
 if __name__ == "__main__":
+    # for _ in [37, 36, 62, 44]:
+    #        my_server.udl.create_link(
+    #            link=UserDefinedLink(
+    #                node_id_a=43,
+    #                node_id_z=_,
+    #                component_label_a="eth0",
+    #                component_label_z="eth1",
+    #                owner="me",
+    #            )
+    #        )
+    # x = my_server.udl.create_link(link=new_link)
+    # x = my_server.udl.get_link(id=1377)
+    # links = my_server.udl.get_links()
+    # for link in links:
+    #    my_server.udl.delete_link(id=link.db_id)
+    # print(links)
     nodes = my_server.nodes.get_nodes(
         limit=5000, batch_size=100, components=[NodeComponents.ALL], threads=100
     )
-    print(f"Devices found: {len(nodes)}")
-    print(nodes)
-
-    events = my_server.events.get_events(limit=50, batch_size=25)
-    print(f"\nEvents found: {len(events)}")
-    print(events)
+    # print(f"Devices found: {len(nodes)}")
+    # print(nodes)
 
-    alarms = my_server.alarms.get_alarms(limit=50, batch_size=25)
-    print(f"\nAlarms found: {len(alarms)}")
+    # events = my_server.events.get_events(limit=50, batch_size=25)
+    # print(f"\nEvents found: {len(events)}")
+    # print(events)
+    # alarms = my_server.alarms.get_alarms(limit=5000, batch_size=25)
+    # for alarm in tqdm(alarms):
+    #    my_server.alarms.ack_alarm(id=alarm.id, ack=False)
+    #    my_server.alarms.clear_alarm(id=alarm.id)
+    # print(f"\nAlarms found: {len(alarms)}")
     # for alarm in alarms:
     #    print([alarm, my_server.nodes.get_node(alarm.nodeId)])
 
     # fs = my_server.fs.get_foreign_sources()
     # req = my_server.requisitions.get_requisitions()
     # act = my_server.requisitions.get_requisition_active_count()
     # dep = my_server.requisitions.get_requisition_deployed_count()
     # print(main)
 
-    bsms = my_server.bsm.get_bsms()
+    # bsms = my_server.bsm.get_bsms()
     # for bsm in bsms:
     #    new = bsm.request()
     #    new.name = new.name + "1"
     #   my_server.bsm.create_bsm(new)
     # status = my_server.info.get_info()
     # health = my_server.health.get_health()
     # print(my_server.health.probe())
     # my_server.reload_daemon(name="blarg")
 
-    sample = requisition.Requisition(foreign_source="Example")
-
-    new_node = requisition.RequisitionNode(foreign_id="py", node_label="text")
-    new_node.asset.append(requisition.AssetField(name="region", value="Blarg"))
-    new_node.meta_data.append(
-        requisition.Metadata(context="requisition", key="key", value="value")
-    )
-    new_node.set_metadata(key="hello", value="there")
-    new_node.set_metadata(key="key", value="new_value")
-
-    my_interface = requisition.Interface(ip_addr="127.4.3.2", snmp_primary="P")
-
-    new_service = requisition.Service(
-        service_name="SNMP",
-        meta_data=[
-            requisition.Metadata(context="requisition", key="key", value="value")
-        ],
-    )
-    my_interface.monitored_service.append(new_service)
-
-    new_node.add_interface(my_interface, merge=False)
+    # sample = requisition.Requisition(foreign_source="Example")
 
-    node2 = requisition.RequisitionNode(foreign_id="two", node_label="text2")
-    node2.add_interface(my_interface, merge=False)
-    node2.change_ip(old_ip="127.4.3.2", new_ip="127.7.8.9")
-
-    sample.add_node(new_node, merge=False)
-    sample.add_node(node2, merge=False)
-    text = json.dumps(sample._to_dict(), indent=3)
-    update = my_server.requisitions.update_requisition(sample)
-    my_server.requisitions.import_requisition(name=sample.foreign_source, rescan=False)
+    # new_node = requisition.RequisitionNode(foreign_id="py", node_label="text")
+    # new_node.asset.append(requisition.AssetField(name="region", value="Blarg"))
+    # new_node.meta_data.append(
+    #     requisition.Metadata(context="requisition", key="key", value="value")
+    # )
+    # new_node.set_metadata(key="hello", value="there")
+    # new_node.set_metadata(key="key", value="new_value")
+
+    # my_interface = requisition.Interface(ip_addr="127.4.3.2", snmp_primary="P")
+
+    # new_service = requisition.Service(
+    #     service_name="SNMP",
+    #     meta_data=[
+    #         requisition.Metadata(context="requisition", key="key", value="value")
+    #     ],
+    # )
+    # my_interface.monitored_service.append(new_service)
+
+    # new_node.add_interface(my_interface, merge=False)
+
+    # node2 = requisition.RequisitionNode(foreign_id="two", node_label="text2")
+    # node2.add_interface(my_interface, merge=False)
+    # node2.change_ip(old_ip="127.4.3.2", new_ip="127.7.8.9")
+
+    # sample.add_node(new_node, merge=False)
+    # sample.add_node(node2, merge=False)
+    # text = json.dumps(sample._to_dict(), indent=3)
+    # update = my_server.requisitions.update_requisition(sample)
+    # my_server.requisitions.import_requisition(name=sample.foreign_source, rescan=False)
     # print(text)
-    new_fs = foreign_source.ForeignSource(name="Example")
-    new_fs.add_detector(
-        foreign_source.Detector(
-            name="ICMP",
-            class_type="org.opennms.netmgt.provision.detector.icmp.IcmpDetector",
-        ),
-        merge=False,
-    )
-    new_fs.add_detector(
-        foreign_source.Detector(
-            name="ICMP2",
-            class_type="org.opennms.netmgt.provision.detector.icmp.IcmpDetector",
-            parameters=[Parameter(key="ipMatch", value="~.*")],
-        ),
-        merge=False,
-    )
-    new_fs.add_policy(
-        foreign_source.Policy(
-            name="blork",
-            class_type="org.opennms.netmgt.provision.persist.policies.MatchingSnmpInterfacePolicy",
-            parameters=[Parameter(key="ifType", value="6")],
-        ),
-        merge=False,
-    )
-    new_fs.add_policy(
-        foreign_source.Policy(
-            name="blosfdgrk",
-            class_type="org.opennms.netmgt.provision.persist.policies.MatchingSnmpInterfacePolicy",
-            parameters=[
-                Parameter(key="ifType", value="6"),
-                Parameter(key="ifAlias", value="~.*"),
-            ],
-        ),
-        merge=False,
-    )
-    update_fs = my_server.fs.update_foreign_source(new_fs)
-    my_server.requisitions.import_requisition(name=new_fs.name, rescan=False)
+    # new_fs = foreign_source.ForeignSource(name="Example")
+    # new_fs.add_detector(
+    #     foreign_source.Detector(
+    #         name="ICMP",
+    #         class_type="org.opennms.netmgt.provision.detector.icmp.IcmpDetector",
+    #     ),
+    #     merge=False,
+    # )
+    # new_fs.add_detector(
+    #     foreign_source.Detector(
+    #         name="ICMP2",
+    #         class_type="org.opennms.netmgt.provision.detector.icmp.IcmpDetector",
+    #         parameters=[Parameter(key="ipMatch", value="~.*")],
+    #     ),
+    #     merge=False,
+    # )
+    # new_fs.add_policy(
+    #     foreign_source.Policy(
+    #         name="blork",
+    #         class_type="org.opennms.netmgt.provision.persist.policies.MatchingSnmpInterfacePolicy",
+    #         parameters=[Parameter(key="ifType", value="6")],
+    #     ),
+    #     merge=False,
+    # )
+    # new_fs.add_policy(
+    #     foreign_source.Policy(
+    #         name="blosfdgrk",
+    #         class_type="org.opennms.netmgt.provision.persist.policies.MatchingSnmpInterfacePolicy",
+    #         parameters=[
+    #             Parameter(key="ifType", value="6"),
+    #             Parameter(key="ifAlias", value="~.*"),
+    #         ],
+    #     ),
+    #     merge=False,
+    # )
+    # update_fs = my_server.fs.update_foreign_source(new_fs)
+    # my_server.requisitions.import_requisition(name=new_fs.name, rescan=False)
     pass
```

### Comparing `pyonms-0.0.8/examples/portal.py` & `pyonms-0.0.9/examples/portal.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/__init__.py` & `pyonms-0.0.9/pyonms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # __init__.py
 
+
+# cSpell: ignore UDLAPI
+
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from multiprocessing import current_process
 from urllib.parse import urlsplit
 
 import pyonms.dao.alarms
 import pyonms.dao.business_services
 import pyonms.dao.events
 import pyonms.dao.foreign_sources
 import pyonms.dao.health
 import pyonms.dao.info
 import pyonms.dao.nodes
 import pyonms.dao.requisitions
+import pyonms.dao.udl
 from pyonms.models.event import Event, EventParameter
+from pyonms.models.exceptions import InvalidValueError
 
 
 class PyONMS:
     def __init__(self, hostname: str, username: str, password: str, name: str = None):
         """Attributes:
             hostname (str): OpenNMS URL
             username (str): Username
             password (str): Password
-            name (str): Instance name
+            name (str): Instance name. Defaults to hostname if omitted.
         Returns:
             `PyONMS` object
         """
         self.hostname = hostname
         args = {
             "hostname": hostname,
             "username": username,
@@ -62,23 +67,29 @@
         """`pyonms.dao.events.EventAPI` endpoint"""
         self.fs = pyonms.dao.foreign_sources.ForeignSourceAPI(args)
         """`pyonms.dao.foreign_sources.ForeignSourceAPI` endpoint"""
         self.nodes = pyonms.dao.nodes.NodeAPI(args)
         """`pyonms.dao.nodes.NodeAPI` endpoint"""
         self.requisitions = pyonms.dao.requisitions.RequisitionsAPI(args)
         """`pyonms.dao.requisitions.RequisitionsAPI` endpoint"""
+        self.udl = pyonms.dao.udl.UDLAPI(args)
+        """`pyonms.dao.udl.UDLAPI` endpoint"""
 
     def __repr__(self):
         return self.hostname
 
     def reload_daemon(self, name: str):
         """Send event to reload a given daemon
         Attributes:
             name (str): Daemon name
         """
+        if name.lower() not in self.server_status.enabled_services:
+            raise InvalidValueError(
+                name="name", value=name, valid=self.server_status.enabled_services
+            )
         reload_event = Event(
             uei="uei.opennms.org/internal/reloadDaemonConfig", source="pyonms"
         )
         reload_event.parameters.append(
             EventParameter(name="daemonName", value=name, type="string")
         )
         self.events.send_event(reload_event)
```

### Comparing `pyonms-0.0.8/pyonms/dao/__init__.py` & `pyonms-0.0.9/pyonms/dao/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # dao.__init__.py
 
 from typing import List
 
 import requests
-
 from requests.auth import HTTPBasicAuth
 from tqdm import tqdm
 
 import pyonms.utils
 from pyonms.models.exceptions import AuthenticationError
 
 
@@ -77,16 +76,20 @@
         #        uri=uri, headers=headers, params=params, endpoint=endpoint
         #    )
         if endpoint != "raw":
             for key, value in self.headers.items():
                 headers[key] = value
         response = requests.get(uri, auth=self.auth, headers=headers, params=params)
         if response.status_code == 200:
+            if response.encoding in ("ISO-8859-1"):
+                return response.text
             if "was not found" not in response.text:
                 return response.json()
+        elif response.status_code == 401:
+            raise AuthenticationError
         return {}
 
     def _get_v1(
         self, uri: str, endpoint: str, headers: dict = {}, params: dict = {}
     ) -> dict:
         response = requests.get(uri, auth=self.auth, headers=headers, params=params)
         if response.status_code == 200:
```

### Comparing `pyonms-0.0.8/pyonms/dao/business_services.py` & `pyonms-0.0.9/pyonms/dao/business_services.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/dao/events.py` & `pyonms-0.0.9/pyonms/dao/events.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dao.events.py
 
 from typing import List, Union
 
-from pyonms.dao import Endpoint
 import pyonms.models.event
 import pyonms.models.node
+from pyonms.dao import Endpoint
 
 
 class EventAPI(Endpoint):
     def __init__(self, kwargs):
         super().__init__(**kwargs)
         self.url = self.base_v2 + "events"
```

### Comparing `pyonms-0.0.8/pyonms/dao/foreign_sources.py` & `pyonms-0.0.9/pyonms/dao/foreign_sources.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # dao.foreign_sources.py
 
 from typing import List, Optional
 
 import requests
 
-from pyonms.dao import Endpoint
 import pyonms.models.foreign_source
+from pyonms.dao import Endpoint
 
 
 class ForeignSourceAPI(Endpoint):
     def __init__(self, kwargs):
         super().__init__(**kwargs)
         self.url = self.base_v1 + "foreignSources"
```

### Comparing `pyonms-0.0.8/pyonms/dao/health.py` & `pyonms-0.0.9/pyonms/dao/health.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # dao.health.py
 
-from pyonms.dao import Endpoint
-
 import pyonms.models.health
+from pyonms.dao import Endpoint
 
 
 class HealthAPI(Endpoint):
     def __init__(self, kwargs):
         super().__init__(**kwargs)
         self.url = self.base_v1 + "health"
 
-    def get_health(self) -> pyonms.models.health.Health:
+    def get_health(self) -> str:
         record = self._get(uri=f"{self.url}", endpoint="raw")
         if record is not None:
             health = self._process_health(record)
-            if health.healthy:
+            if health.healthy is True:
                 print(f"Connected to {self.name}")
-            else:
+            elif health.healthy is False:
                 print(f"{self.name} is not healthy")
+            else:
+                print(f"{self.name} health status unknown")
             return health
         else:
             return None
 
     def probe(self) -> str:
         return self._get(uri=f"{self.url}/probe", endpoint="raw")
```

### Comparing `pyonms-0.0.8/pyonms/dao/info.py` & `pyonms-0.0.9/pyonms/dao/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # dao.info.py
 
-from pyonms.dao import Endpoint
-
 import pyonms.models.info
+from pyonms.dao import Endpoint
 
 
 class InfoAPI(Endpoint):
     def __init__(self, kwargs):
         super().__init__(**kwargs)
         self.url = self.base_v1 + "info"
```

### Comparing `pyonms-0.0.8/pyonms/dao/nodes.py` & `pyonms-0.0.9/pyonms/dao/nodes.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/dao/requisitions.py` & `pyonms-0.0.9/pyonms/dao/requisitions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/models/alarm.py` & `pyonms-0.0.9/pyonms/models/alarm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 # models.alarm.py
 
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import List, Union
+from typing import List, Optional
 
 from pyonms.models.event import Event, EventParameter, Severity
 from pyonms.models.node import ServiceType
 from pyonms.utils import convert_time
 
 
 @dataclass(repr=False)
 class Alarm:
     id: int
-    uei: str
-    location: str
+    reductionKey: str
     type: int
     severity: Severity
     description: str
     logMessage: str
-    suppressedUntil: datetime
-    suppressedTime: datetime
-    x733ProbableCause: int
-    affectedNodeCount: int
-    reductionKey: str
-    count: int
-    firstEventTime: datetime
+    uei: str = None
+    location: str = None
+    suppressedUntil: datetime = None
+    suppressedTime: datetime = None
+    x733ProbableCause: int = None
+    affectedNodeCount: int = None
+    count: int = None
+    firstEventTime: datetime = None
     lastEventTime: datetime = None
     nodeId: int = None
     nodeLabel: str = None
     ipAddress: str = None
     ifIndex: int = None
     clearKey: str = None
     ackUser: str = None
     ackTime: int = None
     stickyMemo: str = None
     reductionKeyMemo: str = None
     troubleTicket: str = None
     troubleTicketLink: str = None
     troubleTicketState: int = None
     qosAlarmState: str = None
-    firstEvent: Union[Event, None] = field(default_factory=dict)
-    lastEvent: Union[Event, None] = field(default_factory=dict)
-    parameters: List[Union[EventParameter, None]] = field(default_factory=list)
+    managedObjectInstance: str = None
+    managedObjectType: str = None
+    label: str = None
+    firstEvent: Optional[Event] = field(default_factory=dict)
+    lastEvent: Optional[Event] = field(default_factory=dict)
+    parameters: List[Optional[EventParameter]] = field(default_factory=list)
+    relatedAlarms: Optional[List["Alarm"]] = field(default_factory=list)
     serviceType: ServiceType = field(default_factory=dict)
 
     def __post_init__(self):
         self.suppressedUntil = convert_time(self.suppressedUntil)
         self.suppressedTime = convert_time(self.suppressedTime)
         self.firstEventTime = convert_time(self.firstEventTime)
         self.lastEventTime = convert_time(self.lastEventTime)
         self.ackTime = convert_time(self.ackTime)
         self.severity = Severity[self.severity]
         if self.lastEvent:
             self.lastEvent = Event(**self.lastEvent)
         self.parameters = [EventParameter(**parameter) for parameter in self.parameters]
         if self.serviceType:
             self.serviceType = ServiceType(**self.serviceType)
+        if self.relatedAlarms:
+            relations = []
+            for related in self.relatedAlarms:
+                relations.append(Alarm(**related))
+            self.relatedAlarms = relations
 
     def __repr__(self):
         return f"Alarm(id={self.id}, reductionKey={self.reductionKey})"
```

### Comparing `pyonms-0.0.8/pyonms/models/business_service.py` & `pyonms-0.0.9/pyonms/models/business_service.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # models.business_service.py
 
-from enum import Enum
 from dataclasses import dataclass, field
+from enum import Enum
 from typing import List, Optional
 
 from pyonms.models import exceptions
 
 
 class Severity(Enum):
     INDETERMINATE = "Indeterminate"
```

### Comparing `pyonms-0.0.8/pyonms/models/exceptions.py` & `pyonms-0.0.9/pyonms/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/models/foreign_source.py` & `pyonms-0.0.9/pyonms/models/foreign_source.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/models/health.py` & `pyonms-0.0.9/pyonms/models/health.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # models.health.py
 
-from dataclasses import dataclass
-
+from dataclasses import dataclass, field
 from typing import List, Optional
 
 
 @dataclass
 class Response:
     description: str
     status: str
@@ -17,16 +16,16 @@
             self.success = True
         else:
             pass
 
 
 @dataclass(repr=False)
 class Health:
-    healthy: bool
-    responses: List[Response]
+    healthy: bool = None
+    responses: List[Response] = field(default_factory=list)
 
     def __post_init__(self):
         responses = []
         for response in self.responses:
             responses.append(Response(**response))
         self.responses = responses
```

### Comparing `pyonms-0.0.8/pyonms/models/info.py` & `pyonms-0.0.9/pyonms/models/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # models.info.py
 
 
-from dataclasses import dataclass
-from typing import List, Optional
+from dataclasses import dataclass, field
+from typing import Dict, List, Optional
 
 
 @dataclass
 class Service:
     name: str
     status: str
 
@@ -44,33 +44,35 @@
 
     def __repr__(self):
         return f"Version({self.version_string})"
 
 
 @dataclass(repr=False)
 class Info:
-    displayVersion: str
-    version: str
-    packageName: str
-    packageDescription: str
-    ticketerConfig: TicketerConfig
-    datetimeformatConfig: DateFormat
-    services: List[Service]
+    displayVersion: str = None
+    version: str = None
+    packageName: str = None
+    packageDescription: str = None
+    ticketerConfig: TicketerConfig = None
+    datetimeformatConfig: DateFormat = None
+    services: List[Service] = field(default_factory=list)
+    enabled_services: List[str] = field(default_factory=list)
 
     def __post_init__(self):
         if isinstance(self.version, str):
             self.version = Version(version_string=self.version)
         if isinstance(self.displayVersion, str):
             self.displayVersion = Version(version_string=self.displayVersion)
         if isinstance(self.ticketerConfig, dict):
             self.ticketerConfig = TicketerConfig(**self.ticketerConfig)
         if isinstance(self.datetimeformatConfig, dict):
             self.datetimeformatConfig = DateFormat(**self.datetimeformatConfig)
         services = []
         for service, status in self.services.items():
             services.append(Service(name=service, status=status))
         self.services = services
+        self.enabled_services = [service.name.lower() for service in self.services]
 
     def __repr__(self):
         text = f"Info(version={self.displayVersion},"
         text += f" running_services={len([service for service in self.services if service.status == 'running'])}/{len(self.services)})"
         return text
```

### Comparing `pyonms-0.0.8/pyonms/models/node.py` & `pyonms-0.0.9/pyonms/models/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Active"
     DELETED = "D"
     "Deleted"
     UNKNOWN = " "
     "Unknown"
 
 
-class Managed(Enum):
+class ManagedIP(Enum):
     MANAGED = "M"
     "Managed"
     UNMANAGED = "U"
     "Unmanaged"
     DELETED = "D"
     "Deleted"
     ALIAS = "A"
@@ -45,14 +45,25 @@
     "Force Unmanaged"
     NOT_POLLED = "N"
     "Not Polled"
     REMOTELY_MONITORED = "X"
     "Remotely Monitored"
 
 
+class ServiceStatus(Enum):
+    MANAGED = "A"
+    UNMANAGED = "U"
+    DELETED = "D"
+    FORCE_UNMANAGED = "F"
+    NOT_MONITORED = "N"
+    RESCAN_TO_RESUME = "R"
+    RESCAN_TO_SUSPEND = "S"
+    REMOTELY_MONITORED = "X"
+
+
 class PrimaryType(Enum):
     PRIMARY = "P"
     "SNMP Primary"
     SECONDARY = "S"
     "SNMP Secondary"
     NOT_ELIGIBLE = "N"
     "No SNMP"
@@ -168,29 +179,31 @@
         return hash((self.id))
 
 
 @dataclass(repr=False)
 class Service:
     id: int
     notify: str = None
-    status: str = None
+    status: Union[ServiceStatus, str] = None
     qualifier: str = None
     down: bool = None
     source: str = None
     serviceType: ServiceType = None
     ipInterfaceId: int = None
     statusLong: str = None
     lastFail: datetime = None
     lastGood: datetime = None
     metadata: List[Optional[Metadata]] = field(default_factory=list)
     applications: List[Optional[str]] = field(default_factory=list)
 
     def __post_init__(self):
         if isinstance(self.serviceType, dict):
             self.serviceType = ServiceType(**self.serviceType)
+        if isinstance(self.status, str):
+            self.status = ServiceStatus(self.status)
         if isinstance(self.lastFail, int):
             self.lastFail = convert_time(self.lastFail)
         if isinstance(self.lastGood, int):
             self.lastGood = convert_time(self.lastGood)
 
     def __repr__(self):
         return f"Service(id={self.id}, serviceType={self.serviceType.name}, down={self.down})"
@@ -250,15 +263,15 @@
     isDown: bool = None
     nodeId: int = None
     ifIndex: int = None
     lastEgressFlow: Union[datetime, int] = None
     lastIngressFlow: Union[datetime, int] = None
     ipAddress: str = None
     snmpPrimary: Union[PrimaryType, str] = None
-    isManaged: Union[Managed, str] = None
+    isManaged: Union[ManagedIP, str] = None
     monitoredServiceCount: Optional[int] = None
     lastCapsdPoll: Optional[Union[datetime, int]] = None
     snmpInterface: Optional[Union[SnmpInterface, dict]] = field(default_factory=dict)
     services: List[Optional[Service]] = field(default_factory=list)
     metadata: List[Optional[Metadata]] = field(default_factory=list)
 
     def __post_init__(self):
@@ -267,15 +280,15 @@
         if isinstance(self.lastCapsdPoll, int):
             self.lastCapsdPoll = convert_time(self.lastCapsdPoll)
         if isinstance(self.lastEgressFlow, int):
             self.lastEgressFlow = convert_time(self.lastEgressFlow)
         if isinstance(self.lastIngressFlow, int):
             self.lastIngressFlow = convert_time(self.lastIngressFlow)
         if isinstance(self.isManaged, str):
-            self.isManaged = Managed(self.isManaged)
+            self.isManaged = ManagedIP(self.isManaged)
         if isinstance(self.snmpPrimary, str):
             self.snmpPrimary = PrimaryType(self.snmpPrimary)
         if self.snmpInterface and isinstance(self.snmpInterface, dict):
             self.snmpInterface = SnmpInterface(**self.snmpInterface)
 
     def __repr__(self):
         return f"IPInterface(id={self.id}, ipAddress={self.ipAddress})"
```

### Comparing `pyonms-0.0.8/pyonms/models/requisition.py` & `pyonms-0.0.9/pyonms/models/requisition.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/portal/__init__.py` & `pyonms-0.0.9/pyonms/portal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 from typing import List, Optional
 
 import requests
 from tqdm import tqdm
 
 from pyonms.models.exceptions import DuplicateEntityError
-
 from pyonms.portal.models import (
     PortalAppliance,
-    PortalApplianceStatus,
     PortalApplianceProfile,
-    PortalInstance,
-    PortalSubscription,
+    PortalApplianceStatus,
     PortalConnectivityProfile,
+    PortalConnectivityProfileCreate,
     PortalFeatureProfile,
-    PortalLocation,
+    PortalInstance,
     PortalInstanceCreate,
-    PortalConnectivityProfileCreate,
+    PortalLocation,
     PortalLocationCreate,
     PortalMinion,
+    PortalSubscription,
 )
 
 
 class Portal:
     def __init__(self, secret: str):
         """OpenNMS Cloud Portal
         Attributes:
```

### Comparing `pyonms-0.0.8/pyonms/portal/models.py` & `pyonms-0.0.9/pyonms/portal/models.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/pyonms/utils/__init__.py` & `pyonms-0.0.9/pyonms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/test-mock/mocks/node_all.json` & `pyonms-0.0.9/test-mock/mocks/node_all.json`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/test_alarms.py` & `pyonms-0.0.9/tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/test_events.py` & `pyonms-0.0.9/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/test_nodes.py` & `pyonms-0.0.9/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/test_requisitions.py` & `pyonms-0.0.9/tests/test_requisitions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_alarm_all.yaml` & `pyonms-0.0.9/tests/cassettes/test_alarm_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_alarm_batch.yaml` & `pyonms-0.0.9/tests/cassettes/test_alarm_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_alarm_one.yaml` & `pyonms-0.0.9/tests/cassettes/test_alarm_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_event_all.yaml` & `pyonms-0.0.9/tests/cassettes/test_event_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_event_batch.yaml` & `pyonms-0.0.9/tests/cassettes/test_event_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_event_one.yaml` & `pyonms-0.0.9/tests/cassettes/test_event_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_all.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_batch.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_ip.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_ip.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_ip_services.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_ip_services.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_metadata.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_one.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_node_snmp.yaml` & `pyonms-0.0.9/tests/cassettes/test_node_snmp.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_add_asset.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_add_asset.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_add_metadata.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_add_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_all.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_batch.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_count_active.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_count_active.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_count_deployed.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_count_deployed.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_import.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_import.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_one.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_update_asset.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_update_asset.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/tests/cassettes/test_requisition_update_metadata.yaml` & `pyonms-0.0.9/tests/cassettes/test_requisition_update_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/.gitignore` & `pyonms-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/LICENSE.txt` & `pyonms-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/README.md` & `pyonms-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 
 Currently supported endpoints include:
 
 * Alarms (read-only)
 * Business Services (read-write)
 * Events (read, send)
 * Foreign Sources (read-write)
-* Heath (read-only)
+* Health (read-only)
 * Info (read-only)
 * Nodes (read-only)
 * Requisitions (read-write)
 
 ## Getting Started
 
+You can install this library by running:
+
+```
+pip3 install pyonms
+```
+
 See the [project documentation](https://mmahacek.github.io/PyONMS/) for instructions on using this library.
```

### Comparing `pyonms-0.0.8/pyproject.toml` & `pyonms-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.8/PKG-INFO` & `pyonms-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonms
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for accessing the OpenNMS REST API.
 Project-URL: Homepage, https://github.com/mmahacek/PyONMS
 Project-URL: Documentation, https://mmahacek.github.io/PyONMS/
 Author-email: Mark Mahacek <mmahacek@opennms.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -43,15 +43,21 @@
 
 Currently supported endpoints include:
 
 * Alarms (read-only)
 * Business Services (read-write)
 * Events (read, send)
 * Foreign Sources (read-write)
-* Heath (read-only)
+* Health (read-only)
 * Info (read-only)
 * Nodes (read-only)
 * Requisitions (read-write)
 
 ## Getting Started
 
+You can install this library by running:
+
+```
+pip3 install pyonms
+```
+
 See the [project documentation](https://mmahacek.github.io/PyONMS/) for instructions on using this library.
```

