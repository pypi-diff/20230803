# Comparing `tmp/edx-event-routing-backends-5.5.3.tar.gz` & `tmp/edx-event-routing-backends-5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-5.5.3.tar", last modified: Wed Aug  2 16:40:56 2023, max compression
+gzip compressed data, was "edx-event-routing-backends-5.5.4.tar", last modified: Thu Aug  3 17:54:44 2023, max compression
```

## Comparing `edx-event-routing-backends-5.5.3.tar` & `edx-event-routing-backends-5.5.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.279588 edx-event-routing-backends-5.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-02 16:40:56.279588 edx-event-routing-backends-5.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.255587 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4995 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-02 16:40:56.000000 edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.255587 edx-event-routing-backends-5.5.3/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.255587 edx-event-routing-backends-5.5.3/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/backends/events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.255587 edx-event-routing-backends-5.5.3/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.255587 edx-event-routing-backends-5.5.3/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/queued_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10799 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.259587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.263587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.267587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/forum_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.267587 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.267587 edx-event-routing-backends-5.5.3/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.251587 edx-event-routing-backends-5.5.3/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.251587 edx-event-routing-backends-5.5.3/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.267587 edx-event-routing-backends-5.5.3/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.251587 edx-event-routing-backends-5.5.3/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.267587 edx-event-routing-backends-5.5.3/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.275587 edx-event-routing-backends-5.5.3/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.275587 edx-event-routing-backends-5.5.3/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:40:56.279588 edx-event-routing-backends-5.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-08-02 16:40:56.279588 edx-event-routing-backends-5.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-08-02 16:40:51.000000 edx-event-routing-backends-5.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4995 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/queued_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10799 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/setup.py
```

### Comparing `edx-event-routing-backends-5.5.3/CHANGELOG.rst` & `edx-event-routing-backends-5.5.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/LICENSE.txt` & `edx-event-routing-backends-5.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/PKG-INFO` & `edx-event-routing-backends-5.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.3
+Version: 5.5.4
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-5.5.3/README.rst` & `edx-event-routing-backends-5.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.3
+Version: 5.5.4
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-5.5.3/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/admin.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/apps.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/backends/events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/test_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/helpers.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/models.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/forum_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/forum_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,24 +147,27 @@
         """
         Get result for xAPI transformed event.
 
         Returns:
             `Result`
         """
         event_data = self.get_data('data')
-        if event_data['weighted_possible'] > 0:
-            scaled = event_data['weighted_earned']/event_data['weighted_possible']
+        weighted_possible = event_data['weighted_possible'] or 0
+        weighted_earned = event_data['weighted_earned'] or 0
+
+        if weighted_possible > 0:
+            scaled = weighted_earned/weighted_possible
         else:
             scaled = 0
         return Result(
-            success=event_data['weighted_earned'] >= event_data['weighted_possible'],
+            success=weighted_earned >= weighted_possible,
             score={
                 'min': 0,
-                'max': event_data['weighted_possible'],
-                'raw': event_data['weighted_earned'],
+                'max': weighted_possible,
+                'raw': weighted_earned,
                 'scaled': scaled
             }
         )
 
 
 @XApiTransformersRegistry.register('problem_check')
 class ProblemCheckTransformer(BaseProblemsTransformer):
```

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/settings/common.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/settings/production.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tasks.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-5.5.4/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/requirements/constraints.txt` & `edx-event-routing-backends-5.5.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.3/setup.py` & `edx-event-routing-backends-5.5.4/setup.py`

 * *Files identical despite different names*

