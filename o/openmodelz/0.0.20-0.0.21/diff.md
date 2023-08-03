# Comparing `tmp/openmodelz-0.0.20.tar.gz` & `tmp/openmodelz-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodelz-0.0.20.tar", last modified: Wed Aug  2 08:02:45 2023, max compression
+gzip compressed data, was "openmodelz-0.0.21.tar", last modified: Thu Aug  3 03:52:09 2023, max compression
```

## Comparing `openmodelz-0.0.20.tar` & `openmodelz-0.0.21.tar`

### file list

```diff
@@ -1,249 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.all-contributorsrc
--rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.goreleaser.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-02 08:00:54.000000 openmodelz-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-02 08:00:54.000000 openmodelz-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-02 08:02:45.494389 openmodelz-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-08-02 08:00:54.000000 openmodelz-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/agent/
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     7231 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/api/types/
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/build.go
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/const.go
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/error.go
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/event.go
--rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_deployment.go
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_deployment_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_status.go
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/info.go
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/log.go
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/namespace.go
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/queue.go
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/requests.go
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/secret.go
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/server.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/client/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/build.go
--rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/client.go
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/const.go
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/errors.go
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/hijack.go
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_remove.go
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_scale.go
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/info.go
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/instance_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/instance_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/log.go
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/namespace_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/options.go
--rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/request.go
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/transport.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/cmd/agent/
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/cmd/agent/main.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/errdefs/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/defs.go
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/doc.go
--rw-r--r--   0 runner    (1001) docker     (122)     5850 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/helpers.go
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/http_helpers.go
--rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/is.go
--rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/go.mod
--rw-r--r--   0 runner    (1001) docker     (122)   114827 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/app/
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/app/config.go
--rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/app/root.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/config/
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/config/config.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/consts/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/consts/consts.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    37721 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/docs/docs.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/event/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/event.go
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/fake.go
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/username.go
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/util.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/k8s/
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_deployment.go
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_inference.go
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_job.go
--rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_pod.go
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/generate_job.go
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/resolver.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/log/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/factory.go
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/k8s.go
--rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/loki.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     4042 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/metrics/exporter.go
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/metrics/metrics.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/prom/
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/prom/prometheus_query.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/query/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/db.go
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/deployment_events.sql.go
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/models.go
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/querier.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.482389 openmodelz-0.0.20/agent/pkg/runtime/
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/build.go
--rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_replicas.go
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/namespace.go
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/runtime.go
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/util_domain.go
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/util_resource.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.482389 openmodelz-0.0.20/agent/pkg/scaling/
--rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/function_scaler.go
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/ranges.go
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/retry.go
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/service_query.go
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/util.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/server/
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/error.go
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_healthz.go
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_instance_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_scale.go
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_info.go
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_namespace_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_namespace_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/middleware_callid.go
--rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_factory.go
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_handlerfunc.go
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_kubernetes.go
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_metrics.go
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_route.go
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_run.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/server/validator/
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/validator/validator.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/version/
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/version/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/sql/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/sql/query/
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sql/query/deployment_events.sql
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sql/schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sqlc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     7866 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/cmd/mdz/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/cmd/mdz/main.go
--rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/go.mod
--rw-r--r--   0 runner    (1001) docker     (122)    26290 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/hack/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/hack/cli-doc-gen/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/hack/cli-doc-gen/main.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/pkg/agentd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/pkg/agentd/runtime/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/create.go
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/delete.go
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/label.go
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/list.go
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/runtime.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/pkg/agentd/server/
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/error.go
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_healthz.go
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_info.go
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/middleware_callid.go
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_factory.go
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_handlerfunc.go
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_init_route.go
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_run.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/deploy.go
--rw-r--r--   0 runner    (1001) docker     (122)     5225 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/exec_stream.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/ioutils/
--rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/ioutils/reader.go
--rw-r--r--   0 runner    (1001) docker     (122)     3634 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/list_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/localagent.go
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/portforward.go
--rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/root.go
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/scale.go
--rw-r--r--   0 runner    (1001) docker     (122)      898 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server.go
--rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_join.go
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_label.go
--rw-r--r--   0 runner    (1001) docker     (122)     3306 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_start.go
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_stop.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/streams/
--rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/in.go
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/out.go
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/stream.go
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/server/
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/agentd_run.go
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/engine.go
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/gpu-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/gpu_install.go
--rw-r--r--   0 runner    (1001) docker     (122)    32313 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_install.go
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_join.go
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_killall.go
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_prepare.go
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/nginx-dep.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/nginx_install.go
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/openmodelz.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/openmodelz_install.go
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/registries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/term/
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/term/interrupt.go
--rw-r--r--   0 runner    (1001) docker     (122)     4045 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/term/term.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/mdz/pkg/version/
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/version/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/openmodelz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6143 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-08-02 08:00:54.000000 openmodelz-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 08:02:45.494389 openmodelz-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-08-02 08:00:54.000000 openmodelz-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.782273 openmodelz-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-08-03 03:50:36.000000 openmodelz-0.0.21/.all-contributorsrc
+-rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-08-03 03:50:36.000000 openmodelz-0.0.21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-08-03 03:50:36.000000 openmodelz-0.0.21/.goreleaser.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-03 03:50:36.000000 openmodelz-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-03 03:50:36.000000 openmodelz-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-03 03:52:09.782273 openmodelz-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-08-03 03:50:36.000000 openmodelz-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.766273 openmodelz-0.0.21/agent/
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     7231 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.758273 openmodelz-0.0.21/agent/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.766273 openmodelz-0.0.21/agent/api/types/
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/const.go
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/event.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/inference_deployment.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/inference_deployment_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/inference_status.go
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/info.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/log.go
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/namespace.go
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/queue.go
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/requests.go
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/secret.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/api/types/server.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.766273 openmodelz-0.0.21/agent/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/client.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/const.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/errors.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/hijack.go
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_remove.go
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/info.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/instance_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/instance_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/log.go
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/namespace_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/options.go
+-rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/request.go
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/client/transport.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.758273 openmodelz-0.0.21/agent/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.766273 openmodelz-0.0.21/agent/cmd/agent/
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/cmd/agent/main.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.766273 openmodelz-0.0.21/agent/errdefs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/errdefs/defs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/errdefs/doc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5850 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/errdefs/helpers.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/errdefs/http_helpers.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/errdefs/is.go
+-rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/go.mod
+-rw-r--r--   0 runner    (1001) docker     (122)   114827 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.762273 openmodelz-0.0.21/agent/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/app/
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/app/config.go
+-rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/app/root.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/config/config.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/consts/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/consts/consts.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    37721 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/docs/docs.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/event/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/event/event.go
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/event/fake.go
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/event/username.go
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/event/util.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/k8s/
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/convert_deployment.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/convert_inference.go
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/convert_job.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/convert_pod.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/generate_job.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/k8s/resolver.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/log/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/log/factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/log/k8s.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/log/loki.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     4042 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/metrics/exporter.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/metrics/metrics.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/prom/
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/prom/prometheus_query.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/query/db.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/query/deployment_events.sql.go
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/query/models.go
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/query/querier.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_replicas.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/namespace.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/runtime.go
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/util_domain.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/runtime/util_resource.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.770273 openmodelz-0.0.21/agent/pkg/scaling/
+-rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/scaling/function_scaler.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/scaling/ranges.go
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/scaling/retry.go
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/scaling/service_query.go
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/scaling/util.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/agent/pkg/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_build_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_build_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_build_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_build_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_healthz.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_instance_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_info.go
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_namespace_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_namespace_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/handler_server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/middleware_callid.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_handlerfunc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_init_kubernetes.go
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_init_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_init_metrics.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_init_route.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/server_run.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/agent/pkg/server/validator/
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/server/validator/validator.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/agent/pkg/version/
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/pkg/version/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/agent/sql/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/agent/sql/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/sql/query/deployment_events.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/sql/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-08-03 03:50:36.000000 openmodelz-0.0.21/agent/sqlc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/mdz/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     7852 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.762273 openmodelz-0.0.21/mdz/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/mdz/cmd/mdz/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/cmd/mdz/main.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/go.mod
+-rw-r--r--   0 runner    (1001) docker     (122)    26658 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.762273 openmodelz-0.0.21/mdz/hack/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/mdz/hack/cli-doc-gen/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/hack/cli-doc-gen/main.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.762273 openmodelz-0.0.21/mdz/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.762273 openmodelz-0.0.21/mdz/pkg/agentd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.774273 openmodelz-0.0.21/mdz/pkg/agentd/runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/label.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/runtime/runtime.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/agentd/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_healthz.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/handler_info.go
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/middleware_callid.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/server_factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/server_handlerfunc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/server_init_route.go
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/agentd/server/server_run.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3801 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/deploy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5225 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/exec_stream.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/cmd/ioutils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/ioutils/reader.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/list_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/localagent.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/portforward.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3424 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/root.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)      898 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_destroy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_join.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_label.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_start.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/server_stop.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/cmd/streams/
+-rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/streams/in.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/streams/out.go
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/streams/stream.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/cmd/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/server/
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/agentd_run.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/engine.go
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/gpu-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/gpu_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)    32313 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s-install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s_destroy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s_join.go
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s_killall.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/k3s_prepare.go
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/nginx-dep.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/nginx_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/openmodelz.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/openmodelz_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/server/registries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/telemetry/telemetry.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/term/
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/term/interrupt.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4045 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/term/term.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/mdz/pkg/version/
+-rw-r--r--   0 runner    (1001) docker     (122)     3563 2023-08-03 03:50:36.000000 openmodelz-0.0.21/mdz/pkg/version/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 03:52:09.778273 openmodelz-0.0.21/openmodelz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-03 03:52:09.000000 openmodelz-0.0.21/openmodelz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-08-03 03:52:09.000000 openmodelz-0.0.21/openmodelz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 03:52:09.000000 openmodelz-0.0.21/openmodelz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 03:52:09.000000 openmodelz-0.0.21/openmodelz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-03 03:52:09.000000 openmodelz-0.0.21/openmodelz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-08-03 03:50:36.000000 openmodelz-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 03:52:09.782273 openmodelz-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-08-03 03:50:36.000000 openmodelz-0.0.21/setup.py
```

### Comparing `openmodelz-0.0.20/.all-contributorsrc` & `openmodelz-0.0.21/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/.gitignore` & `openmodelz-0.0.21/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/.goreleaser.yaml` & `openmodelz-0.0.21/.goreleaser.yaml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/LICENSE` & `openmodelz-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/PKG-INFO` & `openmodelz-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodelz
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simplify machine learning deployment for any environments.
 Home-page: https://github.com/tensorchord/openmodelz
 Author: TensorChord
 Author-email: modelz@tensorchord.ai
 License: Apache License 2.0
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openmodelz Version: 0.0.20 Summary: Simplify
+Metadata-Version: 2.1 Name: openmodelz Version: 0.0.21 Summary: Simplify
 machine learning deployment for any environments. Home-page: https://
 github.com/tensorchord/openmodelz Author: TensorChord Author-email:
 modelz@tensorchord.ai License: Apache License 2.0 Description:
     # OpenModelZ Simplify machine learning deployment for any environment.
      [discord_invitation_link] [trackgit-views] [docs] [all-contributors]
 OpenModelZ (MDZ) provides a simple CLI to deploy and manage your machine
 learning workloads on any cloud or home lab. ## Why use OpenModelZ ð
