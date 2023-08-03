# Comparing `tmp/pulumi_volcengine-0.0.6.tar.gz` & `tmp/pulumi_volcengine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_volcengine-0.0.6.tar", last modified: Mon Jul 31 08:04:20 2023, max compression
+gzip compressed data, was "pulumi_volcengine-0.0.9.tar", last modified: Tue Aug  1 03:59:07 2023, max compression
```

## Comparing `pulumi_volcengine-0.0.6.tar` & `pulumi_volcengine-0.0.9.tar`

### file list

```diff
@@ -1,358 +1,358 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.926908 pulumi_volcengine-0.0.6/
--rw-r--r--   0 bytedance   (502) staff       (20)     1542 2023-07-31 08:04:20.926621 pulumi_volcengine-0.0.6/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)     1190 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/README.md
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.792469 pulumi_volcengine-0.0.6/pulumi_volcengine/
--rw-r--r--   0 bytedance   (502) staff       (20)    26633 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7667 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/_utilities.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.800215 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/
--rw-r--r--   0 bytedance   (502) staff       (20)      782 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6539 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    55363 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8232 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_activities.py
--rw-r--r--   0 bytedance   (502) staff       (20)    62851 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configuration.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7857 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configuration_attachment.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8036 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configurations.py
--rw-r--r--   0 bytedance   (502) staff       (20)    49221 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11113 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_group_enabler.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6525 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_groups.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16664 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_instance_attachment.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9268 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18099 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_lifecycle_hook.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7733 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_lifecycle_hooks.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8769 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_policies.py
--rw-r--r--   0 bytedance   (502) staff       (20)    72672 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_policy.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.803503 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/
--rw-r--r--   0 bytedance   (502) staff       (20)      440 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2195 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14518 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/cluster.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10223 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/cluster_bind.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6506 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/clusters.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8631 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12008 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/workspace.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6548 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/workspaces.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.809293 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/
--rw-r--r--   0 bytedance   (502) staff       (20)      761 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6320 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17651 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/attach_instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7478 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/attach_instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    40630 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_package.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9341 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_package_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10850 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_packages.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18409 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/cen.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6555 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/cens.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14782 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/grant_instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17949 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/inter_region_bandwidth.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5263 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/inter_region_bandwidths.py
--rw-r--r--   0 bytedance   (502) staff       (20)    33417 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8478 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/route_entries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19897 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/route_entry.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8030 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/service_route_entries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    29244 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cen/service_route_entry.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.818129 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/
--rw-r--r--   0 bytedance   (502) staff       (20)      711 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15093 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13978 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acl.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10081 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acl_entry.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6533 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acls.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19104 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/certificate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8008 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/certificates.py
--rw-r--r--   0 bytedance   (502) staff       (20)    49744 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/clb.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8950 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/clbs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    37938 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/listener.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7045 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/listeners.py
--rw-r--r--   0 bytedance   (502) staff       (20)    52849 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13739 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/rule.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4824 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/rules.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12650 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19029 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group_server.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6544 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group_servers.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7307 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_groups.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3904 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/clb/zones.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.819291 pulumi_volcengine-0.0.6/pulumi_volcengine/config/
--rw-r--r--   0 bytedance   (502) staff       (20)      285 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/config/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2197 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/config/vars.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.828081 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/
--rw-r--r--   0 bytedance   (502) staff       (20)      671 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11344 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4857 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/authorization_tokens.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8908 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/endpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4646 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/endpoints.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8913 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/namespace.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5356 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/namespaces.py
--rw-r--r--   0 bytedance   (502) staff       (20)    27397 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6427 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/registries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17666 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/registry.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6997 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/repositories.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15782 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/repository.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8867 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/state.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18511 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/tag.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7103 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/tags.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10656 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/vpc_endpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5971 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/cr/vpc_endpoints.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.829798 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/
--rw-r--r--   0 bytedance   (502) staff       (20)      365 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5254 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    30232 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volume.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13452 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volume_attach.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9490 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volumes.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.836361 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/
--rw-r--r--   0 bytedance   (502) staff       (20)      674 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13407 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14442 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_set.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12441 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_set_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7358 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_sets.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9382 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/images.py
--rw-r--r--   0 bytedance   (502) staff       (20)   101122 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16783 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15623 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pair.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11977 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pair_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8195 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pairs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    54236 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/launch_template.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7791 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/launch_templates.py
--rw-r--r--   0 bytedance   (502) staff       (20)    54843 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14041 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/state.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4419 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/zones.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.838398 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/
--rw-r--r--   0 bytedance   (502) staff       (20)      387 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2124 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    27480 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/address.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11473 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/addresses.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16348 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9583 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/eip/outputs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.840770 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/
--rw-r--r--   0 bytedance   (502) staff       (20)      407 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15571 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10301 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8251 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    59452 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3901 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/regions.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4485 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/zones.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.845101 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/
--rw-r--r--   0 bytedance   (502) staff       (20)      550 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17585 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/access_key.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12553 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/login_profile.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8680 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8035 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/policies.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14748 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/policy.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15917 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/role.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11908 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/role_policy_attachment.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5812 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/roles.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17415 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/user.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11462 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/user_policy_attachment.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5207 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/iam/users.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.851951 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/
--rw-r--r--   0 bytedance   (502) staff       (20)      767 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2126 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5545 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/accounts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16686 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/endpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4764 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/endpoints.py
--rw-r--r--   0 bytedance   (502) staff       (20)    45208 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15361 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameter.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6826 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameter_logs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7142 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameters.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15361 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15215 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_list.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9142 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_list_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6631 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_lists.py
--rw-r--r--   0 bytedance   (502) staff       (20)    59114 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3901 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/regions.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4516 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/specs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12478 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/ssl_state.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4883 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/ssl_states.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4485 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/zones.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.855155 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/
--rw-r--r--   0 bytedance   (502) staff       (20)      469 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2122 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11066 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/dnat_entries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    21460 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/dnat_entry.py
--rw-r--r--   0 bytedance   (502) staff       (20)    24484 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/gateway.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9981 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/gateways.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17244 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8943 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/snat_entries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16541 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/nat/snat_entry.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.860593 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/
--rw-r--r--   0 bytedance   (502) staff       (20)      760 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5912 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    27088 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8974 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/security_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)    25136 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16125 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_connection.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7260 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_connections.py
--rw-r--r--   0 bytedance   (502) staff       (20)    21794 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9551 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_permission.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6285 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_permissions.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9759 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_resource.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6670 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_services.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15528 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_zone.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5155 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_zones.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8721 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoints.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14207 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/provider.py
--rw-r--r--   0 bytedance   (502) staff       (20)       47 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/pulumi-plugin.json
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/py.typed
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.867152 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/
--rw-r--r--   0 bytedance   (502) staff       (20)      608 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7644 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19733 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/account.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16310 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/account_privilege.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6424 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/accounts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13339 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/database.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6394 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/databases.py
--rw-r--r--   0 bytedance   (502) staff       (20)    62931 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10434 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10681 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/ip_list.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5577 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/ip_lists.py
--rw-r--r--   0 bytedance   (502) staff       (20)    32042 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18883 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/parameter_template.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9486 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds/parameter_templates.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.874491 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/
--rw-r--r--   0 bytedance   (502) staff       (20)      583 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    36294 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    22727 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/account.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6377 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/accounts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14773 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlist.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8978 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlist_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5778 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlists.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13233 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/database.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6225 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/databases.py
--rw-r--r--   0 bytedance   (502) staff       (20)    59348 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11868 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instance_readonly_node.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11579 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    75179 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/outputs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.877305 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/
--rw-r--r--   0 bytedance   (502) staff       (20)      377 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19189 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    48086 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    46611 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/rds_instance_v2.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15151 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/rds_instances_v2.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.884431 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/
--rw-r--r--   0 bytedance   (502) staff       (20)      729 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17747 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15632 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/account.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5587 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/accounts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17564 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_list.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9284 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_list_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6205 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_lists.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15012 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backup.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11039 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backup_restore.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7233 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backups.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6694 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/continuous_backup.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8139 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/endpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)    74853 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)    13219 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    57049 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3996 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/pitr_time_windows.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4651 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/regions.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8183 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/state.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4489 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/redis/zones.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.893619 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/
--rw-r--r--   0 bytedance   (502) staff       (20)      835 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    60513 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    34653 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16054 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm_notify_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7837 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm_notify_groups.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8119 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarms.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7913 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host.py
--rw-r--r--   0 bytedance   (502) staff       (20)    31603 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9125 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host_groups.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6164 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/hosts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15625 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/index.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4644 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/indexes.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8573 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/kafka_consumer.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4945 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/kafka_consumers.py
--rw-r--r--   0 bytedance   (502) staff       (20)   174790 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16188 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/project.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9320 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/projects.py
--rw-r--r--   0 bytedance   (502) staff       (20)    35847 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8466 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule_applier.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4798 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule_appliers.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7265 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rules.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4587 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/shards.py
--rw-r--r--   0 bytedance   (502) staff       (20)    29198 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/topic.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9042 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tls/topics.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.896268 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/
--rw-r--r--   0 bytedance   (502) staff       (20)      447 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4038 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    21126 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket.py
--rw-r--r--   0 bytedance   (502) staff       (20)    26865 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_object.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6211 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_objects.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10397 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_policy.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5330 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/buckets.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8963 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/tos/outputs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.900294 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/
--rw-r--r--   0 bytedance   (502) staff       (20)      524 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12370 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6757 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/available_resources.py
--rw-r--r--   0 bytedance   (502) staff       (20)    39679 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/cloud_server.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5485 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/cloud_servers.py
--rw-r--r--   0 bytedance   (502) staff       (20)    22088 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instance.py
--rw-r--r--   0 bytedance   (502) staff       (20)     4291 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instance_types.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7155 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instances.py
--rw-r--r--   0 bytedance   (502) staff       (20)    89670 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11479 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/vpc.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5174 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/vpcs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.906615 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/
--rw-r--r--   0 bytedance   (502) staff       (20)      658 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)   100532 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16470 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/addon.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11017 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/addons.py
--rw-r--r--   0 bytedance   (502) staff       (20)    36420 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/cluster.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14901 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/clusters.py
--rw-r--r--   0 bytedance   (502) staff       (20)    22663 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/default_node_pool.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18342 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/default_node_pool_batch_attach.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10887 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/kubeconfig.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8425 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/kubeconfigs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    25186 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node.py
--rw-r--r--   0 bytedance   (502) staff       (20)    22793 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node_pool.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12142 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node_pools.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10493 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/nodes.py
--rw-r--r--   0 bytedance   (502) staff       (20)   172058 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11310 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vke/support_addons.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.918681 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/
--rw-r--r--   0 bytedance   (502) staff       (20)     1041 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18169 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    24654 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_address_bandwidth.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10257 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_address_bandwidths.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5262 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_addresses.py
--rw-r--r--   0 bytedance   (502) staff       (20)    14212 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_gateway.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6961 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_gateways.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19946 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acl.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9224 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acl_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7707 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acls.py
--rw-r--r--   0 bytedance   (502) staff       (20)    29514 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interface.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9340 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interface_attach.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16172 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interfaces.py
--rw-r--r--   0 bytedance   (502) staff       (20)    82933 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/outputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10137 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_entries.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19950 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_entry.py
--rw-r--r--   0 bytedance   (502) staff       (20)    12293 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_table.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8882 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_table_associate.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7381 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_tables.py
--rw-r--r--   0 bytedance   (502) staff       (20)    16375 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group.py
--rw-r--r--   0 bytedance   (502) staff       (20)    28121 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group_rule.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8326 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group_rules.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8985 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_groups.py
--rw-r--r--   0 bytedance   (502) staff       (20)    21032 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/subnet.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8280 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/subnets.py
--rw-r--r--   0 bytedance   (502) staff       (20)    34172 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/vpc.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7332 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/vpcs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.926071 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/
--rw-r--r--   0 bytedance   (502) staff       (20)      538 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2122 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/_inputs.py
--rw-r--r--   0 bytedance   (502) staff       (20)    85860 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/connection.py
--rw-r--r--   0 bytedance   (502) staff       (20)     8243 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/connections.py
--rw-r--r--   0 bytedance   (502) staff       (20)    19637 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/customer_gateway.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7528 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/customer_gateways.py
--rw-r--r--   0 bytedance   (502) staff       (20)    39600 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway.py
--rw-r--r--   0 bytedance   (502) staff       (20)    15880 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway_route.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7595 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway_routes.py
--rw-r--r--   0 bytedance   (502) staff       (20)     9212 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateways.py
--rw-r--r--   0 bytedance   (502) staff       (20)    32323 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/outputs.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-31 08:04:20.794509 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)     1542 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)    12637 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/not-zip-safe
--rw-r--r--   0 bytedance   (502) staff       (20)       49 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/requires.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       18 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-31 08:04:20.927005 pulumi_volcengine-0.0.6/setup.cfg
--rw-r--r--   0 bytedance   (502) staff       (20)     2147 2023-07-31 08:04:20.000000 pulumi_volcengine-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.345523 pulumi_volcengine-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 03:59:07.345523 pulumi_volcengine-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.309523 pulumi_volcengine-0.0.9/pulumi_volcengine/
+-rw-r--r--   0 runner    (1001) docker     (123)    26633 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.313523 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55363 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62972 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configuration_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49342 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_group_enabler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_instance_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_lifecycle_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_lifecycle_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72793 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.313523 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/cluster_bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.313523 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/attach_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/attach_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40751 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_package_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/cen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/cens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/grant_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/inter_region_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/inter_region_bandwidths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33417 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/route_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/route_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/service_route_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29365 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cen/service_route_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.317523 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acl_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49865 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/clb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/clbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38059 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52849 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/clb/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.317523 pulumi_volcengine-0.0.9/pulumi_volcengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.317523 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/authorization_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27397 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/vpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/cr/vpc_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.317523 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volume_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.321523 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_set_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101243 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pair_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54357 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/launch_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54843 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.321523 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27601 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/eip/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.321523 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59452 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.321523 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/login_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/role_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/user_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/iam/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.325523 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameter_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_list_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59114 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/ssl_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/ssl_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.325523 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/dnat_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21581 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/dnat_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24605 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/snat_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/nat/snat_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.329523 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16246 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.329523 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/account_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63052 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/ip_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/ip_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/parameter_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds/parameter_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.329523 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36294 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlist_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59469 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instance_readonly_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75179 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.329523 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48086 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46732 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/rds_instance_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/rds_instances_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.333523 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17685 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_list_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/continuous_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74974 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57049 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/pitr_time_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/redis/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.337523 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60513 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34774 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm_notify_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm_notify_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/kafka_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/kafka_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174790 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule_applier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule_appliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/shards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29319 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tls/topics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.337523 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/tos/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.337523 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/available_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39800 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/cloud_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22209 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89670 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/vpcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.341523 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100532 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36541 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/default_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/default_node_pool_batch_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/kubeconfigs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25307 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172058 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vke/support_addons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.341523 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_address_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_address_bandwidths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acl_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29635 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interface_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82933 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_table_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34293 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/vpcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.345523 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85981 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/customer_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39721 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32323 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:59:07.309523 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 03:59:07.000000 pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:59:07.345523 pulumi_volcengine-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-01 03:59:06.000000 pulumi_volcengine-0.0.9/setup.py
```

### Comparing `pulumi_volcengine-0.0.6/PKG-INFO` & `pulumi_volcengine-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi_volcengine
-Version: 0.0.6
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing volcengine cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/volcengine/pulumi-volcengine
 Keywords: pulumi volcengine category/cloud
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Volcengine Resource Provider
 
 The Volcengine Resource Provider lets you manage  resources.
 
 ## Installing
