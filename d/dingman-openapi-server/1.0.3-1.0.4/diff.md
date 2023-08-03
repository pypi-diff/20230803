# Comparing `tmp/dingman_openapi_server-1.0.3.tar.gz` & `tmp/dingman_openapi_server-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingman_openapi_server-1.0.3.tar", last modified: Fri Jul 14 21:12:22 2023, max compression
+gzip compressed data, was "dist/dingman_openapi_server-1.0.4.tar", last modified: Fri Jul 14 21:13:42 2023, max compression
```

## Comparing `dingman_openapi_server-1.0.3.tar` & `dingman_openapi_server-1.0.4.tar`

### file list

```diff
@@ -1,87 +1,86 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.334999 dingman_openapi_server-1.0.3/
--rw-r--r--   0 jialening   (501) staff       (20)       44 2023-07-14 18:25:25.000000 dingman_openapi_server-1.0.3/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      259 2023-07-14 21:12:22.334418 dingman_openapi_server-1.0.3/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 dingman_openapi_server-1.0.3/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.274823 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      259 2023-07-14 21:12:22.000000 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     3072 2023-07-14 21:12:22.000000 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-14 21:12:22.000000 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-14 21:12:22.000000 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-14 21:12:22.000000 dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/top_level.txt
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.280714 dingman_openapi_server-1.0.3/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-14 21:11:44.000000 dingman_openapi_server-1.0.3/openapi_server/.DS_Store
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.282492 dingman_openapi_server-1.0.3/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.327276 dingman_openapi_server-1.0.3/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     3696 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     6281 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     5905 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/topology_spread_constraint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 20:08:38.000000 dingman_openapi_server-1.0.3/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    13070 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.328219 dingman_openapi_server-1.0.3/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   172537 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/openapi/openapi.yaml
--rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-14 20:08:40.000000 dingman_openapi_server-1.0.3/openapi_server/openapi_version
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:12:22.332149 dingman_openapi_server-1.0.3/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   129787 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 20:08:39.000000 dingman_openapi_server-1.0.3/openapi_server/util.py
--rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-14 20:08:40.000000 dingman_openapi_server-1.0.3/openapi_version
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-14 21:12:22.335212 dingman_openapi_server-1.0.3/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)      847 2023-07-14 18:25:25.000000 dingman_openapi_server-1.0.3/setup.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.186473 dingman_openapi_server-1.0.4/
+-rw-r--r--   0 jialening   (501) staff       (20)       44 2023-07-14 18:25:25.000000 dingman_openapi_server-1.0.4/MANIFEST.in
+-rw-r--r--   0 jialening   (501) staff       (20)      259 2023-07-14 21:13:42.186020 dingman_openapi_server-1.0.4/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 dingman_openapi_server-1.0.4/README.md
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.143297 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/
+-rw-r--r--   0 jialening   (501) staff       (20)      259 2023-07-14 21:13:42.000000 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)     3047 2023-07-14 21:13:42.000000 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/SOURCES.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-14 21:13:42.000000 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/dependency_links.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-14 21:13:42.000000 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/requires.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-14 21:13:42.000000 dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/top_level.txt
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.147177 dingman_openapi_server-1.0.4/openapi_server/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/__main__.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.149010 dingman_openapi_server-1.0.4/openapi_server/controllers/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/controllers/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/encoder.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.182953 dingman_openapi_server-1.0.4/openapi_server/models/
+-rw-r--r--   0 jialening   (501) staff       (20)     3696 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/models/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/models/base_model_.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/container.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/container_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/dingman_error.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/dingman_response.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/endpoint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/env_from_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/env_var.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/env_var_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/http_get.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ingress.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/node_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/node_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6281 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/pod.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/probe.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/relabel_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/service_monitor.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/service_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5905 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/topology_spread_constraint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/update_strategy.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume_device.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume_mount.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)    13070 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/models/workload.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.183415 dingman_openapi_server-1.0.4/openapi_server/openapi/
+-rw-r--r--   0 jialening   (501) staff       (20)   172537 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/openapi/openapi.yaml
+-rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/openapi_version
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 21:13:42.184846 dingman_openapi_server-1.0.4/openapi_server/test/
+-rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/test/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)   129787 2023-07-14 21:13:37.000000 dingman_openapi_server-1.0.4/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/typing_utils.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_server/util.py
+-rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-14 21:13:38.000000 dingman_openapi_server-1.0.4/openapi_version
+-rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-14 21:13:42.186608 dingman_openapi_server-1.0.4/setup.cfg
+-rw-r--r--   0 jialening   (501) staff       (20)      847 2023-07-14 18:25:25.000000 dingman_openapi_server-1.0.4/setup.py
```

### Comparing `dingman_openapi_server-1.0.3/README.md` & `dingman_openapi_server-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/dingman_openapi_server.egg-info/SOURCES.txt` & `dingman_openapi_server-1.0.4/dingman_openapi_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 openapi_version
 setup.py
 dingman_openapi_server.egg-info/PKG-INFO
 dingman_openapi_server.egg-info/SOURCES.txt
 dingman_openapi_server.egg-info/dependency_links.txt
 dingman_openapi_server.egg-info/requires.txt
 dingman_openapi_server.egg-info/top_level.txt