```

### Comparing `openmodelz-0.0.20/README.md` & `openmodelz-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/.gitignore` & `openmodelz-0.0.21/agent/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/Makefile` & `openmodelz-0.0.21/agent/Makefile`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/build.go` & `openmodelz-0.0.21/agent/api/types/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/inference_deployment.go` & `openmodelz-0.0.21/agent/api/types/inference_deployment.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/inference_deployment_instance.go` & `openmodelz-0.0.21/agent/api/types/inference_deployment_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/inference_status.go` & `openmodelz-0.0.21/agent/api/types/inference_status.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/info.go` & `openmodelz-0.0.21/agent/api/types/info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/log.go` & `openmodelz-0.0.21/agent/api/types/log.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/queue.go` & `openmodelz-0.0.21/agent/api/types/queue.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/requests.go` & `openmodelz-0.0.21/agent/api/types/requests.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/api/types/server.go` & `openmodelz-0.0.21/agent/api/types/server.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/build.go` & `openmodelz-0.0.21/agent/client/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/client.go` & `openmodelz-0.0.21/agent/client/client.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/const.go` & `openmodelz-0.0.21/agent/client/const.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/errors.go` & `openmodelz-0.0.21/agent/client/errors.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/hijack.go` & `openmodelz-0.0.21/agent/client/hijack.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_create.go` & `openmodelz-0.0.21/agent/client/inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_get.go` & `openmodelz-0.0.21/agent/client/inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_list.go` & `openmodelz-0.0.21/agent/client/inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_remove.go` & `openmodelz-0.0.21/agent/client/inference_remove.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_scale.go` & `openmodelz-0.0.21/agent/client/inference_scale.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/inference_update.go` & `openmodelz-0.0.21/agent/client/inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/info.go` & `openmodelz-0.0.21/agent/client/info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/instance_exec.go` & `openmodelz-0.0.21/agent/client/instance_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/instance_list.go` & `openmodelz-0.0.21/agent/client/instance_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/log.go` & `openmodelz-0.0.21/agent/client/log.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/namespace_create.go` & `openmodelz-0.0.21/agent/client/namespace_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/options.go` & `openmodelz-0.0.21/agent/client/options.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/request.go` & `openmodelz-0.0.21/agent/client/request.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/server_label_create.go` & `openmodelz-0.0.21/agent/client/server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/server_list.go` & `openmodelz-0.0.21/agent/client/server_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/client/transport.go` & `openmodelz-0.0.21/agent/client/transport.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/cmd/agent/main.go` & `openmodelz-0.0.21/agent/cmd/agent/main.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/errdefs/defs.go` & `openmodelz-0.0.21/agent/errdefs/defs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/errdefs/doc.go` & `openmodelz-0.0.21/agent/errdefs/doc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/errdefs/helpers.go` & `openmodelz-0.0.21/agent/errdefs/helpers.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/errdefs/http_helpers.go` & `openmodelz-0.0.21/agent/errdefs/http_helpers.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/errdefs/is.go` & `openmodelz-0.0.21/agent/errdefs/is.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/go.mod` & `openmodelz-0.0.21/agent/go.mod`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/go.sum` & `openmodelz-0.0.21/agent/go.sum`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/app/config.go` & `openmodelz-0.0.21/agent/pkg/app/config.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/app/root.go` & `openmodelz-0.0.21/agent/pkg/app/root.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/config/config.go` & `openmodelz-0.0.21/agent/pkg/config/config.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/docs/docs.go` & `openmodelz-0.0.21/agent/pkg/docs/docs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/event/event.go` & `openmodelz-0.0.21/agent/pkg/event/event.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/convert_deployment.go` & `openmodelz-0.0.21/agent/pkg/k8s/convert_deployment.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/convert_inference.go` & `openmodelz-0.0.21/agent/pkg/k8s/convert_inference.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/convert_job.go` & `openmodelz-0.0.21/agent/pkg/k8s/convert_job.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/convert_pod.go` & `openmodelz-0.0.21/agent/pkg/k8s/convert_pod.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/generate_job.go` & `openmodelz-0.0.21/agent/pkg/k8s/generate_job.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/k8s/resolver.go` & `openmodelz-0.0.21/agent/pkg/k8s/resolver.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/log/k8s.go` & `openmodelz-0.0.21/agent/pkg/log/k8s.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/log/loki.go` & `openmodelz-0.0.21/agent/pkg/log/loki.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/metrics/exporter.go` & `openmodelz-0.0.21/agent/pkg/metrics/exporter.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/metrics/metrics.go` & `openmodelz-0.0.21/agent/pkg/metrics/metrics.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/prom/prometheus_query.go` & `openmodelz-0.0.21/agent/pkg/prom/prometheus_query.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/query/db.go` & `openmodelz-0.0.21/agent/pkg/query/db.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/query/deployment_events.sql.go` & `openmodelz-0.0.21/agent/pkg/query/deployment_events.sql.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/build.go` & `openmodelz-0.0.21/agent/pkg/runtime/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_create.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_delete.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_exec.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_get.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_instance.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_list.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_replicas.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_replicas.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/inference_update.go` & `openmodelz-0.0.21/agent/pkg/runtime/inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/namespace.go` & `openmodelz-0.0.21/agent/pkg/runtime/namespace.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/runtime.go` & `openmodelz-0.0.21/agent/pkg/runtime/runtime.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/server_label_create.go` & `openmodelz-0.0.21/agent/pkg/runtime/server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/server_list.go` & `openmodelz-0.0.21/agent/pkg/runtime/server_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/util_domain.go` & `openmodelz-0.0.21/agent/pkg/runtime/util_domain.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/runtime/util_resource.go` & `openmodelz-0.0.21/agent/pkg/runtime/util_resource.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/scaling/function_scaler.go` & `openmodelz-0.0.21/agent/pkg/scaling/function_scaler.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/scaling/ranges.go` & `openmodelz-0.0.21/agent/pkg/scaling/ranges.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/scaling/service_query.go` & `openmodelz-0.0.21/agent/pkg/scaling/service_query.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/scaling/util.go` & `openmodelz-0.0.21/agent/pkg/scaling/util.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/error.go` & `openmodelz-0.0.21/agent/pkg/server/error.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_build_create.go` & `openmodelz-0.0.21/agent/pkg/server/handler_build_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_build_get.go` & `openmodelz-0.0.21/agent/pkg/server/handler_build_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_build_list.go` & `openmodelz-0.0.21/agent/pkg/server/handler_build_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_build_logs.go` & `openmodelz-0.0.21/agent/pkg/server/handler_build_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_create.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_delete.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_get.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_instance.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_instance_exec.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_instance_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_list.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_logs.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_proxy.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_scale.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_scale.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_inference_update.go` & `openmodelz-0.0.21/agent/pkg/server/handler_inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_info.go` & `openmodelz-0.0.21/agent/pkg/server/handler_info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_namespace_create.go` & `openmodelz-0.0.21/agent/pkg/server/handler_namespace_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_namespace_list.go` & `openmodelz-0.0.21/agent/pkg/server/handler_namespace_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/handler_server_label_create.go` & `openmodelz-0.0.21/agent/pkg/server/handler_server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/middleware_callid.go` & `openmodelz-0.0.21/agent/pkg/server/middleware_callid.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/server_factory.go` & `openmodelz-0.0.21/agent/pkg/server/server_factory.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/server_handlerfunc.go` & `openmodelz-0.0.21/agent/pkg/server/server_handlerfunc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/server_init_kubernetes.go` & `openmodelz-0.0.21/agent/pkg/server/server_init_kubernetes.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/server_init_route.go` & `openmodelz-0.0.21/agent/pkg/server/server_init_route.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/server_run.go` & `openmodelz-0.0.21/agent/pkg/server/server_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/server/validator/validator.go` & `openmodelz-0.0.21/agent/pkg/server/validator/validator.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/agent/pkg/version/version.go` & `openmodelz-0.0.21/agent/pkg/version/version.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/.gitignore` & `openmodelz-0.0.21/mdz/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/Makefile` & `openmodelz-0.0.21/mdz/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,20 @@
 #
 
 # All targets.
 .PHONY: help lint test build container push addlicense debug debug-local build-local generate clean test-local addlicense-install release build-image
 
 .DEFAULT_GOAL:=build
 
-build: build-local  ## Build the release version of envd
+build: build-release  ## Build the release version
 
 help:  ## Display this help
 	@awk 'BEGIN {FS = ":.*##"; printf "\nUsage:\n  make \033[36m<target>\033[0m\n"} /^[a-zA-Z0-9_-]+:.*?##/ { printf "  \033[36m%-15s\033[0m %s\n", $$1, $$2 } /^##@/ { printf "\n\033[1m%s\033[0m\n", substr($$0, 5) } ' $(MAKEFILE_LIST)
 
-debug: debug-local  ## Build the debug version of envd
+debug: debug-local  ## Build the debug version
 
 # more info about `GOGC` env: https://github.com/golangci/golangci-lint#memory-usage-of-golangci-lint
 lint: $(GOLANGCI_LINT)  ## Lint GO code
 	@$(GOLANGCI_LINT) run
 
 $(GOLANGCI_LINT):
 	curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $$(go env GOPATH)/bin
```