@@ -60,7 +61,9 @@
 
 - `volcengine:accesskey` (environment: `VOLCENGINE_ACCESS_KEY`) - the API key for `volcengine`
 - `volcengine:region` (environment: `VOLCENGINE_REGION`) - the region in which to deploy resources
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/volcengine/api-docs/).
+
+
```

### Comparing `pulumi_volcengine-0.0.6/README.md` & `pulumi_volcengine-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/_utilities.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,7 +230,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return "github://api.github.com/volcengine"
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_activities.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_activities.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
     __args__['scalingGroupId'] = scaling_group_id
     __args__['startTime'] = start_time
     __args__['statusCode'] = status_code
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingActivities:ScalingActivities', __args__, opts=opts, typ=ScalingActivitiesResult).value
 
     return AwaitableScalingActivitiesResult(
         activities=__ret__.activities,
         end_time=__ret__.end_time,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configuration.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,14 +934,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingConfigurationArgs.__new__(ScalingConfigurationArgs)
 
             __props__.__dict__["eip_bandwidth"] = eip_bandwidth
             __props__.__dict__["eip_billing_type"] = eip_billing_type
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configuration_attachment.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configuration_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingConfigurationAttachmentArgs.__new__(ScalingConfigurationAttachmentArgs)
 
             if scaling_configuration_id is None and not opts.urn:
                 raise TypeError("Missing required property 'scaling_configuration_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_configurations.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['outputFile'] = output_file
     __args__['scalingConfigurationNames'] = scaling_configuration_names
     __args__['scalingGroupId'] = scaling_group_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingConfigurations:ScalingConfigurations', __args__, opts=opts, typ=ScalingConfigurationsResult).value
 
     return AwaitableScalingConfigurationsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,14 +704,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingGroupArgs.__new__(ScalingGroupArgs)
 
             __props__.__dict__["default_cooldown"] = default_cooldown
             __props__.__dict__["desire_instance_number"] = desire_instance_number
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_group_enabler.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_group_enabler.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingGroupEnablerArgs.__new__(ScalingGroupEnablerArgs)
 
             if scaling_group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'scaling_group_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_groups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['scalingGroupNames'] = scaling_group_names
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingGroups:ScalingGroups', __args__, opts=opts, typ=ScalingGroupsResult).value
 
     return AwaitableScalingGroupsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_instance_attachment.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_instance_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingInstanceAttachmentArgs.__new__(ScalingInstanceAttachmentArgs)
 
             __props__.__dict__["delete_type"] = delete_type
             __props__.__dict__["detach_option"] = detach_option
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_instances.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,14 +174,16 @@
     __args__['scalingConfigurationId'] = scaling_configuration_id
     __args__['scalingGroupId'] = scaling_group_id
     __args__['status'] = status
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingInstances:ScalingInstances', __args__, opts=opts, typ=ScalingInstancesResult).value
 
     return AwaitableScalingInstancesResult(
         creation_type=__ret__.creation_type,
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_lifecycle_hook.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_lifecycle_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,14 +293,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingLifecycleHookArgs.__new__(ScalingLifecycleHookArgs)
 
             if lifecycle_hook_name is None and not opts.urn:
                 raise TypeError("Missing required property 'lifecycle_hook_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_lifecycle_hooks.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_lifecycle_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['scalingGroupId'] = scaling_group_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingLifecycleHooks:ScalingLifecycleHooks', __args__, opts=opts, typ=ScalingLifecycleHooksResult).value
 
     return AwaitableScalingLifecycleHooksResult(
         id=__ret__.id,
         ids=__ret__.ids,
         lifecycle_hook_names=__ret__.lifecycle_hook_names,
         lifecycle_hooks=__ret__.lifecycle_hooks,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_policies.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
     __args__['scalingGroupId'] = scaling_group_id
     __args__['scalingPolicyNames'] = scaling_policy_names
     __args__['scalingPolicyType'] = scaling_policy_type
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:autoscaling/scalingPolicies:ScalingPolicies', __args__, opts=opts, typ=ScalingPoliciesResult).value
 
     return AwaitableScalingPoliciesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/autoscaling/scaling_policy.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/autoscaling/scaling_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,14 +772,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ScalingPolicyArgs.__new__(ScalingPolicyArgs)
 
             __props__.__dict__["active"] = active
             if adjustment_type is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/cluster.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,14 +263,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterArgs.__new__(ClusterArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/cluster_bind.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/cluster_bind.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,14 +207,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterBindArgs.__new__(ClusterBindArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/clusters.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/clusters.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['public'] = public
     __args__['statuses'] = statuses
     __args__['types'] = types
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:bioos/clusters:Clusters', __args__, opts=opts, typ=ClustersResult).value
 
     return AwaitableClustersResult(
         id=__ret__.id,
         ids=__ret__.ids,
         items=__ret__.items,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/workspace.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = WorkspaceArgs.__new__(WorkspaceArgs)
 
             __props__.__dict__["cover_path"] = cover_path
             if description is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/bioos/workspaces.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/bioos/workspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     __args__['outputFile'] = output_file
     __args__['sortBy'] = sort_by
     __args__['sortOrder'] = sort_order
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:bioos/workspaces:Workspaces', __args__, opts=opts, typ=WorkspacesResult).value
 
     return AwaitableWorkspacesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         items=__ret__.items,
         keyword=__ret__.keyword,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/attach_instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/attach_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AttachInstanceArgs.__new__(AttachInstanceArgs)
 
             if cen_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cen_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/attach_instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/attach_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,16 @@
     __args__['instanceRegionId'] = instance_region_id
     __args__['instanceType'] = instance_type
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/attachInstances:AttachInstances', __args__, opts=opts, typ=AttachInstancesResult).value
 
     return AwaitableAttachInstancesResult(
         attach_instances=__ret__.attach_instances,
         cen_id=__ret__.cen_id,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_package.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,14 +630,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BandwidthPackageArgs.__new__(BandwidthPackageArgs)
 
             __props__.__dict__["bandwidth"] = bandwidth
             __props__.__dict__["billing_type"] = billing_type
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_package_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_package_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BandwidthPackageAssociateArgs.__new__(BandwidthPackageAssociateArgs)
 
             if cen_bandwidth_package_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cen_bandwidth_package_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/bandwidth_packages.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/bandwidth_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,16 @@
     __args__['outputFile'] = output_file
     __args__['peerGeographicRegionSetId'] = peer_geographic_region_set_id
     __args__['tags'] = tags
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/bandwidthPackages:BandwidthPackages', __args__, opts=opts, typ=BandwidthPackagesResult).value
 
     return AwaitableBandwidthPackagesResult(
         bandwidth_packages=__ret__.bandwidth_packages,
         cen_bandwidth_package_names=__ret__.cen_bandwidth_package_names,
         cen_id=__ret__.cen_id,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/cen.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/cen.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CenArgs.__new__(CenArgs)
 
             __props__.__dict__["cen_name"] = cen_name
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/cens.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/cens.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['tags'] = tags
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/cens:Cens', __args__, opts=opts, typ=CensResult).value
 
     return AwaitableCensResult(
         cen_names=__ret__.cen_names,
         cens=__ret__.cens,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/grant_instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/grant_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GrantInstanceArgs.__new__(GrantInstanceArgs)
 
             if cen_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cen_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/inter_region_bandwidth.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/inter_region_bandwidth.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InterRegionBandwidthArgs.__new__(InterRegionBandwidthArgs)
 
             if bandwidth is None and not opts.urn:
                 raise TypeError("Missing required property 'bandwidth'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/inter_region_bandwidths.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/inter_region_bandwidths.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['ids'] = ids
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/interRegionBandwidths:InterRegionBandwidths', __args__, opts=opts, typ=InterRegionBandwidthsResult).value
 
     return AwaitableInterRegionBandwidthsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         inter_region_bandwidths=__ret__.inter_region_bandwidths,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/route_entries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/route_entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,16 @@
     __args__['instanceRegionId'] = instance_region_id
     __args__['instanceType'] = instance_type
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/routeEntries:RouteEntries', __args__, opts=opts, typ=RouteEntriesResult).value
 
     return AwaitableRouteEntriesResult(
         cen_id=__ret__.cen_id,
         cen_route_entries=__ret__.cen_route_entries,
         destination_cidr_block=__ret__.destination_cidr_block,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/route_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/route_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouteEntryArgs.__new__(RouteEntryArgs)
 
             if cen_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cen_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/service_route_entries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/service_route_entries.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,14 +155,16 @@
     __args__['outputFile'] = output_file
     __args__['serviceRegionId'] = service_region_id
     __args__['serviceVpcId'] = service_vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cen/serviceRouteEntries:ServiceRouteEntries', __args__, opts=opts, typ=ServiceRouteEntriesResult).value
 
     return AwaitableServiceRouteEntriesResult(
         cen_id=__ret__.cen_id,
         destination_cidr_block=__ret__.destination_cidr_block,
         id=__ret__.id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cen/service_route_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cen/service_route_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServiceRouteEntryArgs.__new__(ServiceRouteEntryArgs)
 
             if cen_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cen_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acl.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AclArgs.__new__(AclArgs)
 
             __props__.__dict__["acl_entries"] = acl_entries
             __props__.__dict__["acl_name"] = acl_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acl_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acl_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AclEntryArgs.__new__(AclEntryArgs)
 
             if acl_id is None and not opts.urn:
                 raise TypeError("Missing required property 'acl_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/acls.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/acls.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['projectName'] = project_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/acls:Acls', __args__, opts=opts, typ=AclsResult).value
 
     return AwaitableAclsResult(
         acl_name=__ret__.acl_name,
         acls=__ret__.acls,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/certificate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CertificateArgs.__new__(CertificateArgs)
 
             __props__.__dict__["certificate_name"] = certificate_name
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/certificates.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/certificates.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     __args__['outputFile'] = output_file
     __args__['projectName'] = project_name
     __args__['tags'] = tags
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/certificates:Certificates', __args__, opts=opts, typ=CertificatesResult).value
 
     return AwaitableCertificatesResult(
         certificate_name=__ret__.certificate_name,
         certificates=__ret__.certificates,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/clb.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/clb.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,14 +793,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClbArgs.__new__(ClbArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["eip_billing_config"] = eip_billing_config
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/clbs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/clbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,16 @@
     __args__['projectName'] = project_name
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/clbs:Clbs', __args__, opts=opts, typ=ClbsResult).value
 
     return AwaitableClbsResult(
         clbs=__ret__.clbs,
         eni_address=__ret__.eni_address,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/listener.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ListenerArgs.__new__(ListenerArgs)
 
             __props__.__dict__["acl_ids"] = acl_ids
             __props__.__dict__["acl_status"] = acl_status
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/listeners.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/listeners.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,14 +149,16 @@
     __args__['loadBalancerId'] = load_balancer_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/listeners:Listeners', __args__, opts=opts, typ=ListenersResult).value
 
     return AwaitableListenersResult(
         id=__ret__.id,
         ids=__ret__.ids,
         listener_name=__ret__.listener_name,
         listeners=__ret__.listeners,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/rule.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RuleArgs.__new__(RuleArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["domain"] = domain
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/rules.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,16 @@
     __args__['ids'] = ids
     __args__['listenerId'] = listener_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/rules:Rules', __args__, opts=opts, typ=RulesResult).value
 
     return AwaitableRulesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         listener_id=__ret__.listener_id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServerGroupArgs.__new__(ServerGroupArgs)
 
             __props__.__dict__["description"] = description
             if load_balancer_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group_server.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServerGroupServerArgs.__new__(ServerGroupServerArgs)
 
             __props__.__dict__["description"] = description
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_group_servers.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_group_servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['serverGroupId'] = server_group_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/serverGroupServers:ServerGroupServers', __args__, opts=opts, typ=ServerGroupServersResult).value
 
     return AwaitableServerGroupServersResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/server_groups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/server_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['serverGroupName'] = server_group_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/serverGroups:ServerGroups', __args__, opts=opts, typ=ServerGroupsResult).value
 
     return AwaitableServerGroupsResult(
         groups=__ret__.groups,
         id=__ret__.id,
         ids=__ret__.ids,
         load_balancer_id=__ret__.load_balancer_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/clb/zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/clb/zones.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     """
     __args__ = dict()
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:clb/zones:Zones', __args__, opts=opts, typ=ZonesResult).value
 
     return AwaitableZonesResult(
         id=__ret__.id,
         master_zones=__ret__.master_zones,
         output_file=__ret__.output_file,
         total_count=__ret__.total_count)
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/config/vars.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/authorization_tokens.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/authorization_tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['registry'] = registry
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/authorizationTokens:AuthorizationTokens', __args__, opts=opts, typ=AuthorizationTokensResult).value
 
     return AwaitableAuthorizationTokensResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         registry=__ret__.registry,
         tokens=__ret__.tokens,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/endpoint.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EndpointArgs.__new__(EndpointArgs)
 
             __props__.__dict__["enabled"] = enabled
             if registry is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/endpoints.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['registry'] = registry
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/endpoints:Endpoints', __args__, opts=opts, typ=EndpointsResult).value
 
     return AwaitableEndpointsResult(
         endpoints=__ret__.endpoints,
         id=__ret__.id,
         output_file=__ret__.output_file,
         registry=__ret__.registry,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/namespace.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NamespaceArgs.__new__(NamespaceArgs)
 
             __props__.__dict__["name"] = name
             if registry is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/namespaces.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/namespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
     __args__['names'] = names
     __args__['outputFile'] = output_file
     __args__['registry'] = registry
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/namespaces:Namespaces', __args__, opts=opts, typ=NamespacesResult).value
 
     return AwaitableNamespacesResult(
         id=__ret__.id,
         names=__ret__.names,
         namespaces=__ret__.namespaces,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/registries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     __args__['outputFile'] = output_file
     __args__['statuses'] = statuses
     __args__['types'] = types
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/registries:Registries', __args__, opts=opts, typ=RegistriesResult).value
 
     return AwaitableRegistriesResult(
         id=__ret__.id,
         names=__ret__.names,
         output_file=__ret__.output_file,
         registries=__ret__.registries,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/registry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,14 +320,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RegistryArgs.__new__(RegistryArgs)
 
             __props__.__dict__["delete_immediately"] = delete_immediately
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/repositories.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     __args__['namespaces'] = namespaces
     __args__['outputFile'] = output_file
     __args__['registry'] = registry
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/repositories:Repositories', __args__, opts=opts, typ=RepositoriesResult).value
 
     return AwaitableRepositoriesResult(
         access_levels=__ret__.access_levels,
         id=__ret__.id,
         names=__ret__.names,
         namespaces=__ret__.namespaces,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/repository.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RepositoryArgs.__new__(RepositoryArgs)
 
             __props__.__dict__["access_level"] = access_level
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/state.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StateArgs.__new__(StateArgs)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/tag.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TagArgs.__new__(TagArgs)
 
             __props__.__dict__["name"] = name
             if namespace is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/tags.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,16 @@
     __args__['registry'] = registry
     __args__['repository'] = repository
     __args__['types'] = types
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/tags:Tags', __args__, opts=opts, typ=TagsResult).value
 
     return AwaitableTagsResult(
         id=__ret__.id,
         names=__ret__.names,
         namespace=__ret__.namespace,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/vpc_endpoint.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/vpc_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointArgs.__new__(VpcEndpointArgs)
 
             if registry is None and not opts.urn:
                 raise TypeError("Missing required property 'registry'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/cr/vpc_endpoints.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/cr/vpc_endpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,14 +128,16 @@
     __args__['outputFile'] = output_file
     __args__['registry'] = registry
     __args__['statuses'] = statuses
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:cr/vpcEndpoints:VpcEndpoints', __args__, opts=opts, typ=VpcEndpointsResult).value
 
     return AwaitableVpcEndpointsResult(
         endpoints=__ret__.endpoints,
         id=__ret__.id,
         output_file=__ret__.output_file,
         registry=__ret__.registry,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volume.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,14 +524,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeArgs.__new__(VolumeArgs)
 
             __props__.__dict__["delete_with_instance"] = delete_with_instance
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volume_attach.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volume_attach.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeAttachArgs.__new__(VolumeAttachArgs)
 
             __props__.__dict__["delete_with_instance"] = delete_with_instance
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ebs/volumes.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ebs/volumes.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,16 @@
     __args__['volumeStatus'] = volume_status
     __args__['volumeType'] = volume_type
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ebs/volumes:Volumes', __args__, opts=opts, typ=VolumesResult).value
 
     return AwaitableVolumesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         instance_id=__ret__.instance_id,
         kind=__ret__.kind,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_set.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DeploymentSetArgs.__new__(DeploymentSetArgs)
 
             if deployment_set_name is None and not opts.urn:
                 raise TypeError("Missing required property 'deployment_set_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_set_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_set_associate.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DeploymentSetAssociateArgs.__new__(DeploymentSetAssociateArgs)
 
             if deployment_set_id is None and not opts.urn:
                 raise TypeError("Missing required property 'deployment_set_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/deployment_sets.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/deployment_sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,16 @@
     __args__['ids'] = ids
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/deploymentSets:DeploymentSets', __args__, opts=opts, typ=DeploymentSetsResult).value
 
     return AwaitableDeploymentSetsResult(
         deployment_sets=__ret__.deployment_sets,
         granularity=__ret__.granularity,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/images.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,16 @@
     __args__['outputFile'] = output_file
     __args__['statuses'] = statuses
     __args__['visibility'] = visibility
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/images:Images', __args__, opts=opts, typ=ImagesResult).value
 
     return AwaitableImagesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         images=__ret__.images,
         instance_type_id=__ret__.instance_type_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1484,14 +1484,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["auto_renew"] = auto_renew
             __props__.__dict__["auto_renew_period"] = auto_renew_period
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,16 @@
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         deployment_set_ids=__ret__.deployment_set_ids,
         hpc_cluster_id=__ret__.hpc_cluster_id,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pair.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KeyPairArgs.__new__(KeyPairArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["key_file"] = key_file
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pair_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pair_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KeyPairAssociateArgs.__new__(KeyPairAssociateArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/key_pairs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/key_pairs.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,16 @@
     __args__['keyPairNames'] = key_pair_names
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/keyPairs:KeyPairs', __args__, opts=opts, typ=KeyPairsResult).value
 
     return AwaitableKeyPairsResult(
         finger_print=__ret__.finger_print,
         id=__ret__.id,
         key_pair_ids=__ret__.key_pair_ids,
         key_pair_name=__ret__.key_pair_name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/launch_template.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/launch_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,14 +871,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LaunchTemplateArgs.__new__(LaunchTemplateArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["eip_bandwidth"] = eip_bandwidth
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/launch_templates.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/launch_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     __args__['launchTemplateNames'] = launch_template_names
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/launchTemplates:LaunchTemplates', __args__, opts=opts, typ=LaunchTemplatesResult).value
 
     return AwaitableLaunchTemplatesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         launch_template_names=__ret__.launch_template_names,
         launch_templates=__ret__.launch_templates,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/state.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StateArgs.__new__(StateArgs)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/ecs/zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/ecs/zones.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['ids'] = ids
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:ecs/zones:Zones', __args__, opts=opts, typ=ZonesResult).value
 
     return AwaitableZonesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/eip/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/eip/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/eip/address.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/eip/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,14 +466,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AddressArgs.__new__(AddressArgs)
 
             __props__.__dict__["bandwidth"] = bandwidth
             if billing_type is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/eip/addresses.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/eip/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,16 @@
     __args__['projectName'] = project_name
     __args__['status'] = status
     __args__['tags'] = tags
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:eip/addresses:Addresses', __args__, opts=opts, typ=AddressesResult).value
 
     return AwaitableAddressesResult(
         addresses=__ret__.addresses,
         associated_instance_id=__ret__.associated_instance_id,
         associated_instance_type=__ret__.associated_instance_type,
         eip_addresses=__ret__.eip_addresses,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/eip/associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/eip/associate.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssociateArgs.__new__(AssociateArgs)
 
             if allocation_id is None and not opts.urn:
                 raise TypeError("Missing required property 'allocation_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/eip/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/eip/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             if instance_configuration is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_configuration'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,16 @@
     __args__['statuses'] = statuses
     __args__['versions'] = versions
     __args__['zoneIds'] = zone_ids
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:escloud/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         charge_types=__ret__.charge_types,
         id=__ret__.id,
         ids=__ret__.ids,
         instances=__ret__.instances,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/regions.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,53 +76,55 @@
             regions=self.regions,
             total_count=self.total_count)
 
 
 def regions(output_file: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableRegionsResult:
     """
-    Use this data source to query detailed information of escloud regions
+    Use this data source to query detailed information of mongodb regions
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_volcengine as volcengine
 
-    default = volcengine.escloud.regions()
+    default = volcengine.mongodb.regions()
     ```
 
 
     :param str output_file: File name where to save data source results.
     """
     __args__ = dict()
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
-    __ret__ = pulumi.runtime.invoke('volcengine:escloud/regions:Regions', __args__, opts=opts, typ=RegionsResult).value
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    __ret__ = pulumi.runtime.invoke('volcengine:mongodb/regions:Regions', __args__, opts=opts, typ=RegionsResult).value
 
     return AwaitableRegionsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         regions=__ret__.regions,
         total_count=__ret__.total_count)
 
 
 @_utilities.lift_output_func(regions)
 def regions_output(output_file: Optional[pulumi.Input[Optional[str]]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[RegionsResult]:
     """
-    Use this data source to query detailed information of escloud regions
+    Use this data source to query detailed information of mongodb regions
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_volcengine as volcengine
 
-    default = volcengine.escloud.regions()
+    default = volcengine.mongodb.regions()
     ```
 
 
     :param str output_file: File name where to save data source results.
     """
     ...
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/escloud/zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/zones.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:escloud/zones:Zones', __args__, opts=opts, typ=ZonesResult).value
 
     return AwaitableZonesResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         region_id=__ret__.region_id,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/access_key.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/access_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccessKeyArgs.__new__(AccessKeyArgs)
 
             __props__.__dict__["pgp_key"] = pgp_key
             __props__.__dict__["secret_file"] = secret_file
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/login_profile.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/login_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LoginProfileArgs.__new__(LoginProfileArgs)
 
             __props__.__dict__["login_allowed"] = login_allowed
             if password is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/policies.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,14 +173,16 @@
     __args__['scope'] = scope
     __args__['status'] = status
     __args__['userName'] = user_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:iam/policies:Policies', __args__, opts=opts, typ=PoliciesResult).value
 
     return AwaitablePoliciesResult(
         id=__ret__.id,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
         policies=__ret__.policies,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/policy.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PolicyArgs.__new__(PolicyArgs)
 
             __props__.__dict__["description"] = description
             if policy_document is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/role.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleArgs.__new__(RoleArgs)
 
             __props__.__dict__["description"] = description
             if display_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/role_policy_attachment.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/role_policy_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RolePolicyAttachmentArgs.__new__(RolePolicyAttachmentArgs)
 
             if policy_name is None and not opts.urn:
                 raise TypeError("Missing required property 'policy_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/roles.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/roles.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     __args__['outputFile'] = output_file
     __args__['query'] = query
     __args__['roleName'] = role_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:iam/roles:Roles', __args__, opts=opts, typ=RolesResult).value
 
     return AwaitableRolesResult(
         id=__ret__.id,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
         query=__ret__.query,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/user.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["display_name"] = display_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/user_policy_attachment.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/user_policy_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserPolicyAttachmentArgs.__new__(UserPolicyAttachmentArgs)
 
             if policy_name is None and not opts.urn:
                 raise TypeError("Missing required property 'policy_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/iam/users.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/iam/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['userNames'] = user_names
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:iam/users:Users', __args__, opts=opts, typ=UsersResult).value
 
     return AwaitableUsersResult(
         id=__ret__.id,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/accounts.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     __args__['accountName'] = account_name
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/accounts:Accounts', __args__, opts=opts, typ=AccountsResult).value
 
     return AwaitableAccountsResult(
         account_name=__ret__.account_name,
         accounts=__ret__.accounts,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/endpoint.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EndpointArgs.__new__(EndpointArgs)
 
             __props__.__dict__["eip_ids"] = eip_ids
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/endpoints.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/endpoints:Endpoints', __args__, opts=opts, typ=EndpointsResult).value
 
     return AwaitableEndpointsResult(
         endpoints=__ret__.endpoints,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -752,14 +752,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["auto_renew"] = auto_renew
             __props__.__dict__["charge_type"] = charge_type
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameter.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceParameterArgs.__new__(InstanceParameterArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameter_logs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameter_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     __args__['startTime'] = start_time
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/instanceParameterLogs:InstanceParameterLogs', __args__, opts=opts, typ=InstanceParameterLogsResult).value
 
     return AwaitableInstanceParameterLogsResult(
         end_time=__ret__.end_time,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instance_parameters.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instance_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,16 @@
     __args__['outputFile'] = output_file
     __args__['parameterNames'] = parameter_names
     __args__['parameterRole'] = parameter_role
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/instanceParameters:InstanceParameters', __args__, opts=opts, typ=InstanceParametersResult).value
 
     return AwaitableInstanceParametersResult(
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         output_file=__ret__.output_file,
         parameter_names=__ret__.parameter_names,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,16 @@
     __args__['updateStartTime'] = update_start_time
     __args__['vpcId'] = vpc_id
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         create_end_time=__ret__.create_end_time,
         create_start_time=__ret__.create_start_time,
         db_engine=__ret__.db_engine,
         db_engine_version=__ret__.db_engine_version,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_list.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MongoAllowListArgs.__new__(MongoAllowListArgs)
 
             if allow_list is None and not opts.urn:
                 raise TypeError("Missing required property 'allow_list'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_list_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_list_associate.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MongoAllowListAssociateArgs.__new__(MongoAllowListAssociateArgs)
 
             if allow_list_id is None and not opts.urn:
                 raise TypeError("Missing required property 'allow_list_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/mongo_allow_lists.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/mongo_allow_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/mongoAllowLists:MongoAllowLists', __args__, opts=opts, typ=MongoAllowListsResult).value
 
     return AwaitableMongoAllowListsResult(
         allow_list_ids=__ret__.allow_list_ids,
         allow_lists=__ret__.allow_lists,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/regions.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/escloud/regions.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,53 +76,55 @@
             regions=self.regions,
             total_count=self.total_count)
 
 
 def regions(output_file: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableRegionsResult:
     """
-    Use this data source to query detailed information of mongodb regions
+    Use this data source to query detailed information of escloud regions
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_volcengine as volcengine
 
-    default = volcengine.mongodb.regions()
+    default = volcengine.escloud.regions()
     ```
 
 
     :param str output_file: File name where to save data source results.
     """
     __args__ = dict()
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
-    __ret__ = pulumi.runtime.invoke('volcengine:mongodb/regions:Regions', __args__, opts=opts, typ=RegionsResult).value
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    __ret__ = pulumi.runtime.invoke('volcengine:escloud/regions:Regions', __args__, opts=opts, typ=RegionsResult).value
 
     return AwaitableRegionsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         regions=__ret__.regions,
         total_count=__ret__.total_count)
 
 
 @_utilities.lift_output_func(regions)
 def regions_output(output_file: Optional[pulumi.Input[Optional[str]]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[RegionsResult]:
     """
-    Use this data source to query detailed information of mongodb regions
+    Use this data source to query detailed information of escloud regions
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_volcengine as volcengine
 
-    default = volcengine.mongodb.regions()
+    default = volcengine.escloud.regions()
     ```
 
 
     :param str output_file: File name where to save data source results.
     """
     ...
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/specs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/specs:Specs', __args__, opts=opts, typ=SpecsResult).value
 
     return AwaitableSpecsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         region_id=__ret__.region_id,
         specs=__ret__.specs,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/ssl_state.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/ssl_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SslStateArgs.__new__(SslStateArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/ssl_states.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/ssl_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     __args__ = dict()
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/sslStates:SslStates', __args__, opts=opts, typ=SslStatesResult).value
 
     return AwaitableSslStatesResult(
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         output_file=__ret__.output_file,
         ssl_states=__ret__.ssl_states,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/mongodb/zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/mongodb/zones.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:mongodb/zones:Zones', __args__, opts=opts, typ=ZonesResult).value
 
     return AwaitableZonesResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         region_id=__ret__.region_id,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/dnat_entries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/dnat_entries.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,16 @@
     __args__['natGatewayId'] = nat_gateway_id
     __args__['outputFile'] = output_file
     __args__['protocol'] = protocol
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:nat/dnatEntries:DnatEntries', __args__, opts=opts, typ=DnatEntriesResult).value
 
     return AwaitableDnatEntriesResult(
         dnat_entries=__ret__.dnat_entries,
         dnat_entry_name=__ret__.dnat_entry_name,
         external_ip=__ret__.external_ip,
         external_port=__ret__.external_port,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/dnat_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/dnat_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DnatEntryArgs.__new__(DnatEntryArgs)
 
             __props__.__dict__["dnat_entry_name"] = dnat_entry_name
             if external_ip is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/gateway.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,14 +424,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GatewayArgs.__new__(GatewayArgs)
 
             __props__.__dict__["billing_type"] = billing_type
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/gateways.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/gateways.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,16 @@
     __args__['subnetId'] = subnet_id
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:nat/gateways:Gateways', __args__, opts=opts, typ=GatewaysResult).value
 
     return AwaitableGatewaysResult(
         description=__ret__.description,
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/snat_entries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/snat_entries.py`

 * *Files 7% similar despite different names*

```diff
@@ -182,14 +182,16 @@
     __args__['snatEntryName'] = snat_entry_name
     __args__['sourceCidr'] = source_cidr
     __args__['subnetId'] = subnet_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:nat/snatEntries:SnatEntries', __args__, opts=opts, typ=SnatEntriesResult).value
 
     return AwaitableSnatEntriesResult(
         eip_id=__ret__.eip_id,
         id=__ret__.id,
         ids=__ret__.ids,
         nat_gateway_id=__ret__.nat_gateway_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/nat/snat_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/nat/snat_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SnatEntryArgs.__new__(SnatEntryArgs)
 
             if eip_id is None and not opts.urn:
                 raise TypeError("Missing required property 'eip_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/security_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecurityGroupArgs.__new__(SecurityGroupArgs)
 
             if endpoint_id is None and not opts.urn:
                 raise TypeError("Missing required property 'endpoint_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,14 +430,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointArgs.__new__(VpcEndpointArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["endpoint_name"] = endpoint_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_connection.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointConnectionArgs.__new__(VpcEndpointConnectionArgs)
 
             if endpoint_id is None and not opts.urn:
                 raise TypeError("Missing required property 'endpoint_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_connections.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,16 @@
     __args__['endpointOwnerAccountId'] = endpoint_owner_account_id
     __args__['outputFile'] = output_file
     __args__['serviceId'] = service_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:privatelink/vpcEndpointConnections:VpcEndpointConnections', __args__, opts=opts, typ=VpcEndpointConnectionsResult).value
 
     return AwaitableVpcEndpointConnectionsResult(
         connections=__ret__.connections,
         endpoint_id=__ret__.endpoint_id,
         endpoint_owner_account_id=__ret__.endpoint_owner_account_id,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointServiceArgs.__new__(VpcEndpointServiceArgs)
 
             __props__.__dict__["auto_accept_enabled"] = auto_accept_enabled
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_permission.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_permission.py`

 * *Files 7% similar despite different names*

```diff
@@ -175,14 +175,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointServicePermissionArgs.__new__(VpcEndpointServicePermissionArgs)
 
             if permit_account_id is None and not opts.urn:
                 raise TypeError("Missing required property 'permit_account_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_permissions.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     __args__['outputFile'] = output_file
     __args__['permitAccountId'] = permit_account_id
     __args__['serviceId'] = service_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:privatelink/vpcEndpointServicePermissions:VpcEndpointServicePermissions', __args__, opts=opts, typ=VpcEndpointServicePermissionsResult).value
 
     return AwaitableVpcEndpointServicePermissionsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         permissions=__ret__.permissions,
         permit_account_id=__ret__.permit_account_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_service_resource.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointServiceResourceInitArgs.__new__(VpcEndpointServiceResourceInitArgs)
 
             if resource_id is None and not opts.urn:
                 raise TypeError("Missing required property 'resource_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_services.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['serviceName'] = service_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:privatelink/vpcEndpointServices:VpcEndpointServices', __args__, opts=opts, typ=VpcEndpointServicesResult).value
 
     return AwaitableVpcEndpointServicesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_zone.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcEndpointZoneArgs.__new__(VpcEndpointZoneArgs)
 
             if endpoint_id is None and not opts.urn:
                 raise TypeError("Missing required property 'endpoint_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoint_zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoint_zones.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['endpointId'] = endpoint_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:privatelink/vpcEndpointZones:VpcEndpointZones', __args__, opts=opts, typ=VpcEndpointZonesResult).value
 
     return AwaitableVpcEndpointZonesResult(
         endpoint_id=__ret__.endpoint_id,
         id=__ret__.id,
         output_file=__ret__.output_file,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/privatelink/vpc_endpoints.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/privatelink/vpc_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,16 @@
     __args__['serviceName'] = service_name
     __args__['status'] = status
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:privatelink/vpcEndpoints:VpcEndpoints', __args__, opts=opts, typ=VpcEndpointsResult).value
 
     return AwaitableVpcEndpointsResult(
         endpoint_name=__ret__.endpoint_name,
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/provider.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             if access_key is None:
                 access_key = _utilities.get_env('VOLCENGINE_ACCESS_KEY')
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/account.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountArgs.__new__(AccountArgs)
 
             if account_name is None and not opts.urn:
                 raise TypeError("Missing required property 'account_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/account_privilege.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/account_privilege.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,14 +270,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountPrivilegeArgs.__new__(AccountPrivilegeArgs)
 
             if account_name is None and not opts.urn:
                 raise TypeError("Missing required property 'account_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/accounts.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     __args__['instanceId'] = instance_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds/accounts:Accounts', __args__, opts=opts, typ=AccountsResult).value
 
     return AwaitableAccountsResult(
         account_name=__ret__.account_name,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/database.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseArgs.__new__(DatabaseArgs)
 
             if character_set_name is None and not opts.urn:
                 raise TypeError("Missing required property 'character_set_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/databases.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/databases.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     __args__['instanceId'] = instance_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds/databases:Databases', __args__, opts=opts, typ=DatabasesResult).value
 
     return AwaitableDatabasesResult(
         db_status=__ret__.db_status,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -954,14 +954,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["auto_renew"] = auto_renew
             if charge_type is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,16 @@
     __args__['outputFile'] = output_file
     __args__['region'] = region
     __args__['zone'] = zone
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         create_end_time=__ret__.create_end_time,
         create_start_time=__ret__.create_start_time,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/ip_list.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/ip_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IpListArgs.__new__(IpListArgs)
 
             if group_name is None and not opts.urn:
                 raise TypeError("Missing required property 'group_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/ip_lists.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/ip_lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     __args__['instanceId'] = instance_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds/ipLists:IpLists', __args__, opts=opts, typ=IpListsResult).value
 
     return AwaitableIpListsResult(
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/parameter_template.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/parameter_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ParameterTemplateArgs.__new__(ParameterTemplateArgs)
 
             __props__.__dict__["template_desc"] = template_desc
             if template_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds/parameter_templates.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds/parameter_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,16 @@
     __args__['templateSource'] = template_source
     __args__['templateType'] = template_type
     __args__['templateTypeVersion'] = template_type_version
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds/parameterTemplates:ParameterTemplates', __args__, opts=opts, typ=ParameterTemplatesResult).value
 
     return AwaitableParameterTemplatesResult(
         id=__ret__.id,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
         rds_parameter_templates=__ret__.rds_parameter_templates,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/account.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountArgs.__new__(AccountArgs)
 
             if account_name is None and not opts.urn:
                 raise TypeError("Missing required property 'account_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/accounts.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     __args__['instanceId'] = instance_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds_mysql/accounts:Accounts', __args__, opts=opts, typ=AccountsResult).value
 
     return AwaitableAccountsResult(
         account_name=__ret__.account_name,
         accounts=__ret__.accounts,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlist.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AllowlistArgs.__new__(AllowlistArgs)
 
             __props__.__dict__["allow_list_desc"] = allow_list_desc
             if allow_list_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlist_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlist_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AllowlistAssociateArgs.__new__(AllowlistAssociateArgs)
 
             if allow_list_id is None and not opts.urn:
                 raise TypeError("Missing required property 'allow_list_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/allowlists.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/allowlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds_mysql/allowlists:Allowlists', __args__, opts=opts, typ=AllowlistsResult).value
 
     return AwaitableAllowlistsResult(
         allow_lists=__ret__.allow_lists,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/database.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,14 +236,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseArgs.__new__(DatabaseArgs)
 
             __props__.__dict__["character_set_name"] = character_set_name
             if db_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/databases.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     __args__['instanceId'] = instance_id
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds_mysql/databases:Databases', __args__, opts=opts, typ=DatabasesResult).value
 
     return AwaitableDatabasesResult(
         databases=__ret__.databases,
         db_name=__ret__.db_name,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -926,14 +926,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["allow_list_ids"] = allow_list_ids
             if charge_info is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instance_readonly_node.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instance_readonly_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceReadonlyNodeArgs.__new__(InstanceReadonlyNodeArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds_mysql/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         charge_type=__ret__.charge_type,
         create_time_end=__ret__.create_time_end,
         create_time_start=__ret__.create_time_start,
         db_engine_version=__ret__.db_engine_version,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_mysql/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_mysql/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/rds_instance_v2.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/rds_instance_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,14 +686,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RdsInstanceV2Args.__new__(RdsInstanceV2Args)
 
             if charge_info is None and not opts.urn:
                 raise TypeError("Missing required property 'charge_info'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/rds_v2/rds_instances_v2.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/rds_v2/rds_instances_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:rds_v2/rdsInstancesV2:RdsInstancesV2', __args__, opts=opts, typ=RdsInstancesV2Result).value
 
     return AwaitableRdsInstancesV2Result(
         charge_type=__ret__.charge_type,
         create_time_end=__ret__.create_time_end,
         create_time_start=__ret__.create_time_start,
         db_engine_version=__ret__.db_engine_version,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/account.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountArgs.__new__(AccountArgs)
 
             if account_name is None and not opts.urn:
                 raise TypeError("Missing required property 'account_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/accounts.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
     __args__['accountName'] = account_name
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/accounts:Accounts', __args__, opts=opts, typ=AccountsResult).value
 
     return AwaitableAccountsResult(
         account_name=__ret__.account_name,
         accounts=__ret__.accounts,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_list.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AllowListArgs.__new__(AllowListArgs)
 
             __props__.__dict__["allow_list_desc"] = allow_list_desc
             if allow_list_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_list_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_list_associate.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AllowListAssociateArgs.__new__(AllowListAssociateArgs)
 
             if allow_list_id is None and not opts.urn:
                 raise TypeError("Missing required property 'allow_list_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/allow_lists.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/allow_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/allowLists:AllowLists', __args__, opts=opts, typ=AllowListsResult).value
 
     return AwaitableAllowListsResult(
         allow_lists=__ret__.allow_lists,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backup.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BackupArgs.__new__(BackupArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backup_restore.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backup_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BackupRestoreArgs.__new__(BackupRestoreArgs)
 
             __props__.__dict__["backup_type"] = backup_type
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/backups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     __args__['instanceId'] = instance_id
     __args__['outputFile'] = output_file
     __args__['startTime'] = start_time
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/backups:Backups', __args__, opts=opts, typ=BackupsResult).value
 
     return AwaitableBackupsResult(
         backup_strategy_lists=__ret__.backup_strategy_lists,
         backups=__ret__.backups,
         end_time=__ret__.end_time,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/continuous_backup.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/continuous_backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ContinuousBackupArgs.__new__(ContinuousBackupArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/endpoint.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EndpointArgs.__new__(EndpointArgs)
 
             if eip_id is None and not opts.urn:
                 raise TypeError("Missing required property 'eip_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,14 +1007,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["apply_immediately"] = apply_immediately
             __props__.__dict__["auto_renew"] = auto_renew
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,16 @@
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         charge_type=__ret__.charge_type,
         engine_version=__ret__.engine_version,
         id=__ret__.id,
         instance_id=__ret__.instance_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/pitr_time_windows.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/pitr_time_windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     __args__ = dict()
     __args__['ids'] = ids
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/pitrTimeWindows:PitrTimeWindows', __args__, opts=opts, typ=PitrTimeWindowsResult).value
 
     return AwaitablePitrTimeWindowsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
         periods=__ret__.periods,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/regions.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/regions:Regions', __args__, opts=opts, typ=RegionsResult).value
 
     return AwaitableRegionsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         region_id=__ret__.region_id,
         regions=__ret__.regions,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/state.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StateArgs.__new__(StateArgs)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/redis/zones.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/redis/zones.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['regionId'] = region_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:redis/zones:Zones', __args__, opts=opts, typ=ZonesResult).value
 
     return AwaitableZonesResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         region_id=__ret__.region_id,
         total_count=__ret__.total_count,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AlarmArgs.__new__(AlarmArgs)
 
             if alarm_name is None and not opts.urn:
                 raise TypeError("Missing required property 'alarm_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm_notify_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm_notify_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AlarmNotifyGroupArgs.__new__(AlarmNotifyGroupArgs)
 
             if alarm_notify_group_name is None and not opts.urn:
                 raise TypeError("Missing required property 'alarm_notify_group_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarm_notify_groups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarm_notify_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,16 @@
     __args__['iamProjectName'] = iam_project_name
     __args__['outputFile'] = output_file
     __args__['receiverName'] = receiver_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/alarmNotifyGroups:AlarmNotifyGroups', __args__, opts=opts, typ=AlarmNotifyGroupsResult).value
 
     return AwaitableAlarmNotifyGroupsResult(
         alarm_notify_group_id=__ret__.alarm_notify_group_id,
         alarm_notify_group_name=__ret__.alarm_notify_group_name,
         groups=__ret__.groups,
         iam_project_name=__ret__.iam_project_name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/alarms.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/alarms.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,14 +185,16 @@
     __args__['status'] = status
     __args__['topicId'] = topic_id
     __args__['topicName'] = topic_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/alarms:Alarms', __args__, opts=opts, typ=AlarmsResult).value
 
     return AwaitableAlarmsResult(
         alarm_id=__ret__.alarm_id,
         alarm_name=__ret__.alarm_name,
         alarms=__ret__.alarms,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = HostArgs.__new__(HostArgs)
 
             if host_group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'host_group_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,14 +532,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = HostGroupArgs.__new__(HostGroupArgs)
 
             __props__.__dict__["auto_update"] = auto_update
             if host_group_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/host_groups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/host_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,16 @@
     __args__['iamProjectName'] = iam_project_name
     __args__['outputFile'] = output_file
     __args__['serviceLogging'] = service_logging
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/hostGroups:HostGroups', __args__, opts=opts, typ=HostGroupsResult).value
 
     return AwaitableHostGroupsResult(
         auto_update=__ret__.auto_update,
         host_group_id=__ret__.host_group_id,
         host_group_name=__ret__.host_group_name,
         host_identifier=__ret__.host_identifier,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/hosts.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/hosts.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,16 @@
     __args__['hostGroupId'] = host_group_id
     __args__['ip'] = ip
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/hosts:Hosts', __args__, opts=opts, typ=HostsResult).value
 
     return AwaitableHostsResult(
         heartbeat_status=__ret__.heartbeat_status,
         host_group_id=__ret__.host_group_id,
         host_infos=__ret__.host_infos,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/index.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IndexArgs.__new__(IndexArgs)
 
             __props__.__dict__["full_text"] = full_text
             __props__.__dict__["key_values"] = key_values
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/indexes.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/indexes.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['ids'] = ids
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/indexes:Indexes', __args__, opts=opts, typ=IndexesResult).value
 
     return AwaitableIndexesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
         tls_indexes=__ret__.tls_indexes,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/kafka_consumer.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/kafka_consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,14 +163,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaConsumerArgs.__new__(KafkaConsumerArgs)
 
             if topic_id is None and not opts.urn:
                 raise TypeError("Missing required property 'topic_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/kafka_consumers.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/kafka_consumers.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     __args__ = dict()
     __args__['ids'] = ids
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/kafkaConsumers:KafkaConsumers', __args__, opts=opts, typ=KafkaConsumersResult).value
 
     return AwaitableKafkaConsumersResult(
         datas=__ret__.datas,
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/project.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["iam_project_name"] = iam_project_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/projects.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,16 @@
     __args__['projectId'] = project_id
     __args__['projectName'] = project_name
     __args__['tags'] = tags
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/projects:Projects', __args__, opts=opts, typ=ProjectsResult).value
 
     return AwaitableProjectsResult(
         iam_project_name=__ret__.iam_project_name,
         id=__ret__.id,
         is_full_name=__ret__.is_full_name,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -663,14 +663,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RuleArgs.__new__(RuleArgs)
 
             __props__.__dict__["container_rule"] = container_rule
             __props__.__dict__["exclude_paths"] = exclude_paths
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule_applier.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule_applier.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RuleApplierArgs.__new__(RuleApplierArgs)
 
             if host_group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'host_group_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rule_appliers.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rule_appliers.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['hostGroupId'] = host_group_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/ruleAppliers:RuleAppliers', __args__, opts=opts, typ=RuleAppliersResult).value
 
     return AwaitableRuleAppliersResult(
         host_group_id=__ret__.host_group_id,
         id=__ret__.id,
         output_file=__ret__.output_file,
         rules=__ret__.rules,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/rules.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,16 @@
     __args__['ruleName'] = rule_name
     __args__['topicId'] = topic_id
     __args__['topicName'] = topic_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/rules:Rules', __args__, opts=opts, typ=RulesResult).value
 
     return AwaitableRulesResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         project_id=__ret__.project_id,
         rule_id=__ret__.rule_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/shards.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/shards.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     __args__ = dict()
     __args__['outputFile'] = output_file
     __args__['topicId'] = topic_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/shards:Shards', __args__, opts=opts, typ=ShardsResult).value
 
     return AwaitableShardsResult(
         id=__ret__.id,
         output_file=__ret__.output_file,
         shards=__ret__.shards,
         topic_id=__ret__.topic_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/topic.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,14 +540,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TopicArgs.__new__(TopicArgs)
 
             __props__.__dict__["auto_split"] = auto_split
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tls/topics.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tls/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,16 @@
     __args__['tags'] = tags
     __args__['topicId'] = topic_id
     __args__['topicName'] = topic_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tls/topics:Topics', __args__, opts=opts, typ=TopicsResult).value
 
     return AwaitableTopicsResult(
         id=__ret__.id,
         is_full_name=__ret__.is_full_name,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BucketArgs.__new__(BucketArgs)
 
             __props__.__dict__["account_acls"] = account_acls
             if bucket_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_object.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,14 +473,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BucketObjectArgs.__new__(BucketObjectArgs)
 
             __props__.__dict__["account_acls"] = account_acls
             if bucket_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_objects.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,14 +131,16 @@
     __args__['nameRegex'] = name_regex
     __args__['objectName'] = object_name
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tos/bucketObjects:BucketObjects', __args__, opts=opts, typ=BucketObjectsResult).value
 
     return AwaitableBucketObjectsResult(
         bucket_name=__ret__.bucket_name,
         id=__ret__.id,
         name_regex=__ret__.name_regex,
         object_name=__ret__.object_name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/bucket_policy.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/bucket_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BucketPolicyArgs.__new__(BucketPolicyArgs)
 
             if bucket_name is None and not opts.urn:
                 raise TypeError("Missing required property 'bucket_name'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/buckets.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/buckets.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     __args__['bucketName'] = bucket_name
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:tos/buckets:Buckets', __args__, opts=opts, typ=BucketsResult).value
 
     return AwaitableBucketsResult(
         bucket_name=__ret__.bucket_name,
         buckets=__ret__.buckets,
         id=__ret__.id,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/tos/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/tos/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/available_resources.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/available_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
     __args__['cloudDiskType'] = cloud_disk_type
     __args__['instanceType'] = instance_type
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:veenedge/availableResources:AvailableResources', __args__, opts=opts, typ=AvailableResourcesResult).value
 
     return AwaitableAvailableResourcesResult(
         bandwith_limit=__ret__.bandwith_limit,
         cloud_disk_type=__ret__.cloud_disk_type,
         id=__ret__.id,
         instance_type=__ret__.instance_type,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/cloud_server.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/cloud_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,14 +663,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CloudServerArgs.__new__(CloudServerArgs)
 
             __props__.__dict__["billing_config"] = billing_config
             if cloudserver_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/cloud_servers.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/cloud_servers.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     __args__['ids'] = ids
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:veenedge/cloudServers:CloudServers', __args__, opts=opts, typ=CloudServersResult).value
 
     return AwaitableCloudServersResult(
         cloud_servers=__ret__.cloud_servers,
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instance.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,14 +420,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["area_name"] = area_name
             __props__.__dict__["cloudserver_id"] = cloudserver_id
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instance_types.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instance_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     """
     __args__ = dict()
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:veenedge/instanceTypes:InstanceTypes', __args__, opts=opts, typ=InstanceTypesResult).value
 
     return AwaitableInstanceTypesResult(
         id=__ret__.id,
         instance_type_configs=__ret__.instance_type_configs,
         output_file=__ret__.output_file,
         total_count=__ret__.total_count)
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/instances.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['names'] = names
     __args__['outputFile'] = output_file
     __args__['statuses'] = statuses
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:veenedge/instances:Instances', __args__, opts=opts, typ=InstancesResult).value
 
     return AwaitableInstancesResult(
         cloud_server_ids=__ret__.cloud_server_ids,
         id=__ret__.id,
         ids=__ret__.ids,
         instances=__ret__.instances,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/vpc.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/vpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcArgs.__new__(VpcArgs)
 
             __props__.__dict__["cidr"] = cidr
             if cluster_name is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/veenedge/vpcs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/veenedge/vpcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     __args__['ids'] = ids
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:veenedge/vpcs:Vpcs', __args__, opts=opts, typ=VpcsResult).value
 
     return AwaitableVpcsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/addon.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/addon.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AddonArgs.__new__(AddonArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/addons.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/addons.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,16 @@
     __args__['outputFile'] = output_file
     __args__['statuses'] = statuses
     __args__['updateClientToken'] = update_client_token
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/addons:Addons', __args__, opts=opts, typ=AddonsResult).value
 
     return AwaitableAddonsResult(
         addons=__ret__.addons,
         cluster_ids=__ret__.cluster_ids,
         create_client_token=__ret__.create_client_token,
         deploy_modes=__ret__.deploy_modes,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/cluster.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,14 +568,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterArgs.__new__(ClusterArgs)
 
             __props__.__dict__["client_token"] = client_token
             if cluster_config is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/clusters.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,16 @@
     __args__['statuses'] = statuses
     __args__['tags'] = tags
     __args__['updateClientToken'] = update_client_token
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/clusters:Clusters', __args__, opts=opts, typ=ClustersResult).value
 
     return AwaitableClustersResult(
         clusters=__ret__.clusters,
         create_client_token=__ret__.create_client_token,
         delete_protection_enabled=__ret__.delete_protection_enabled,
         id=__ret__.id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/default_node_pool.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/default_node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DefaultNodePoolArgs.__new__(DefaultNodePoolArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/default_node_pool_batch_attach.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/default_node_pool_batch_attach.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DefaultNodePoolBatchAttachArgs.__new__(DefaultNodePoolBatchAttachArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/kubeconfig.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/kubeconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KubeconfigArgs.__new__(KubeconfigArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/kubeconfigs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/kubeconfigs.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,16 @@
     __args__['pageNumber'] = page_number
     __args__['pageSize'] = page_size
     __args__['types'] = types
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/kubeconfigs:Kubeconfigs', __args__, opts=opts, typ=KubeconfigsResult).value
 
     return AwaitableKubeconfigsResult(
         cluster_ids=__ret__.cluster_ids,
         id=__ret__.id,
         ids=__ret__.ids,
         kubeconfigs=__ret__.kubeconfigs,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,14 +438,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodeArgs.__new__(NodeArgs)
 
             __props__.__dict__["additional_container_storage_enabled"] = additional_container_storage_enabled
             __props__.__dict__["client_token"] = client_token
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node_pool.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodePoolArgs.__new__(NodePoolArgs)
 
             __props__.__dict__["auto_scaling"] = auto_scaling
             __props__.__dict__["client_token"] = client_token
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/node_pools.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/node_pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,16 @@
     __args__['statuses'] = statuses
     __args__['tags'] = tags
     __args__['updateClientToken'] = update_client_token
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/nodePools:NodePools', __args__, opts=opts, typ=NodePoolsResult).value
 
     return AwaitableNodePoolsResult(
         auto_scaling_enabled=__ret__.auto_scaling_enabled,
         cluster_id=__ret__.cluster_id,
         cluster_ids=__ret__.cluster_ids,
         create_client_token=__ret__.create_client_token,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/nodes.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,14 +212,16 @@
     __args__['outputFile'] = output_file
     __args__['statuses'] = statuses
     __args__['zoneIds'] = zone_ids
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/nodes:Nodes', __args__, opts=opts, typ=NodesResult).value
 
     return AwaitableNodesResult(
         cluster_ids=__ret__.cluster_ids,
         create_client_token=__ret__.create_client_token,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vke/support_addons.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vke/support_addons.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     __args__['necessaries'] = necessaries
     __args__['outputFile'] = output_file
     __args__['podNetworkModes'] = pod_network_modes
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vke/supportAddons:SupportAddons', __args__, opts=opts, typ=SupportAddonsResult).value
 
     return AwaitableSupportAddonsResult(
         addons=__ret__.addons,
         categories=__ret__.categories,
         deploy_modes=__ret__.deploy_modes,
         deploy_node_types=__ret__.deploy_node_types,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_address_bandwidth.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_address_bandwidth.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,14 +400,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = Ipv6AddressBandwidthArgs.__new__(Ipv6AddressBandwidthArgs)
 
             __props__.__dict__["bandwidth"] = bandwidth
             if billing_type is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_address_bandwidths.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_address_bandwidths.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,14 +185,16 @@
     __args__['networkType'] = network_type
     __args__['outputFile'] = output_file
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/ipv6AddressBandwidths:Ipv6AddressBandwidths', __args__, opts=opts, typ=Ipv6AddressBandwidthsResult).value
 
     return AwaitableIpv6AddressBandwidthsResult(
         associated_instance_id=__ret__.associated_instance_id,
         associated_instance_type=__ret__.associated_instance_type,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_addresses.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_addresses.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     __args__ = dict()
     __args__['associatedInstanceId'] = associated_instance_id
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/ipv6Addresses:Ipv6Addresses', __args__, opts=opts, typ=Ipv6AddressesResult).value
 
     return AwaitableIpv6AddressesResult(
         associated_instance_id=__ret__.associated_instance_id,
         id=__ret__.id,
         ipv6_addresses=__ret__.ipv6_addresses,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_gateway.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = Ipv6GatewayArgs.__new__(Ipv6GatewayArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/ipv6_gateways.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/ipv6_gateways.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     __args__['vpcIds'] = vpc_ids
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/ipv6Gateways:Ipv6Gateways', __args__, opts=opts, typ=Ipv6GatewaysResult).value
 
     return AwaitableIpv6GatewaysResult(
         id=__ret__.id,
         ids=__ret__.ids,
         ipv6_gateways=__ret__.ipv6_gateways,
         name=__ret__.name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acl.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkAclArgs.__new__(NetworkAclArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["egress_acl_entries"] = egress_acl_entries
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acl_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acl_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkAclAssociateArgs.__new__(NetworkAclAssociateArgs)
 
             if network_acl_id is None and not opts.urn:
                 raise TypeError("Missing required property 'network_acl_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_acls.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_acls.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,16 @@
     __args__['outputFile'] = output_file
     __args__['subnetId'] = subnet_id
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/networkAcls:NetworkAcls', __args__, opts=opts, typ=NetworkAclsResult).value
 
     return AwaitableNetworkAclsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         network_acl_name=__ret__.network_acl_name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interface.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,14 +479,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkInterfaceArgs.__new__(NetworkInterfaceArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["network_interface_name"] = network_interface_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interface_attach.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interface_attach.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkInterfaceAttachArgs.__new__(NetworkInterfaceAttachArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/network_interfaces.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/network_interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,16 @@
     __args__['type'] = type
     __args__['vpcId'] = vpc_id
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/networkInterfaces:NetworkInterfaces', __args__, opts=opts, typ=NetworkInterfacesResult).value
 
     return AwaitableNetworkInterfacesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         instance_id=__ret__.instance_id,
         network_interface_ids=__ret__.network_interface_ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_entries.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,16 @@
     __args__['routeEntryName'] = route_entry_name
     __args__['routeEntryType'] = route_entry_type
     __args__['routeTableId'] = route_table_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/routeEntries:RouteEntries', __args__, opts=opts, typ=RouteEntriesResult).value
 
     return AwaitableRouteEntriesResult(
         destination_cidr_block=__ret__.destination_cidr_block,
         id=__ret__.id,
         ids=__ret__.ids,
         next_hop_id=__ret__.next_hop_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_entry.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouteEntryArgs.__new__(RouteEntryArgs)
 
             __props__.__dict__["description"] = description
             if destination_cidr_block is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_table.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,14 +244,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouteTableArgs.__new__(RouteTableArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["project_name"] = project_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_table_associate.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_table_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouteTableAssociateArgs.__new__(RouteTableAssociateArgs)
 
             if route_table_id is None and not opts.urn:
                 raise TypeError("Missing required property 'route_table_id'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/route_tables.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/route_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,16 @@
     __args__['projectName'] = project_name
     __args__['routeTableName'] = route_table_name
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/routeTables:RouteTables', __args__, opts=opts, typ=RouteTablesResult).value
 
     return AwaitableRouteTablesResult(
         id=__ret__.id,
         ids=__ret__.ids,
         output_file=__ret__.output_file,
         project_name=__ret__.project_name,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,14 +309,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecurityGroupArgs.__new__(SecurityGroupArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["project_name"] = project_name
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group_rule.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecurityGroupRuleArgs.__new__(SecurityGroupRuleArgs)
 
             __props__.__dict__["cidr_ip"] = cidr_ip
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_group_rules.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_group_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,16 @@
     __args__['protocol'] = protocol
     __args__['securityGroupId'] = security_group_id
     __args__['sourceGroupId'] = source_group_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/securityGroupRules:SecurityGroupRules', __args__, opts=opts, typ=SecurityGroupRulesResult).value
 
     return AwaitableSecurityGroupRulesResult(
         cidr_ip=__ret__.cidr_ip,
         direction=__ret__.direction,
         id=__ret__.id,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/security_groups.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/security_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,16 @@
     __args__['securityGroupNames'] = security_group_names
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/securityGroups:SecurityGroups', __args__, opts=opts, typ=SecurityGroupsResult).value
 
     return AwaitableSecurityGroupsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/subnet.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/subnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SubnetArgs.__new__(SubnetArgs)
 
             if cidr_block is None and not opts.urn:
                 raise TypeError("Missing required property 'cidr_block'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/subnets.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/subnets.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,14 +179,16 @@
     __args__['subnetName'] = subnet_name
     __args__['vpcId'] = vpc_id
     __args__['zoneId'] = zone_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/subnets:Subnets', __args__, opts=opts, typ=SubnetsResult).value
 
     return AwaitableSubnetsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/vpc.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/vpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,14 +568,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcArgs.__new__(VpcArgs)
 
             if cidr_block is None and not opts.urn:
                 raise TypeError("Missing required property 'cidr_block'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpc/vpcs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpc/vpcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     __args__['projectName'] = project_name
     __args__['tags'] = tags
     __args__['vpcName'] = vpc_name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpc/vpcs:Vpcs', __args__, opts=opts, typ=VpcsResult).value
 
     return AwaitableVpcsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
         output_file=__ret__.output_file,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/__init__.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/_inputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/connection.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1220,14 +1220,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ConnectionArgs.__new__(ConnectionArgs)
 
             __props__.__dict__["attach_type"] = attach_type
             if customer_gateway_id is None and not opts.urn:
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/connections.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
     __args__['outputFile'] = output_file
     __args__['vpnConnectionNames'] = vpn_connection_names
     __args__['vpnGatewayId'] = vpn_gateway_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpn/connections:Connections', __args__, opts=opts, typ=ConnectionsResult).value
 
     return AwaitableConnectionsResult(
         customer_gateway_id=__ret__.customer_gateway_id,
         id=__ret__.id,
         ids=__ret__.ids,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/customer_gateway.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/customer_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CustomerGatewayArgs.__new__(CustomerGatewayArgs)
 
             __props__.__dict__["customer_gateway_name"] = customer_gateway_name
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/customer_gateways.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/customer_gateways.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     __args__['ipAddress'] = ip_address
     __args__['nameRegex'] = name_regex
     __args__['outputFile'] = output_file
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpn/customerGateways:CustomerGateways', __args__, opts=opts, typ=CustomerGatewaysResult).value
 
     return AwaitableCustomerGatewaysResult(
         customer_gateway_names=__ret__.customer_gateway_names,
         customer_gateways=__ret__.customer_gateways,
         id=__ret__.id,
         ids=__ret__.ids,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,14 +641,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GatewayArgs.__new__(GatewayArgs)
 
             if bandwidth is None and not opts.urn:
                 raise TypeError("Missing required property 'bandwidth'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway_route.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,16 @@
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GatewayRouteArgs.__new__(GatewayRouteArgs)
 
             if destination_cidr_block is None and not opts.urn:
                 raise TypeError("Missing required property 'destination_cidr_block'")
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateway_routes.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateway_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,16 @@
     __args__['nextHopId'] = next_hop_id
     __args__['outputFile'] = output_file
     __args__['vpnGatewayId'] = vpn_gateway_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpn/gatewayRoutes:GatewayRoutes', __args__, opts=opts, typ=GatewayRoutesResult).value
 
     return AwaitableGatewayRoutesResult(
         destination_cidr_block=__ret__.destination_cidr_block,
         id=__ret__.id,
         ids=__ret__.ids,
         next_hop_id=__ret__.next_hop_id,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/gateways.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/gateways.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     __args__['tags'] = tags
     __args__['vpcId'] = vpc_id
     __args__['vpnGatewayNames'] = vpn_gateway_names
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
+        if opts.plugin_download_url is None:
+            opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('volcengine:vpn/gateways:Gateways', __args__, opts=opts, typ=GatewaysResult).value
 
     return AwaitableGatewaysResult(
         id=__ret__.id,
         ids=__ret__.ids,
         ip_address=__ret__.ip_address,
         name_regex=__ret__.name_regex,
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine/vpn/outputs.py` & `pulumi_volcengine-0.0.9/pulumi_volcengine/vpn/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/PKG-INFO` & `pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi-volcengine
-Version: 0.0.6
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing volcengine cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/volcengine/pulumi-volcengine
 Keywords: pulumi volcengine category/cloud
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Volcengine Resource Provider
 
 The Volcengine Resource Provider lets you manage  resources.
 
 ## Installing
@@ -60,7 +61,9 @@
 
 - `volcengine:accesskey` (environment: `VOLCENGINE_ACCESS_KEY`) - the API key for `volcengine`
 - `volcengine:region` (environment: `VOLCENGINE_REGION`) - the region in which to deploy resources
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/volcengine/api-docs/).
+
+
```

### Comparing `pulumi_volcengine-0.0.6/pulumi_volcengine.egg-info/SOURCES.txt` & `pulumi_volcengine-0.0.9/pulumi_volcengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_volcengine-0.0.6/setup.py` & `pulumi_volcengine-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.6"
-PLUGIN_VERSION = "0.0.6"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'volcengine', PLUGIN_VERSION])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'volcengine', PLUGIN_VERSION, '--server', 'github://api.github.com/volcengine'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the volcengine resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