-openapi_server/.DS_Store
 openapi_server/__init__.py
 openapi_server/__main__.py
 openapi_server/encoder.py
 openapi_server/openapi_version
 openapi_server/typing_utils.py
 openapi_server/util.py
 openapi_server/controllers/__init__.py
```

### Comparing `dingman_openapi_server-1.0.3/openapi_server/controllers/deploy_resources_controller.py` & `dingman_openapi_server-1.0.4/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/controllers/security_controller_.py` & `dingman_openapi_server-1.0.4/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/encoder.py` & `dingman_openapi_server-1.0.4/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/__init__.py` & `dingman_openapi_server-1.0.4/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/affinity.py` & `dingman_openapi_server-1.0.4/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/base_model_.py` & `dingman_openapi_server-1.0.4/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/config.py` & `dingman_openapi_server-1.0.4/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/config_templates_inner.py` & `dingman_openapi_server-1.0.4/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/container.py` & `dingman_openapi_server-1.0.4/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/container_life_cycle.py` & `dingman_openapi_server-1.0.4/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/container_port.py` & `dingman_openapi_server-1.0.4/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/container_sec_context.py` & `dingman_openapi_server-1.0.4/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/container_sec_context_capabilities.py` & `dingman_openapi_server-1.0.4/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/deploy_platform_resource.py` & `dingman_openapi_server-1.0.4/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/deploy_resources.py` & `dingman_openapi_server-1.0.4/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/dingman_error.py` & `dingman_openapi_server-1.0.4/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/dingman_response.py` & `dingman_openapi_server-1.0.4/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/endpoint.py` & `dingman_openapi_server-1.0.4/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/env_from_source.py` & `dingman_openapi_server-1.0.4/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/env_var.py` & `dingman_openapi_server-1.0.4/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/env_var_source.py` & `dingman_openapi_server-1.0.4/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/http_get.py` & `dingman_openapi_server-1.0.4/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/http_ingress_path.py` & `dingman_openapi_server-1.0.4/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ingress.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ingress_backend.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ingress_backend_service.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ingress_rule.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ingress_tls.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/life_cycle_handler.py` & `dingman_openapi_server-1.0.4/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/node_affinity.py` & `dingman_openapi_server-1.0.4/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/node_selector.py` & `dingman_openapi_server-1.0.4/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/node_selector_term.py` & `dingman_openapi_server-1.0.4/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/object_field_selector.py` & `dingman_openapi_server-1.0.4/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/persistent_volume_claim.py` & `dingman_openapi_server-1.0.4/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/pod.py` & `dingman_openapi_server-1.0.4/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/pod_affinity.py` & `dingman_openapi_server-1.0.4/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/pod_affinity_term.py` & `dingman_openapi_server-1.0.4/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/pod_anti_affinity.py` & `dingman_openapi_server-1.0.4/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/preferred_scheduling_term.py` & `dingman_openapi_server-1.0.4/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/probe.py` & `dingman_openapi_server-1.0.4/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/ref_volume_source.py` & `dingman_openapi_server-1.0.4/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/relabel_config.py` & `dingman_openapi_server-1.0.4/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/resource_requirements.py` & `dingman_openapi_server-1.0.4/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/service.py` & `dingman_openapi_server-1.0.4/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/service_monitor.py` & `dingman_openapi_server-1.0.4/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/service_monitor_namespace_selector.py` & `dingman_openapi_server-1.0.4/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/service_port.py` & `dingman_openapi_server-1.0.4/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/tcp_socket.py` & `dingman_openapi_server-1.0.4/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/topology_spread_constraint.py` & `dingman_openapi_server-1.0.4/openapi_server/models/topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/update_strategy.py` & `dingman_openapi_server-1.0.4/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/update_strategy_rolling_update_config.py` & `dingman_openapi_server-1.0.4/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume_device.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume_empty_dir.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume_host_path.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume_mount.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/volume_persistent_volume_claim.py` & `dingman_openapi_server-1.0.4/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/weighted_pod_affinity_term.py` & `dingman_openapi_server-1.0.4/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/models/workload.py` & `dingman_openapi_server-1.0.4/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/openapi/openapi.yaml` & `dingman_openapi_server-1.0.4/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/test/test_deploy_resources_controller.py` & `dingman_openapi_server-1.0.4/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/typing_utils.py` & `dingman_openapi_server-1.0.4/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/openapi_server/util.py` & `dingman_openapi_server-1.0.4/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.3/setup.py` & `dingman_openapi_server-1.0.4/setup.py`

 * *Files identical despite different names*