### Comparing `openmodelz-0.0.20/mdz/go.mod` & `openmodelz-0.0.21/mdz/go.mod`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 	github.com/opencontainers/go-digest v1.0.0 // indirect
 	github.com/opencontainers/image-spec v1.1.0-rc2 // indirect
 	github.com/pelletier/go-toml/v2 v2.0.8 // indirect
 	github.com/pkg/errors v0.9.1 // indirect
 	github.com/rivo/uniseg v0.2.0 // indirect
 	github.com/rogpeppe/go-internal v1.10.0 // indirect
 	github.com/russross/blackfriday/v2 v2.1.0 // indirect
+	github.com/segmentio/analytics-go/v3 v3.2.1 // indirect
+	github.com/segmentio/backo-go v1.0.0 // indirect
 	github.com/spf13/pflag v1.0.5 // indirect
 	github.com/swaggo/swag v1.8.12 // indirect
 	github.com/twitchyliquid64/golang-asm v0.15.1 // indirect
 	github.com/ugorji/go/codec v1.2.11 // indirect
 	golang.org/x/arch v0.3.0 // indirect
 	golang.org/x/crypto v0.9.0 // indirect
 	golang.org/x/mod v0.9.0 // indirect
```

### Comparing `openmodelz-0.0.20/mdz/go.sum` & `openmodelz-0.0.21/mdz/go.sum`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,18 @@
 github.com/rogpeppe/go-internal v1.6.1/go.mod h1:xXDCJY+GAPziupqXw64V24skbSoqbTEfhy4qGm1nDQc=
 github.com/rogpeppe/go-internal v1.8.0/go.mod h1:WmiCO8CzOY8rg0OYDC4/i/2WRWAB6poM+XZ2dLUbcbE=
 github.com/rogpeppe/go-internal v1.9.0/go.mod h1:WtVeX8xhTBvf0smdhujwtBcq4Qrzq/fJaraNFVN+nFs=
 github.com/rogpeppe/go-internal v1.10.0 h1:TMyTOH3F/DB16zRVcYyreMH6GnZZrwQVAoYjRBZyWFQ=
 github.com/rogpeppe/go-internal v1.10.0/go.mod h1:UQnix2H7Ngw/k4C5ijL5+65zddjncjaFoBhdsK/akog=
 github.com/russross/blackfriday/v2 v2.1.0 h1:JIOH55/0cWyOuilr9/qlrm0BSXldqnqwMsf35Ld67mk=
 github.com/russross/blackfriday/v2 v2.1.0/go.mod h1:+Rmxgy9KzJVeS9/2gXHxylqXiyQDYRxCVz55jmeOWTM=
+github.com/segmentio/analytics-go/v3 v3.2.1 h1:G+f90zxtc1p9G+WigVyTR0xNfOghOGs/PYAlljLOyeg=
+github.com/segmentio/analytics-go/v3 v3.2.1/go.mod h1:p8owAF8X+5o27jmvUognuXxdtqvSGtD0ZrfY2kcS9bE=
+github.com/segmentio/backo-go v1.0.0 h1:kbOAtGJY2DqOR0jfRkYEorx/b18RgtepGtY3+Cpe6qA=
+github.com/segmentio/backo-go v1.0.0/go.mod h1:kJ9mm9YmoWSkk+oQ+5Cj8DEoRCX2JT6As4kEtIIOp1M=
 github.com/sirupsen/logrus v1.9.3 h1:dueUQJ1C2q9oE3F7wvmSGAaVtTmUizReu6fjN8uqzbQ=
 github.com/sirupsen/logrus v1.9.3/go.mod h1:naHLuLoDiP4jHNo9R0sCBMtWGeIprob74mVsIT4qYEQ=
 github.com/spf13/cobra v1.7.0 h1:hyqWnYt1ZQShIddO5kBpj3vu05/++x6tJ6dg8EC572I=
 github.com/spf13/cobra v1.7.0/go.mod h1:uLxZILRyS/50WlhOIKD7W6V5bgeIt+4sICxh6uRMrb0=
 github.com/spf13/pflag v1.0.5 h1:iy+VFUOCP1a+8yFto/drg2CJ5u0yRoB7fZw3DKv/JXA=
 github.com/spf13/pflag v1.0.5/go.mod h1:McXfInJRrz4CZXVZOBLb0bTZqETkiAhM9Iw0y3An2Bg=
 github.com/stretchr/objx v0.1.0/go.mod h1:HFkY916IF+rwdDfMAkV7OtwuqBVzrE8GR6GFx+wExME=
```

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/runtime/create.go` & `openmodelz-0.0.21/mdz/pkg/agentd/runtime/create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/runtime/delete.go` & `openmodelz-0.0.21/mdz/pkg/agentd/runtime/delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/runtime/list.go` & `openmodelz-0.0.21/mdz/pkg/agentd/runtime/list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/runtime/proxy.go` & `openmodelz-0.0.21/mdz/pkg/agentd/runtime/proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/runtime/runtime.go` & `openmodelz-0.0.21/mdz/pkg/agentd/runtime/runtime.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/error.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/error.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_create.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_delete.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_get.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_list.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_logs.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_proxy.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_inference_proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_info.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/handler_info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/middleware_callid.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/middleware_callid.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/server_factory.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/server_factory.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/server_handlerfunc.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/server_handlerfunc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/server_init_route.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/server_init_route.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/agentd/server/server_run.go` & `openmodelz-0.0.21/mdz/pkg/agentd/server/server_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/delete.go` & `openmodelz-0.0.21/mdz/pkg/cmd/delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/deploy.go` & `openmodelz-0.0.21/mdz/pkg/cmd/deploy.go`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 	"strconv"
 	"time"
 
 	"github.com/cockroachdb/errors"
 	petname "github.com/dustinkirkland/golang-petname"
 	"github.com/spf13/cobra"
 	"github.com/tensorchord/openmodelz/agent/api/types"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 var (
 	// Used for flags.
 	deployImage       string
 	deployPort        int32
 	deployMinReplicas int32
@@ -106,14 +107,20 @@
 			// no need to set Requests for GPU
 			Limits: types.ResourceList{
 				types.ResourceGPU: GPUNum,
 			},
 		}
 	}
 
+	telemetry.GetTelemetry().Record(
+		"deploy",
+		telemetry.AddField("GPU", deployGPU),
+		telemetry.AddField("FromZero", deployMinReplicas == 0),
+	)
+
 	if _, err := agentClient.InferenceCreate(
 		cmd.Context(), namespace, inf); err != nil {
 		cmd.PrintErrf("Failed to create the inference: %s\n", errors.Cause(err))
 		return err
 	}
 
 	cmd.Printf("Inference %s is created\n", inf.Spec.Name)
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/exec.go` & `openmodelz-0.0.21/mdz/pkg/cmd/exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/exec_stream.go` & `openmodelz-0.0.21/mdz/pkg/cmd/exec_stream.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/ioutils/reader.go` & `openmodelz-0.0.21/mdz/pkg/cmd/ioutils/reader.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/list.go` & `openmodelz-0.0.21/mdz/pkg/cmd/list.go`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 	"fmt"
 	"sort"
 	"strings"
 
 	"github.com/jedib0t/go-pretty/v6/table"
 	"github.com/spf13/cobra"
 	"github.com/tensorchord/openmodelz/agent/api/types"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 const (
 	annotationDomain = "ai.tensorchord.domain"
 )
 
 var (
@@ -44,14 +45,15 @@
 	// Cobra supports local flags which will only run when this command
 	// is called directly, e.g.:
 	listCommand.Flags().BoolVarP(&listQuiet, "quiet", "q", false, "Quiet mode - print out only the inference names")
 	listCommand.Flags().BoolVarP(&listVerbose, "verbose", "v", false, "Verbose mode - print out all inference details")
 }
 
 func commandList(cmd *cobra.Command, args []string) error {
+	telemetry.GetTelemetry().Record("list")
 	infs, err := agentClient.InferenceList(cmd.Context(), namespace)
 	if err != nil {
 		cmd.PrintErrf("Failed to list inferences: %v\n", err)
 		return err
 	}
 
 	sort.Sort(byName(infs))
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/list_instance.go` & `openmodelz-0.0.21/mdz/pkg/cmd/list_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/localagent.go` & `openmodelz-0.0.21/mdz/pkg/cmd/localagent.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/logs.go` & `openmodelz-0.0.21/mdz/pkg/cmd/logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/portforward.go` & `openmodelz-0.0.21/mdz/pkg/cmd/portforward.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/root.go` & `openmodelz-0.0.21/mdz/pkg/cmd/root.go`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 	"github.com/cockroachdb/errors"
 	"github.com/sirupsen/logrus"
 	"github.com/spf13/cobra"
 	"github.com/spf13/cobra/doc"
 
 	"github.com/tensorchord/openmodelz/agent/client"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 var (
 	// Used for flags.
-	mdzURL    string
-	namespace string
-	debug     bool
+	mdzURL           string
+	namespace        string
+	debug            bool
+	disableTelemetry bool
 
 	agentClient *client.Client
 )
 
 // rootCmd represents the base command when called without any subcommands
 var rootCmd = &cobra.Command{
 	Use:   "mdz",
@@ -58,14 +60,16 @@
 	rootCmd.PersistentFlags().StringVarP(&mdzURL, "url", "u", "", "URL to use for the server (MDZ_URL) (default http://localhost:80)")
 
 	rootCmd.PersistentFlags().StringVarP(&namespace, "namespace", "n", "default", "Namespace to use for OpenModelZ inferences")
 	rootCmd.PersistentFlags().MarkHidden("namespace")
 
 	rootCmd.PersistentFlags().BoolVarP(&debug, "debug", "", false, "Enable debug logging")
 
+	rootCmd.PersistentFlags().BoolVarP(&disableTelemetry, "disable-telemetry", "", false, "Disable anonymous telemetry")
+
 	// Cobra also supports local flags, which will only run
 	// when this action is called directly.
 	rootCmd.AddGroup(&cobra.Group{ID: "basic", Title: "Basic Commands:"})
 	rootCmd.AddGroup(&cobra.Group{ID: "debug", Title: "Troubleshooting and Debugging Commands:"})
 	rootCmd.AddGroup(&cobra.Group{ID: "management", Title: "Management Commands:"})
 }
 
@@ -85,14 +89,18 @@
 		var err error
 		agentClient, err = client.NewClientWithOpts(client.WithHost(mdzURL))
 		if err != nil {
 			cmd.PrintErrf("Failed to connect to agent: %s\n", errors.Cause(err))
 			return err
 		}
 	}
+
+	if err := telemetry.Initialize(!disableTelemetry); err != nil {
+		logrus.WithError(err).Debug("Failed to initialize telemetry")
+	}
 	return nil
 }
 
 func commandInitLog(cmd *cobra.Command, args []string) error {
 	if debug {
 		logrus.SetLevel(logrus.DebugLevel)
 		logrus.Debug("Debug logging enabled")
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/scale.go` & `openmodelz-0.0.21/mdz/pkg/cmd/scale.go`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 package cmd
 
 import (
 	"github.com/spf13/cobra"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 var (
 	// Used for flags.
 	replicas               int32
 	min                    int32
 	max                    int32
@@ -69,14 +70,16 @@
 	if max != 0 {
 		deployment.Spec.Scaling.MaxReplicas = int32Ptr(max)
 	}
 	if targetInflightRequests != 0 {
 		deployment.Spec.Scaling.TargetLoad = int32Ptr(targetInflightRequests)
 	}
 
+	telemetry.GetTelemetry().Record("scale")
+
 	if _, err := agentClient.DeploymentUpdate(cmd.Context(), namespace, deployment); err != nil {
 		cmd.PrintErrf("Failed to update deployment: %s\n", err)
 		return err
 	}
 
 	return nil
 }
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server_join.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server_join.go`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 package cmd
 
 import (
 	"github.com/cockroachdb/errors"
 	"github.com/spf13/cobra"
 
 	"github.com/tensorchord/openmodelz/mdz/pkg/server"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 // serverJoinCmd represents the server join command
 var serverJoinCmd = &cobra.Command{
 	Use:     "join",
 	Short:   "Join to the cluster",
 	Long:    `Join to the cluster`,
@@ -42,18 +43,20 @@
 		ServerIP:      args[0],
 		Mirror: server.Mirror{
 			Name:      serverRegistryMirrorName,
 			Endpoints: serverRegistryMirrorEndpoints,
 		},
 	})
 	if err != nil {
-		cmd.PrintErrf("Failed to join the cluster: %s\n", errors.Cause(err))
+		cmd.PrintErrf("Failed to configure before join: %s\n", errors.Cause(err))
 		return err
 	}
 
+	telemetry.GetTelemetry().Record("server join")
+
 	_, err = engine.Run()
 	if err != nil {
 		cmd.PrintErrf("Failed to join the cluster: %s\n", errors.Cause(err))
 		return err
 	}
 	cmd.Printf("✅ Server joined\n")
 	return nil
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server_label.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server_label.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server_list.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server_list.go`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import (
 	"fmt"
 
 	"github.com/cockroachdb/errors"
 	"github.com/jedib0t/go-pretty/v6/table"
 	"github.com/spf13/cobra"
 	"github.com/tensorchord/openmodelz/agent/api/types"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 )
 
 var (
 	// Used for flags.
 	serverListQuiet   bool
 	serverListVerbose bool
 )
@@ -36,14 +37,15 @@
 	// Cobra supports local flags which will only run when this command
 	// is called directly, e.g.:
 	serverListCmd.Flags().BoolVarP(&serverListQuiet, "quiet", "q", false, "Quiet mode - print out only the server names")
 	serverListCmd.Flags().BoolVarP(&serverListVerbose, "verbose", "v", false, "Verbose mode - print out all server details")
 }
 
 func commandServerList(cmd *cobra.Command, args []string) error {
+	telemetry.GetTelemetry().Record("server list")
 	servers, err := agentClient.ServerList(cmd.Context())
 	if err != nil {
 		cmd.PrintErrf("Failed to list servers: %s\n", errors.Cause(err))
 		return err
 	}
 
 	if serverListQuiet {
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server_start.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server_start.go`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 	"time"
 
 	"github.com/cockroachdb/errors"
 	"github.com/spf13/cobra"
 
 	"github.com/tensorchord/openmodelz/agent/pkg/consts"
 	"github.com/tensorchord/openmodelz/mdz/pkg/server"
+	"github.com/tensorchord/openmodelz/mdz/pkg/telemetry"
 	"github.com/tensorchord/openmodelz/mdz/pkg/version"
 )
 
 var (
 	serverStartRuntime string
 	serverStartDomain  string = consts.Domain
 	serverStartVersion string
@@ -56,14 +57,20 @@
 
 func commandServerStart(cmd *cobra.Command, args []string) error {
 	var domain *string
 	if len(args) > 0 {
 		domainWithSuffix := fmt.Sprintf("%s.%s", args[0], serverStartDomain)
 		domain = &domainWithSuffix
 	}
+	defer func(start time.Time) {
+		telemetry.GetTelemetry().Record(
+			"server start",
+			telemetry.AddField("duration", time.Since(start).Seconds()),
+		)
+	}(time.Now())
 	engine, err := server.NewStart(server.Options{
 		Verbose:       serverVerbose,
 		Runtime:       server.Runtime(serverStartRuntime),
 		OutputStream:  cmd.ErrOrStderr(),
 		RetryInternal: serverPollingInterval,
 		Domain:        domain,
 		Version:       serverStartVersion,
```

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/server_stop.go` & `openmodelz-0.0.21/mdz/pkg/cmd/server_stop.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/streams/in.go` & `openmodelz-0.0.21/mdz/pkg/cmd/streams/in.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/streams/out.go` & `openmodelz-0.0.21/mdz/pkg/cmd/streams/out.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/streams/stream.go` & `openmodelz-0.0.21/mdz/pkg/cmd/streams/stream.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/cmd/version.go` & `openmodelz-0.0.21/mdz/pkg/cmd/version.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/agentd_run.go` & `openmodelz-0.0.21/mdz/pkg/server/agentd_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/engine.go` & `openmodelz-0.0.21/mdz/pkg/server/engine.go`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,26 @@
 			&k3sKillAllStep{
 				options: o,
 			},
 		},
 	}, nil
 }
 
+func NewDestroy(o Options) (*Engine, error) {
+	return &Engine{
+		options: o,
+		Steps: []Step{
+			// Destroy all k3s and related tools.
+			&k3sDestroyAllStep{
+				options: o,
+			},
+		},
+	}, nil
+}
+
 func NewJoin(o Options) (*Engine, error) {
 	return &Engine{
 		options: o,
 		Steps: []Step{
 			// Kill all k3s and related tools.
 			&k3sJoinStep{
 				options: o,
```

### Comparing `openmodelz-0.0.20/mdz/pkg/server/gpu_install.go` & `openmodelz-0.0.21/mdz/pkg/server/gpu_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/k3s-install.sh` & `openmodelz-0.0.21/mdz/pkg/server/k3s-install.sh`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/k3s_install.go` & `openmodelz-0.0.21/mdz/pkg/server/k3s_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/k3s_join.go` & `openmodelz-0.0.21/mdz/pkg/server/k3s_join.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/k3s_killall.go` & `openmodelz-0.0.21/mdz/pkg/server/k3s_killall.go`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 // k3sKillAllStep installs k3s and related tools.
 type k3sKillAllStep struct {
 	options Options
 }
 
 func (s *k3sKillAllStep) Run() error {
-	fmt.Fprintf(s.options.OutputStream, "🚧 Stopping all the processes...\n")
+	fmt.Fprintf(s.options.OutputStream, "🚧 Stopping the OpenModelz Cluster...\n")
 	// TODO(gaocegege): Embed the script into the binary.
 	cmd := exec.Command("/bin/sh", "-c", "/usr/local/bin/k3s-killall.sh")
 	cmd.SysProcAttr = &syscall.SysProcAttr{
 		Pdeathsig: syscall.SIGKILL,
 	}
 	if s.options.Verbose {
 		cmd.Stderr = s.options.OutputStream
```

### Comparing `openmodelz-0.0.20/mdz/pkg/server/k3s_prepare.go` & `openmodelz-0.0.21/mdz/pkg/server/k3s_prepare.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/nginx-dep.yaml` & `openmodelz-0.0.21/mdz/pkg/server/nginx-dep.yaml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/nginx_install.go` & `openmodelz-0.0.21/mdz/pkg/server/nginx_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/server/openmodelz_install.go` & `openmodelz-0.0.21/mdz/pkg/server/openmodelz_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/term/interrupt.go` & `openmodelz-0.0.21/mdz/pkg/term/interrupt.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/term/term.go` & `openmodelz-0.0.21/mdz/pkg/term/term.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/mdz/pkg/version/version.go` & `openmodelz-0.0.21/mdz/pkg/version/version.go`

 * *Files 13% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 	buildDate       = "1970-01-01T00:00:00Z" // output from `date -u +'%Y-%m-%dT%H:%M:%SZ'`
 	gitCommit       = ""                     // output from `git rev-parse HEAD`
 	gitTag          = ""                     // output from `git describe --exact-match --tags HEAD` (if clean tree state)
 	gitTreeState    = ""                     // determined from `git status --porcelain`. either 'clean' or 'dirty'
 	developmentFlag = "false"
 )
 
-// Version contains envd version information
+// Version contains OpenModelz version information
 type Version struct {
 	Version      string
 	BuildDate    string
 	GitCommit    string
 	GitTag       string
 	GitTreeState string
 	GoVersion    string
@@ -61,16 +61,16 @@
 }
 
 // SetGitTagForE2ETest sets the gitTag for test purpose.
 func SetGitTagForE2ETest(tag string) {
 	gitTag = tag
 }
 
-// GetEnvdVersion gets Envd version information
-func GetEnvdVersion() string {
+// GetOpenModelzVersion gets OpenModelz version information
+func GetOpenModelzVersion() string {
 	var versionStr string
 
 	if gitCommit != "" && gitTag != "" &&
 		gitTreeState == "clean" && developmentFlag == "false" {
 		// if we have a clean tree state and the current commit is tagged,
 		// this is an official release.
 		versionStr = gitTag
@@ -93,15 +93,15 @@
 	}
 	return versionStr
 }
 
 // GetVersion returns the version information
 func GetVersion() Version {
 	return Version{
-		Version:      GetEnvdVersion(),
+		Version:      GetOpenModelzVersion(),
 		BuildDate:    buildDate,
 		GitCommit:    gitCommit,
 		GitTag:       gitTag,
 		GitTreeState: gitTreeState,
 		GoVersion:    runtime.Version(),
 		Compiler:     runtime.Compiler,
 		Platform:     fmt.Sprintf("%s/%s", runtime.GOOS, runtime.GOARCH),
@@ -124,9 +124,9 @@
 
 	if matches := reRelease.FindAllStringSubmatch(version, 1); len(matches) > 0 {
 		version = matches[0][1]
 	} else if matches := reDev.FindAllStringSubmatch(version, 1); len(matches) > 0 {
 		version = matches[0][1] + "-dev"
 	}
 
-	return "envd/" + version
+	return "modelz/" + version
 }
```

### Comparing `openmodelz-0.0.20/openmodelz.egg-info/PKG-INFO` & `openmodelz-0.0.21/openmodelz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodelz
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simplify machine learning deployment for any environments.
 Home-page: https://github.com/tensorchord/openmodelz
 Author: TensorChord
 Author-email: modelz@tensorchord.ai
 License: Apache License 2.0
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openmodelz Version: 0.0.20 Summary: Simplify
+Metadata-Version: 2.1 Name: openmodelz Version: 0.0.21 Summary: Simplify
 machine learning deployment for any environments. Home-page: https://
 github.com/tensorchord/openmodelz Author: TensorChord Author-email:
 modelz@tensorchord.ai License: Apache License 2.0 Description:
     # OpenModelZ Simplify machine learning deployment for any environment.
      [discord_invitation_link] [trackgit-views] [docs] [all-contributors]
 OpenModelZ (MDZ) provides a simple CLI to deploy and manage your machine
 learning workloads on any cloud or home lab. ## Why use OpenModelZ ð
```

### Comparing `openmodelz-0.0.20/openmodelz.egg-info/SOURCES.txt` & `openmodelz-0.0.21/openmodelz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 mdz/pkg/cmd/list_instance.go
 mdz/pkg/cmd/localagent.go
 mdz/pkg/cmd/logs.go
 mdz/pkg/cmd/portforward.go
 mdz/pkg/cmd/root.go
 mdz/pkg/cmd/scale.go
 mdz/pkg/cmd/server.go
+mdz/pkg/cmd/server_destroy.go
 mdz/pkg/cmd/server_join.go
 mdz/pkg/cmd/server_label.go
 mdz/pkg/cmd/server_list.go
 mdz/pkg/cmd/server_start.go
 mdz/pkg/cmd/server_stop.go
 mdz/pkg/cmd/version.go
 mdz/pkg/cmd/ioutils/reader.go
@@ -182,23 +183,25 @@
 mdz/pkg/cmd/streams/out.go
 mdz/pkg/cmd/streams/stream.go
 mdz/pkg/server/agentd_run.go
 mdz/pkg/server/engine.go
 mdz/pkg/server/gpu-resource.yaml
 mdz/pkg/server/gpu_install.go
 mdz/pkg/server/k3s-install.sh
+mdz/pkg/server/k3s_destroy.go
 mdz/pkg/server/k3s_install.go
 mdz/pkg/server/k3s_join.go
 mdz/pkg/server/k3s_killall.go
 mdz/pkg/server/k3s_prepare.go
 mdz/pkg/server/nginx-dep.yaml
 mdz/pkg/server/nginx_install.go
 mdz/pkg/server/openmodelz.yaml
 mdz/pkg/server/openmodelz_install.go
 mdz/pkg/server/registries.yaml
+mdz/pkg/telemetry/telemetry.go
 mdz/pkg/term/interrupt.go
 mdz/pkg/term/term.go
 mdz/pkg/version/version.go
 openmodelz.egg-info/PKG-INFO
 openmodelz.egg-info/SOURCES.txt
 openmodelz.egg-info/dependency_links.txt
 openmodelz.egg-info/not-zip-safe
```

### Comparing `openmodelz-0.0.20/pyproject.toml` & `openmodelz-0.0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.20/setup.py` & `openmodelz-0.0.21/setup.py`

 * *Files identical despite different names*

