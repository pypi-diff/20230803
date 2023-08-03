# Comparing `tmp/rally-openstack-2.2.0.tar.gz` & `tmp/rally-openstack-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rally-openstack-2.2.0.tar", last modified: Tue Oct 26 10:57:49 2021, max compression
+gzip compressed data, was "rally-openstack-2.3.0.tar", last modified: Thu Aug  3 12:50:27 2023, max compression
```

## Comparing `rally-openstack-2.2.0.tar` & `rally-openstack-2.3.0.tar`

### file list

```diff
@@ -1,1763 +1,1757 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.dockerignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.392201 rally-openstack-2.2.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/docker-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-barbican.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-basic-with-existing-users.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-cinder.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-designate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-ironic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-keystone-glance-swift.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-magnum.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5059 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-manila.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-mistral.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-monasca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-murano.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-neutron-trunk.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-neutron-with-extensions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-octavia.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-senlin.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-simple-job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-telemetry.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-watcher.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      502 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-task-zaqar.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-tox-functional.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/rally-verify-tempest.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/.zuul.d/zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12966 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18434 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/CHANGELOG.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    91081 2021-10-26 10:57:48.000000 rally-openstack-2.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2669 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/DOCKER_README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.392201 rally-openstack-2.2.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.392201 rally-openstack-2.2.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4039 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/devstack/lib/rally
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.392201 rally-openstack-2.2.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/etc/motd
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.392201 rally-openstack-2.2.0/etc/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/etc/rally/rally-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30337 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/etc/rally/rally.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.396201 rally-openstack-2.2.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/barbican.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/basic-with-existing-users.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/certifcation_task_args.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    28561 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/cinder.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/designate.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.400201 rally-openstack-2.2.0/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/autoscaling_group.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/autoscaling_policy.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/default.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/hook_example_script.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/install_benchmark.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/instance_test.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/mistral_input.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/mistral_params.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/mistral_wb.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.356200 rally-openstack-2.2.0/rally-jobs/extra/murano/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/Classes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/Classes/HelloReporter.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/ui.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/manifest.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34575 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/murano/applications/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/random_strings.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/resource_group.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/resource_group_server_with_volume.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/resource_group_with_constraint.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/resource_group_with_outputs.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/server_with_ports.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/server_with_volume.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_autoscaling_policy_inplace.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_random_strings_add.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_random_strings_delete.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_random_strings_replace.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_resource_group_increase.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/updated_resource_group_reduce.yaml.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/extra/workload/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6154 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/workload/wordpress_heat_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/extra/workload/wp-instances.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8858 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/ironic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11275 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/keystone-glance-swift.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/magnum.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4030 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/manila.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2875 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/mistral.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/monasca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3362 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/murano.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/neutron-trunk.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2748 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/neutron-with-extensions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18809 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/neutron.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29381 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4102 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/octavia.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/fake_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/rally_profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally-jobs/plugins/test_relative_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/test_relative_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/plugins/test_relative_import/zzz.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/rally_args.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/self-rally.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/senlin.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/simple-job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5798 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/telemetry.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/watcher.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally-jobs/zaqar.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.404201 rally-openstack-2.2.0/rally_openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6151 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/_compat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.408201 rally-openstack-2.2.0/rally_openstack/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.412201 rally-openstack-2.2.0/rally_openstack/common/cfg/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2265 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/cleanup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/glance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5359 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/ironic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/keystone_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/keystone_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/magnum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/manila.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/mistral.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/monasca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/murano.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13981 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/octavia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/osclients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/sahara.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/senlin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4094 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/tempest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/vm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/cfg/watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4852 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/consts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34144 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/osclients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.412201 rally-openstack-2.2.0/rally_openstack/common/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.412201 rally-openstack-2.2.0/rally_openstack/common/services/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/gnocchi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/gnocchi/metric.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.412201 rally-openstack-2.2.0/rally_openstack/common/services/grafana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/grafana/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/grafana/grafana.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.412201 rally-openstack-2.2.0/rally_openstack/common/services/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2953 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/heat/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9650 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/identity/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7013 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13199 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/image/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3370 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/image/glance_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8299 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/image/glance_v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/image/glance_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4656 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/image/image.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/key_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/key_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9892 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/key_manager/barbican.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/loadbalancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/loadbalancer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21306 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/loadbalancer/octavia.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1834 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/network/net_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61438 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/network/neutron.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.416201 rally-openstack-2.2.0/rally_openstack/common/services/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18099 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/block.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29597 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13780 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v1.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16568 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v2.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16799 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27481 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/common/wrappers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/wrappers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14960 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/common/wrappers/network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/environment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/environment/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/environment/platforms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/environment/platforms/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15697 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/environment/platforms/existing.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/task/cleanup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/cleanup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5043 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/cleanup/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11027 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/cleanup/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33577 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/cleanup/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10396 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/api_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/volume_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/volumes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.420201 rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1730 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/user.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/dataplane/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/dataplane/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/dataplane/heat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/designate/zones.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/glance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8862 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/glance/images.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/heat/stacks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13926 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.424201 rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5460 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/ca_certs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3918 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/cluster_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/clusters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/consts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/monasca/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/monasca/metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/murano/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/murano/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2398 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/murano/murano_environments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3039 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/murano/murano_packages.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4511 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/allow_ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/existing_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/networking_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4235 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/network/routers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/neutron/lbaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.428201 rally-openstack-2.2.0/rally_openstack/task/contexts/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4683 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/nova/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2432 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/nova/keypairs.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5508 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/nova/servers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/cinder_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1941 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/designate_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/manila_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/neutron_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/nova_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/quotas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6741 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4902 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5173 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_input_data_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_job_binaries.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_output_data_sources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/senlin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/senlin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2305 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/senlin/profiles.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/swift/objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6033 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/swift/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/vm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8122 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/vm/custom_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/vm/image_command_customizer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/contexts/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/watcher/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4257 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/contexts/watcher/audit_templates.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.432201 rally-openstack-2.2.0/rally_openstack/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/hooks/fault_injection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5520 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenario.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/authenticate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/authenticate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/authenticate/authenticate.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2579 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5606 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5445 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/qos_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2720 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volume_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18732 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volume_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40893 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volumes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4316 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/elasticsearch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/elasticsearch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4961 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/elasticsearch/logging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.436201 rally-openstack-2.2.0/rally_openstack/task/scenarios/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/glance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17414 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/glance/images.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.440201 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3040 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/archive_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/archive_policy_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/metric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1307 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.440201 rally-openstack-2.2.0/rally_openstack/task/scenarios/grafana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/grafana/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6945 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/grafana/metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.440201 rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17046 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/stacks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12868 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.440201 rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/nodes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.440201 rally-openstack-2.2.0/rally_openstack/task/scenarios/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/keystone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18690 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/keystone/basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.444202 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/cluster_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3315 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/k8s_pods.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10533 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.444202 rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23993 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16706 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.444202 rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/executions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4765 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/workbooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.444202 rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1850 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.444202 rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/environments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/packages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10241 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.448202 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16861 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12754 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/loadbalancer_v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/loadbalancer_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38218 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9506 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34380 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.448202 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8558 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/aggregates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11818 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/hypervisors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/keypairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/server_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56253 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49724 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.448202 rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10949 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/loadbalancers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.448202 rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5246 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11670 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8141 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/consts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/jobs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5178 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/node_group_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24625 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5649 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6192 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4889 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8493 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26389 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/vmtasks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/workloads/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/workloads/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/workloads/siege.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.452202 rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4151 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10421 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/rally_openstack/task/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/rally_openstack/task/ui/charts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/ui/charts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5199 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/task/ui/charts/osprofilerchart.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/rally_openstack/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/rally_openstack/verification/tempest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      850 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/config.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10198 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/consts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17054 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9180 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/rally_openstack/verification/tempest/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.408201 rally-openstack-2.2.0/rally_openstack.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    80540 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-10-26 10:57:49.000000 rally-openstack-2.2.0/rally_openstack.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/samples/deployments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing-api.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing-keystone-v3-osprofiler.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing-keystone-v3-user.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing-keystone-v3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing-with-predefined-users.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/deployments/existing.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.456202 rally-openstack-2.2.0/samples/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.472202 rally-openstack-2.2.0/samples/tasks/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/allow-ssh.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/allow-ssh.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/api-versions.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/api-versions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/audit-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/audit-templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1442 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/ca-certs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/ca-certs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/cluster-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/cluster-templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/clusters.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/clusters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/dummy-context.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/dummy-context.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/existing-network.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/existing-network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/flavors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/flavors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/heat-dataplane.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/heat-dataplane.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/image-command-customizer.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/image-command-customizer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/images.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/images.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/keypair.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/keypair.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/lbaas.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/lbaas.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-security-services.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-security-services.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-share-networks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-share-networks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-shares.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/manila-shares.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/monasca-metrics.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/monasca-metrics.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/murano-environments.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/murano-environments.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/murano-packages.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/murano-packages.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/network.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/networking-agents.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/networking-agents.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/profiles.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/profiles.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/quotas.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/quotas.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/roles.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/roles.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/router.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/router.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-cluster.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-input-data-sources.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-input-data-sources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1686 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-job-binaries.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-job-binaries.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-output-data-sources.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/sahara-output-data-sources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/servers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/servers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/stacks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/stacks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/swift-objects.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/swift-objects.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/users.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/users.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/volume-types.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/volume-types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/volumes.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/volumes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/zones.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/contexts/zones.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.472202 rally-openstack-2.2.0/samples/tasks/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.472202 rally-openstack-2.2.0/samples/tasks/runners/constant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/constant/constant-for-duration.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/constant/constant-for-duration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/constant/constant-timeout.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/constant/constant-timeout.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.472202 rally-openstack-2.2.0/samples/tasks/runners/rps/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/rps/rps.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/rps/rps.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.472202 rally-openstack-2.2.0/samples/tasks/runners/serial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/serial/serial.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/runners/serial/serial.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.476202 rally-openstack-2.2.0/samples/tasks/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.476202 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/keystone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/keystone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-cinder.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-cinder.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-glance.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-glance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-heat.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-monasca.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-monasca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-neutron.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-nova.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-octavia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-octavia.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.484202 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-add-container.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-add-container.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-asymmetric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-asymmetric.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-certificate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-certificate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-container.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-container.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-keys.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-keys.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-order-certificate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-order-certificate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-rsa-container.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-rsa-container.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-get-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-get-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-list-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-list-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/get-secret.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/get-secret.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-containers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-containers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-orders.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-orders.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-secrets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/barbican/list-secrets.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.500203 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-attach-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-attach-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-extend-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-extend-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-qos.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-qos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-qos.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-qos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-qos.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-qos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-encryption-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-encryption-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1162 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-and-clone.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      589 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-and-clone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-backup.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-backup.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      643 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      338 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-transfers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-transfers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-types.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-volumes.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-volumes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/modify-volume-metadata.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/cinder/modify-volume-metadata.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.500203 rally-openstack-2.2.0/samples/tasks/scenarios/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-zone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-zone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-recordsets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-recordsets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-zones.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-zones.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/list-recordsets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/list-recordsets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/list-zones.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/designate/list-zones.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.504202 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-exception.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-failure.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-openstack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-openstack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-output.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-random-action.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/dummy/dummy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.504202 rally-openstack-2.2.0/samples/tasks/scenarios/elasticsearch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/elasticsearch/log-instance.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/elasticsearch/log-instance.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.508203 rally-openstack-2.2.0/samples/tasks/scenarios/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-deactivate-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-deactivate-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-delete-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-delete-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-download-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-download-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-get-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-get-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-list-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-list-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-update-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-update-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/list-images.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/glance/list-images.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.512203 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-archive-policy-rule.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-archive-policy-rule.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-archive-policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-archive-policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy-rule.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy-rule.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-metric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-metric.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-resource.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-resource.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-metric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-metric.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-resource-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-resource-type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-resource.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-resource.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/get-status.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/get-status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-archive-policy-rule.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-archive-policy-rule.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-archive-policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-archive-policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-capabilities.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-capabilities.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-metric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-metric.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-resource-type.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-resource-type.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.512203 rally-openstack-2.2.0/samples/tasks/scenarios/grafana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-from-instance.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-from-instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-locally.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-locally.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.520203 rally-openstack-2.2.0/samples/tasks/scenarios/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-list-stack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-list-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-check-delete-stack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-check-delete-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-scale.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-scale.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-event.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-event.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-resources.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-resources.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.524203 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/autoscaling-group.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/autoscaling-policy.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/default.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/random-strings.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group-server-with-volume.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group-with-constraint.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group-with-outputs.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/server-with-ports.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/server-with-volume.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-autoscaling-policy-inplace.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-random-strings-add.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-random-strings-delete.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-random-strings-replace.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-resource-group-increase.yaml.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-resource-group-reduce.yaml.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.524203 rally-openstack-2.2.0/samples/tasks/scenarios/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-delete-node.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-delete-node.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-list-node.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-list-node.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.532203 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/add-and-remove-user-role.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/add-and-remove-user-role.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/authenticate-user-and-validate-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/authenticate-user-and-validate-token.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-add-and-list-user-roles.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-add-and-list-user-roles.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-ec2credential.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-ec2credential.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-role.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-role.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-service.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-user.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-delete-user.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-get-role.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-get-role.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-ec2credentials.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-ec2credentials.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-roles.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-roles.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-services.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-services.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-tenants.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-tenants.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-users.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-users.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-update-user.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-update-user.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-tenant-with-users.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-tenant-with-users.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-tenant.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-tenant.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-update-and-delete-tenant.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-update-and-delete-tenant.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user-update-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user-update-password.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/get-entities.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/keystone/get-entities.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.536203 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.536203 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/artifacts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/artifacts/nginx.yaml.k8s
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/artifacts/rc_nginx.yaml.k8s
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-and-list-clusters.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-and-list-clusters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-pods.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-pods.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-rcs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-rcs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-cluster-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-cluster-templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-clusters.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1580 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-clusters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-pods.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-pods.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.540203 rally-openstack-2.2.0/samples/tasks/scenarios/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-security-service-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-security-service-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-extend.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-extend.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-shrink.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-shrink.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-list.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1660 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/list-share-servers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/list-share-servers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/list-shares.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/manila/list-shares.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.544203 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-workbook.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-workbook.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-params.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-workbook.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-workbook.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/list-executions.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/list-executions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/list-workbooks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/mistral/list-workbooks.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.544203 rally-openstack-2.2.0/samples/tasks/scenarios/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/monasca/list-metrics.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/monasca/list-metrics.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.548203 rally-openstack-2.2.0/samples/tasks/scenarios/murano/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      502 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-delete-environment.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-delete-environment.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-deploy-environment.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-deploy-environment.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-delete-package.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-delete-package.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-filter-applications.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-filter-applications.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-list-packages.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-list-packages.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/list-environments.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/list-environments.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/package-lifecycle.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/murano/package-lifecycle.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.568204 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-with-subports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-with-subports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-bind-ports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-bind-ports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-networks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-networks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-ports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-ports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-routers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-routers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-vips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-vips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-ports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-ports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-subnets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-subnets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-trunks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-trunks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-vips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-vips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-network.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-ports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-ports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-routers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-routers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-subnets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-subnets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-networks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-networks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-ports.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-ports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-routers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-routers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-subnets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-subnets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-vips.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-vips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/delete-subnets.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/delete-subnets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/list-agents.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/list-agents.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.588204 rally-openstack-2.2.0/samples/tasks/scenarios/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-block-migrate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-block-migrate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-url.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-list.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-live-migrate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-live-migrate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-migrate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-migrate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-rebuild.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-rebuild.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-show-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-show-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-update-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-update-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-bounce-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-bounce-delete.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      568 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      895 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      538 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      886 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      529 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      555 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-flavor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-keypair.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-keypair.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-server-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-server-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-flavor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-keypair.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-keypair.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-server-group.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-server-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-aggregates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-aggregates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-flavor-access.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-flavor-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-keypairs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-keypairs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-server-groups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-server-groups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-update-aggregate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-update-aggregate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-agents.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-agents.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-aggregates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-aggregates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-get-hypervisors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-get-hypervisors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-search-hypervisor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-and-search-hypervisor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-availability-zones.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-availability-zones.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-flavors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-flavors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-hypervisors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-hypervisors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-servers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-servers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-services.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-services.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/pause-and-unpause.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/pause-and-unpause.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-shutoff-server.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-shutoff-server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/shelve-and-unshelve.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/shelve-and-unshelve.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/statistics-hypervisors.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/statistics-hypervisors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/suspend-and-resume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/nova/suspend-and-resume.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.592204 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.596204 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-get.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-get.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/neutron-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/neutron-update.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-get.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-get.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.596204 rally-openstack-2.2.0/samples/tasks/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/requests/check-random-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/requests/check-random-request.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/requests/check-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/requests/check-request.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.596204 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.600204 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2359 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/java-action-job.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/java-action-job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2191 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.600204 rally-openstack-2.2.0/samples/tasks/scenarios/senlin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.600204 rally-openstack-2.2.0/samples/tasks/scenarios/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-objects-in-containers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-objects-in-containers.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.604204 rally-openstack-2.2.0/samples/tasks/scenarios/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/dd-load-test.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/vm/dd-load-test.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.604204 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/list-audit-templates.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/watcher/list-audit-templates.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.604204 rally-openstack-2.2.0/samples/tasks/scenarios/workload/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/workload/wordpress.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/workload/wordpress.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.604204 rally-openstack-2.2.0/samples/tasks/scenarios/zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/zaqar/create-queue.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/zaqar/create-queue.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/zaqar/producer-consumer.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/scenarios/zaqar/producer-consumer.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/samples/tasks/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/sla/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/sla/create-and-delete-user.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/sla/create-and-delete-user.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/samples/tasks/support/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/support/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      920 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/support/instance_linpack.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      163 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/samples/tasks/support/instance_test.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2021-10-26 10:57:49.668206 rally-openstack-2.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tasks/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tasks/openstack/macro/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/macro/macro.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tasks/openstack/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/authentication.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/cinder.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/glance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/keystone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10050 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6144 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/scenario/nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/task.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack/task_arguments.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tasks/openstack_metrics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tasks/openstack_metrics/task.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.608204 rally-openstack-2.2.0/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2347 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/cover.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/pages/task-index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/pages/verify-index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/docker-build-and-check.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/docker-build-check-and-push.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/post-rally-task.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/post-rally-verify.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/ci/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.372200 rally-openstack-2.2.0/tests/ci/playbooks/roles/check-task-sla/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/check-task-sla/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/check-task-sla/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.372200 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.372200 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.372200 rally-openstack-2.2.0/tests/ci/playbooks/roles/fetch-rally-task-results/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.372200 rally-openstack-2.2.0/tests/ci/playbooks/roles/import-task-results/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/import-task-results/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/import-task-results/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.612204 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/library/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19105 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/library/osresources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_and_compare_resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/make_env_spec_with_existing_users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/prepare-env-with-existing-users.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/ci/playbooks/roles/process-task-results/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/process-task-results/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/process-task-results/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/ci/playbooks/roles/run-rally-task/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/run-rally-task/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/run-rally-task/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-install/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-install/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-install/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-run/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.616205 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-run/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/roles/tox-run/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/run-rally-task.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/run-rally-verify.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/playbooks/tox-functional-env-run.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4665 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/pytest_launcher.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      526 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/rally_functional_job.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18780 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/rally_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13953 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/ci/sync_requirements.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.620205 rally-openstack-2.2.0/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.376200 rally-openstack-2.2.0/tests/functional/extra/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.620205 rally-openstack-2.2.0/tests/functional/extra/fake_dir/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/extra/fake_dir/fake_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/test_certification_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4980 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/test_cli_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8458 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/test_cli_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/test_cli_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5738 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/test_task_samples.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8500 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.620205 rally-openstack-2.2.0/tests/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/hacking/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21684 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.620205 rally-openstack-2.2.0/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/barbican/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6538 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/barbican/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/gnocchi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9016 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/gnocchi/test_metric.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4467 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/heat/test_main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9411 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/identity/test_identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19738 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23839 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/image/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8186 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9233 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5007 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/image/test_image.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.624205 rally-openstack-2.2.0/tests/unit/common/services/loadbalancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/loadbalancer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/loadbalancer/test_octavia.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/common/services/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/network/test_net_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46806 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/network/test_neutron.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/common/services/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12557 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/test_block.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29047 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16509 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v1.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19421 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v2.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19506 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/test_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48612 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/test_osclients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42038 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/common/wrappers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/wrappers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20310 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/common/wrappers/test_network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/test_docker_readme.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5380 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/test_docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/test_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8648 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/test_jsonschemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7209 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/doc/test_task_samples.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/environment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/environment/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.628205 rally-openstack-2.2.0/tests/unit/environment/platforms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/environment/platforms/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16278 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/environment/platforms/test_existing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55058 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/rally_jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/rally_jobs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/rally_jobs/test_jobs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5719 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/rally_jobs/test_zuul_jobs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/cleanup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/cleanup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/cleanup/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15996 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/cleanup/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45947 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/cleanup/test_resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/contexts/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cinder/test_volume_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cinder/test_volumes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3117 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/test_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/test_user.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/contexts/dataplane/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/dataplane/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4325 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/dataplane/test_heat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.632205 rally-openstack-2.2.0/tests/unit/task/contexts/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6015 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/designate/test_zones.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/glance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10270 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/glance/test_images.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/heat/test_stacks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/keystone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6353 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/keystone/test_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20718 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/keystone/test_users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/magnum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/magnum/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9844 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_ca_certs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4273 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_cluster_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5986 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_clusters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/manila/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6587 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16045 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/monasca/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/monasca/test_metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.636205 rally-openstack-2.2.0/tests/unit/task/contexts/murano/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/murano/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3207 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/murano/test_murano_environments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4233 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/murano/test_murano_packages.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.640205 rally-openstack-2.2.0/tests/unit/task/contexts/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4365 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/test_allow_ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3501 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/test_existing_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/test_networking_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/network/test_routers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.640205 rally-openstack-2.2.0/tests/unit/task/contexts/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7718 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/neutron/test_lbaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.640205 rally-openstack-2.2.0/tests/unit/task/contexts/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_keypairs.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6108 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_servers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.640205 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_cinder_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2074 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_designate_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_manila_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_neutron_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_nova_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11482 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_quotas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5540 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6653 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_input_data_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5578 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_job_binaries.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5821 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_output_data_sources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/contexts/senlin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/senlin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/senlin/test_profiles.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/contexts/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8636 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/swift/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7423 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/swift/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/test_api_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/contexts/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/vm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7068 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/vm/test_custom_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/vm/test_image_command_customizer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/contexts/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/watcher/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3576 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/contexts/watcher/test_audit_templates.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/hooks/test_fault_injection.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/scenarios/authenticate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/authenticate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4574 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/authenticate/test_authenticate.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.644205 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.648205 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_qos_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volume_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13281 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volume_types.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    26519 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volumes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.648205 rally-openstack-2.2.0/tests/unit/task/scenarios/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4946 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/designate/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5797 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/designate/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.648205 rally-openstack-2.2.0/tests/unit/task/scenarios/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/glance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10389 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/glance/test_images.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.648205 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2972 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_archive_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_archive_policy_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_metric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1787 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15225 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/heat/test_stacks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16100 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/heat/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/test_nodes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/keystone/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    15416 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/keystone/test_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4926 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_loadbalancers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_cluster_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5071 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3810 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_k8s_pods.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18192 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.652205 rally-openstack-2.2.0/tests/unit/task/scenarios/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/manila/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23508 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/manila/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17160 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/manila/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.656205 rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7604 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_executions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7045 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_workbooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.656205 rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/test_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.656205 rally-openstack-2.2.0/tests/unit/task/scenarios/murano/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/murano/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6014 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_environments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_packages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9946 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.656205 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9802 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12483 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v1.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2225 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32309 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17331 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6318 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62282 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.660205 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7875 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_aggregates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6241 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_hypervisors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4298 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_keypairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7190 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_server_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51492 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60048 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.660205 rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4493 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.660205 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6303 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8171 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_jobs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3493 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_node_group_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19431 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.660205 rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6622 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/scenarios/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6489 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/swift/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6362 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/swift/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12436 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25424 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/test_vmtasks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/workloads/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/workloads/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/vm/workloads/test_siege.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3892 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6964 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/test_scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19518 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/test_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/task/ui/charts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7626 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/task/ui/charts/test_osprofilerchart.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8400 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test__compat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15398 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_pytest_launcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14784 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_test_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/test_workarounds.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/verification/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:49.664205 rally-openstack-2.2.0/tests/unit/verification/tempest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/verification/tempest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12311 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/verification/tempest/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21028 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/verification/tempest/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10931 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tests/unit/verification/tempest/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3927 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2021-10-26 10:57:09.000000 rally-openstack-2.2.0/upper-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.dockerignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.466343 rally-openstack-2.3.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/docker-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-barbican.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-basic-with-existing-users.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-cinder.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-designate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-ironic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-keystone-glance-swift.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-magnum.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5134 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-manila.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-mistral.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-monasca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-murano.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-neutron-trunk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-neutron-with-extensions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-octavia.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-senlin.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-simple-job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-telemetry.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-watcher.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-task-zaqar.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-tox-functional.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/rally-verify-tempest.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4684 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/.zuul.d/zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13503 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19018 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/CHANGELOG.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    92136 2023-08-03 12:50:26.000000 rally-openstack-2.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2669 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/DOCKER_README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.466343 rally-openstack-2.3.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.466343 rally-openstack-2.3.0/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/devstack/lib/rally
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.466343 rally-openstack-2.3.0/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/etc/motd
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.466343 rally-openstack-2.3.0/etc/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/etc/rally/rally-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30337 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/etc/rally/rally.conf.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.474343 rally-openstack-2.3.0/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/barbican.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/basic-with-existing-users.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/certifcation_task_args.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    28561 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/cinder.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/designate.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/autoscaling_group.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/autoscaling_policy.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/default.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/hook_example_script.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/install_benchmark.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/instance_test.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/mistral_input.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/mistral_params.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/mistral_wb.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.430345 rally-openstack-2.3.0/rally-jobs/extra/murano/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/Classes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/Classes/HelloReporter.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/ui.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/manifest.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34575 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/murano/applications/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/random_strings.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/resource_group.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/resource_group_server_with_volume.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/resource_group_with_constraint.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/resource_group_with_outputs.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/server_with_ports.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/server_with_volume.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_autoscaling_policy_inplace.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_random_strings_add.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_random_strings_delete.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_random_strings_replace.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_resource_group_increase.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/updated_resource_group_reduce.yaml.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/extra/workload/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6154 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/workload/wordpress_heat_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/extra/workload/wp-instances.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8858 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/ironic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11275 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/keystone-glance-swift.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/magnum.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4030 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/manila.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2875 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/mistral.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/monasca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3362 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/murano.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/neutron-trunk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2748 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/neutron-with-extensions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16347 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/neutron.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29769 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4102 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/octavia.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/fake_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/rally_profile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally-jobs/plugins/test_relative_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/test_relative_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/plugins/test_relative_import/zzz.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/rally_args.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/self-rally.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/senlin.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/simple-job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5798 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/telemetry.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/watcher.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally-jobs/zaqar.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.478343 rally-openstack-2.3.0/rally_openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6151 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/_compat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.482343 rally-openstack-2.3.0/rally_openstack/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.486342 rally-openstack-2.3.0/rally_openstack/common/cfg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2265 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/cleanup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/glance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5359 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/ironic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/keystone_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/keystone_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/magnum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/manila.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/mistral.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/monasca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/murano.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13981 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/octavia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/osclients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/sahara.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/senlin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/tempest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/vm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/cfg/watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4852 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34144 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/osclients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.486342 rally-openstack-2.3.0/rally_openstack/common/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.486342 rally-openstack-2.3.0/rally_openstack/common/services/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/gnocchi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/gnocchi/metric.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.486342 rally-openstack-2.3.0/rally_openstack/common/services/grafana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/grafana/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/grafana/grafana.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.486342 rally-openstack-2.3.0/rally_openstack/common/services/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2953 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/heat/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9650 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/identity/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7013 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13199 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/image/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3370 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/image/glance_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8299 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/image/glance_v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/image/glance_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4656 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/image/image.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/key_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/key_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9892 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/key_manager/barbican.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/loadbalancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/loadbalancer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21306 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/loadbalancer/octavia.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1834 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/network/net_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61438 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/network/neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.490342 rally-openstack-2.3.0/rally_openstack/common/services/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19711 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/block.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    31076 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14228 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v1.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16501 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v2.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16708 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27481 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/common/wrappers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/wrappers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14960 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/common/wrappers/network.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/environment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/environment/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/environment/platforms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/environment/platforms/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15697 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/environment/platforms/existing.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/task/cleanup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/cleanup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5043 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/cleanup/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11027 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/cleanup/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33577 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/cleanup/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10396 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/api_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/volume_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/volumes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.494342 rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1730 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/user.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/dataplane/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/dataplane/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/dataplane/heat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/designate/zones.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/glance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8862 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/glance/images.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/heat/stacks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13926 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5460 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/ca_certs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3918 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/cluster_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/clusters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.498342 rally-openstack-2.3.0/rally_openstack/task/contexts/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/monasca/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/monasca/metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.502341 rally-openstack-2.3.0/rally_openstack/task/contexts/murano/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/murano/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2398 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/murano/murano_environments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3039 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/murano/murano_packages.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.502341 rally-openstack-2.3.0/rally_openstack/task/contexts/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/allow_ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/existing_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/networking_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4235 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/network/routers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.502341 rally-openstack-2.3.0/rally_openstack/task/contexts/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/neutron/lbaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.502341 rally-openstack-2.3.0/rally_openstack/task/contexts/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4683 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/nova/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2432 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/nova/keypairs.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5508 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/nova/servers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.502341 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/cinder_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1939 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/designate_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/manila_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/neutron_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/nova_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/quotas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6741 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4902 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5173 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_input_data_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_job_binaries.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_output_data_sources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/contexts/senlin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/senlin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2305 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/senlin/profiles.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/contexts/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/swift/objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6033 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/swift/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/contexts/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/vm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8122 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/vm/custom_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/vm/image_command_customizer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/contexts/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/watcher/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4257 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/contexts/watcher/audit_templates.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/hooks/fault_injection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5520 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenario.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.506341 rally-openstack-2.3.0/rally_openstack/task/scenarios/authenticate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/authenticate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/authenticate/authenticate.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.510341 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5606 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.510341 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5445 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/qos_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2721 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volume_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18603 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volume_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40893 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volumes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.510341 rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4316 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.510341 rally-openstack-2.3.0/rally_openstack/task/scenarios/elasticsearch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/elasticsearch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4961 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/elasticsearch/logging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.510341 rally-openstack-2.3.0/rally_openstack/task/scenarios/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/glance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17414 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/glance/images.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3040 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/archive_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/archive_policy_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/metric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1307 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/grafana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/grafana/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6945 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/grafana/metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17046 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/stacks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12868 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/nodes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/keystone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18690 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/keystone/basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.514341 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/cluster_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3315 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/k8s_pods.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10533 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.518341 rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23998 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16737 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.518341 rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/executions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4765 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/workbooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.518341 rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1850 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.518341 rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/environments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/packages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10241 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.518341 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16861 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12754 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/loadbalancer_v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/loadbalancer_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38218 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9390 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34380 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.522340 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8558 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/aggregates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11818 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/hypervisors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/keypairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/server_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58927 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50063 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.522340 rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10949 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/loadbalancers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.522340 rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5246 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11670 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8141 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/jobs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5178 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/node_group_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24625 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5649 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6192 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4889 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8493 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26382 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/vmtasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/workloads/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/workloads/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/workloads/siege.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4151 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10421 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.526340 rally-openstack-2.3.0/rally_openstack/task/ui/charts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/ui/charts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5199 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/task/ui/charts/osprofilerchart.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.530340 rally-openstack-2.3.0/rally_openstack/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.530340 rally-openstack-2.3.0/rally_openstack/verification/tempest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      850 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/config.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10198 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17054 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9180 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/rally_openstack/verification/tempest/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.482343 rally-openstack-2.3.0/rally_openstack.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    80436 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-08-03 12:50:27.000000 rally-openstack-2.3.0/rally_openstack.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.530340 rally-openstack-2.3.0/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.530340 rally-openstack-2.3.0/samples/deployments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing-api.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing-keystone-v3-osprofiler.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing-keystone-v3-user.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing-keystone-v3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing-with-predefined-users.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/deployments/existing.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.530340 rally-openstack-2.3.0/samples/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/allow-ssh.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/allow-ssh.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/api-versions.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/api-versions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/audit-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/audit-templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1442 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/ca-certs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/ca-certs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/cluster-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/cluster-templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/clusters.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/clusters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/dummy-context.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/dummy-context.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/existing-network.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/existing-network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/flavors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/flavors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/heat-dataplane.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/heat-dataplane.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/image-command-customizer.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/image-command-customizer.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/images.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/images.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/keypair.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/keypair.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/lbaas.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/lbaas.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-security-services.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-security-services.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-share-networks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-share-networks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-shares.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/manila-shares.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/monasca-metrics.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/monasca-metrics.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/murano-environments.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/murano-environments.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/murano-packages.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/murano-packages.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/network.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/networking-agents.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/networking-agents.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/profiles.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/profiles.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/quotas.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/quotas.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/roles.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/roles.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/router.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/router.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-cluster.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-input-data-sources.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-input-data-sources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1686 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-job-binaries.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-job-binaries.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-output-data-sources.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/sahara-output-data-sources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/servers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/servers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/stacks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/stacks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/swift-objects.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/swift-objects.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/users.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/users.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/volume-types.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/volume-types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/volumes.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/volumes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/zones.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/contexts/zones.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/runners/constant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/constant/constant-for-duration.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/constant/constant-for-duration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/constant/constant-timeout.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/constant/constant-timeout.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/runners/rps/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/rps/rps.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/rps/rps.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/runners/serial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/serial/serial.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/runners/serial/serial.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.546339 rally-openstack-2.3.0/samples/tasks/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.550339 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/keystone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/keystone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-cinder.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-cinder.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-glance.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-glance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-heat.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-monasca.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-monasca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-neutron.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-nova.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-octavia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-octavia.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.558338 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-add-container.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-add-container.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-asymmetric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-asymmetric.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-certificate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-certificate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-container.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-container.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-keys.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-keys.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-order-certificate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-order-certificate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-rsa-container.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-rsa-container.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-get-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-get-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-list-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-list-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/get-secret.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/get-secret.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-containers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-containers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-orders.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-orders.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-secrets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/barbican/list-secrets.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.570338 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-attach-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-attach-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-extend-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-extend-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-qos.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-qos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-qos.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-qos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-qos.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-qos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-encryption-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-encryption-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1162 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-and-clone.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      589 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-and-clone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-backup.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-backup.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      643 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      338 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-transfers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-transfers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-types.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-volumes.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-volumes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/modify-volume-metadata.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/cinder/modify-volume-metadata.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.574338 rally-openstack-2.3.0/samples/tasks/scenarios/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-zone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-zone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-recordsets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-recordsets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-zones.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-zones.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/list-recordsets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/list-recordsets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/list-zones.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/designate/list-zones.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.578337 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-exception.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-failure.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-openstack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-openstack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-output.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-output.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-random-action.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/dummy/dummy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.578337 rally-openstack-2.3.0/samples/tasks/scenarios/elasticsearch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/elasticsearch/log-instance.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/elasticsearch/log-instance.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.578337 rally-openstack-2.3.0/samples/tasks/scenarios/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-deactivate-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-deactivate-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-delete-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-delete-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-download-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-download-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-get-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-get-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-list-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-list-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-update-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-update-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/list-images.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/glance/list-images.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.586337 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-archive-policy-rule.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-archive-policy-rule.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-archive-policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-archive-policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy-rule.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy-rule.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-metric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-metric.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-resource.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-resource.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-metric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-metric.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-resource-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-resource-type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-resource.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-resource.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/get-status.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/get-status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-archive-policy-rule.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-archive-policy-rule.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-archive-policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-archive-policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-capabilities.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-capabilities.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-metric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-metric.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-resource-type.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-resource-type.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.586337 rally-openstack-2.3.0/samples/tasks/scenarios/grafana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-from-instance.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-from-instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-locally.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-locally.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.594336 rally-openstack-2.3.0/samples/tasks/scenarios/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-list-stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-list-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-check-delete-stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-check-delete-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-scale.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-scale.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-event.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-event.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-resources.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-resources.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.598336 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/autoscaling-group.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/autoscaling-policy.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/default.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/random-strings.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group-server-with-volume.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group-with-constraint.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group-with-outputs.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/server-with-ports.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/server-with-volume.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-autoscaling-policy-inplace.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-random-strings-add.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-random-strings-delete.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-random-strings-replace.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-resource-group-increase.yaml.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-resource-group-reduce.yaml.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.598336 rally-openstack-2.3.0/samples/tasks/scenarios/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-delete-node.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-delete-node.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-list-node.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-list-node.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.606336 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/add-and-remove-user-role.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/add-and-remove-user-role.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/authenticate-user-and-validate-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/authenticate-user-and-validate-token.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-add-and-list-user-roles.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-add-and-list-user-roles.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-ec2credential.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-ec2credential.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-role.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-role.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-service.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-user.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-delete-user.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-get-role.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-get-role.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-ec2credentials.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-ec2credentials.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-roles.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-roles.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-services.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-services.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-tenants.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-tenants.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-users.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-users.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-update-user.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-update-user.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-tenant-with-users.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-tenant-with-users.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-tenant.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-tenant.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-update-and-delete-tenant.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-update-and-delete-tenant.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user-update-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user-update-password.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/get-entities.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/keystone/get-entities.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.606336 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.606336 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/artifacts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/artifacts/nginx.yaml.k8s
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/artifacts/rc_nginx.yaml.k8s
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-and-list-clusters.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-and-list-clusters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-pods.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-pods.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-rcs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-rcs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-cluster-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-cluster-templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-clusters.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1580 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-clusters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-pods.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-pods.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.614335 rally-openstack-2.3.0/samples/tasks/scenarios/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-security-service-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-security-service-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-extend.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-extend.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-shrink.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-shrink.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-list.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1660 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/list-share-servers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/list-share-servers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/list-shares.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/manila/list-shares.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.618335 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-workbook.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-workbook.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-params.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-workbook.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-workbook.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/list-executions.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/list-executions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/list-workbooks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/mistral/list-workbooks.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.618335 rally-openstack-2.3.0/samples/tasks/scenarios/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/monasca/list-metrics.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/monasca/list-metrics.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.622335 rally-openstack-2.3.0/samples/tasks/scenarios/murano/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      502 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-delete-environment.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-delete-environment.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-deploy-environment.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-deploy-environment.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-delete-package.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-delete-package.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-filter-applications.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-filter-applications.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-list-packages.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-list-packages.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/list-environments.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/list-environments.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/package-lifecycle.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/murano/package-lifecycle.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.638334 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-with-subports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-with-subports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-bind-ports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-bind-ports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-networks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-networks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-ports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-ports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-routers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-routers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-vips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-vips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-ports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-ports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-subnets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-subnets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-trunks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-trunks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-vips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-vips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-network.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-ports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-ports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-routers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-routers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-subnets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-subnets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-networks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-networks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-ports.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-ports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-routers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-routers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-subnets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-subnets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-vips.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-vips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/delete-subnets.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/delete-subnets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/list-agents.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/list-agents.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.662333 rally-openstack-2.3.0/samples/tasks/scenarios/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-block-migrate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-block-migrate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-url.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-list.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-live-migrate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-live-migrate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-migrate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-migrate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-rebuild.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-rebuild.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-show-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-show-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-update-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-update-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-bounce-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-bounce-delete.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      568 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      895 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      538 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      886 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      529 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-extend.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-extend.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      555 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-flavor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-keypair.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-keypair.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-server-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-server-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-flavor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-keypair.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-keypair.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-server-group.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-server-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-aggregates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-aggregates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-flavor-access.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-flavor-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-keypairs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-keypairs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-server-groups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-server-groups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-update-aggregate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-update-aggregate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-aggregates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-aggregates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-get-hypervisors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-get-hypervisors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-search-hypervisor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-and-search-hypervisor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-availability-zones.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-availability-zones.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-flavors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-flavors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-hypervisors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-hypervisors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-servers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-servers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-services.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-services.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/pause-and-unpause.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/pause-and-unpause.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-shutoff-server.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-shutoff-server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/shelve-and-unshelve.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/shelve-and-unshelve.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/statistics-hypervisors.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/statistics-hypervisors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/suspend-and-resume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/nova/suspend-and-resume.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.666333 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.666333 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-get.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-get.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/neutron-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/neutron-update.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-get.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-get.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.670332 rally-openstack-2.3.0/samples/tasks/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-random-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-random-request.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-request.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.670332 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.670332 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2359 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/java-action-job.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/java-action-job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2191 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.670332 rally-openstack-2.3.0/samples/tasks/scenarios/senlin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.674332 rally-openstack-2.3.0/samples/tasks/scenarios/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-objects-in-containers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-objects-in-containers.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.674332 rally-openstack-2.3.0/samples/tasks/scenarios/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/dd-load-test.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/vm/dd-load-test.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/list-audit-templates.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/watcher/list-audit-templates.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/samples/tasks/scenarios/workload/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/workload/wordpress.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/workload/wordpress.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/samples/tasks/scenarios/zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/zaqar/create-queue.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/zaqar/create-queue.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/zaqar/producer-consumer.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/scenarios/zaqar/producer-consumer.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/samples/tasks/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/sla/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/sla/create-and-delete-user.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/sla/create-and-delete-user.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/samples/tasks/support/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/support/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      920 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/support/instance_linpack.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      163 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/samples/tasks/support/instance_test.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.678332 rally-openstack-2.3.0/tasks/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tasks/openstack/macro/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/macro/macro.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tasks/openstack/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/authentication.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/cinder.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/glance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/keystone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10050 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6144 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/scenario/nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/task.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack/task_arguments.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tasks/openstack_metrics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tasks/openstack_metrics/task.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tests/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2347 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/cover.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.682332 rally-openstack-2.3.0/tests/ci/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/pages/task-index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/pages/verify-index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/docker-build-and-check.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/docker-build-check-and-push.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/post-rally-task.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/post-rally-verify.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.450344 rally-openstack-2.3.0/tests/ci/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.446344 rally-openstack-2.3.0/tests/ci/playbooks/roles/check-task-sla/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/check-task-sla/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/check-task-sla/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.446344 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.446344 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.446344 rally-openstack-2.3.0/tests/ci/playbooks/roles/fetch-rally-task-results/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.446344 rally-openstack-2.3.0/tests/ci/playbooks/roles/import-task-results/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/import-task-results/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/import-task-results/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/library/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18152 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/library/osresources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_and_compare_resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.686332 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/make_env_spec_with_existing_users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/prepare-env-with-existing-users.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.450344 rally-openstack-2.3.0/tests/ci/playbooks/roles/process-task-results/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/ci/playbooks/roles/process-task-results/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/process-task-results/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.450344 rally-openstack-2.3.0/tests/ci/playbooks/roles/run-rally-task/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/ci/playbooks/roles/run-rally-task/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/run-rally-task/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.450344 rally-openstack-2.3.0/tests/ci/playbooks/roles/tox-run/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/ci/playbooks/roles/tox-run/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/roles/tox-run/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/run-rally-task.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/run-rally-verify.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/playbooks/tox-functional-env-run.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4665 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/pytest_launcher.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      526 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/rally_functional_job.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17894 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/rally_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13972 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/ci/sync_requirements.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.450344 rally-openstack-2.3.0/tests/functional/extra/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/functional/extra/fake_dir/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/extra/fake_dir/fake_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/test_certification_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/test_cli_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8458 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/test_cli_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/test_cli_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5738 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/test_task_samples.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8490 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.690331 rally-openstack-2.3.0/tests/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20148 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/common/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/common/services/barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/barbican/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6538 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/barbican/test_secrets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/common/services/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/gnocchi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9016 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/gnocchi/test_metric.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.694331 rally-openstack-2.3.0/tests/unit/common/services/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4467 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/heat/test_main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/services/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9411 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/identity/test_identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19738 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23839 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/services/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/image/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8186 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9233 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5007 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/image/test_image.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/services/loadbalancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/loadbalancer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/loadbalancer/test_octavia.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/services/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/network/test_net_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46806 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/network/test_neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/services/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12557 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/test_block.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    30087 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16934 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v1.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19363 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v2.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19441 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/test_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48612 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/test_osclients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42038 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.698331 rally-openstack-2.3.0/tests/unit/common/wrappers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/wrappers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20310 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/common/wrappers/test_network.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/test_docker_readme.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5380 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/test_docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/test_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8648 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/test_jsonschemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7209 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/doc/test_task_samples.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/environment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/environment/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/environment/platforms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/environment/platforms/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16278 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/environment/platforms/test_existing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55056 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/rally_jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/rally_jobs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/rally_jobs/test_jobs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6159 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/rally_jobs/test_zuul_jobs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.702331 rally-openstack-2.3.0/tests/unit/task/cleanup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/cleanup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/cleanup/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15996 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/cleanup/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45947 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/cleanup/test_resources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cinder/test_volume_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cinder/test_volumes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3117 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/test_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/test_user.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/dataplane/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/dataplane/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4325 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/dataplane/test_heat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6015 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/designate/test_zones.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/glance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10270 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/glance/test_images.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/heat/test_stacks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/keystone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6353 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/keystone/test_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20718 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/keystone/test_users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.706330 rally-openstack-2.3.0/tests/unit/task/contexts/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/magnum/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9844 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_ca_certs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4273 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_cluster_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5986 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_clusters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/manila/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6587 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16045 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/monasca/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/monasca/test_metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/murano/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/murano/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3207 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/murano/test_murano_environments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4233 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/murano/test_murano_packages.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4365 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/test_allow_ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3501 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/test_existing_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/test_networking_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/network/test_routers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7718 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/neutron/test_lbaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.710330 rally-openstack-2.3.0/tests/unit/task/contexts/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_keypairs.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6108 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_servers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_cinder_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_designate_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_manila_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_neutron_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_nova_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11482 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_quotas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5540 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6653 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_input_data_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5578 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_job_binaries.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5821 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_output_data_sources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/senlin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/senlin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/senlin/test_profiles.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8636 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/swift/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7423 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/swift/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/test_api_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/vm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7068 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/vm/test_custom_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/vm/test_image_command_customizer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.714330 rally-openstack-2.3.0/tests/unit/task/contexts/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/watcher/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3576 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/contexts/watcher/test_audit_templates.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/hooks/test_fault_injection.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/authenticate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/authenticate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4574 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/authenticate/test_authenticate.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_qos_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volume_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12988 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volume_types.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    26519 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volumes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4946 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/designate/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5797 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/designate/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.718330 rally-openstack-2.3.0/tests/unit/task/scenarios/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/glance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10389 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/glance/test_images.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.722329 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2972 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_archive_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_archive_policy_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_metric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1787 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.722329 rally-openstack-2.3.0/tests/unit/task/scenarios/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15225 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/heat/test_stacks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16100 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/heat/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.722329 rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/test_nodes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.722329 rally-openstack-2.3.0/tests/unit/task/scenarios/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/keystone/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    15416 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/keystone/test_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.722329 rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4926 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_loadbalancers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.726329 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_cluster_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5071 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3810 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_k8s_pods.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18192 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.726329 rally-openstack-2.3.0/tests/unit/task/scenarios/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/manila/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23508 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/manila/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17209 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/manila/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.726329 rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7604 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_executions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7045 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_workbooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.726329 rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/test_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.730329 rally-openstack-2.3.0/tests/unit/task/scenarios/murano/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/murano/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6014 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_environments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_packages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9946 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.730329 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9802 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12483 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v1.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2225 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32309 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17331 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6126 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62282 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7875 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_aggregates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6241 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_hypervisors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4298 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_keypairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7190 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_server_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53460 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60487 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4493 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6303 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8171 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_jobs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3493 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_node_group_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19431 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6622 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6489 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/swift/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6362 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/swift/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12436 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25424 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/test_vmtasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.734329 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/workloads/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/workloads/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/vm/workloads/test_siege.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3892 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6964 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/test_scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19518 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/test_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/task/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/task/ui/charts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7626 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/task/ui/charts/test_osprofilerchart.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8400 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test__compat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14649 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_pytest_launcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14784 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_test_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/test_workarounds.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/verification/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:27.738329 rally-openstack-2.3.0/tests/unit/verification/tempest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/verification/tempest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12311 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/verification/tempest/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21028 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/verification/tempest/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10931 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tests/unit/verification/tempest/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5290 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6861 2023-08-03 12:49:59.000000 rally-openstack-2.3.0/upper-constraints.txt
```

### Comparing `rally-openstack-2.2.0/.zuul.d/README.rst` & `rally-openstack-2.3.0/.zuul.d/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/.zuul.d/base.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-tox-functional.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 - job:
-    name: rally-task-at-devstack
+    name: rally-dsvm-tox-functional
     parent: devstack
-    description: Base job for launching Rally task at Devstack
+    description:
+      Run functional test for rally-openstack project.
+      Uses tox with the ``functional`` environment.
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally-openstack
       # NOTE(andreykurilin): it is a required project to fetch the latest
       #   version and test master of rally-openstack with master of rally
       - name: openstack/rally
     timeout: 7200
     roles:
       - zuul: openstack/devstack
     vars:
+      devstack_localrc:
+        # TODO(frickler): drop this once python-keystoneclient no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-    run: tests/ci/playbooks/run-rally-task.yaml
-    post-run: tests/ci/playbooks/post-rally-task.yaml
+      tox_env: "functional"
+    run: tests/ci/playbooks/tox-functional-env-run.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/docker-jobs.yaml` & `rally-openstack-2.3.0/.zuul.d/docker-jobs.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-barbican.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-heat.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 - job:
-    name: rally-task-barbican
+    name: rally-task-heat
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
-      - name: openstack/barbican
-      - name: openstack/python-barbicanclient
+      - name: openstack/heat
     vars:
+      devstack_localrc:
+        # TODO(frickler): drop this once heat no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-        barbican: https://opendev.org/openstack/barbican
+        heat: https://opendev.org/openstack/heat
       devstack_services:
-        barbican: true
         # disable redundant services for the job
         ceilometer-acentral: false
         ceilometer-acompute: false
         ceilometer-alarm-evaluator: false
         ceilometer-alarm-notifier: false
         ceilometer-anotification: false
         ceilometer-api: false
         ceilometer-collector: false
         horizon: false
         tempest: false
-      rally_task: rally-jobs/barbican.yaml
+      rally_task: rally-jobs/heat.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-designate.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-designate.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,14 @@
       - openstack/designate
       - openstack/designate-dashboard
       - openstack/python-designateclient
     vars:
       rally_task: rally-jobs/designate.yaml
       devstack_localrc:
         DESIGNATE_SERVICE_PORT_DNS: 5322
-        USE_PYTHON3: true
       devstack_plugins:
         designate: https://opendev.org/openstack/designate
         rally-openstack: https://opendev.org/openstack/rally-openstack
       devstack_services:
         designate: true
         s-account: false
         s-container: false
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-heat.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-watcher.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 - job:
-    name: rally-task-heat
+    name: rally-task-watcher
     parent: rally-task-at-devstack
     required-projects:
-      - name: openstack/devstack
-      - name: openstack/devstack-gate
-      - name: openstack/rally
-      - name: openstack/rally-openstack
-      - name: openstack/heat
+      - openstack/ceilometer
+      - openstack/python-openstackclient
+      - openstack/python-watcherclient
+      - openstack/watcher
+      - openstack/watcher-tempest-plugin
+      - openstack/tempest
+      - openstack/rally
+      - openstack/rally-openstack
     vars:
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-        heat: https://opendev.org/openstack/heat
+        watcher: https://opendev.org/openstack/watcher
       devstack_services:
-        # disable redundant services for the job
-        ceilometer-acentral: false
-        ceilometer-acompute: false
-        ceilometer-alarm-evaluator: false
-        ceilometer-alarm-notifier: false
-        ceilometer-anotification: false
-        ceilometer-api: false
-        ceilometer-collector: false
-        horizon: false
-        tempest: false
-      rally_task: rally-jobs/heat.yaml
+        watcher-api: true
+        watcher-decision-engine: true
+        watcher-applier: true
+        s-account: false
+        s-container: false
+        s-object: false
+        s-proxy: false
+      rally_task: rally-jobs/watcher.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-ironic.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-ironic.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 -  job:
     name: rally-task-ironic
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
       - name: openstack/ironic
     vars:
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
         ironic: https://opendev.org/openstack/ironic
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-magnum.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-telemetry.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 - job:
-    name: rally-task-magnum
+    name: rally-task-telemetry
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
-      - name: openstack/magnum
-      - name: openstack/python-magnumclient
       - name: openstack/heat
+      - name: openstack/ceilometer
     vars:
+      devstack_localrc:
+        CEILOMETER_BACKEND: gnocchi
+        # TODO(frickler): drop this once heat no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-        magnum: https://opendev.org/openstack/magnum
-        heat: https://opendev.org/openstack/heat
+        ceilometer: https://opendev.org/openstack/ceilometer
       devstack_services:
-        magnum: true
-        # disable redundant services for the job
-        ceilometer-acentral: false
-        ceilometer-acompute: false
-        ceilometer-alarm-evaluator: false
-        ceilometer-alarm-notifier: false
-        ceilometer-anotification: false
-        ceilometer-api: false
-        ceilometer-collector: false
-        horizon: false
-        tempest: false
-      rally_task: rally-jobs/magnum.yaml
+        ceilometer-acentral: true
+        ceilometer-acompute: true
+        ceilometer-alarm-evaluator: true
+        ceilometer-alarm-notifier: true
+        ceilometer-anotification: true
+        ceilometer-api: true
+        ceilometer-collector: true
+      rally_task: rally-jobs/telemetry.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-manila.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-manila.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 - job:
     name: rally-task-manila
     parent: rally-task-at-devstack
     vars:
       rally_task: rally-jobs/manila.yaml
+      devstack_localrc:
+        # TODO(frickler): drop this once heat no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_services:
         # disable redundant services for the job
         ceilometer-acentral: false
         ceilometer-acompute: false
         ceilometer-alarm-evaluator: false
         ceilometer-alarm-notifier: false
         ceilometer-anotification: false
@@ -23,15 +26,14 @@
 
 - job:
     name: rally-task-manila-no-ss
     parent: rally-task-manila
     vars:
       rally_task: rally-jobs/manila-no-ss.yaml
       devstack_localrc:
-        USE_PYTHON3: true
         LIBS_FROM_GIT: python-manilaclient
         SHARE_DRIVER: manila.tests.share.drivers.dummy.DummyDriver
         MANILA_ENABLED_BACKENDS: alpha,beta,gamma
         MANILA_USE_UWSGI: false
         MANILA_USE_MOD_WSGI: false
         SUPPRESS_ERRORS_IN_CLEANUP: false
         MANILA_SERVICE_IMAGE_ENABLED: false
@@ -55,15 +57,14 @@
 
 - job:
     name: rally-task-manila-ss
     parent: rally-task-manila
     vars:
       rally_task: rally-jobs/manila.yaml
       devstack_localrc:
-        USE_PYTHON3: true
         LIBS_FROM_GIT: python-manilaclient
         SHARE_DRIVER: manila.tests.share.drivers.dummy.DummyDriver
         MANILA_ENABLED_BACKENDS: alpha,beta,gamma
         MANILA_USE_UWSGI: false
         MANILA_USE_MOD_WSGI: false
         SUPPRESS_ERRORS_IN_CLEANUP: false
         MANILA_SERVICE_IMAGE_ENABLED: false
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-mistral.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-barbican.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 - job:
-    name: rally-task-mistral
+    name: rally-task-barbican
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
-      - name: openstack/heat
-      - name: openstack/mistral
-      - name: openstack/python-mistralclient
+      - name: openstack/barbican
+      - name: openstack/python-barbicanclient
     vars:
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-        mistral: https://opendev.org/openstack/mistral
+        barbican: https://opendev.org/openstack/barbican
       devstack_services:
-        mistral: true
+        barbican: true
         # disable redundant services for the job
         ceilometer-acentral: false
         ceilometer-acompute: false
         ceilometer-alarm-evaluator: false
         ceilometer-alarm-notifier: false
         ceilometer-anotification: false
         ceilometer-api: false
         ceilometer-collector: false
         horizon: false
         tempest: false
-      rally_task: rally-jobs/mistral.yaml
+      rally_task: rally-jobs/barbican.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-murano.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-murano.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 - job:
     name: rally-task-murano
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
       - name: openstack/heat
       - name: openstack/murano
     vars:
+      devstack_localrc:
+        # TODO(frickler): drop this once heat no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
         murano: https://opendev.org/openstack/murano
         heat: https://opendev.org/openstack/heat
       devstack_services:
         murano: true
         # disable redundant services for the job
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-neutron-with-extensions.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-neutron-with-extensions.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 - job:
     name: rally-task-neutron-with-extensions
     parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally
       - name: openstack/rally-openstack
       - name: openstack/networking-bgpvpn
       # NOTE(andreykurilin): this neutron plugin uses an old naming of
       #   devstack neutron services. The wrong check triggers call of
       #   an old (legacy) neutron devstack plugin and turns off all neutron
       #   services except q-svc
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-neutron.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-neutron.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - job:
     name: rally-task-neutron
     parent: rally-task-at-devstack
     vars:
       rally_task: rally-jobs/neutron.yaml
       devstack_localrc:
         Q_ML2_TENANT_NETWORK_TYPE: vxlan
-        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch,linuxbridge
+        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch
         Q_AGENT: openvswitch
       devstack_services:
         neutron-trunk: true
         # Cinder services
         c-api: true
         c-bak: true
         c-sch: true
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-task-octavia.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-octavia.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 - job:
     name: rally-task-octavia
     description: A Rally job for checking Octavia Plugin
     parent: rally-task-at-devstack
     required-projects:
-      - name: openstack/devstack-gate
       - name: openstack/diskimage-builder
       - name: openstack/octavia
       - name: openstack/octavia-lib
       - name: openstack/python-octaviaclient
       - name: openstack/barbican
       - name: openstack/python-barbicanclient
     vars:
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-tox-functional.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-task-magnum.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 - job:
-    name: rally-dsvm-tox-functional
-    parent: devstack
-    description:
-      Run functional test for rally-openstack project.
-      Uses tox with the ``functional`` environment.
+    name: rally-task-magnum
+    parent: rally-task-at-devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
-      - name: openstack/rally-openstack
-      # NOTE(andreykurilin): it is a required project to fetch the latest
-      #   version and test master of rally-openstack with master of rally
       - name: openstack/rally
-    timeout: 7200
-    roles:
-      - zuul: openstack/devstack
+      - name: openstack/rally-openstack
+      - name: openstack/magnum
+      - name: openstack/python-magnumclient
+      - name: openstack/heat
     vars:
+      devstack_localrc:
+        # TODO(frickler): drop this once heat no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
-      devstack_localrc:
-        USE_PYTHON3: true
-      tox_env: "functional"
-    run: tests/ci/playbooks/tox-functional-env-run.yaml
+        magnum: https://opendev.org/openstack/magnum
+        heat: https://opendev.org/openstack/heat
+      devstack_services:
+        magnum: true
+        # disable redundant services for the job
+        ceilometer-acentral: false
+        ceilometer-acompute: false
+        ceilometer-alarm-evaluator: false
+        ceilometer-alarm-notifier: false
+        ceilometer-anotification: false
+        ceilometer-api: false
+        ceilometer-collector: false
+        horizon: false
+        tempest: false
+      rally_task: rally-jobs/magnum.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/rally-verify-tempest.yaml` & `rally-openstack-2.3.0/.zuul.d/rally-verify-tempest.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 - job:
     name: rally-verify-tempest
     parent: devstack
     required-projects:
       - name: openstack/devstack
-      - name: openstack/devstack-gate
       - name: openstack/rally-openstack
       - name: openstack/rally
     timeout: 7200
     roles:
       - zuul: openstack/devstack
     vars:
       devstack_localrc:
-        USE_PYTHON3: true
+        # TODO(frickler): drop this once python-keystoneclient no longer needs it
+        KEYSTONE_ADMIN_ENDPOINT: true
       devstack_plugins:
         rally-openstack: https://opendev.org/openstack/rally-openstack
     run: tests/ci/playbooks/run-rally-verify.yaml
     post-run: tests/ci/playbooks/post-rally-verify.yaml
```

### Comparing `rally-openstack-2.2.0/.zuul.d/zuul.yaml` & `rally-openstack-2.3.0/.zuul.d/zuul.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,30 @@
     check:
       jobs:
         - rally-tox-cover
         - rally-tox-pep8
         - rally-tox-py36
         - rally-tox-py37
         - rally-tox-py38
+        - rally-tox-py39
+        - rally-tox-py310
         - rally-dsvm-tox-functional
         - rally-openstack-docker-build
         - rally-task-basic-with-existing-users
         - rally-task-simple-job
         - rally-task-barbican:
             files:
               - .zuul.d/zuul.yaml
               - rally-jobs/barbican.yaml
               - rally_openstack/common/osclients.py
               - rally_openstack/common/services/key_manager
               - rally_openstack/task/cleanup/resources.py
               - rally_openstack/task/scenarios/barbican
               - tests/ci/playbooks
-        - rally-task-cinder:
-            voting: false
+        - rally-task-cinder
         - rally-task-designate:
             files:
               - .zuul.d/zuul.yaml
               - rally-jobs/designate.yaml
               - rally_openstack/common/osclients.py
               - rally_openstack/task/cleanup/resources.py
               - rally_openstack/task/contexts/designate
@@ -74,36 +75,40 @@
         #- rally-task-octavia:
         #    voting: false
         - rally-task-telemetry:
             voting: false
         - rally-task-watcher:
             # watcher-api did not start last time
             voting: false
-        - rally-task-zaqar
+        - rally-task-zaqar:
+            voting: false
         - rally-verify-tempest
     gate:
       jobs:
         - rally-tox-cover
         - rally-tox-pep8
         - rally-tox-py36
         - rally-tox-py37
         - rally-tox-py38
+        - rally-tox-py39
+        - rally-tox-py310
         - rally-dsvm-tox-functional
         - rally-openstack-docker-build
-        - rally-task-basic-with-existing-users
+        #- rally-task-basic-with-existing-users
         - rally-task-simple-job
         - rally-task-barbican:
             files:
               - .zuul.d/zuul.yaml
               - rally-jobs/barbican.yaml
               - rally_openstack/common/osclients.py
               - rally_openstack/common/services/key_manager
               - rally_openstack/task/cleanup/resources.py
               - rally_openstack/task/scenarios/barbican
               - tests/ci/playbooks
+        - rally-task-cinder
         #- rally-task-heat
         - rally-task-ironic
         - rally-task-keystone-glance-swift
         - rally-task-mistral
         - rally-task-neutron
         - rally-task-neutron-trunk:
             files:
@@ -111,15 +116,14 @@
               - rally_openstack/common/osclients.py
               - rally_openstack/common/services/network
               - rally_openstack/task/cleanup/resources.py
               - rally_openstack/task/contexts/network
               - rally_openstack/task/scenarios/neutron/trunk.py
               - rally_openstack/task/scenarios/neutron/network.py
               - tests/ci/playbooks
-        - rally-task-zaqar
         - rally-verify-tempest
     post:
       jobs:
         - rally-openstack-docker-build-and-push:
             vars:
               docker_image_version: latest
     release:
```

### Comparing `rally-openstack-2.2.0/AUTHORS` & `rally-openstack-2.3.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 Anthony Washington <anthony.washington@intel.com>
 Anton Arefiev <aarefiev@mirantis.com>
 Anton Kremenetsky <akremenetsky@dev.rtsoft.ru>
 Anton Staroverov <astaroverov@mirantis.com>
 Anton Studenov <astudenov@mirantis.com>
 Antonio Messina <antonio.s.messina@gmail.com>
 Arata Notsu <notsu@virtualtech.jp>
+Arkady Shtempler <arkadysh@gmail.com>
+Arnaud Morin <arnaud.morin@ovhcloud.com>
 Arx Cruz <acruz@redhat.com>
+Asma Syed Hameed <asyedham@redhat.com>
 Aswad Rangnekar <aswad@wanclouds.net>
 Atsushi SAKAI <sakaia@jp.fujitsu.com>
 Bence Romsics <bence.romsics@ericsson.com>
 Bence Romsics <bence.romsics@gmail.com>
 Bertrand Lallau <bertrand.lallau@gmail.com>
 Bo Chi <chibo.michael@foxmail.com>
 Bo Chi <shcbo@cn.ibm.com>
@@ -58,26 +61,28 @@
 Christian Berendt <berendt@b1-systems.de>
 Christopher Brown <snecklifter@gmail.com>
 Chuck Short <chucks@redhat.com>
 Ciprian Barbu <ciprian.barbu@gmail.com>
 Cyril Roelandt <cyril.roelandt@enovance.com>
 Cédric Ollivier <ollivier.cedric@gmail.com>
 Cédric Savignan <cedric.savignan@orange.com>
+Damian Dabrowski <damian.dabrowski@cleura.com>
 Daniel Gonzalez <daniel@gonzalez-nothnagel.de>
 Dao Cong Tien <tiendc@vn.fujitsu.com>
 Darla Ahlert <da741q@att.com>
 Davanum Srinivas <davanum@gmail.com>
 Dave Spano <dspano@spano.us>
 DeepaJon <deepak.os31@yahoo.com>
 Dina Belova <dbelova@mirantis.com>
 Dmitrii Shcherbakov <dmitrii.shcherbakov@canonical.com>
 Dmitriy Uvarenkov <duvarenkov@mirantis.com>
 Dmitry Ratushnyy <dratushn@cisco.com>
 Doug Hellmann <doug.hellmann@dreamhost.com>
 Doug Hellmann <doug@doughellmann.com>
+Dr. Jens Harbott <harbott@osism.tech>
 Edgar Magana <emagana@gmail.com>
 Endre Karlson <endre.karlson@hp.com>
 Evgeny Ivanov <eivanov@mirantis.com>
 Evgeny Sikachev <esikachev@mirantis.com>
 Fei Long Wang <flwang@catalyst.net.nz>
 Filip Hubik <fhubik@redhat.com>
 Flavio Percoco <flaper87@gmail.com>
@@ -149,14 +154,15 @@
 Marie-Donnie <marie.delavergne@inria.fr>
 Mathieu Velten <mathieu.velten@cern.ch>
 Michal Gershenzon <michal.gershenzon@nokia.com>
 Michal Rostecki <michal.rostecki@allegrogroup.com>
 Mike Durnosvistov <mdurnosvistov@mirantis.com>
 Mikhail Dubov <mdubov@mirantis.com>
 Mikhail Lelyakin <mlelyakin@mirantis.com>
+Mitya_Eremeev <mitossvyaz@mail.ru>
 Mohammad Banikazemi <mb@us.ibm.com>
 Monty Taylor <mordred@inaugust.com>
 Mykhailo Dovgal <mdovgal@mirantis.com>
 Neependra Khare <nkhare@redhat.com>
 Ngo Quoc Cuong <cuongnq@vn.fujitsu.com>
 Nguyen Hung Phuong <phuongnh@vn.fujitsu.com>
 Nikita Konovalov <nkonovalov@mirantis.com>
@@ -169,15 +175,17 @@
 Ondrej Duchon <ondrej.duchon@ultimum.io>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
 Paul Belanger <pabelanger@redhat.com>
 Paul Peereboom <paulpeereboom@hotmail.com>
 Pavel Boldin <pboldin@mirantis.com>
 Peter Razumovsky <prazumovsky@Peters-MacBook-Pro.local>
 Peter Razumovsky <prazumovsky@mirantis.com>
+Pierre Libeau <pierre.libeau@corp.ovh.com>
 Pierre Riteau <pierre@stackhpc.com>
+Piotr Parczewski <piotr@stackhpc.com>
 Piyush <piyush2011257@gmail.com>
 Piyush Raman Srivastava <pirsriva@in.ibm.com>
 Prabhjyot Singh Sodhi <prabhjyotsingh95@gmail.com>
 Pradeep K Surisetty <psuriset@linux.vnet.ibm.com>
 Pradeep Kumar Surisetty <psuriset@redhat.com>
 Prateek Arora <parora@redhat.com>
 Rajath Agasthya <rajathagasthya@gmail.com>
@@ -209,19 +217,22 @@
 Staroverov Anton <astaroverov@mirantis.com>
 Steve Wilkerson <sw5822@att.com>
 Stig Telfer <stig.openstack@telfer.org>
 Sumant Murke <sumant.murke@intel.com>
 Sunil Mamillapalli <sunil_mamillapalli@persistent.co.in>
 Swapnil Kulkarni <coolsvap@redhat.com>
 Swapnil Kulkarni <me@coolsvap.net>
+Tadas <tadasas@gmail.com>
 Takyuki Mitsui <tkyk.mitsui@gmail.com>
 Thobias Salazar Trevisan <thobiast@gmail.com>
 Thomas Bechtold <tbechtold@suse.com>
+Thomas Goirand <zigo@debian.org>
 Timur Nurlygayanov <tnurlygayanov@mirantis.com>
 TimurNurlygayanov <tnurlygayanov@mirantis.com>
+Tobias Urdin <tobias.urdin@binero.com>
 Tom Patzig <tom.patzig@sap.com>
 Tzanetos Balitsaris <tzabal@freebsd.org>
 Valeriy Ponomaryov <vponomaryov@mirantis.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Victor Sergeyev <vsergeyev@mirantis.com>
 Victoria Martínez de la Cruz <victoria@vmartinezdelacruz.com>
 Vieri <15050873171@163.com>
@@ -239,14 +250,15 @@
 Yaroslav Lobankov <ylobankov@mirantis.com>
 Yatin Kumbhare <yatinkumbhare@gmail.com>
 Yuki Nishiwaki <uckey.1067@gmail.com>
 Yuriy Nesenenko <ynesenenko@mirantis.com>
 Zhongcheng Lao <zlao@vmware.com>
 abdelal ali <ali.abdelal@nokia.com>
 akrzos <akrzos@redhat.com>
+alexv <alexv@mirantis.com>
 alexz <azvyagintsev@mirantis.com>
 ali <ali.abdelal@nokia.com>
 april <xiaolixu@cn.ibm.com>
 astarove <astarove@astarove-VirtualBox.localdomain>
 astaroverov <astaroverov@mirantis.com>
 bailinzhang <zhang.bailin@zte.com.cn>
 baiwenteng <baiwenteng@inspur.com>
@@ -262,20 +274,22 @@
 chenxing <chen.xing@99cloud.net>
 cxhuawei <424024687@qq.com>
 cxhuawei <xuchen1990xx@gmail.com>
 dagnello <dagnello@hp.com>
 dagnello <davide_agnello@hotmail.com>
 dlutton <eyedea32@gmail.com>
 ekonstantinov <ekonstantinov@mirantis.com>
+elajkat <lajos.katona@est.tech>
 gaofei <gao.fei@inspur.com>
 gecong1973 <ge.cong@zte.com.cn>
 gengchc2 <geng.changcai2@zte.com.cn>
 haishi <shihai1992@gmail.com>
 harikrishna-mallavolu <harikrishna.mallavolu@tcs.com>
 huang.huayong <huang.huayong2@zte.com.cn>
+hwang <sxmatch1986@gmail.com>
 jacky06 <zhang.min@99cloud.net>
 jacobliberman <jacobliberman@gmail.com>
 janonymous <janonymous.codevulture@gmail.com>
 jinyuanliu <liujinyuan@inspur.com>
 juhyun.park <juhyun.park@samsung.com>
 kaiokassiano <kaiokmo@lsd.ufcg.edu.br>
 kairat_kushaev <kkushaev@mirantis.com>
@@ -324,14 +338,15 @@
 vigny_wu <398776277@qq.com>
 vrovachev <vrovachev@mirantis.com>
 wanghui <wang_hui@inspur.com>
 wangqiangbj <wangqiangbj@inspur.com>
 wu.chunyang <wuchunyang@yovole.com>
 xuchao <xu.chao@99cloud.net>
 yanyanhu <yanyanhu@cn.ibm.com>
+yatinkarel <ykarel@redhat.com>
 yuhui_inspur <yuhui@inspur.com>
 yuriy_n <ynesenenko@mirantis.com>
 yuyafei <yu.yafei@zte.com.cn>
 zhangboye <zhangboye@inspur.com>
 zhangdaolong <zhangdaolong@fiberhome.com>
 zhangdelong <zhangdelong@cmss.chinamobile.com>
 zhangyanxian <zhang.yanxian@zte.com.cn>
```

### Comparing `rally-openstack-2.2.0/CHANGELOG.rst` & `rally-openstack-2.3.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,40 @@
     - **Removed** for now removed features/plugins.
     - **Fixed** for any bug fixes.
 
 .. Release notes for existing releases are MUTABLE! If there is something that
    was missed or can be improved, feel free to change it!
 
 
+[2.3.0] - 2023-08-01
+--------------------
+
+Deprecated
+~~~~~~~~~~
+This is the last release with support of Python 3.6 and Python 3.7
+
+Changed
+~~~~~~~
+
+* Bumped min required version of Rally to 3.4.0.
+* Switch docker image to rally 3.4.0 base.
+
+Removed
+~~~~~~~
+
+* Nova API doesn't include listing agents for a long time, so no need to
+  provide *NovaAgents.list_agents* scenario any more.
+
+Fixed
+~~~~~
+
+* Two cinder scenarios *CinderVolumeTypes.create_and_update_volume_type* and
+  *CinderVolumeTypes.create_volume_type_add_and_list_type_access* were
+  incompatible with Cinder API v3
+
 [2.2.0] - 2021-10-25
 --------------------
 
 Changed
 ~~~~~~~
 
 * Switch docker image to rally 3.3.0 base.
```

### Comparing `rally-openstack-2.2.0/CONTRIBUTING.rst` & `rally-openstack-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/ChangeLog` & `rally-openstack-2.3.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,42 @@
 CHANGES
 =======
 
+2.3.0
+-----
+
+* Update release date for 2.3.0
+* Release 2.3.0
+* Bring back tempita to u-c
+* Correct some cases' description
+* Update uc file
+* Fix rally test can't update device\_id
+* Require Rally>=3.4.0
+* Fix the issue of unshelving vm fail failure
+* Designate DNS - fix quota names according to U/S Doc
+* Keep CI up-to-date
+* Ignore pytest-cover warning
+* Update tox.ini to work with tox 4
+* Fix creating of Rally DB
+* Use absolute path for rally plugin dir check
+* Add new boot\_server\_attach\_created\_volume\_and\_extend test
+* Bump default Cirros version
+* Update rally-task-neutron to have only ovs as mech driver
+* [ci] Fix list-os-resources role
+* Suppress 2 warnings from Docutils
+* Update gnocchiclient requirement
+* fix use cinder "update\_volume\_type() got an unexpected keyword argument 'name' "
+* Fix exec of cloud-init at CreateShareAndAccessFromVM
+* Use resolvectl, not systemd-resolve
+* [ci] run unittests at py3.9 env
+* Multiple fixes for CI
+* Add sg rules with ipv6 ethertype
+* Fix use of keystone endpoint URL
+* Fix some CI issues
+
 2.2.0
 -----
 
 * [docker] Update ca-certs
 * Avoid poll\_interval to be the same as HTTP Keep-Alive timeout
 * Update requirements and release 2.2.0
 * Clean up extra spaces
```

### Comparing `rally-openstack-2.2.0/DOCKER_README.md` & `rally-openstack-2.3.0/DOCKER_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 Rally-OpenStack is a package of Rally plugins for OpenStack platform. 
 
 # How to run and use xrally-openstack container
 
 First of all, you need to pull the container. We suggest to use the last
 tagged version:
 
-    # pull the 2.2.0 image (the latest release at the point of writing the note)
-    $ docker pull xrally/xrally-openstack:2.2.0
+    # pull the 2.3.0 image (the latest release at the point of writing the note)
+    $ docker pull xrally/xrally-openstack:2.3.0
 
 **WARNING: never attach folders and volumes to `/rally` inside the container. It can break everything.**
 
 The default configuration file is located at `/etc/rally/rally.conf`. You
 should not be aware of it. If you want to override some options, use
 `/home/rally/.rally/rally.conf` location instead. Rally does not load all
 configuration files, so the primary one will be used.
@@ -23,15 +23,15 @@
 The default place for rally database file is `/home/rally/.rally/rally.sqlite`.
 To make the storage persistent across all container runs, you may want to use
 docker volumes or mount the directory.
 
 * use docker volumes. It is the easiest way. You just need to do something like:
 
       $ docker volume create --name rally_volume
-      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally-openstack:2.2.0 env create --name "foo"
+      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally-openstack:2.3.0 env create --name "foo"
 
 * mount outer directory inside the container
 
       # you can create directory in whatever you want to place, but you
       # may wish to make the data available for all users
       $ sudo mkdir /var/lib/rally_container
       
@@ -40,18 +40,18 @@
       # 65500 *outside* the container as well, which is why it is created
       # in ``/var/lib/rally_container``. Creating it in your home directory is
       # only likely to work if your home directory has excessively open
       # permissions (e.g., ``0755``), which is not recommended.
       $ sudo chown 65500 /var/lib/rally_container
 
       # As opposed to mounting docker image, you must initialize rally database*
-      $ docker run -v /var/lib/rally_container:/home/rally/.rally xrally/xrally-openstack:2.2.0 db create
+      $ docker run -v /var/lib/rally_container:/home/rally/.rally xrally/xrally-openstack:2.3.0 db create
 
       # And finally, you can start doing your things.*
-      $ docker run -v /var/lib/rally_container:/home/rally/.rally xrally/xrally-openstack:2.2.0 env create --name "foo"
+      $ docker run -v /var/lib/rally_container:/home/rally/.rally xrally/xrally-openstack:2.3.0 env create --name "foo"
 
 Have fun!
 
 # Links
 
 * Free software: Apache license
 * Documentation: https://rally.readthedocs.io
```

### Comparing `rally-openstack-2.2.0/Dockerfile` & `rally-openstack-2.3.0/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM xrally/xrally:3.3.0
+FROM xrally/xrally:3.4.0
 
 # "rally" user (which is selected by-default) is owner of "/rally" directory,
 #   so there is no need to call chown or switch the user
 COPY . /rally/xrally_openstack
 WORKDIR /rally/xrally_openstack
 
 # to install package system-wide, we need to temporary switch to root user
```

### Comparing `rally-openstack-2.2.0/LICENSE` & `rally-openstack-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/PKG-INFO` & `rally-openstack-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rally-openstack
-Version: 2.2.0
+Version: 2.3.0
 Summary: Rally plugins for OpenStack platform
 Home-page: https://docs.openstack.org/rally/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ===============
         rally-openstack
```

### Comparing `rally-openstack-2.2.0/README.rst` & `rally-openstack-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/bindep.txt` & `rally-openstack-2.3.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/devstack/README.rst` & `rally-openstack-2.3.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/devstack/lib/rally` & `rally-openstack-2.3.0/devstack/lib/rally`

 * *Files 18% similar despite different names*

```diff
@@ -39,57 +39,39 @@
 
 # Functions
 # ---------
 
 # Creates a configuration file for the current deployment
 # Uses the following variables:
 #
-# - ``ADMIN_PASSWORD``, ``KEYSTONE_SERVICE_PROTOCOL``,
-#   ``KEYSTONE_SERVICE_HOST``, ``KEYSTONE_SERVICE_PORT``,
-#   ``IDENTITY_API_VERSION`` - must be defined
+# - ``ADMIN_PASSWORD``, ``REGION_NAME``
+#   ``KEYSTONE_SERVICE_URI``
 #   ``OSPROFILER_HMAC_KEYS`` - optional, for integration with osprofiler
 #   ``OSPROFILER_CONNECTION_STRING`` - optional, if this is set together with
 #       OSPROFILER_HMAC_KEYS rally html report will use osprofiler api to
 #       generate html report for each trace and embed it as iframe to our
-#       native html repor
+#       native html report
 #   ``RALLY_OSPROFILER_CHART`` - optional, a path to store osprofiler's reports
 #
 
 # _create_deployment_config filename
 function _create_deployment_config() {
-if [[ "$IDENTITY_API_VERSION" == 2.0 ]]
-then
-    cat >$1 <<EOF
+cat >$1 <<EOF
 {
     "openstack": {
-        "auth_url": "$OS_AUTH_URL",
-        "region_name": "$REGION_NAME",
-        "admin": {
-            "username": "admin",
-            "password": "$ADMIN_PASSWORD",
-            "tenant_name": "admin",
-        }
-EOF
-fi
-if [[ "$IDENTITY_API_VERSION" == 3 ]]
-then
-    cat >$1 <<EOF
-{
-    "openstack": {
-        "auth_url": "$OS_AUTH_URL",
+        "auth_url": "$KEYSTONE_SERVICE_URI",
         "region_name": "$REGION_NAME",
         "admin": {
             "username": "admin",
             "password": "$ADMIN_PASSWORD",
             "project_name": "admin",
             "user_domain_name": "Default",
             "project_domain_name": "Default"
         },
 EOF
-fi
 
 # Now add osprofiler config if necessary
 if [[ ! -z "$OSPROFILER_HMAC_KEYS" ]]; then
     cat >>$1 <<EOF
         "profiler_hmac_key": $OSPROFILER_HMAC_KEYS,
 EOF
 fi
```

### Comparing `rally-openstack-2.2.0/devstack/plugin.sh` & `rally-openstack-2.3.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/etc/motd` & `rally-openstack-2.3.0/etc/motd`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/etc/rally/rally.conf.sample` & `rally-openstack-2.3.0/etc/rally/rally.conf.sample`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,15 @@
 # Watcher audit launch interval (floating point value)
 #watcher_audit_launch_poll_interval = 2.0
 
 # Watcher audit launch timeout (integer value)
 #watcher_audit_launch_timeout = 300
 
 # image URL (string value)
-#img_url = http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img
+#img_url = http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img
 
 # Image disk format to use when creating the image (string value)
 #img_disk_format = qcow2
 
 # Image container format to use when creating the image (string value)
 #img_container_format = bare
```

### Comparing `rally-openstack-2.2.0/rally-jobs/README.rst` & `rally-openstack-2.3.0/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/barbican.yaml` & `rally-openstack-2.3.0/rally-jobs/barbican.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/basic-with-existing-users.yaml` & `rally-openstack-2.3.0/rally-jobs/basic-with-existing-users.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% set flavor_name = "m1.tiny" %}
 {% set image_name = "^cirros.*-disk$" %}
-{% set cirros_image_url = "https://github.com/cirros-dev/cirros/releases/download/0.3.5/cirros-0.3.5-x86_64-disk.img" %}
 {% set smoke = 0 %}
 
 ---
   version: 2
   title: Rally task that is called for an evironment with existing users
   description: >
     The task contains various scenarios that do not require admin user
@@ -108,29 +107,7 @@
           runner:
             constant:
               times: 2
               concurrency: 2
           sla:
             failure_rate:
               max: 0
-
-    - title: Test VMTask scenario
-      workloads:
-        -
-          scenario:
-            VMTasks.dd_load_test:
-              flavor:
-                name: "m1.tiny"
-              image:
-                name: {{image_name}}
-              floating_network: "public"
-              force_delete: false
-              username: "cirros"
-          contexts:
-            network: {}
-          runner:
-            constant:
-              times: 2
-              concurrency: 2
-          sla:
-            failure_rate:
-              max: 0
```

### Comparing `rally-openstack-2.2.0/rally-jobs/cinder.yaml` & `rally-openstack-2.3.0/rally-jobs/cinder.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/designate.yaml` & `rally-openstack-2.3.0/rally-jobs/designate.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/autoscaling_group.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/autoscaling_group.yaml.template`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   flavor:
     type: string
     default: m1.tiny
     constraints:
       - custom_constraint: nova.flavor
   image:
     type: string
-    default: cirros-0.4.0-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
     constraints:
       - custom_constraint: glance.image
   scaling_adjustment:
     type: number
     default: 1
   max_size:
     type: number
```

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/hook_example_script.sh` & `rally-openstack-2.3.0/rally-jobs/extra/hook_example_script.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/instance_test.sh` & `rally-openstack-2.3.0/rally-jobs/extra/instance_test.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/ui.yaml` & `rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter/UI/ui.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter.zip` & `rally-openstack-2.3.0/rally-jobs/extra/murano/applications/HelloReporter/io.murano.apps.HelloReporter.zip`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/resource_group_server_with_volume.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/resource_group_server_with_volume.yaml.template`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   num_instances:
     type: number
     description: number of instances that should be created in resource group
     constraints:
       - range: {min: 1}
   instance_image:
     type: string
-    default: cirros-0.4.0-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   instance_volume_size:
     type: number
     description: Size of volume to attach to instance
     default: 1
     constraints:
       - range: {min: 1, max: 1024}
   instance_flavor:
```

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/resource_group_with_outputs.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/resource_group_with_outputs.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/server_with_ports.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/server_with_ports.yaml.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 parameters:
   # set all correct defaults for parameters before launch test
   public_net:
     type: string
     default: public
   image:
     type: string
-    default: cirros-0.4.0-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   flavor:
     type: string
     default: m1.tiny
   cidr:
     type: string
     default: 11.11.11.0/24
```

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/server_with_volume.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/server_with_volume.yaml.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 heat_template_version: 2013-05-23
 
 parameters:
   # set all correct defaults for parameters before launch test
   image:
     type: string
-    default: cirros-0.4.0-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   flavor:
     type: string
     default: m1.tiny
   availability_zone:
     type: string
     description: The Availability Zone to launch the instance.
     default: nova
```

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/updated_autoscaling_policy_inplace.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/updated_autoscaling_policy_inplace.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/updated_random_strings_replace.yaml.template` & `rally-openstack-2.3.0/rally-jobs/extra/updated_random_strings_replace.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/workload/wordpress_heat_template.yaml` & `rally-openstack-2.3.0/rally-jobs/extra/workload/wordpress_heat_template.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/extra/workload/wp-instances.yaml` & `rally-openstack-2.3.0/rally-jobs/extra/workload/wp-instances.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/heat.yaml` & `rally-openstack-2.3.0/rally-jobs/heat.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/ironic.yaml` & `rally-openstack-2.3.0/rally-jobs/ironic.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/keystone-glance-swift.yaml` & `rally-openstack-2.3.0/rally-jobs/keystone-glance-swift.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set cirros_image_url = "https://github.com/cirros-dev/cirros/releases/download/0.3.5/cirros-0.3.5-x86_64-disk.img" %}
+{%- set cirros_image_url = "https://github.com/cirros-dev/cirros/releases/download/0.5.2/cirros-0.5.2-x86_64-disk.img" %}
 ---
   KeystoneBasic.authenticate_user_and_validate_token:
     -
       args: {}
       runner:
         type: "constant"
         times: 20
```

### Comparing `rally-openstack-2.2.0/rally-jobs/magnum.yaml` & `rally-openstack-2.3.0/rally-jobs/magnum.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/manila-no-ss.yaml` & `rally-openstack-2.3.0/rally-jobs/manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/manila.yaml` & `rally-openstack-2.3.0/rally-jobs/manila.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/mistral.yaml` & `rally-openstack-2.3.0/rally-jobs/mistral.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/monasca.yaml` & `rally-openstack-2.3.0/rally-jobs/monasca.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/murano.yaml` & `rally-openstack-2.3.0/rally-jobs/murano.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/neutron-trunk.yaml` & `rally-openstack-2.3.0/rally-jobs/neutron-trunk.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/neutron-with-extensions.yaml` & `rally-openstack-2.3.0/rally-jobs/neutron-with-extensions.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/neutron.yaml` & `rally-openstack-2.3.0/rally-jobs/neutron.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -715,109 +715,7 @@
             - "8.8.8.8"
             - "8.8.4.4"
           router:
             external: false
       sla:
         failure_rate:
           max: 0
-
-  VMTasks.boot_runcommand_delete:
-    -
-      args:
-        flavor:
-            name: "m1.tiny"
-        image:
-            name: {{image_name}}
-        command:
-          script_file: "~/.rally/extra/instance_test.sh"
-          interpreter: "/bin/sh"
-        username: "cirros"
-      runner:
-        type: "constant"
-        times: {{smoke or 2}}
-        concurrency: {{smoke or 2}}
-      context:
-        users:
-          tenants: {{smoke or 2}}
-          users_per_tenant: {{smoke or 2}}
-        network: {}
-      sla:
-        failure_rate:
-          max: 0
-    -
-      args:
-        flavor:
-            name: "m1.tiny"
-        image:
-            name: {{image_name}}
-        command:
-          script_file: "~/.rally/extra/instance_test.sh"
-          interpreter: "/bin/sh"
-        username: "cirros"
-        volume_args:
-            size: 2
-      runner:
-        type: "constant"
-        times: {{smoke or 2}}
-        concurrency: {{smoke or 2}}
-      context:
-        users:
-          tenants: {{smoke or 2}}
-          users_per_tenant: {{smoke or 1}}
-        network: {}
-      sla:
-        failure_rate:
-          max: 0
-    -
-      args:
-        flavor:
-          name: {{flavor_name}}
-        image:
-          name: {{image_name}}
-        floating_network: "public"
-        command:
-          script_inline: |
-            time_seconds(){ (time -p $1 ) 2>&1 |awk '/real/{print $2}'; }
-            file=/tmp/test.img
-            c=100 #100M
-            write_seq=$(time_seconds "dd if=/dev/zero of=$file bs=1M count=$c")
-            read_seq=$(time_seconds "dd if=$file of=/dev/null bs=1M count=$c")
-            [ -f $file ] && rm $file
-
-            echo "{
-                \"write_seq\": $write_seq,
-                \"read_seq\": $read_seq
-                }"
-          interpreter: "/bin/sh"
-        username: "cirros"
-      runner:
-        type: "constant"
-        times: 2
-        concurrency: 2
-      context:
-        users:
-          tenants: 1
-          users_per_tenant: 1
-        network: {}
-      sla:
-        failure_rate:
-          max: 0
-
-  VMTasks.dd_load_test:
-    -
-      args:
-        flavor:
-            name: "m1.tiny"
-        image:
-            name: {{image_name}}
-        floating_network: "public"
-        force_delete: false
-        username: "cirros"
-      runner:
-        type: "constant"
-        times: 2
-        concurrency: 2
-      context:
-        users:
-          tenants: 2
-          users_per_tenant: 1
-        network: {}
```

### Comparing `rally-openstack-2.2.0/rally-jobs/nova.yaml` & `rally-openstack-2.3.0/rally-jobs/nova.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set cirros_image_url = "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img" %}
+{%- set cirros_image_url = "https://github.com/cirros-dev/cirros/releases/download/0.5.2/cirros-0.5.2-x86_64-disk.img" %}
 {% set image_name = "^(cirros.*-disk|TestVM)$" %}
 {% set flavor_name = "m1.tiny" %}
 {% set volume_type = "" %}
 ---
   version: 2
   title: Task for gate-rally-dsvm-rally-nova-nv job
   description: >
@@ -374,33 +374,30 @@
       contexts:
         users:
           tenants: 2
           users_per_tenant: 1
     -
       title: NovaServers.boot_and_get_console_url tests
       workloads:
-      {% for s in ("novnc", "xvpvnc") %}
         -
           scenario:
             NovaServers.boot_and_get_console_url:
               flavor:
                 name: "{{flavor_name}}"
               image:
                 name: "{{image_name}}"
-              console_type: {{s}}
+              console_type: novnc
           runner:
             constant:
               times: 4
               concurrency: 2
           contexts:
             users:
               tenants: 2
               users_per_tenant: 2
-      {% endfor %}
-
     -
       title: NovaServers.resize_server tests
       workloads:
         -
           scenario:
             NovaServers.resize_server:
               flavor:
@@ -480,14 +477,36 @@
           times: 2
           concurrency: 2
       contexts:
         users:
           tenants: 2
           users_per_tenant: 1
     -
+      title: NovaServers.boot_server_attach_created_volume_and_extend tests
+      scenario:
+        NovaServers.boot_server_attach_created_volume_and_extend:
+          flavor:
+            name: {{flavor_name}}
+          image:
+            name: {{image_name}}
+          volume_size: 1
+          new_volume_size: 2
+          force_delete: false
+          do_delete: true
+          boot_server_kwargs: {}
+          create_volume_kwargs: {}
+      runner:
+        constant:
+          times: 2
+          concurrency: 2
+      contexts:
+        users:
+          tenants: 2
+          users_per_tenant: 1
+    -
       title: NovaServers.boot_server_from_volume_and_resize tests
       scenario:
         NovaServers.boot_server_from_volume_and_resize:
           flavor:
             name: {{flavor_name}}
           image:
             name: {{image_name}}
@@ -871,22 +890,14 @@
           times: 4
           concurrency: 2
       contexts:
         users:
           tenants: 2
           users_per_tenant: 2
     -
-      title: NovaAgents.list_agents tests
-      scenario:
-        NovaAgents.list_agents: {}
-      runner:
-        constant:
-          concurrency: 2
-          times: 4
-    -
       title: NovaAggregates.list_aggregates tests
       scenario:
         NovaAggregates.list_aggregates: {}
       runner:
         constant:
           concurrency: 2
           times : 4
```

### Comparing `rally-openstack-2.2.0/rally-jobs/octavia.yaml` & `rally-openstack-2.3.0/rally-jobs/octavia.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/plugins/fake_plugin.py` & `rally-openstack-2.3.0/rally-jobs/plugins/fake_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/plugins/rally_profile.py` & `rally-openstack-2.3.0/rally-jobs/plugins/rally_profile.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/plugins/test_relative_import/zzz.py` & `rally-openstack-2.3.0/rally-jobs/plugins/test_relative_import/zzz.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/self-rally.yaml` & `rally-openstack-2.3.0/rally-jobs/self-rally.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/senlin.yaml` & `rally-openstack-2.3.0/rally-jobs/senlin.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
           users_per_tenant: 2
         profiles:
           type: os.nova.server
           version: "1.0"
           properties:
             name: cirros_server
             flavor: 1
-            image: "cirros-0.4.0-x86_64-disk"
+            image: "cirros-0.5.2-x86_64-disk"
             networks:
               - network: private
```

### Comparing `rally-openstack-2.2.0/rally-jobs/simple-job.yaml` & `rally-openstack-2.3.0/rally-jobs/simple-job.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/telemetry.yaml` & `rally-openstack-2.3.0/rally-jobs/telemetry.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/watcher.yaml` & `rally-openstack-2.3.0/rally-jobs/watcher.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally-jobs/zaqar.yaml` & `rally-openstack-2.3.0/rally-jobs/zaqar.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/__init__.py` & `rally-openstack-2.3.0/rally_openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/_compat.py` & `rally-openstack-2.3.0/rally_openstack/_compat.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/cinder.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/cinder.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/cleanup.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/cleanup.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/glance.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/glance.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/heat.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/heat.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/ironic.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/ironic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/keystone_roles.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/keystone_roles.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/keystone_users.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/keystone_users.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/magnum.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/magnum.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/manila.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/manila.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/mistral.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/mistral.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/monasca.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/monasca.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/murano.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/murano.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/neutron.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/neutron.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/nova.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/nova.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/octavia.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/octavia.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/opts.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/opts.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/osclients.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/osclients.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/profiler.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/profiler.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/sahara.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/sahara.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/senlin.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/senlin.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/tempest.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/tempest.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    under the License.
 
 from rally.common import cfg
 
 OPTS = {"openstack": [
     cfg.StrOpt("img_url",
                default="http://download.cirros-cloud.net/"
-                       "0.3.5/cirros-0.3.5-x86_64-disk.img",
+                       "0.5.2/cirros-0.5.2-x86_64-disk.img",
                deprecated_group="tempest",
                help="image URL"),
     cfg.StrOpt("img_disk_format",
                default="qcow2",
                deprecated_group="tempest",
                help="Image disk format to use when creating the image"),
     cfg.StrOpt("img_container_format",
@@ -55,33 +55,33 @@
                help="Role required for users "
                     "to be able to manage Heat stacks"),
     cfg.StrOpt("heat_stack_user_role",
                default="heat_stack_user",
                deprecated_group="tempest",
                help="Role for Heat template-defined users"),
     cfg.IntOpt("flavor_ref_ram",
-               default="64",
+               default="128",
                deprecated_group="tempest",
                help="Primary flavor RAM size used by most of the test cases"),
     cfg.IntOpt("flavor_ref_alt_ram",
-               default="128",
+               default="192",
                deprecated_group="tempest",
                help="Alternate reference flavor RAM size used by test that "
                "need two flavors, like those that resize an instance"),
     cfg.IntOpt("flavor_ref_disk",
                default="5",
                help="Primary flavor disk size in GiB used by most of the test "
                "cases"),
     cfg.IntOpt("flavor_ref_alt_disk",
                default="5",
                help="Alternate reference flavor disk size in GiB used by "
                "tests that need two flavors, like those that resize an "
                "instance"),
     cfg.IntOpt("heat_instance_type_ram",
-               default="64",
+               default="128",
                deprecated_group="tempest",
                help="RAM size flavor used for orchestration test cases"),
     cfg.IntOpt("heat_instance_type_disk",
                default="5",
                deprecated_group="tempest",
                help="Disk size requirement in GiB flavor used for "
                "orchestration test cases"),
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/vm.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/vm.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/cfg/watcher.py` & `rally-openstack-2.3.0/rally_openstack/common/cfg/watcher.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/consts.py` & `rally-openstack-2.3.0/rally_openstack/common/consts.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/credential.py` & `rally-openstack-2.3.0/rally_openstack/common/credential.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/exceptions.py` & `rally-openstack-2.3.0/rally_openstack/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/osclients.py` & `rally-openstack-2.3.0/rally_openstack/common/osclients.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/service.py` & `rally-openstack-2.3.0/rally_openstack/common/service.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/gnocchi/metric.py` & `rally-openstack-2.3.0/rally_openstack/common/services/gnocchi/metric.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/grafana/grafana.py` & `rally-openstack-2.3.0/rally_openstack/common/services/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/heat/main.py` & `rally-openstack-2.3.0/rally_openstack/common/services/heat/main.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/identity/identity.py` & `rally-openstack-2.3.0/rally_openstack/common/services/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_common.py` & `rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_common.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_v2.py` & `rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/identity/keystone_v3.py` & `rally-openstack-2.3.0/rally_openstack/common/services/identity/keystone_v3.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/image/glance_common.py` & `rally-openstack-2.3.0/rally_openstack/common/services/image/glance_common.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/image/glance_v1.py` & `rally-openstack-2.3.0/rally_openstack/common/services/image/glance_v1.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/image/glance_v2.py` & `rally-openstack-2.3.0/rally_openstack/common/services/image/glance_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/image/image.py` & `rally-openstack-2.3.0/rally_openstack/common/services/image/image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/key_manager/barbican.py` & `rally-openstack-2.3.0/rally_openstack/common/services/key_manager/barbican.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/loadbalancer/octavia.py` & `rally-openstack-2.3.0/rally_openstack/common/services/loadbalancer/octavia.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/network/net_utils.py` & `rally-openstack-2.3.0/rally_openstack/common/services/network/net_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/network/neutron.py` & `rally-openstack-2.3.0/rally_openstack/common/services/network/neutron.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/storage/block.py` & `rally-openstack-2.3.0/rally_openstack/common/services/storage/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,14 +351,53 @@
         :returns: Return the created volume type.
         """
         return self._impl.create_volume_type(name=name,
                                              description=description,
                                              is_public=is_public)
 
     @service.should_be_overridden
+    def update_volume_type(self, volume_type, name=None,
+                           description=None, is_public=None):
+        """Update the name and/or description for a volume type.
+
+        :param volume_type: The ID or an instance of the :class:`VolumeType`
+                            to update.
+        :param name: if None, updates name by generating random name.
+                     else updates name with provided name
+        :param description: Description of the volume type.
+        :returns: Returns an updated volume type object.
+        """
+        return self._impl.update_volume_type(
+            volume_type=volume_type, name=name, description=description,
+            is_public=is_public
+        )
+
+    @service.should_be_overridden
+    def add_type_access(self, volume_type, project):
+        """Add a project to the given volume type access list.
+
+        :param volume_type: Volume type name or ID to add access for the given
+                            project
+        :param project: Project ID to add volume type access for
+        :return: An instance of cinderclient.apiclient.base.TupleWithMeta
+        """
+        return self._impl.add_type_access(
+            volume_type=volume_type, project=project
+        )
+
+    @service.should_be_overridden
+    def list_type_access(self, volume_type):
+        """Print access information about the given volume type
+
+        :param volume_type: Filter results by volume type name or ID
+        :return: VolumeTypeAccess of specific project
+        """
+        return self._impl.list_type_access(volume_type)
+
+    @service.should_be_overridden
     def get_volume_type(self, volume_type):
         """get details of volume_type.
 
         :param volume_type: The ID of the :class:`VolumeType` to get
         :returns: :class:`VolumeType`
         """
         return self._impl.get_volume_type(volume_type)
@@ -429,24 +468,24 @@
         :param search_opts: Options used when search for encryption types
         :return: a list of :class: VolumeEncryptionType instances
         """
         return self._impl.list_encryption_type(search_opts=search_opts)
 
     @service.should_be_overridden
     def delete_encryption_type(self, volume_type):
-        """Delete the encryption type information for the specified volume type.
+        """Delete the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             must be deleted
         """
         self._impl.delete_encryption_type(volume_type)
 
     @service.should_be_overridden
     def update_encryption_type(self, volume_type, specs):
-        """Update the encryption type information for the specified volume type.
+        """Update the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             will be updated
         :param specs: the encryption type specifications to update
         :return: an instance of :class: VolumeEncryptionType
         """
         return self._impl.update_encryption_type(volume_type, specs=specs)
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_common.py` & `rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         :returns: base on client response return True if the request
                   has been accepted or not
         """
         aname = "cinder_v%s.delete_volume_type" % self.version
         with atomic.ActionTimer(self, aname):
             tuple_res = self._get_client().volume_types.delete(
                 volume_type)
-            return (tuple_res[0].status_code == 202)
+            return tuple_res[0].status_code == 202
 
     def set_volume_type_keys(self, volume_type, metadata):
         """Set extra specs on a volume type.
 
         :param volume_type: The :class:`VolumeType` to set extra spec on
         :param metadata: A dict of key/value pairs to be set
         :returns: extra_specs if the request has been accepted
@@ -434,29 +434,29 @@
         """
         aname = "cinder_v%s.list_encryption_type" % self.version
         with atomic.ActionTimer(self, aname):
             return self._get_client().volume_encryption_types.list(
                 search_opts)
 
     def delete_encryption_type(self, volume_type):
-        """Delete the encryption type information for the specified volume type.
+        """Delete the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             must be deleted
         """
         aname = "cinder_v%s.delete_encryption_type" % self.version
         with atomic.ActionTimer(self, aname):
             resp = self._get_client().volume_encryption_types.delete(
                 volume_type)
             if (resp[0].status_code != 202):
                 raise exceptions.RallyException(
                     "EncryptionType Deletion Failed")
 
     def update_encryption_type(self, volume_type, specs):
-        """Update the encryption type information for the specified volume type.
+        """Update the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             must be updated
         :param specs: the encryption type specifications to update
         :return: an instance of :class: VolumeEncryptionType
         """
         aname = "cinder_v%s.update_encryption_type" % self.version
@@ -647,14 +647,50 @@
 
         :param volume_type: Name or Id of the volume type
         :returns: base on client response return True if the request
                   has been accepted or not
         """
         return self._impl.delete_volume_type(volume_type)
 
+    def update_volume_type(self, volume_type, name=None,
+                           description=None, is_public=None):
+        """Update the name and/or description for a volume type.
+
+        :param volume_type: The ID or an instance of the :class:`VolumeType`
+                            to update.
+        :param name: if None, updates name by generating random name.
+                     else updates name with provided name
+        :param description: Description of the volume type.
+        :rtype: :class:`VolumeType`
+        """
+        return self._impl.update_volume_type(
+            volume_type=volume_type, name=name, description=description,
+            is_public=is_public
+        )
+
+    def add_type_access(self, volume_type, project):
+        """Add a project to the given volume type access list.
+
+        :param volume_type: Volume type name or ID to add access for the given
+                            project
+        :project: Project ID to add volume type access for
+        :return: An instance of cinderclient.apiclient.base.TupleWithMeta
+        """
+        return self._impl.add_type_access(
+            volume_type=volume_type, project=project
+        )
+
+    def list_type_access(self, volume_type):
+        """Print access information about the given volume type
+
+        :param volume_type: Filter results by volume type name or ID
+        :return: VolumeTypeAccess of specific project
+        """
+        return self._impl.list_type_access(volume_type)
+
     def set_volume_type_keys(self, volume_type, metadata):
         """Set extra specs on a volume type.
 
         :param volume_type: The :class:`VolumeType` to set extra spec on
         :param metadata: A dict of key/value pairs to be set
         :returns: extra_specs if the request has been accepted
         """
@@ -706,23 +742,23 @@
         :return: a list of :class: VolumeEncryptionType instances
         """
         return [self._unify_encryption_type(encryption_type)
                 for encryption_type in self._impl.list_encryption_type(
                     search_opts=search_opts)]
 
     def delete_encryption_type(self, volume_type):
-        """Delete the encryption type information for the specified volume type.
+        """Delete the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             must be deleted
         """
         return self._impl.delete_encryption_type(volume_type)
 
     def update_encryption_type(self, volume_type, specs):
-        """Update the encryption type information for the specified volume type.
+        """Update the encryption type information for the specified volume type
 
         :param volume_type: the volume type whose encryption type information
                             must be updated
         :param specs: the encryption type specifications to update
         :return: an instance of :class: VolumeEncryptionType
         """
         return self._impl.update_encryption_type(volume_type, specs=specs)
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v1.py` & `rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -313,14 +313,24 @@
         :param name: Descriptive name of the volume type
         :param description: Description of the volume type
         :param is_public: Volume type visibility
         :returns: Return the created volume type.
         """
         return self._impl.create_volume_type(name=name)
 
+    def update_volume_type(self, volume_type, name=None,
+                           description=None, is_public=None):
+        raise NotImplementedError("Cinder V1 doesn't support this method.")
+
+    def add_type_access(self, volume_type, project):
+        raise NotImplementedError("Cinder V1 doesn't support this method.")
+
+    def list_type_access(self, volume_type):
+        raise NotImplementedError("Cinder V1 doesn't support this method.")
+
     def restore_backup(self, backup_id, volume_id=None):
         """Restore the given backup.
 
         :param backup_id: The ID of the backup to restore.
         :param volume_id: The ID of the volume to restore the backup to.
 
         :returns: Return the restored backup.
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v2.py` & `rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,19 @@
     @atomic.action_timer("cinder_v2.update_volume_type")
     def update_volume_type(self, volume_type, name=None,
                            description=None, is_public=None):
         """Update the name and/or description for a volume type.
 
         :param volume_type: The ID or an instance of the :class:`VolumeType`
                             to update.
-        :param name: if None, updates name by generating random name.
+        :param name: if None, name cannot be updated.
                      else updates name with provided name
         :param description: Description of the volume type.
         :rtype: :class:`VolumeType`
         """
-        name = name or self.generate_random_name()
 
         return self._get_client().volume_types.update(volume_type, name,
                                                       description, is_public)
 
     @atomic.action_timer("cinder_v2.add_type_access")
     def add_type_access(self, volume_type, project):
         """Add a project to the given volume type access list.
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/services/storage/cinder_v3.py` & `rally-openstack-2.3.0/rally_openstack/common/services/storage/cinder_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,39 +174,38 @@
         """
         kwargs = {"name": name or self.generate_random_name(),
                   "description": description,
                   "is_public": is_public}
         return self._get_client().volume_types.create(**kwargs)
 
     @atomic.action_timer("cinder_v3.update_volume_type")
-    def update_volume_type(self, volume_type, update_name=False,
+    def update_volume_type(self, volume_type, name=None,
                            description=None, is_public=None):
         """Update the name and/or description for a volume type.
 
         :param volume_type: The ID or a instance of the :class:`VolumeType`
                             to update.
-        :param update_name: if True, can update name by generating random name.
-                            if False, don't update name.
+        :param name: if None, name cannot be updated.
+                     else updates name with provided name
         :param description: Description of the volume type.
+        :param is_public:
         :rtype: :class:`VolumeType`
         """
-        name = None
-        if update_name:
-            name = self.generate_random_name()
+
         return self._get_client().volume_types.update(
             volume_type=volume_type, name=name, description=description,
             is_public=is_public)
 
     @atomic.action_timer("cinder_v3.add_type_access")
     def add_type_access(self, volume_type, project):
         """Add a project to the given volume type access list.
 
         :param volume_type: Volume type name or ID to add access for the given
                             project
-        :project: Project ID to add volume type access for
+        :param project: Project ID to add volume type access for
         :return: An instance of cinderclient.apiclient.base.TupleWithMeta
         """
         return self._get_client().volume_type_access.add_project_access(
             volume_type=volume_type, project=project)
 
     @atomic.action_timer("cinder_v3.list_type_access")
     def list_type_access(self, volume_type):
```

### Comparing `rally-openstack-2.2.0/rally_openstack/common/validators.py` & `rally-openstack-2.3.0/rally_openstack/common/validators.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/common/wrappers/network.py` & `rally-openstack-2.3.0/rally_openstack/common/wrappers/network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/environment/platforms/existing.py` & `rally-openstack-2.3.0/rally_openstack/environment/platforms/existing.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/cleanup/base.py` & `rally-openstack-2.3.0/rally_openstack/task/cleanup/base.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/cleanup/manager.py` & `rally-openstack-2.3.0/rally_openstack/task/cleanup/manager.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/cleanup/resources.py` & `rally-openstack-2.3.0/rally_openstack/task/cleanup/resources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/context.py` & `rally-openstack-2.3.0/rally_openstack/task/context.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/api_versions.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/api_versions.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/volume_types.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/volume_types.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/cinder/volumes.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/cinder/volumes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/admin.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/admin.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/base.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/base.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/cleanup/user.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/cleanup/user.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/dataplane/heat.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/dataplane/heat.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/designate/zones.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/designate/zones.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/glance/images.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/glance/images.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/heat/stacks.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/heat/stacks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/roles.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/roles.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/keystone/users.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/keystone/users.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/ca_certs.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/ca_certs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/cluster_templates.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/cluster_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/magnum/clusters.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/magnum/clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/manila/consts.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/manila/consts.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_security_services.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_security_services.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_share_networks.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_share_networks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/manila/manila_shares.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/manila/manila_shares.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/monasca/metrics.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/monasca/metrics.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/murano/murano_environments.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/murano/murano_environments.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/murano/murano_packages.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/murano/murano_packages.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/network/allow_ssh.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/network/allow_ssh.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,43 +42,69 @@
         elif value is None:
             return default.get(key, none_char)
         return str(value)
 
     # NOTE(andreykurilin): there are more actual comparison keys, but this set
     #   should be enough for us.
     comparison_keys = [
+        "ethertype",
         "direction",
         "port_range_max",
         "port_range_min",
         "protocol",
         "remote_ip_prefix"
     ]
     return "_".join([_normalize_rule_value(x, rule.get(x))
                      for x in comparison_keys])
 
 
 _RULES_TO_ADD = [
     {
+        "ethertype": "IPv4",
         "protocol": "tcp",
         "port_range_max": 65535,
         "port_range_min": 1,
         "remote_ip_prefix": "0.0.0.0/0",
         "direction": "ingress"
     },
     {
+        "ethertype": "IPv6",
+        "protocol": "tcp",
+        "port_range_max": 65535,
+        "port_range_min": 1,
+        "remote_ip_prefix": "::/0",
+        "direction": "ingress"
+    },
+    {
+        "ethertype": "IPv4",
         "protocol": "udp",
         "port_range_max": 65535,
         "port_range_min": 1,
         "remote_ip_prefix": "0.0.0.0/0",
         "direction": "ingress"
     },
     {
+        "ethertype": "IPv6",
+        "protocol": "udp",
+        "port_range_max": 65535,
+        "port_range_min": 1,
+        "remote_ip_prefix": "::/0",
+        "direction": "ingress"
+    },
+    {
+        "ethertype": "IPv4",
         "protocol": "icmp",
         "remote_ip_prefix": "0.0.0.0/0",
         "direction": "ingress"
+    },
+    {
+        "ethertype": "IPv6",
+        "protocol": "ipv6-icmp",
+        "remote_ip_prefix": "::/0",
+        "direction": "ingress"
     }
 ]
 
 
 @validation.add("required_platform", platform="openstack", users=True)
 @context.configure(name="allow_ssh", platform="openstack", order=320)
 class AllowSSH(context.OpenStackContext):
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/network/existing_network.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/network/existing_network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/network/networking_agents.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/network/networking_agents.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/network/networks.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/network/networks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/network/routers.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/network/routers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/neutron/lbaas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/neutron/lbaas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/nova/flavors.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/nova/flavors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/nova/keypairs.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/nova/keypairs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/nova/servers.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/nova/servers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/cinder_quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/cinder_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/designate_quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/designate_quotas.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
                 "type": "integer",
                 "minimum": 1
             },
             "zones": {
                 "type": "integer",
                 "minimum": 1
             },
-            "zones_recordsets": {
+            "zone_recordsets": {
                 "type": "integer",
                 "minimum": 1
             },
-            "zones_records": {
+            "zone_records": {
                 "type": "integer",
                 "minimum": 1
             },
             "recordset_records": {
                 "type": "integer",
                 "minimum": 1
             },
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/manila_quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/manila_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/neutron_quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/neutron_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/nova_quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/nova_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/quotas/quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/quotas/quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_cluster.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_cluster.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_image.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_input_data_sources.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_input_data_sources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_job_binaries.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_job_binaries.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/sahara/sahara_output_data_sources.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/sahara/sahara_output_data_sources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/senlin/profiles.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/senlin/profiles.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/swift/objects.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/swift/objects.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/swift/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/swift/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/vm/custom_image.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/vm/custom_image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/vm/image_command_customizer.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/vm/image_command_customizer.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/contexts/watcher/audit_templates.py` & `rally-openstack-2.3.0/rally_openstack/task/contexts/watcher/audit_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/hooks/fault_injection.py` & `rally-openstack-2.3.0/rally_openstack/task/hooks/fault_injection.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenario.py` & `rally-openstack-2.3.0/rally_openstack/task/scenario.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/authenticate/authenticate.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/authenticate/authenticate.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/containers.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @validation.add("required_services", services=[consts.Service.BARBICAN])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(name="BarbicanContainers.list")
 class BarbicanContainersList(utils.BarbicanBase):
     def run(self):
-        """List secrets."""
+        """List Containers."""
         self.admin_barbican.list_container()
 
 
 @validation.add("required_services", services=[consts.Service.BARBICAN])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(name="BarbicanContainers.create_and_delete")
 class BarbicanContainersGenericCreateAndDelete(utils.BarbicanBase):
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/orders.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @validation.add("required_services", services=[consts.Service.BARBICAN])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(name="BarbicanOrders.list")
 class BarbicanOrdersList(utils.BarbicanBase):
     def run(self):
-        """List secrets."""
+        """List Orders."""
         self.admin_barbican.orders_list()
 
 
 @validation.add("required_services", services=[consts.Service.BARBICAN])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(name="BarbicanOrders.create_key_and_delete")
 class BarbicanOrdersCreateKeyAndDelete(utils.BarbicanBase):
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/secrets.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/secrets.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/barbican/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/barbican/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/qos_specs.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/qos_specs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volume_backups.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volume_backups.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @scenario.configure(
     context={"cleanup@openstack": ["cinder"]},
     name="CinderVolumeBackups.create_incremental_volume_backup",
     platform="openstack")
 class CreateIncrementalVolumeBackup(cinder_utils.CinderBasic):
     def run(self, size, do_delete=True, create_volume_kwargs=None,
             create_backup_kwargs=None):
-        """Create a incremental volume backup.
+        """Create an incremental volume backup.
 
         The scenario first create a volume, the create a backup, the backup
         is full backup. Because Incremental backup must be based on the
         full backup. finally create a incremental backup.
 
         :param size: volume size in GB
         :param do_delete: deletes backup and volume after creating if True
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volume_types.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volume_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from rally.common import logging
 from rally.task import validation
 
 from rally_openstack.common import consts
-from rally_openstack.common.services.storage import cinder_v2
 from rally_openstack.task import scenario
 from rally_openstack.task.scenarios.cinder import utils as cinder_utils
 
 
 LOG = logging.getLogger(__name__)
 
 
@@ -68,40 +67,44 @@
 @validation.add("required_services", services=[consts.Service.CINDER])
 @validation.add("required_api_versions", component="cinder",
                 versions=["2", "3"])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(context={"admin_cleanup@openstack": ["cinder"]},
                     name="CinderVolumeTypes.create_and_update_volume_type",
                     platform="openstack")
-class CreateAndUpdateVolumeType(scenario.OpenStackScenario):
+class CreateAndUpdateVolumeType(cinder_utils.CinderBasic):
 
     def run(self, description=None, is_public=True, update_name=False,
             update_description=None, update_is_public=None):
         """create a volume type, then update the type.
 
         :param description: Description of the volume type
         :param is_public: Volume type visibility
         :param update_name: if True, can update name by generating random name.
                             if False, don't update name.
-        :param update_description: update Description of the volume type
+        :param update_description: a description to set while update
         :param update_is_public: update Volume type visibility
         """
-        service = cinder_v2.CinderV2Service(self._admin_clients,
-                                            self.generate_random_name,
-                                            atomic_inst=self.atomic_actions())
-
-        volume_type = service.create_volume_type(
+        volume_type = self.admin_cinder.create_volume_type(
             description=description,
             is_public=is_public)
 
-        service.update_volume_type(
+        updated_name = self.generate_random_name() if update_name else None
+        if not update_name and not update_description and not update_is_public:
+            LOG.warning("Something should be updated.")
+            # transmit at least some value to update api call
+            updated_name = volume_type.name
+
+        updated_is_public = not is_public if update_is_public else None
+
+        self.admin_cinder.update_volume_type(
             volume_type,
-            name=volume_type.name if not update_name else False,
+            name=updated_name,
             description=update_description,
-            is_public=update_is_public)
+            is_public=updated_is_public)
 
 
 @validation.add("required_services", services=[consts.Service.CINDER])
 @validation.add("required_platform", platform="openstack", admin=True)
 @scenario.configure(context={"admin_cleanup@openstack": ["cinder"]},
                     name="CinderVolumeTypes.create_and_list_volume_types",
                     platform="openstack")
@@ -384,26 +387,25 @@
 @validation.add("required_api_versions", component="cinder",
                 versions=["2", "3"])
 @validation.add("required_services", services=consts.Service.CINDER)
 @scenario.configure(
     context={"admin_cleanup@openstack": ["cinder"]},
     name="CinderVolumeTypes.create_volume_type_add_and_list_type_access",
     platform="openstack")
-class CreateVolumeTypeAddAndListTypeAccess(scenario.OpenStackScenario):
+class CreateVolumeTypeAddAndListTypeAccess(cinder_utils.CinderBasic):
 
     def run(self, description=None, is_public=False):
         """Add and list volume type access for the given project.
 
         This scenario first creates a private volume type, then add project
         access and list project access to it.
 
         :param description: Description of the volume type
         :param is_public: Volume type visibility
         """
-        service = cinder_v2.CinderV2Service(self._admin_clients,
-                                            self.generate_random_name,
-                                            atomic_inst=self.atomic_actions())
-        volume_type = service.create_volume_type(description=description,
-                                                 is_public=is_public)
-        service.add_type_access(volume_type,
-                                project=self.context["tenant"]["id"])
-        service.list_type_access(volume_type)
+        volume_type = self.admin_cinder.create_volume_type(
+            description=description, is_public=is_public
+        )
+        self.admin_cinder.add_type_access(
+            volume_type, project=self.context["tenant"]["id"]
+        )
+        self.admin_cinder.list_type_access(volume_type)
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/cinder/volumes.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/cinder/volumes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/basic.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/designate/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/designate/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/dummy.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/elasticsearch/logging.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/elasticsearch/logging.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/glance/images.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/glance/images.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/archive_policy.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/archive_policy.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/archive_policy_rule.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/archive_policy_rule.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/capabilities.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/capabilities.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/metric.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/metric.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/resource.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/resource.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/resource_type.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/resource_type.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/status.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/status.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/gnocchi/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/gnocchi/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/grafana/metrics.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/grafana/metrics.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/stacks.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/stacks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/heat/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/heat/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/nodes.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/nodes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/ironic/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/ironic/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/keystone/basic.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/keystone/basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/cluster_templates.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/cluster_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/clusters.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/k8s_pods.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/k8s_pods.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/magnum/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/magnum/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/shares.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/shares.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             image, flavor, use_floating_ip=use_floating_ip,
             floating_network=floating_network,
             key_name=self.context["user"]["keypair"]["name"],
             userdata="#cloud-config\npackages:\n - nfs-common",
             **kwargs)
         self._allow_access_share(share, "ip", fip["ip"], "rw")
         mount_opt = "-t nfs -o nfsvers=4.1,proto=tcp"
-        script = f"cloud-init status -w;" \
+        script = f"sudo cloud-init status -w;" \
                  f"sudo mount {mount_opt} {location[0]} /mnt || exit 1;" \
                  f"sudo touch /mnt/testfile || exit 2"
 
         command = {
             "script_inline": script,
             "interpreter": "/bin/bash"
         }
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/manila/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/manila/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     @atomic.action_timer("manila.extend_share")
     def _extend_share(self, share, new_size):
         """Extend the given share
 
         :param share: :class:`Share`
         :param new_size: new size of the share
         """
-        share.extend(new_size)
+        self.clients("manila").shares.extend(share, new_size)
         utils.wait_for_status(
             share,
             ready_statuses=["available"],
             update_resource=utils.get_from_manager(),
             timeout=CONF.openstack.manila_share_create_timeout,
             check_interval=CONF.openstack.manila_share_create_poll_interval)
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/executions.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/executions.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/mistral/workbooks.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/mistral/workbooks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/metrics.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/metrics.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/monasca/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/monasca/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/environments.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/environments.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/packages.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/packages.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/murano/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/murano/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/bgpvpn.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/bgpvpn.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/loadbalancer_v1.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/loadbalancer_v1.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/loadbalancer_v2.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/loadbalancer_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/network.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/security_groups.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/security_groups.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/trunk.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/trunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @validation.add("required_services", services=[consts.Service.NEUTRON])
 @validation.add("required_platform", platform="openstack", users=True)
 @scenario.configure(context={"cleanup@openstack": ["neutron"]},
                     name="NeutronTrunks.create_and_list_trunks")
 class CreateAndListTrunks(neutron_utils.NeutronScenario):
 
     def run(self, network_create_args=None, subport_count=10):
-        """Create and a given number of trunks with subports and list all trunks
+        """Create a given number of trunks with subports and list all trunks.
 
         :param network_create_args: dict, POST /v2.0/networks request
                                     options. Deprecated.
         :param trunk_count: int, number of trunk ports
         :param subport_count: int, number of subports per trunk
         """
         net = self._create_network(network_create_args or {})
@@ -50,18 +50,16 @@
         subport_payload = [{"port_id": p["port"]["id"],
                             "segmentation_type": "vlan",
                             "segmentation_id": seg_id}
                            for seg_id, p in enumerate(subports, start=1)]
         trunk_payload = {"port_id": parent["port"]["id"],
                          "sub_ports": subport_payload}
         trunk = self._create_trunk(trunk_payload)
-        self._update_port(parent, {"device_id": "sometrunk"})
         self._list_trunks()
         self._list_subports_by_trunk(trunk["trunk"]["id"])
-        self._list_ports_by_device_id("sometrunk")
 
 
 @types.convert(image={"type": "glance_image"},
                flavor={"type": "nova_flavor"})
 @validation.add("image_valid_on_flavor", flavor_param="flavor",
                 image_param="image")
 @validation.add("required_services", services=(consts.Service.NOVA,
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/neutron/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/neutron/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/agents.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 
 """Scenarios for Nova agents."""
 
 
 @validation.add("required_services", services=[consts.Service.NOVA])
 @validation.add("required_platform", platform="openstack", admin=True)
-@scenario.configure(name="NovaAgents.list_agents", platform="openstack")
-class ListAgents(utils.NovaScenario):
-    def run(self, hypervisor=None):
-        """List all builds.
-
-        Measure the "nova agent-list" command performance.
-
-        :param hypervisor: List agent builds on a specific hypervisor.
-                           None (default value) means list for all
-                           hypervisors
+@scenario.configure(name="NovaServices.list_services", platform="openstack")
+class ListServices(utils.NovaScenario):
+
+    def run(self, host=None, binary=None):
+        """List all nova services.
+
+        Measure the "nova service-list" command performance.
+
+        :param host: List nova services on host
+        :param binary: List nova services matching given binary
         """
-        self._list_agents(hypervisor)
+        self._list_services(host, binary)
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/aggregates.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/aggregates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/availability_zones.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/availability_zones.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/flavors.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/flavors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/hypervisors.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/hypervisors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/keypairs.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/keypairs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/server_groups.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/server_groups.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/servers.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,14 +487,69 @@
 
         if do_delete:
             self._detach_volume(server, volume)
             self.cinder.delete_volume(volume)
             self._delete_server(server, force=force_delete)
 
 
+@types.convert(image={"type": "glance_image"},
+               flavor={"type": "nova_flavor"})
+@validation.add("image_valid_on_flavor", flavor_param="flavor",
+                image_param="image")
+@validation.add("required_services", services=[consts.Service.NOVA,
+                                               consts.Service.CINDER])
+@validation.add("required_platform", platform="openstack", users=True)
+@scenario.configure(
+    context={"cleanup@openstack": ["cinder", "nova"]},
+    name="NovaServers.boot_server_attach_created_volume_and_extend",
+    platform="openstack")
+class BootServerAttachCreatedVolumeAndExtend(utils.NovaScenario,
+                                             cinder_utils.CinderBasic):
+
+    def run(self, image, flavor, volume_size, new_volume_size, min_sleep=0,
+            max_sleep=0, force_delete=False, do_delete=True,
+            boot_server_kwargs=None, create_volume_kwargs=None):
+        """Create a VM from image, attach a volume then extend volume
+
+        Simple test to create a VM and attach a volume, then extend the
+        volume while its running, detach the volume then delete volume
+        and VM.
+
+        Optional 'min_sleep' and 'max_sleep' parameters allow the scenario
+        to simulate a pause between attaching a volume and running resize
+        (of random duration from range [min_sleep, max_sleep]).
+
+        :param image: Glance image name to use for the VM
+        :param flavor: VM flavor name
+        :param volume_size: volume size (in GB)
+        :param new_volume_size: new volume size (in GB)
+        :param min_sleep: Minimum sleep time in seconds (non-negative)
+        :param max_sleep: Maximum sleep time in seconds (non-negative)
+        :param force_delete: True if force_delete should be used
+        :param do_delete: True if resources needs to be deleted explicitly
+                        else use rally cleanup to remove resources
+        :param boot_server_kwargs: optional arguments for VM creation
+        :param create_volume_kwargs: optional arguments for volume creation
+        """
+        boot_server_kwargs = boot_server_kwargs or {}
+        create_volume_kwargs = create_volume_kwargs or {}
+
+        server = self._boot_server(image, flavor, **boot_server_kwargs)
+        volume = self.cinder.create_volume(volume_size, **create_volume_kwargs)
+
+        self._attach_volume(server, volume)
+        self.sleep_between(min_sleep, max_sleep)
+        self.cinder.extend_volume(volume, new_size=new_volume_size)
+
+        if do_delete:
+            self._detach_volume(server, volume)
+            self.cinder.delete_volume(volume)
+            self._delete_server(server, force=force_delete)
+
+
 @validation.add("number", param_name="volume_num", minval=1,
                 integer_only=True)
 @validation.add("number", param_name="volume_size", minval=1,
                 integer_only=True)
 @types.convert(image={"type": "glance_image"},
                flavor={"type": "nova_flavor"})
 @validation.add("image_valid_on_flavor", flavor_param="flavor",
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/services.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_services.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,31 +9,21 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from rally.task import validation
+from unittest import mock
 
-from rally_openstack.common import consts
-from rally_openstack.task import scenario
-from rally_openstack.task.scenarios.nova import utils
+from rally_openstack.task.scenarios.nova import services
+from tests.unit import test
 
 
-"""Scenarios for Nova agents."""
+class NovaServicesTestCase(test.TestCase):
 
-
-@validation.add("required_services", services=[consts.Service.NOVA])
-@validation.add("required_platform", platform="openstack", admin=True)
-@scenario.configure(name="NovaServices.list_services", platform="openstack")
-class ListServices(utils.NovaScenario):
-
-    def run(self, host=None, binary=None):
-        """List all nova services.
-
-        Measure the "nova service-list" command performance.
-
-        :param host: List nova services on host
-        :param binary: List nova services matching given binary
-        """
-        self._list_services(host, binary)
+    def test_list_services(self):
+        scenario = services.ListServices()
+        scenario._list_services = mock.Mock()
+        scenario.run(host="foo_host", binary="foo_hypervisor")
+        scenario._list_services.assert_called_once_with("foo_host",
+                                                        "foo_hypervisor")
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/nova/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/nova/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,22 @@
         utils.wait_for_status(
             server,
             ready_statuses=["SHELVED_OFFLOADED"],
             update_resource=utils.get_from_manager(),
             timeout=CONF.openstack.nova_server_shelve_timeout,
             check_interval=CONF.openstack.nova_server_shelve_poll_interval
         )
+        utils.wait_for_status(
+            server,
+            ready_statuses=["None"],
+            status_attr="OS-EXT-STS:task_state",
+            update_resource=utils.get_from_manager(),
+            timeout=CONF.openstack.nova_server_shelve_timeout,
+            check_interval=CONF.openstack.nova_server_shelve_poll_interval
+        )
 
     @atomic.action_timer("nova.unshelve_server")
     def _unshelve_server(self, server):
         """Unshelve the given server.
 
         Returns when the server is unshelved and is in the "ACTIVE" state.
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/loadbalancers.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/pools.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/pools.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/octavia/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/octavia/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/quotas.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/quotas/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/quotas/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/clusters.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/consts.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/consts.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/jobs.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/jobs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/node_group_templates.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/node_group_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/sahara/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/sahara/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/clusters.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/senlin/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/senlin/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/objects.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/objects.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/swift/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/swift/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/vmtasks.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/vmtasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
 
         server, fip = self._boot_server_with_fip(
             image, flavor, use_floating_ip=use_floating_ip,
             floating_network=floating_network,
             key_name=self.context["user"]["keypair"]["name"],
             **kwargs)
 
-        script = f"cloud-init status -w; systemd-resolve --status; "\
+        script = f"cloud-init status -w; resolvectl status; "\
                  f"dig $(hostname).{zone}"
 
         command = {
             "script_inline": script,
             "interpreter": "/bin/bash"
         }
         try:
```

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/vm/workloads/siege.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/vm/workloads/siege.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/basic.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/watcher/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/watcher/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/basic.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/scenarios/zaqar/utils.py` & `rally-openstack-2.3.0/rally_openstack/task/scenarios/zaqar/utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/types.py` & `rally-openstack-2.3.0/rally_openstack/task/types.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/task/ui/charts/osprofilerchart.py` & `rally-openstack-2.3.0/rally_openstack/task/ui/charts/osprofilerchart.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/verification/tempest/config.ini` & `rally-openstack-2.3.0/rally_openstack/verification/tempest/config.ini`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/verification/tempest/config.py` & `rally-openstack-2.3.0/rally_openstack/verification/tempest/config.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/verification/tempest/consts.py` & `rally-openstack-2.3.0/rally_openstack/verification/tempest/consts.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/verification/tempest/context.py` & `rally-openstack-2.3.0/rally_openstack/verification/tempest/context.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack/verification/tempest/manager.py` & `rally-openstack-2.3.0/rally_openstack/verification/tempest/manager.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/rally_openstack.egg-info/PKG-INFO` & `rally-openstack-2.3.0/rally_openstack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rally-openstack
-Version: 2.2.0
+Version: 2.3.0
 Summary: Rally plugins for OpenStack platform
 Home-page: https://docs.openstack.org/rally/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ===============
         rally-openstack
```

### Comparing `rally-openstack-2.2.0/rally_openstack.egg-info/SOURCES.txt` & `rally-openstack-2.3.0/rally_openstack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,14 @@
 rally_openstack/task/scenarios/neutron/loadbalancer_v1.py
 rally_openstack/task/scenarios/neutron/loadbalancer_v2.py
 rally_openstack/task/scenarios/neutron/network.py
 rally_openstack/task/scenarios/neutron/security_groups.py
 rally_openstack/task/scenarios/neutron/trunk.py
 rally_openstack/task/scenarios/neutron/utils.py
 rally_openstack/task/scenarios/nova/__init__.py
-rally_openstack/task/scenarios/nova/agents.py
 rally_openstack/task/scenarios/nova/aggregates.py
 rally_openstack/task/scenarios/nova/availability_zones.py
 rally_openstack/task/scenarios/nova/flavors.py
 rally_openstack/task/scenarios/nova/hypervisors.py
 rally_openstack/task/scenarios/nova/keypairs.py
 rally_openstack/task/scenarios/nova/server_groups.py
 rally_openstack/task/scenarios/nova/servers.py
@@ -1027,14 +1026,16 @@
 samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.yaml
 samples/tasks/scenarios/nova/boot-server-and-attach-interface.json
 samples/tasks/scenarios/nova/boot-server-and-attach-interface.yaml
 samples/tasks/scenarios/nova/boot-server-and-list-interfaces.json
 samples/tasks/scenarios/nova/boot-server-and-list-interfaces.yaml
 samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.json
 samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.yaml
+samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-extend.json
+samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-extend.yaml
 samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.json
 samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.yaml
 samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.json
 samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.yaml
 samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.json
 samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.yaml
 samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.json
@@ -1075,16 +1076,14 @@
 samples/tasks/scenarios/nova/create-and-update-aggregate.yaml
 samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.json
 samples/tasks/scenarios/nova/create-flavor-and-add-tenant-access.yaml
 samples/tasks/scenarios/nova/create-flavor-and-set-keys.json
 samples/tasks/scenarios/nova/create-flavor-and-set-keys.yaml
 samples/tasks/scenarios/nova/create-flavor.json
 samples/tasks/scenarios/nova/create-flavor.yaml
-samples/tasks/scenarios/nova/list-agents.json
-samples/tasks/scenarios/nova/list-agents.yaml
 samples/tasks/scenarios/nova/list-aggregates.json
 samples/tasks/scenarios/nova/list-aggregates.yaml
 samples/tasks/scenarios/nova/list-and-get-hypervisors.json
 samples/tasks/scenarios/nova/list-and-get-hypervisors.yaml
 samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.json
 samples/tasks/scenarios/nova/list-and-get-uptime-hypervisors.yaml
 samples/tasks/scenarios/nova/list-and-search-hypervisor.json
@@ -1253,25 +1252,23 @@
 tests/ci/playbooks/roles/prepare-for-rally-task/defaults/main.yaml
 tests/ci/playbooks/roles/prepare-for-rally-task/library/__init__.py
 tests/ci/playbooks/roles/prepare-for-rally-task/library/make_env_spec_with_existing_users.py
 tests/ci/playbooks/roles/prepare-for-rally-task/tasks/main.yaml
 tests/ci/playbooks/roles/prepare-for-rally-task/tasks/prepare-env-with-existing-users.yaml
 tests/ci/playbooks/roles/process-task-results/tasks/main.yaml
 tests/ci/playbooks/roles/run-rally-task/tasks/main.yaml
-tests/ci/playbooks/roles/tox-install/tasks/main.yaml
 tests/ci/playbooks/roles/tox-run/tasks/main.yaml
 tests/functional/__init__.py
 tests/functional/test_certification_task.py
 tests/functional/test_cli_deployment.py
 tests/functional/test_cli_env.py
 tests/functional/test_cli_task.py
 tests/functional/test_task_samples.py
 tests/functional/utils.py
 tests/functional/extra/fake_dir/fake_plugin.py
-tests/hacking/README.rst
 tests/hacking/__init__.py
 tests/hacking/checks.py
 tests/unit/__init__.py
 tests/unit/fakes.py
 tests/unit/test.py
 tests/unit/test__compat.py
 tests/unit/test_ddt.py
@@ -1469,15 +1466,14 @@
 tests/unit/task/scenarios/neutron/test_loadbalancer_v1.py
 tests/unit/task/scenarios/neutron/test_loadbalancer_v2.py
 tests/unit/task/scenarios/neutron/test_network.py
 tests/unit/task/scenarios/neutron/test_security_groups.py
 tests/unit/task/scenarios/neutron/test_trunk.py
 tests/unit/task/scenarios/neutron/test_utils.py
 tests/unit/task/scenarios/nova/__init__.py
-tests/unit/task/scenarios/nova/test_agents.py
 tests/unit/task/scenarios/nova/test_aggregates.py
 tests/unit/task/scenarios/nova/test_availability_zones.py
 tests/unit/task/scenarios/nova/test_flavors.py
 tests/unit/task/scenarios/nova/test_hypervisors.py
 tests/unit/task/scenarios/nova/test_keypairs.py
 tests/unit/task/scenarios/nova/test_server_groups.py
 tests/unit/task/scenarios/nova/test_servers.py
```

### Comparing `rally-openstack-2.2.0/rally_openstack.egg-info/requires.txt` & `rally-openstack-2.3.0/rally_openstack.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-gnocchiclient!=7.0.7
+gnocchiclient
 keystoneauth1
 kubernetes
 os-faults>=0.2.0
 osprofiler
 python-barbicanclient
 python-cinderclient!=4.0.0
 python-designateclient
@@ -20,9 +20,9 @@
 python-octaviaclient
 python-saharaclient
 python-senlinclient
 python-swiftclient
 python-troveclient
 python-watcherclient
 python-zaqarclient
-rally>=3.1.0
+rally>=3.4.0
 requests!=2.20.0,!=2.24.0
```

### Comparing `rally-openstack-2.2.0/requirements.txt` & `rally-openstack-2.3.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 requests!=2.20.0,!=2.24.0                              # Apache License, Version 2.0
 
-rally>=3.1.0                                           # Apache License, Version 2.0
+rally>=3.4.0                                           # Apache License, Version 2.0
 
 # OpenStack related
-gnocchiclient!=7.0.7                                   # Apache Software License
+gnocchiclient                                          # Apache Software License
 keystoneauth1                                          # Apache Software License
 kubernetes                                             # Apache License Version 2.0
 os-faults>=0.2.0                                       # Apache Software License
 osprofiler                                             # Apache Software License
 python-barbicanclient                                  # Apache Software License
 python-cinderclient!=4.0.0                             # Apache Software License
 python-designateclient                                 # Apache License, Version 2.0
@@ -24,11 +24,11 @@
 python-muranoclient                                    # Apache License, Version 2.0
 python-monascaclient                                   # Apache Software License
 python-neutronclient                                   # Apache Software License
 python-novaclient                                      # Apache License, Version 2.0
 python-octaviaclient                                   # Apache Software License
 python-saharaclient                                    # Apache License, Version 2.0
 python-senlinclient                                    # Apache Software License
-python-swiftclient                                     # Apache Software License
+python-swiftclient                                     # Apache License, Version 2.0
 python-troveclient                                     # Apache Software License
 python-watcherclient                                   # Apache Software License
 python-zaqarclient                                     # Apache Software License
```

### Comparing `rally-openstack-2.2.0/samples/deployments/README.rst` & `rally-openstack-2.3.0/samples/deployments/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/deployments/existing-api.json` & `rally-openstack-2.3.0/samples/deployments/existing-api.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/deployments/existing-keystone-v3-osprofiler.json` & `rally-openstack-2.3.0/samples/deployments/existing-keystone-v3-osprofiler.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/deployments/existing-with-predefined-users.json` & `rally-openstack-2.3.0/samples/deployments/existing-with-predefined-users.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/README.rst` & `rally-openstack-2.3.0/samples/tasks/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/api-versions.json` & `rally-openstack-2.3.0/samples/tasks/contexts/api-versions.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/audit-templates.json` & `rally-openstack-2.3.0/samples/tasks/contexts/audit-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/audit-templates.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/audit-templates.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/ca-certs.json` & `rally-openstack-2.3.0/samples/tasks/contexts/ca-certs.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/ca-certs.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/ca-certs.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/cluster-templates.json` & `rally-openstack-2.3.0/samples/tasks/contexts/cluster-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/cluster-templates.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/cluster-templates.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/clusters.json` & `rally-openstack-2.3.0/samples/tasks/contexts/clusters.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/clusters.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/clusters.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/dummy-context.json` & `rally-openstack-2.3.0/samples/tasks/contexts/dummy-context.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/flavors.json` & `rally-openstack-2.3.0/samples/tasks/contexts/flavors.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/heat-dataplane.json` & `rally-openstack-2.3.0/samples/tasks/contexts/heat-dataplane.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/heat-dataplane.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/heat-dataplane.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/image-command-customizer.json` & `rally-openstack-2.3.0/samples/tasks/contexts/image-command-customizer.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/image-command-customizer.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/image-command-customizer.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/images.json` & `rally-openstack-2.3.0/samples/tasks/contexts/images.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'Dummy.openstack'": "{0: {'context': {'images': {'image_url': "*

 * *                      "'http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img'}}}}"}*

```diff
@@ -4,15 +4,15 @@
             "args": {
                 "sleep": 0.1
             },
             "context": {
                 "images": {
                     "image_container": "bare",
                     "image_type": "qcow2",
-                    "image_url": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img",
+                    "image_url": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img",
                     "images_per_tenant": 4
                 },
                 "users": {
                     "tenants": 1,
                     "users_per_tenant": 2
                 }
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/lbaas.json` & `rally-openstack-2.3.0/samples/tasks/contexts/lbaas.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/lbaas.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/lbaas.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/contexts/loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-security-services.json` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-security-services.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-security-services.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-security-services.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-share-networks.json` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-share-networks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-share-networks.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-share-networks.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-shares.json` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-shares.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/manila-shares.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/manila-shares.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/monasca-metrics.json` & `rally-openstack-2.3.0/samples/tasks/contexts/monasca-metrics.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/murano-environments.json` & `rally-openstack-2.3.0/samples/tasks/contexts/murano-environments.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/murano-packages.json` & `rally-openstack-2.3.0/samples/tasks/contexts/murano-packages.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/murano-packages.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/murano-packages.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/network.json` & `rally-openstack-2.3.0/samples/tasks/contexts/network.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/network.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/network.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/profiles.json` & `rally-openstack-2.3.0/samples/tasks/contexts/profiles.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222221%*

 * *Differences: {"'Dummy.openstack'": "{0: {'context': {'profiles': {'properties': {'image': "*

 * *                      "'cirros-0.5.2-x86_64-disk'}}}}}"}*

```diff
@@ -4,15 +4,15 @@
             "args": {
                 "sleep": 0.1
             },
             "context": {
                 "profiles": {
                     "properties": {
                         "flavor": 1,
-                        "image": "cirros-0.3.5-x86_64-disk",
+                        "image": "cirros-0.5.2-x86_64-disk",
                         "name": "cirros_server",
                         "networks": [
                             {
                                 "network": "private"
                             }
                         ]
                     },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/quotas.json` & `rally-openstack-2.3.0/samples/tasks/contexts/quotas.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/quotas.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/quotas.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/router.json` & `rally-openstack-2.3.0/samples/tasks/contexts/router.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-cluster.json` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-cluster.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-image.json` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-image.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-input-data-sources.json` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-input-data-sources.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-job-binaries.json` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-job-binaries.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-job-binaries.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-job-binaries.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/sahara-output-data-sources.json` & `rally-openstack-2.3.0/samples/tasks/contexts/sahara-output-data-sources.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/servers.json` & `rally-openstack-2.3.0/samples/tasks/contexts/servers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/stacks.json` & `rally-openstack-2.3.0/samples/tasks/contexts/stacks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/swift-objects.json` & `rally-openstack-2.3.0/samples/tasks/contexts/swift-objects.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/users.json` & `rally-openstack-2.3.0/samples/tasks/contexts/users.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/users.yaml` & `rally-openstack-2.3.0/samples/tasks/contexts/users.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/contexts/volumes.json` & `rally-openstack-2.3.0/samples/tasks/contexts/volumes.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-ceilometer.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-cinder.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-cinder.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-glance.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-glance.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-heat.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-heat.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-monasca.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-monasca.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-neutron.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-neutron.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-nova.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-nova.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/authenticate/token-validate-octavia.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/authenticate/token-validate-octavia.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/barbican/create-and-delete-symmetric-secret.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/creat-qos-and-associate-type.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-accept-transfer.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-attach-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-attach-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-attach-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-attach-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-encryption-type.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-snapshot.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-delete-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-delete-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-extend-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-extend-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-extend-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-extend-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-qos.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-qos.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-get-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-get-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-encryption-type.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-qos.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-qos.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-snapshots.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-backups.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume-types.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-list-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-list-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-restore-volume-backup.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-qos.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-qos.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-set-volume-type-keys.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-encryption-type.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-readonly-flag.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-update-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-update-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-and-upload-volume-to-image.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-encryption-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-encryption-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-image-and-delete-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-from-volume-and-delete-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-get-and-delete-encryption-type.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-incremental-volume-backup.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-nested-snapshots-and-attach-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-snapshot-and-attach-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-and-clone.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-and-clone.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-and-clone.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-and-clone.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-backup.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-backup.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-from-snapshot.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume-type-add-and-list-type-access.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/create-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/create-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-transfers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-transfers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-types.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-types.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/list-volumes.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/list-volumes.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/cinder/modify-volume-metadata.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/cinder/modify-volume-metadata.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'DesignateBasic.create_and_delete_recordsets'": "{0: {'context': {'quotas': {'designate': "*

 * *                                                  "{'zone_recordsets': 2000, 'zone_records': 2000, "*

 * *                                                  "delete: ['zones_recordsets', "*

 * *                                                  "'zones_records']}}}}}"}*

```diff
@@ -4,17 +4,17 @@
             "args": {
                 "recordsets_per_zone": 10
             },
             "context": {
                 "quotas": {
                     "designate": {
                         "recordset_records": 2000,
-                        "zones": 100,
-                        "zones_records": 2000,
-                        "zones_recordsets": 2000
+                        "zone_records": 2000,
+                        "zone_recordsets": 2000,
+                        "zones": 100
                     }
                 },
                 "users": {
                     "tenants": 2,
                     "users_per_tenant": 2
                 },
                 "zones": {
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-recordsets.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         type: "constant"
         times: 10
         concurrency: 10
       context:
         quotas:
           designate:
             zones: 100
-            zones_recordsets: 2000
-            zones_records: 2000
+            zone_recordsets: 2000
+            zone_records: 2000
             recordset_records: 2000
         users:
           tenants: 2
           users_per_tenant: 2
         zones:
           zones_per_tenant: 1
       sla:
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-delete-zone.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-delete-zone.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'DesignateBasic.create_and_delete_zone'": "{0: {'context': {'quotas': {'designate': "*

 * *                                            "{'zone_recordsets': 500, 'zone_records': 2000, "*

 * *                                            "delete: ['zones_recordsets', 'zones_records']}}}}}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "DesignateBasic.create_and_delete_zone": [
         {
             "context": {
                 "quotas": {
                     "designate": {
                         "recordset_records": 2000,
-                        "zones": 100,
-                        "zones_records": 2000,
-                        "zones_recordsets": 500
+                        "zone_records": 2000,
+                        "zone_recordsets": 500,
+                        "zones": 100
                     }
                 },
                 "users": {
                     "tenants": 2,
                     "users_per_tenant": 2
                 }
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-recordsets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-recordsets.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'DesignateBasic.create_and_list_recordsets'": "{0: {'context': {'quotas': {'designate': "*

 * *                                                "{'zone_recordsets': 2000, 'zone_records': 2000, "*

 * *                                                "delete: ['zones_recordsets', "*

 * *                                                "'zones_records']}}}}}"}*

```diff
@@ -4,17 +4,17 @@
             "args": {
                 "recordsets_per_zone": 10
             },
             "context": {
                 "quotas": {
                     "designate": {
                         "recordset_records": 2000,
-                        "zones": 100,
-                        "zones_records": 2000,
-                        "zones_recordsets": 2000
+                        "zone_records": 2000,
+                        "zone_recordsets": 2000,
+                        "zones": 100
                     }
                 },
                 "users": {
                     "tenants": 2,
                     "users_per_tenant": 2
                 },
                 "zones": {
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-recordsets.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-recordsets.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         type: "constant"
         times: 10
         concurrency: 10
       context:
         quotas:
           designate:
             zones: 100
-            zones_recordsets: 2000
-            zones_records: 2000
+            zone_recordsets: 2000
+            zone_records: 2000
             recordset_records: 2000
         users:
           tenants: 2
           users_per_tenant: 2
         zones:
           zones_per_tenant: 1
       sla:
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/create-and-list-zones.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/create-and-list-zones.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'DesignateBasic.create_and_list_zones'": "{0: {'context': {'quotas': {'designate': "*

 * *                                           "{'zone_recordsets': 500, 'zone_records': 2000, delete: "*

 * *                                           "['zones_recordsets', 'zones_records']}}}}}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "DesignateBasic.create_and_list_zones": [
         {
             "context": {
                 "quotas": {
                     "designate": {
                         "recordset_records": 2000,
-                        "zones": 100,
-                        "zones_records": 2000,
-                        "zones_recordsets": 500
+                        "zone_records": 2000,
+                        "zone_recordsets": 500,
+                        "zones": 100
                     }
                 },
                 "users": {
                     "tenants": 2,
                     "users_per_tenant": 2
                 }
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/designate/list-recordsets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/designate/list-recordsets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/elasticsearch/log-instance.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/elasticsearch/log-instance.json`

 * *Files 8% similar despite different names*

```diff
@@ -56,21 +56,21 @@
                         "ram": 512,
                         "disk": 1,
                         "vcpus": 1
                     }
                 ],
                 "images": {
                     "image_name": "{{ image_name }}",
-                    "image_url": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img",
+                    "image_url": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img",
                     "disk_format": "qcow2",
                     "container_format": "bare",
                     "visibility": "public"
                 }
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
             }
         }
     ]
-}
+}
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/elasticsearch/log-instance.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-from-instance.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-{% set flavor_name = flavor_name or "esc_test.small" %}
+{% set flavor_name = flavor_name or "grafana_test.small" %}
 {% set image_name = image_name or "testVM" %}
 ---
-  ElasticsearchLogging.log_instance:
+  GrafanaMetrics.push_metric_from_instance:
     -
       args:
         flavor:
           name: {{ flavor_name }}
         image:
           name: {{ image_name }}
-        logging_vip: 10.0.0.5
-        elasticsearch_port: 5601
+        monitor_vip: 10.0.0.5
+        pushgateway_port: 9091
+        grafana:
+          user: admin
+          password: password
+          port: 3000
+        datasource_id: 1
+        job_name: rally_test
         sleep_time: 5
         retries_total: 30
-        additional_query:
-          must_not:
-          - match_phrase:
-              Payload: GET
-          - match_phrase:
-              http_method: GET
-          should:
-          - range:
-              Timestamp:
-                gte: now-2m
-                lte: now
-          minimum_should_match: 1
       runner:
         type: "constant"
         times: 10
         concurrency: 1
       context:
         users:
           tenants: 1
@@ -36,14 +30,14 @@
           -
             name: {{ flavor_name }}
             ram: 512
             disk: 1
             vcpus: 1
         images:
           image_name: {{ image_name }}
-          image_url: http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img
+          image_url: http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img
           disk_format: qcow2
           container_format: bare
           visibility: public
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-deactivate-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-deactivate-image.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'GlanceImages.create_and_deactivate_image'": "{0: {'args': {'image_location': "*

 * *                                               "'http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img'}}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "GlanceImages.create_and_deactivate_image": [
         {
             "args": {
                 "container_format": "bare",
                 "disk_format": "qcow2",
-                "image_location": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img"
+                "image_location": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img"
             },
             "context": {
                 "users": {
                     "tenants": 1,
                     "users_per_tenant": 1
                 }
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-delete-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-delete-image.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'GlanceImages.create_and_delete_image'": "{0: {'args': {'image_location': "*

 * *                                           "'http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img'}}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "GlanceImages.create_and_delete_image": [
         {
             "args": {
                 "container_format": "bare",
                 "disk_format": "qcow2",
-                "image_location": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img"
+                "image_location": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img"
             },
             "context": {
                 "users": {
                     "tenants": 2,
                     "users_per_tenant": 3
                 }
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-download-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/list-images.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('GlanceImages.list_images', [OrderedDict([('runner', "*

 * *            "OrderedDict([('type', 'constant'), ('times', 10), ('concurrency', 1)])), ('context', "*

 * *            "OrderedDict([('users', OrderedDict([('tenants', 2), ('users_per_tenant', 2)])), "*

 * *            "('images', OrderedDict([('image_url', "*

 * *            "'http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img'), "*

 * *            "('disk_format', 'qcow2'), ('container_format', 'bare'), ('images_per_tenant', "*

 * *   […]*

```diff
@@ -1,23 +1,24 @@
 {
-    "GlanceImages.create_and_download_image": [
+    "GlanceImages.list_images": [
         {
-            "args": {
-                "container_format": "bare",
-                "disk_format": "qcow2",
-                "image_location": "http://download.cirros-cloud.net/0.3.4/cirros-0.3.4-x86_64-disk.img"
-            },
             "context": {
+                "images": {
+                    "container_format": "bare",
+                    "disk_format": "qcow2",
+                    "image_url": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img",
+                    "images_per_tenant": 4
+                },
                 "users": {
                     "tenants": 2,
-                    "users_per_tenant": 3
+                    "users_per_tenant": 2
                 }
             },
             "runner": {
-                "concurrency": 2,
+                "concurrency": 1,
                 "times": 10,
                 "type": "constant"
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-get-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('NovaAggregates.create_and_get_aggregate_details', "*

 * *            "[OrderedDict([('args', OrderedDict([('availability_zone', 'nova')])), ('runner', "*

 * *            "OrderedDict([('type', 'constant'), ('times', 10), ('concurrency', 2)])), ('context', "*

 * *            "OrderedDict([('users', OrderedDict([('tenants', 3), ('users_per_tenant', 2)]))])), "*

 * *            "('sla', OrderedDict([('failure_rate', OrderedDict([('max', 0)]))]))])])])"}*

```diff
@@ -1,24 +1,22 @@
 {
-    "GlanceImages.create_and_get_image": [
+    "NovaAggregates.create_and_get_aggregate_details": [
         {
             "args": {
-                "container_format": "bare",
-                "disk_format": "qcow2",
-                "image_location": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img"
+                "availability_zone": "nova"
             },
             "context": {
                 "users": {
-                    "tenants": 2,
+                    "tenants": 3,
                     "users_per_tenant": 2
                 }
             },
             "runner": {
                 "concurrency": 2,
-                "times": 4,
+                "times": 10,
                 "type": "constant"
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
             }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-list-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-list.json`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-00000000: 7b0a 2020 2020 2247 6c61 6e63 6549 6d61  {.    "GlanceIma
-00000010: 6765 732e 6372 6561 7465 5f61 6e64 5f6c  ges.create_and_l
-00000020: 6973 745f 696d 6167 6522 3a20 5b0a 2020  ist_image": [.  
-00000030: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00000040: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00000050: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00000060: 6d61 6765 5f6c 6f63 6174 696f 6e22 3a20  mage_location": 
-00000070: 2268 7474 703a 2f2f 646f 776e 6c6f 6164  "http://download
-00000080: 2e63 6972 726f 732d 636c 6f75 642e 6e65  .cirros-cloud.ne
-00000090: 742f 302e 332e 352f 6369 7272 6f73 2d30  t/0.3.5/cirros-0
-000000a0: 2e33 2e35 2d78 3836 5f36 342d 6469 736b  .3.5-x86_64-disk
-000000b0: 2e69 6d67 222c 0a20 2020 2020 2020 2020  .img",.         
-000000c0: 2020 2020 2020 2022 636f 6e74 6169 6e65         "containe
-000000d0: 725f 666f 726d 6174 223a 2022 6261 7265  r_format": "bare
-000000e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000000f0: 2020 2022 6469 736b 5f66 6f72 6d61 7422     "disk_format"
-00000100: 3a20 2271 636f 7732 220a 2020 2020 2020  : "qcow2".      
-00000110: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000120: 2020 2020 2022 7275 6e6e 6572 223a 207b       "runner": {
-00000130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000140: 2022 7479 7065 223a 2022 636f 6e73 7461   "type": "consta
-00000150: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-00000160: 2020 2020 2022 7469 6d65 7322 3a20 3130       "times": 10
-00000170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000180: 2020 2263 6f6e 6375 7272 656e 6379 223a    "concurrency":
-00000190: 2031 0a20 2020 2020 2020 2020 2020 207d   1.            }
-000001a0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
-000001b0: 6f6e 7465 7874 223a 207b 0a20 2020 2020  ontext": {.     
-000001c0: 2020 2020 2020 2020 2020 2022 7573 6572             "user
-000001d0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000001e0: 2020 2020 2020 2020 2020 2274 656e 616e            "tenan
-000001f0: 7473 223a 2031 2c0a 2020 2020 2020 2020  ts": 1,.        
-00000200: 2020 2020 2020 2020 2020 2020 2275 7365              "use
-00000210: 7273 5f70 6572 5f74 656e 616e 7422 3a20  rs_per_tenant": 
-00000220: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00000230: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000240: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00000250: 736c 6122 3a20 7b0a 2020 2020 2020 2020  sla": {.        
-00000260: 2020 2020 2020 2020 2266 6169 6c75 7265          "failure
-00000270: 5f72 6174 6522 3a20 7b0a 2020 2020 2020  _rate": {.      
-00000280: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00000290: 6178 223a 2030 0a20 2020 2020 2020 2020  ax": 0.         
-000002a0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000002b0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000002c0: 0a20 2020 205d 0a7d 0a                   .    ].}.
+00000000: 7b25 2073 6574 2066 6c61 766f 725f 6e61  {% set flavor_na
+00000010: 6d65 203d 2066 6c61 766f 725f 6e61 6d65  me = flavor_name
+00000020: 206f 7220 226d 312e 7469 6e79 2220 257d   or "m1.tiny" %}
+00000030: 0a7b 0a20 2020 2022 4e6f 7661 5365 7276  .{.    "NovaServ
+00000040: 6572 732e 626f 6f74 5f61 6e64 5f6c 6973  ers.boot_and_lis
+00000050: 745f 7365 7276 6572 223a 205b 0a20 2020  t_server": [.   
+00000060: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000070: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00000080: 2020 2020 2020 2020 2020 2020 2022 666c               "fl
+00000090: 6176 6f72 223a 207b 0a20 2020 2020 2020  avor": {.       
+000000a0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+000000b0: 6d65 223a 2022 7b7b 666c 6176 6f72 5f6e  me": "{{flavor_n
+000000c0: 616d 657d 7d22 0a20 2020 2020 2020 2020  ame}}".         
+000000d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000000e0: 2020 2020 2020 2020 2020 2269 6d61 6765            "image
+000000f0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000100: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+00000110: 2022 5e63 6972 726f 732e 2a2d 6469 736b   "^cirros.*-disk
+00000120: 2422 0a20 2020 2020 2020 2020 2020 2020  $".             
+00000130: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00000140: 2020 2020 2020 2264 6574 6169 6c65 6422        "detailed"
+00000150: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
+00000160: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00000170: 2020 2272 756e 6e65 7222 3a20 7b0a 2020    "runner": {.  
+00000180: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00000190: 7970 6522 3a20 2263 6f6e 7374 616e 7422  ype": "constant"
+000001a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000001b0: 2020 2274 696d 6573 223a 2031 2c0a 2020    "times": 1,.  
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000001d0: 6f6e 6375 7272 656e 6379 223a 2031 0a20  oncurrency": 1. 
+000001e0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000001f0: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00000200: 7874 223a 207b 0a20 2020 2020 2020 2020  xt": {.         
+00000210: 2020 2020 2020 2022 7573 6572 7322 3a20         "users": 
+00000220: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000230: 2020 2020 2020 2274 656e 616e 7473 223a        "tenants":
+00000240: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+00000250: 2020 2020 2020 2020 2275 7365 7273 5f70          "users_p
+00000260: 6572 5f74 656e 616e 7422 3a20 310a 2020  er_tenant": 1.  
+00000270: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00000280: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000290: 2020 2020 2020 2020 2020 2022 736c 6122             "sla"
+000002a0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000002b0: 2020 2020 2266 6169 6c75 7265 5f72 6174      "failure_rat
+000002c0: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+000002d0: 2020 2020 2020 2020 2020 226d 6178 223a            "max":
+000002e0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+000002f0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00000300: 207d 0a20 2020 2020 2020 207d 0a20 2020   }.        }.   
+00000310: 205d 0a7d 0a0a                            ].}..
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-and-update-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-update-image.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'GlanceImages.create_and_update_image'": "{0: {'args': {'image_location': "*

 * *                                           "'http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img'}}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "GlanceImages.create_and_update_image": [
         {
             "args": {
                 "container_format": "bare",
                 "disk_format": "qcow2",
-                "image_location": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img"
+                "image_location": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img"
             },
             "context": {
                 "api_versions": {
                     "glance": {
                         "version": 2
                     }
                 },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.json`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 {
     "GlanceImages.create_image_and_boot_instances": [
         {
             "args": {
-                "image_location": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img",
+                "image_location": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img",
                 "container_format": "bare",
                 "disk_format": "qcow2",
                 "flavor": {
                     "name": "{{flavor_name}}"
                 },
                 "number_instances": 2
             },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/create-image-and-boot-instances.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 ---
-  GlanceImages.create_image_and_boot_instances:
+  VMTasks.boot_runcommand_delete:
     -
       args:
-        image_location: "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img"
-        container_format: "bare"
-        disk_format: "qcow2"
         flavor:
             name: "{{flavor_name}}"
-        number_instances: 2
+        image:
+            name: "^cirros.*-disk$"
+        floating_network: "public"
+        force_delete: false
+        command:
+            interpreter: "/bin/sh"
+            script_inline: "ls -la"
+        username: "cirros"
       runner:
         type: "constant"
         times: 10
         concurrency: 2
       context:
         users:
           tenants: 3
-          users_per_tenant: 5
+          users_per_tenant: 2
+        network: {}
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/glance/list-images.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-update-aggregate.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('NovaAggregates.create_and_update_aggregate', [OrderedDict([('args', "*

 * *            "OrderedDict([('availability_zone', 'nova')])), ('runner', OrderedDict([('type', "*

 * *            "'constant'), ('times', 10), ('concurrency', 2)])), ('context', OrderedDict([('users', "*

 * *            "OrderedDict([('tenants', 3), ('users_per_tenant', 2)]))])), ('sla', "*

 * *            "OrderedDict([('failure_rate', OrderedDict([('max', 0)]))]))])])])"}*

```diff
@@ -1,24 +1,21 @@
 {
-    "GlanceImages.list_images": [
+    "NovaAggregates.create_and_update_aggregate": [
         {
+            "args": {
+                "availability_zone": "nova"
+            },
             "context": {
-                "images": {
-                    "container_format": "bare",
-                    "disk_format": "qcow2",
-                    "image_url": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img",
-                    "images_per_tenant": 4
-                },
                 "users": {
-                    "tenants": 2,
+                    "tenants": 3,
                     "users_per_tenant": 2
                 }
             },
             "runner": {
-                "concurrency": 1,
+                "concurrency": 2,
                 "times": 10,
                 "type": "constant"
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-archive-policy.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-archive-policy.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-archive-policy.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-metric.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-metric.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-delete-resource-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-metric.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-metric.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/create-resource-type.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/create-resource-type.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/gnocchi/list-metric.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/gnocchi/list-metric.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-from-instance.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-from-instance.json`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         "ram": 512,
                         "disk": 1,
                         "vcpus": 1
                     }
                 ],
                 "images": {
                     "image_name": "{{ image_name }}",
-                    "image_url": "http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img",
+                    "image_url": "http://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img",
                     "disk_format": "qcow2",
                     "container_format": "bare",
                     "visibility": "public"
                 }
             },
             "sla": {
                 "failure_rate": {
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-from-instance.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-pods.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,53 @@
-{% set flavor_name = flavor_name or "grafana_test.small" %}
-{% set image_name = image_name or "testVM" %}
 ---
-  GrafanaMetrics.push_metric_from_instance:
+  K8sPods.create_pods:
     -
       args:
-        flavor:
-          name: {{ flavor_name }}
-        image:
-          name: {{ image_name }}
-        monitor_vip: 10.0.0.5
-        pushgateway_port: 9091
-        grafana:
-          user: admin
-          password: password
-          port: 3000
-        datasource_id: 1
-        job_name: rally_test
-        sleep_time: 5
-        retries_total: 30
+        manifests: ["artifacts/nginx.yaml.k8s"]
       runner:
         type: "constant"
-        times: 10
+        times: 1
         concurrency: 1
       context:
         users:
           tenants: 1
           users_per_tenant: 1
-        flavors:
-          -
-            name: {{ flavor_name }}
-            ram: 512
-            disk: 1
-            vcpus: 1
-        images:
-          image_name: {{ image_name }}
-          image_url: http://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img
-          disk_format: qcow2
-          container_format: bare
-          visibility: public
+        cluster_templates:
+          image_id: "fedora-atomic-latest"
+          external_network_id: "public"
+          dns_nameserver: "8.8.8.8"
+          flavor_id: "m1.small"
+          docker_volume_size: 5
+          network_driver: "flannel"
+          coe: "kubernetes"
+        clusters:
+          node_count: 2
+        ca_certs:
+          directory: "/home/stack"
+      sla:
+        failure_rate:
+          max: 0
+    -
+      args:
+        manifests: ["artifacts/nginx.yaml.k8s"]
+      runner:
+        type: "constant"
+        times: 1
+        concurrency: 1
+      context:
+        users:
+          tenants: 1
+          users_per_tenant: 1
+        cluster_templates:
+          image_id: "fedora-atomic-latest"
+          external_network_id: "public"
+          dns_nameserver: "8.8.8.8"
+          flavor_id: "m1.small"
+          docker_volume_size: 5
+          network_driver: "flannel"
+          coe: "kubernetes"
+          tls_disabled: True
+        clusters:
+          node_count: 2
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-locally.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-locally.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/grafana/push-metric-locally.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/grafana/push-metric-locally.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-resource-group.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-delay.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-neutron.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack-with-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-delete-stack.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-delete-stack.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-and-list-stack.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-and-list-stack.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-check-delete-stack.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-check-delete-stack.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-snapshot-restore-delete-stack.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-list-output-resource-group.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-scale.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-scale.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-stack-and-show-output-resource-group.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-suspend-resume-delete-stack.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-add-res.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-del-res.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-increase.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-inplace.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-reduce.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/create-update-delete-stack-replace.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-event.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-event.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/list-stack-and-resources.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/list-stack-and-resources.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/autoscaling-group.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/autoscaling-group.yaml.template`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   flavor:
     type: string
     default: m1.tiny
     constraints:
       - custom_constraint: nova.flavor
   image:
     type: string
-    default: cirros-0.3.5-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
     constraints:
       - custom_constraint: glance.image
   scaling_adjustment:
     type: number
     default: 1
   max_size:
     type: number
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group-server-with-volume.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group-server-with-volume.yaml.template`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   num_instances:
     type: number
     description: number of instances that should be created in resource group
     constraints:
       - range: {min: 1}
   instance_image:
     type: string
-    default: cirros-0.3.5-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   instance_volume_size:
     type: number
     description: Size of volume to attach to instance
     default: 1
     constraints:
       - range: {min: 1, max: 1024}
   instance_flavor:
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/resource-group-with-outputs.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/resource-group-with-outputs.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/server-with-ports.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/server-with-ports.yaml.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 parameters:
   # set all correct defaults for parameters before launch test
   public_net:
     type: string
     default: public
   image:
     type: string
-    default: cirros-0.3.5-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   flavor:
     type: string
     default: m1.tiny
   cidr:
     type: string
     default: 11.11.11.0/24
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/server-with-volume.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/server-with-volume.yaml.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 heat_template_version: 2013-05-23
 
 parameters:
   # set all correct defaults for parameters before launch test
   image:
     type: string
-    default: cirros-0.3.5-x86_64-disk
+    default: cirros-0.5.2-x86_64-disk
   flavor:
     type: string
     default: m1.tiny
   availability_zone:
     type: string
     description: The Availability Zone to launch the instance.
     default: nova
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-autoscaling-policy-inplace.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-autoscaling-policy-inplace.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/heat/templates/updated-random-strings-replace.yaml.template` & `rally-openstack-2.3.0/samples/tasks/scenarios/heat/templates/updated-random-strings-replace.yaml.template`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-delete-node.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-delete-node.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/ironic/create-and-list-node.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/ironic/create-and-list-node.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-list-roles.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-list-roles.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-and-update-user.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-and-update-user.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/keystone/create-user-set-enabled-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/artifacts/rc_nginx.yaml.k8s` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/artifacts/rc_nginx.yaml.k8s`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-and-list-clusters.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-and-list-clusters.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-and-list-clusters.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-and-list-clusters.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-pods.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-pods.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-pods.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-pods.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 ---
-  K8sPods.create_pods:
+  K8sPods.list_pods:
     -
-      args:
-        manifests: ["artifacts/nginx.yaml.k8s"]
       runner:
         type: "constant"
         times: 1
         concurrency: 1
       context:
         users:
           tenants: 1
@@ -18,21 +16,19 @@
           flavor_id: "m1.small"
           docker_volume_size: 5
           network_driver: "flannel"
           coe: "kubernetes"
         clusters:
           node_count: 2
         ca_certs:
-          directory: "/home/stack"
+          directory: ""
       sla:
         failure_rate:
           max: 0
     -
-      args:
-        manifests: ["artifacts/nginx.yaml.k8s"]
       runner:
         type: "constant"
         times: 1
         concurrency: 1
       context:
         users:
           tenants: 1
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-rcs.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-rcs.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/create-rcs.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/create-rcs.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-cluster-templates.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-cluster-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-cluster-templates.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-cluster-templates.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-clusters.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-clusters.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-clusters.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-clusters.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-pods.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/magnum/list-pods.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/magnum/list-pods.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,42 @@
+{% set flavor_name = flavor_name or "m1.tiny" %}
 ---
-  K8sPods.list_pods:
+  NovaServers.boot_and_delete_server:
     -
+      args:
+        flavor:
+            name: "{{flavor_name}}"
+        image:
+            name: "^cirros.*-disk$"
+        force_delete: false
       runner:
         type: "constant"
-        times: 1
-        concurrency: 1
+        times: 10
+        concurrency: 2
       context:
         users:
-          tenants: 1
-          users_per_tenant: 1
-        cluster_templates:
-          image_id: "fedora-atomic-latest"
-          external_network_id: "public"
-          dns_nameserver: "8.8.8.8"
-          flavor_id: "m1.small"
-          docker_volume_size: 5
-          network_driver: "flannel"
-          coe: "kubernetes"
-        clusters:
-          node_count: 2
-        ca_certs:
-          directory: ""
+          tenants: 3
+          users_per_tenant: 2
       sla:
         failure_rate:
           max: 0
     -
+      args:
+        flavor:
+            name: "{{flavor_name}}"
+        image:
+            name: "^cirros.*-disk$"
+        auto_assign_nic: true
       runner:
         type: "constant"
-        times: 1
-        concurrency: 1
+        times: 10
+        concurrency: 2
       context:
         users:
-          tenants: 1
-          users_per_tenant: 1
-        cluster_templates:
-          image_id: "fedora-atomic-latest"
-          external_network_id: "public"
-          dns_nameserver: "8.8.8.8"
-          flavor_id: "m1.small"
-          docker_volume_size: 5
-          network_driver: "flannel"
-          coe: "kubernetes"
-          tls_disabled: True
-        clusters:
-          node_count: 2
+          tenants: 3
+          users_per_tenant: 2
+        network:
+          start_cidr: "10.2.0.0/24"
+          networks_per_tenant: 2
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/attach-security-service-to-share-network.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-security-service-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-security-service-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-security-service-and-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-security-service-and-delete.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-allow-and-deny-access.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-access-from-vm.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-extend.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-extend.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-and-shrink.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-and-shrink.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-network-and-list.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-network-and-list.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-delete.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-list.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-with-autocreated-share-networks-and-set-metadata.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-list.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/create-share-without-share-networks-and-set-metadata.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/manila/list-shares.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/manila/list-shares.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution-with-workflow-name.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-execution.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-execution.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-delete-workbook.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-delete-workbook.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-inputs.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-params.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-params.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution-with-workflow-name.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-execution.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-execution.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/mistral/create-workbook.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/mistral/create-workbook.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/monasca/list-metrics.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/monasca/list-metrics.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/monasca/list-metrics.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/monasca/list-metrics.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-deploy-environment.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-deploy-environment.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/create-and-deploy-environment.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/create-and-deploy-environment.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-delete-package.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-delete-package.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-filter-applications.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-filter-applications.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/import-and-list-packages.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/import-and-list-packages.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/list-environments.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/list-environments.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/murano/package-lifecycle.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/murano/package-lifecycle.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/associate-and-dissociate-floating-ips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-add-subports.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-and-batch-add-subports.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-with-subports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-with-subports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/boot-server-with-subports.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/boot-server-with-subports.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-networks-bgpvpns.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-assoc-disassoc-routers-bgpvpns.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-bind-ports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-bind-ports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-bgpvpns.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-floating-ips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-healthmonitors.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-networks.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-networks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-ports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-ports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-routers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-routers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-routers.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-routers.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-group-rule.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-security-groups.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-subnets.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-delete-vips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-delete-vips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-bgpvpns.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-floating-ips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-healthmonitors.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks-associations.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-networks.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-networks.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-ports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-ports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers-associations.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-routers.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-routers.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-group-rules.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-security-groups.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-subnets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-subnets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-subnets.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-subnets.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-trunks.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-trunks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-list-vips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-list-vips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-network.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-network.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-ports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-ports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-routers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-routers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group-rule.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-security-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-security-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-subnets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-subnets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-show-subnets.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-show-subnets.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-bgpvpns.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-healthmonitors.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-networks.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-networks.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-ports.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-ports.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-ports.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-ports.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-routers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-routers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-routers.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-routers.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-security-groups.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-subnets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-subnets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/create-and-update-vips.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/create-and-update-vips.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/delete-subnets.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/delete-subnets.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/list-agents.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/list-agents.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/neutron/set-and-clear-router-gateway.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-associate-floating-ip.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-block-migrate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-block-migrate.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-multiple.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete-server-with-keypairs.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 ---
-  NovaServers.boot_and_delete_server:
+  VMTasks.boot_runcommand_delete:
     -
       args:
         flavor:
             name: "{{flavor_name}}"
         image:
             name: "^cirros.*-disk$"
+        volume_args:
+            size: 2
+        fixed_network: "private"
+        floating_network: "public"
+        use_floating_ip: true
         force_delete: false
+        command:
+            interpreter: "/bin/sh"
+            script_file: "samples/tasks/support/instance_test.sh"
+        username: "cirros"
       runner:
         type: "constant"
         times: 10
         concurrency: 2
       context:
         users:
           tenants: 3
           users_per_tenant: 2
       sla:
         failure_rate:
           max: 0
-    -
-      args:
-        flavor:
-            name: "{{flavor_name}}"
-        image:
-            name: "^cirros.*-disk$"
-        auto_assign_nic: true
-      runner:
-        type: "constant"
-        times: 10
-        concurrency: 2
-      context:
-        users:
-          tenants: 3
-          users_per_tenant: 2
-        network:
-          start_cidr: "10.2.0.0/24"
-          networks_per_tenant: 2
-      sla:
-        failure_rate:
-          max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-get-console-url.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-get-console-url.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-list.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-rebuild.json`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 {
-    "NovaServers.boot_and_list_server": [
+   "NovaServers.boot_and_rebuild_server": [
         {
             "args": {
                 "flavor": {
                     "name": "{{flavor_name}}"
                 },
-                "image": {
+                "from_image": {
                     "name": "^cirros.*-disk$"
                 },
-                "detailed": true
+                "to_image": {
+                    "name": "^cirros.*-disk$"
+                }
             },
             "runner": {
                 "type": "constant",
-                "times": 1,
-                "concurrency": 1
+                "times": 5,
+                "concurrency": 2
             },
             "context": {
                 "users": {
                     "tenants": 1,
                     "users_per_tenant": 1
                 }
             },
@@ -26,8 +28,7 @@
                 "failure_rate": {
                     "max": 0
                 }
             }
         }
     ]
 }
-
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-live-migrate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-live-migrate.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-migrate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-migrate.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-rebuild.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.json`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
+{% set volume_type = volume_type or "" %}
 {
-   "NovaServers.boot_and_rebuild_server": [
+   "NovaServers.boot_server_from_volume_and_live_migrate": [
         {
             "args": {
                 "flavor": {
                     "name": "{{flavor_name}}"
                 },
-                "from_image": {
+                "image": {
                     "name": "^cirros.*-disk$"
                 },
-                "to_image": {
-                    "name": "^cirros.*-disk$"
-                }
+                "block_migration": false,
+                "volume_size": 10,
+                "volume_type": "{{volume_type}}",
+                "force_delete": false
             },
             "runner": {
                 "type": "constant",
-                "times": 5,
+                "times": 10,
                 "concurrency": 2
             },
             "context": {
                 "users": {
                     "tenants": 1,
                     "users_per_tenant": 1
                 }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-show-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-show-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-and-update-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-and-update-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-bounce-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-bounce-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-bounce-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-bounce-delete.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-delete.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-and-resize.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume-snapshot.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-from-volume.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-from-volume.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-lock-unlock-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-attach-interface.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-and-list-interfaces.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-associate-and-dissociate-floating-ip.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-live-migrate.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-resize.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-volume-and-list-attachments.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/suspend-and-resume.json`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
-{% set volume_type = volume_type or "" %}
 {
-   "NovaServers.boot_server_from_volume_and_live_migrate": [
+    "NovaServers.suspend_and_resume_server": [
         {
             "args": {
                 "flavor": {
                     "name": "{{flavor_name}}"
                 },
                 "image": {
                     "name": "^cirros.*-disk$"
                 },
-                "block_migration": false,
-                "volume_size": 10,
-                "volume_type": "{{volume_type}}",
                 "force_delete": false
             },
             "runner": {
                 "type": "constant",
                 "times": 10,
                 "concurrency": 2
             },
             "context": {
                 "users": {
-                    "tenants": 1,
-                    "users_per_tenant": 1
+                    "tenants": 3,
+                    "users_per_tenant": 2
                 }
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
             }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-from-volume-and-live-migrate.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-snapshot-boot-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/boot.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-and-remove-host.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-aggregate-add-host-and-boot-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-aggregate.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-delete-server-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-delete-server-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-aggregate-details.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-aggregates.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('NovaAggregates.create_and_list_aggregates', [OrderedDict([('args', "*

 * *            "OrderedDict([('availability_zone', 'nova')])), ('runner', OrderedDict([('type', "*

 * *            "'constant'), ('times', 10), ('concurrency', 2)])), ('context', OrderedDict([('users', "*

 * *            "OrderedDict([('tenants', 3), ('users_per_tenant', 2)]))])), ('sla', "*

 * *            "OrderedDict([('failure_rate', OrderedDict([('max', 0)]))]))])])])"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "NovaAggregates.create_and_get_aggregate_details": [
+    "NovaAggregates.create_and_list_aggregates": [
         {
             "args": {
                 "availability_zone": "nova"
             },
             "context": {
                 "users": {
                     "tenants": 3,
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-keypair.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-keypair.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-get-server-group.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-get-server-group.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-aggregates.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-request.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('HttpRequests.check_request', [OrderedDict([('args', "*

 * *            "OrderedDict([('url', 'http://www.example.com'), ('method', 'GET'), ('status_code', "*

 * *            "200), ('allow_redirects', False)])), ('runner', OrderedDict([('type', 'constant'), "*

 * *            "('times', 20), ('concurrency', 5)])), ('sla', OrderedDict([('failure_rate', "*

 * *            "OrderedDict([('max', 0)]))]))])])])"}*

```diff
@@ -1,22 +1,19 @@
 {
-    "NovaAggregates.create_and_list_aggregates": [
+    "HttpRequests.check_request": [
         {
             "args": {
-                "availability_zone": "nova"
-            },
-            "context": {
-                "users": {
-                    "tenants": 3,
-                    "users_per_tenant": 2
-                }
+                "allow_redirects": false,
+                "method": "GET",
+                "status_code": 200,
+                "url": "http://www.example.com"
             },
             "runner": {
-                "concurrency": 2,
-                "times": 10,
+                "concurrency": 5,
+                "times": 20,
                 "type": "constant"
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
             }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-list-server-groups.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-and-list-server-groups.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-and-update-aggregate.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('VMTasks.check_designate_dns_resolving', [OrderedDict([('args', "*

 * *            "OrderedDict([('flavor', OrderedDict([('name', 'm1.tiny')])), ('image', "*

 * *            "OrderedDict([('name', '^cirros.*-disk$')])), ('username', 'ubuntu')])), ('context', "*

 * *            "OrderedDict([('users', OrderedDict([('tenants', 2), ('users_per_tenant', 3)])), "*

 * *            "('network', OrderedDict([('dns_nameservers', ['8.8.8.8', '192.168.1.12'])])), "*

 * *            "('zones', OrderedDict([('set_zone […]*

```diff
@@ -1,22 +1,37 @@
 {
-    "NovaAggregates.create_and_update_aggregate": [
+    "VMTasks.check_designate_dns_resolving": [
         {
             "args": {
-                "availability_zone": "nova"
+                "flavor": {
+                    "name": "m1.tiny"
+                },
+                "image": {
+                    "name": "^cirros.*-disk$"
+                },
+                "username": "ubuntu"
             },
             "context": {
+                "network": {
+                    "dns_nameservers": [
+                        "8.8.8.8",
+                        "192.168.1.12"
+                    ]
+                },
                 "users": {
-                    "tenants": 3,
-                    "users_per_tenant": 2
+                    "tenants": 2,
+                    "users_per_tenant": 3
+                },
+                "zones": {
+                    "set_zone_in_network": true
                 }
             },
             "runner": {
-                "concurrency": 2,
-                "times": 10,
+                "concurrency": 3,
+                "times": 6,
                 "type": "constant"
             },
             "sla": {
                 "failure_rate": {
                     "max": 0
                 }
             }
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/create-flavor-and-set-keys.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/list-servers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/list-servers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/pause-and-unpause.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/pause-and-unpause.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-server.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-server.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-shutoff-server.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-shutoff-server.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/resize-shutoff-server.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/resize-shutoff-server.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/shelve-and-unshelve.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/shelve-and-unshelve.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/nova/suspend-and-resume.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-get-image.json`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-00000000: 7b25 2073 6574 2066 6c61 766f 725f 6e61  {% set flavor_na
-00000010: 6d65 203d 2066 6c61 766f 725f 6e61 6d65  me = flavor_name
-00000020: 206f 7220 226d 312e 7469 6e79 2220 257d   or "m1.tiny" %}
-00000030: 0a7b 0a20 2020 2022 4e6f 7661 5365 7276  .{.    "NovaServ
-00000040: 6572 732e 7375 7370 656e 645f 616e 645f  ers.suspend_and_
-00000050: 7265 7375 6d65 5f73 6572 7665 7222 3a20  resume_server": 
-00000060: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-00000070: 2020 2020 2020 2020 2261 7267 7322 3a20          "args": 
-00000080: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000090: 2020 2266 6c61 766f 7222 3a20 7b0a 2020    "flavor": {.  
-000000a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000b0: 2020 226e 616d 6522 3a20 227b 7b66 6c61    "name": "{{fla
-000000c0: 766f 725f 6e61 6d65 7d7d 220a 2020 2020  vor_name}}".    
-000000d0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000000e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000000f0: 696d 6167 6522 3a20 7b0a 2020 2020 2020  image": {.      
-00000100: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00000110: 616d 6522 3a20 225e 6369 7272 6f73 2e2a  ame": "^cirros.*
-00000120: 2d64 6973 6b24 220a 2020 2020 2020 2020  -disk$".        
-00000130: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000140: 2020 2020 2020 2020 2020 2022 666f 7263             "forc
-00000150: 655f 6465 6c65 7465 223a 2066 616c 7365  e_delete": false
-00000160: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00000170: 2020 2020 2020 2020 2020 2020 2272 756e              "run
-00000180: 6e65 7222 3a20 7b0a 2020 2020 2020 2020  ner": {.        
-00000190: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000001a0: 2263 6f6e 7374 616e 7422 2c0a 2020 2020  "constant",.    
-000001b0: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
-000001c0: 6573 223a 2031 302c 0a20 2020 2020 2020  es": 10,.       
-000001d0: 2020 2020 2020 2020 2022 636f 6e63 7572           "concur
-000001e0: 7265 6e63 7922 3a20 320a 2020 2020 2020  rency": 2.      
-000001f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000200: 2020 2020 2022 636f 6e74 6578 7422 3a20       "context": 
-00000210: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000220: 2020 2275 7365 7273 223a 207b 0a20 2020    "users": {.   
-00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000240: 2022 7465 6e61 6e74 7322 3a20 332c 0a20   "tenants": 3,. 
-00000250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000260: 2020 2022 7573 6572 735f 7065 725f 7465     "users_per_te
-00000270: 6e61 6e74 223a 2032 0a20 2020 2020 2020  nant": 2.       
-00000280: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000290: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000002a0: 2020 2020 2020 2273 6c61 223a 207b 0a20        "sla": {. 
-000002b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000002c0: 6661 696c 7572 655f 7261 7465 223a 207b  failure_rate": {
-000002d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000002e0: 2020 2020 2022 6d61 7822 3a20 300a 2020       "max": 0.  
-000002f0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000300: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000310: 2020 2020 2020 7d0a 2020 2020 5d0a 7d0a        }.    ].}.
+00000000: 7b0a 2020 2020 2247 6c61 6e63 6549 6d61  {.    "GlanceIma
+00000010: 6765 732e 6372 6561 7465 5f61 6e64 5f67  ges.create_and_g
+00000020: 6574 5f69 6d61 6765 223a 205b 0a20 2020  et_image": [.   
+00000030: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000040: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00000050: 2020 2020 2020 2020 2020 2020 2022 696d               "im
+00000060: 6167 655f 6c6f 6361 7469 6f6e 223a 2022  age_location": "
+00000070: 6874 7470 3a2f 2f64 6f77 6e6c 6f61 642e  http://download.
+00000080: 6369 7272 6f73 2d63 6c6f 7564 2e6e 6574  cirros-cloud.net
+00000090: 2f30 2e35 2e32 2f63 6972 726f 732d 302e  /0.5.2/cirros-0.
+000000a0: 352e 322d 7838 365f 3634 2d64 6973 6b2e  5.2-x86_64-disk.
+000000b0: 696d 6722 2c0a 2020 2020 2020 2020 2020  img",.          
+000000c0: 2020 2020 2020 2263 6f6e 7461 696e 6572        "container
+000000d0: 5f66 6f72 6d61 7422 3a20 2262 6172 6522  _format": "bare"
+000000e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000000f0: 2020 2264 6973 6b5f 666f 726d 6174 223a    "disk_format":
+00000100: 2022 7163 6f77 3222 0a20 2020 2020 2020   "qcow2".       
+00000110: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000120: 2020 2020 2272 756e 6e65 7222 3a20 7b0a      "runner": {.
+00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 2274 7970 6522 3a20 2263 6f6e 7374 616e  "type": "constan
+00000150: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00000160: 2020 2020 2274 696d 6573 223a 2034 2c0a      "times": 4,.
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2263 6f6e 6375 7272 656e 6379 223a 2032  "concurrency": 2
+00000190: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+000001a0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+000001b0: 7465 7874 223a 207b 0a20 2020 2020 2020  text": {.       
+000001c0: 2020 2020 2020 2020 2022 7573 6572 7322           "users"
+000001d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000001e0: 2020 2020 2020 2020 2274 656e 616e 7473          "tenants
+000001f0: 223a 2032 2c0a 2020 2020 2020 2020 2020  ": 2,.          
+00000200: 2020 2020 2020 2020 2020 2275 7365 7273            "users
+00000210: 5f70 6572 5f74 656e 616e 7422 3a20 320a  _per_tenant": 2.
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 7d0a 2020 2020 2020 2020 2020 2020 7d2c  }.            },
+00000240: 0a20 2020 2020 2020 2020 2020 2022 736c  .            "sl
+00000250: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00000260: 2020 2020 2020 2266 6169 6c75 7265 5f72        "failure_r
+00000270: 6174 6522 3a20 7b0a 2020 2020 2020 2020  ate": {.        
+00000280: 2020 2020 2020 2020 2020 2020 226d 6178              "max
+00000290: 223a 2030 0a20 2020 2020 2020 2020 2020  ": 0.           
+000002a0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000002b0: 2020 207d 0a20 2020 2020 2020 207d 0a20     }.        }. 
+000002c0: 2020 205d 0a7d 0a                           ].}.
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-delete-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-list-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-show-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-stats-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-loadbalancers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/octavia/octavia-create-and-update-pools.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/quotas/cinder-update.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/quotas/cinder-update.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/quotas/neutron-update.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/quotas/neutron-update.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/quotas/nova-update.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/quotas/nova-update.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/requests/check-random-request.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/requests/check-random-request.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-delete-cluster.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-and-list-node-group-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-delete-node-group-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/create-scale-delete-cluster.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence-scaling.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/dfsio-job-sequence.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/java-action-job.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/java-action-job.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/java-action-job.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/java-action-job.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/sahara/jobs/pig-script-job.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/senlin/create-and-delete-profile-cluster.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666666%*

 * *Differences: {"'SenlinClusters.create_and_delete_cluster'": "{0: {'context': {'profiles': {'properties': "*

 * *                                               "{'image': 'cirros-0.5.2-x86_64-disk'}}}}}"}*

```diff
@@ -6,15 +6,15 @@
                 "max_size": 5,
                 "min_size": 0
             },
             "context": {
                 "profiles": {
                     "properties": {
                         "flavor": 1,
-                        "image": "cirros-0.3.5-x86_64-disk",
+                        "image": "cirros-0.5.2-x86_64-disk",
                         "name": "cirros_server",
                         "networks": [
                             {
                                 "network": "private"
                             }
                         ]
                     },
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-delete-all.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-download-object.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/swift/create-container-and-object-then-list-objects.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-and-download-objects-in-containers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/swift/list-objects-in-containers.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/swift/list-objects-in-containers.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-custom-image.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-script-inline.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/nova/boot-server-attach-created-volume-and-extend.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 ---
-  VMTasks.boot_runcommand_delete:
+  NovaServers.boot_server_attach_created_volume_and_extend:
     -
       args:
         flavor:
             name: "{{flavor_name}}"
         image:
             name: "^cirros.*-disk$"
-        floating_network: "public"
+        volume_size: 1
+        new_volume_size: 2
         force_delete: false
-        command:
-            interpreter: "/bin/sh"
-            script_inline: "ls -la"
-        username: "cirros"
+        do_delete: true
+        boot_server_kwargs: {}
+        create_volume_kwargs: {}
       runner:
         type: "constant"
         times: 10
         concurrency: 2
       context:
         users:
           tenants: 3
           users_per_tenant: 2
-        network: {}
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete-with-disk.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,25 @@
   VMTasks.boot_runcommand_delete:
     -
       args:
         flavor:
             name: "{{flavor_name}}"
         image:
             name: "^cirros.*-disk$"
-        volume_args:
-            size: 2
-        fixed_network: "private"
         floating_network: "public"
-        use_floating_ip: true
         force_delete: false
         command:
             interpreter: "/bin/sh"
             script_file: "samples/tasks/support/instance_test.sh"
         username: "cirros"
       runner:
         type: "constant"
         times: 10
         concurrency: 2
       context:
         users:
           tenants: 3
           users_per_tenant: 2
+        network: {}
       sla:
         failure_rate:
           max: 0
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/boot-runcommand-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/boot-runcommand-delete.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/dd-load-test.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 {% set flavor_name = flavor_name or "m1.tiny" %}
 ---
-  VMTasks.boot_runcommand_delete:
+  VMTasks.dd_load_test:
     -
       args:
         flavor:
             name: "{{flavor_name}}"
         image:
             name: "^cirros.*-disk$"
         floating_network: "public"
         force_delete: false
-        command:
-            interpreter: "/bin/sh"
-            script_file: "samples/tasks/support/instance_test.sh"
+        interpreter: "/bin/sh"
         username: "cirros"
       runner:
         type: "constant"
         times: 10
         concurrency: 2
       context:
         users:
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/check-designate-dns-resolving.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/vm/dd-load-test.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-00000000: 7b0a 2020 2020 2256 4d54 6173 6b73 2e63  {.    "VMTasks.c
-00000010: 6865 636b 5f64 6573 6967 6e61 7465 5f64  heck_designate_d
-00000020: 6e73 5f72 6573 6f6c 7669 6e67 223a 205b  ns_resolving": [
-00000030: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00000040: 2020 2020 2020 2022 6172 6773 223a 207b         "args": {
-00000050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000060: 2022 666c 6176 6f72 223a 207b 0a20 2020   "flavor": {.   
-00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2022 6e61 6d65 223a 2022 6d31 2e74 696e   "name": "m1.tin
-00000090: 7922 0a20 2020 2020 2020 2020 2020 2020  y".             
-000000a0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000000b0: 2020 2020 2020 2269 6d61 6765 223a 207b        "image": {
-000000c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000000d0: 2020 2020 2022 6e61 6d65 223a 2022 5e63       "name": "^c
-000000e0: 6972 726f 732e 2a2d 6469 736b 2422 0a20  irros.*-disk$". 
-000000f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000100: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000110: 2020 2275 7365 726e 616d 6522 3a20 2275    "username": "u
-00000120: 6275 6e74 7522 0a20 2020 2020 2020 2020  buntu".         
-00000130: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000140: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
-00000150: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000160: 7573 6572 7322 3a20 7b0a 2020 2020 2020  users": {.      
-00000170: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000180: 656e 616e 7473 223a 2032 2c0a 2020 2020  enants": 2,.    
-00000190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001a0: 2275 7365 7273 5f70 6572 5f74 656e 616e  "users_per_tenan
-000001b0: 7422 3a20 330a 2020 2020 2020 2020 2020  t": 3.          
-000001c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000001d0: 2020 2020 2020 2020 2022 6e65 7477 6f72           "networ
-000001e0: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
-000001f0: 2020 2020 2020 2020 2020 2264 6e73 5f6e            "dns_n
-00000200: 616d 6573 6572 7665 7273 223a 205b 0a20  ameservers": [. 
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2020 2020 2022 382e 382e 382e 3822         "8.8.8.8"
-00000230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000240: 2020 2020 2020 2020 2020 2231 3932 2e31            "192.1
-00000250: 3638 2e31 2e31 3222 0a20 2020 2020 2020  68.1.12".       
-00000260: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-00000270: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000290: 2020 227a 6f6e 6573 223a 207b 0a20 2020    "zones": {.   
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002b0: 2022 7365 745f 7a6f 6e65 5f69 6e5f 6e65   "set_zone_in_ne
-000002c0: 7477 6f72 6b22 3a20 7472 7565 0a20 2020  twork": true.   
-000002d0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-000002e0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000002f0: 2020 2020 2020 2020 2020 2272 756e 6e65            "runne
-00000300: 7222 3a20 7b0a 2020 2020 2020 2020 2020  r": {.          
-00000310: 2020 2020 2020 2263 6f6e 6375 7272 656e        "concurren
-00000320: 6379 223a 2033 2c0a 2020 2020 2020 2020  cy": 3,.        
-00000330: 2020 2020 2020 2020 2274 696d 6573 223a          "times":
-00000340: 2036 2c0a 2020 2020 2020 2020 2020 2020   6,.            
-00000350: 2020 2020 2274 7970 6522 3a20 2263 6f6e      "type": "con
-00000360: 7374 616e 7422 0a20 2020 2020 2020 2020  stant".         
-00000370: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000380: 2020 2273 6c61 223a 207b 0a20 2020 2020    "sla": {.     
-00000390: 2020 2020 2020 2020 2020 2022 6661 696c             "fail
-000003a0: 7572 655f 7261 7465 223a 207b 0a20 2020  ure_rate": {.   
-000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003c0: 2022 6d61 7822 3a20 300a 2020 2020 2020   "max": 0.      
-000003d0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000003e0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000003f0: 2020 7d0a 2020 2020 5d0a 7d                }.    ].}
+00000000: 7b25 2073 6574 2066 6c61 766f 725f 6e61  {% set flavor_na
+00000010: 6d65 203d 2066 6c61 766f 725f 6e61 6d65  me = flavor_name
+00000020: 206f 7220 226d 312e 7469 6e79 2220 257d   or "m1.tiny" %}
+00000030: 0a7b 0a20 2020 2022 564d 5461 736b 732e  .{.    "VMTasks.
+00000040: 6464 5f6c 6f61 645f 7465 7374 223a 205b  dd_load_test": [
+00000050: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000060: 2020 2020 2020 2022 6172 6773 223a 207b         "args": {
+00000070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000080: 2022 666c 6176 6f72 223a 207b 0a20 2020   "flavor": {.   
+00000090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000a0: 2022 6e61 6d65 223a 2022 7b7b 666c 6176   "name": "{{flav
+000000b0: 6f72 5f6e 616d 657d 7d22 0a20 2020 2020  or_name}}".     
+000000c0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000000d0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+000000e0: 6d61 6765 223a 207b 0a20 2020 2020 2020  mage": {.       
+000000f0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+00000100: 6d65 223a 2022 5e63 6972 726f 732e 2a2d  me": "^cirros.*-
+00000110: 6469 736b 2422 0a20 2020 2020 2020 2020  disk$".         
+00000120: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000130: 2020 2020 2020 2020 2020 2266 6c6f 6174            "float
+00000140: 696e 675f 6e65 7477 6f72 6b22 3a20 2270  ing_network": "p
+00000150: 7562 6c69 6322 2c0a 2020 2020 2020 2020  ublic",.        
+00000160: 2020 2020 2020 2020 2266 6f72 6365 5f64          "force_d
+00000170: 656c 6574 6522 3a20 6661 6c73 652c 0a20  elete": false,. 
+00000180: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000190: 696e 7465 7270 7265 7465 7222 3a20 222f  interpreter": "/
+000001a0: 6269 6e2f 7368 222c 0a20 2020 2020 2020  bin/sh",.       
+000001b0: 2020 2020 2020 2020 2022 7573 6572 6e61           "userna
+000001c0: 6d65 223a 2022 6369 7272 6f73 220a 2020  me": "cirros".  
+000001d0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000001e0: 2020 2020 2020 2020 2022 7275 6e6e 6572           "runner
+000001f0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000200: 2020 2020 2022 7479 7065 223a 2022 636f       "type": "co
+00000210: 6e73 7461 6e74 222c 0a20 2020 2020 2020  nstant",.       
+00000220: 2020 2020 2020 2020 2022 7469 6d65 7322           "times"
+00000230: 3a20 3130 2c0a 2020 2020 2020 2020 2020  : 10,.          
+00000240: 2020 2020 2020 2263 6f6e 6375 7272 656e        "concurren
+00000250: 6379 223a 2032 0a20 2020 2020 2020 2020  cy": 2.         
+00000260: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00000270: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
+00000280: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000290: 7573 6572 7322 3a20 7b0a 2020 2020 2020  users": {.      
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000002b0: 656e 616e 7473 223a 2033 2c0a 2020 2020  enants": 3,.    
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2275 7365 7273 5f70 6572 5f74 656e 616e  "users_per_tenan
+000002e0: 7422 3a20 320a 2020 2020 2020 2020 2020  t": 2.          
+000002f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000300: 2020 2020 2020 2020 2022 6e65 7477 6f72           "networ
+00000310: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
+00000320: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000330: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000340: 2020 2022 736c 6122 3a20 7b0a 2020 2020     "sla": {.    
+00000350: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
+00000360: 6c75 7265 5f72 6174 6522 3a20 7b0a 2020  lure_rate": {.  
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 226d 6178 223a 2030 0a20 2020 2020    "max": 0.     
+00000390: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000003a0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000003b0: 2020 207d 0a20 2020 205d 0a7d 0a            }.    ].}.
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/vm/dd-load-test.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/glance/create-and-download-image.json`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,45 @@
-00000000: 7b25 2073 6574 2066 6c61 766f 725f 6e61  {% set flavor_na
-00000010: 6d65 203d 2066 6c61 766f 725f 6e61 6d65  me = flavor_name
-00000020: 206f 7220 226d 312e 7469 6e79 2220 257d   or "m1.tiny" %}
-00000030: 0a7b 0a20 2020 2022 564d 5461 736b 732e  .{.    "VMTasks.
-00000040: 6464 5f6c 6f61 645f 7465 7374 223a 205b  dd_load_test": [
-00000050: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00000060: 2020 2020 2020 2022 6172 6773 223a 207b         "args": {
-00000070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000080: 2022 666c 6176 6f72 223a 207b 0a20 2020   "flavor": {.   
-00000090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000a0: 2022 6e61 6d65 223a 2022 7b7b 666c 6176   "name": "{{flav
-000000b0: 6f72 5f6e 616d 657d 7d22 0a20 2020 2020  or_name}}".     
-000000c0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000000d0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000000e0: 6d61 6765 223a 207b 0a20 2020 2020 2020  mage": {.       
-000000f0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00000100: 6d65 223a 2022 5e63 6972 726f 732e 2a2d  me": "^cirros.*-
-00000110: 6469 736b 2422 0a20 2020 2020 2020 2020  disk$".         
-00000120: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000130: 2020 2020 2020 2020 2020 2266 6c6f 6174            "float
-00000140: 696e 675f 6e65 7477 6f72 6b22 3a20 2270  ing_network": "p
-00000150: 7562 6c69 6322 2c0a 2020 2020 2020 2020  ublic",.        
-00000160: 2020 2020 2020 2020 2266 6f72 6365 5f64          "force_d
-00000170: 656c 6574 6522 3a20 6661 6c73 652c 0a20  elete": false,. 
-00000180: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000190: 696e 7465 7270 7265 7465 7222 3a20 222f  interpreter": "/
-000001a0: 6269 6e2f 7368 222c 0a20 2020 2020 2020  bin/sh",.       
-000001b0: 2020 2020 2020 2020 2022 7573 6572 6e61           "userna
-000001c0: 6d65 223a 2022 6369 7272 6f73 220a 2020  me": "cirros".  
-000001d0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000001e0: 2020 2020 2020 2020 2022 7275 6e6e 6572           "runner
-000001f0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000200: 2020 2020 2022 7479 7065 223a 2022 636f       "type": "co
-00000210: 6e73 7461 6e74 222c 0a20 2020 2020 2020  nstant",.       
-00000220: 2020 2020 2020 2020 2022 7469 6d65 7322           "times"
-00000230: 3a20 3130 2c0a 2020 2020 2020 2020 2020  : 10,.          
-00000240: 2020 2020 2020 2263 6f6e 6375 7272 656e        "concurren
-00000250: 6379 223a 2032 0a20 2020 2020 2020 2020  cy": 2.         
-00000260: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000270: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
-00000280: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000290: 7573 6572 7322 3a20 7b0a 2020 2020 2020  users": {.      
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000002b0: 656e 616e 7473 223a 2033 2c0a 2020 2020  enants": 3,.    
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 2275 7365 7273 5f70 6572 5f74 656e 616e  "users_per_tenan
-000002e0: 7422 3a20 320a 2020 2020 2020 2020 2020  t": 2.          
-000002f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000300: 2020 2020 2020 2020 2022 6e65 7477 6f72           "networ
-00000310: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
-00000320: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000330: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000340: 2020 2022 736c 6122 3a20 7b0a 2020 2020     "sla": {.    
-00000350: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
-00000360: 6c75 7265 5f72 6174 6522 3a20 7b0a 2020  lure_rate": {.  
-00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000380: 2020 226d 6178 223a 2030 0a20 2020 2020    "max": 0.     
-00000390: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000003a0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000003b0: 2020 207d 0a20 2020 205d 0a7d 0a            }.    ].}.
+00000000: 7b0a 2020 2020 2247 6c61 6e63 6549 6d61  {.    "GlanceIma
+00000010: 6765 732e 6372 6561 7465 5f61 6e64 5f64  ges.create_and_d
+00000020: 6f77 6e6c 6f61 645f 696d 6167 6522 3a20  ownload_image": 
+00000030: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00000040: 2020 2020 2020 2020 2261 7267 7322 3a20          "args": 
+00000050: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000060: 2020 2269 6d61 6765 5f6c 6f63 6174 696f    "image_locatio
+00000070: 6e22 3a20 2268 7474 703a 2f2f 646f 776e  n": "http://down
+00000080: 6c6f 6164 2e63 6972 726f 732d 636c 6f75  load.cirros-clou
+00000090: 642e 6e65 742f 302e 352e 322f 6369 7272  d.net/0.5.2/cirr
+000000a0: 6f73 2d30 2e35 2e32 2d78 3836 5f36 342d  os-0.5.2-x86_64-
+000000b0: 6469 736b 2e69 6d67 222c 0a20 2020 2020  disk.img",.     
+000000c0: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+000000d0: 6169 6e65 725f 666f 726d 6174 223a 2022  ainer_format": "
+000000e0: 6261 7265 222c 0a20 2020 2020 2020 2020  bare",.         
+000000f0: 2020 2020 2020 2022 6469 736b 5f66 6f72         "disk_for
+00000100: 6d61 7422 3a20 2271 636f 7732 220a 2020  mat": "qcow2".  
+00000110: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000120: 2020 2020 2020 2020 2022 7275 6e6e 6572           "runner
+00000130: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000140: 2020 2020 2022 7479 7065 223a 2022 636f       "type": "co
+00000150: 6e73 7461 6e74 222c 0a20 2020 2020 2020  nstant",.       
+00000160: 2020 2020 2020 2020 2022 7469 6d65 7322           "times"
+00000170: 3a20 3130 2c0a 2020 2020 2020 2020 2020  : 10,.          
+00000180: 2020 2020 2020 2263 6f6e 6375 7272 656e        "concurren
+00000190: 6379 223a 2032 0a20 2020 2020 2020 2020  cy": 2.         
+000001a0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000001b0: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000001d0: 7573 6572 7322 3a20 7b0a 2020 2020 2020  users": {.      
+000001e0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000001f0: 656e 616e 7473 223a 2032 2c0a 2020 2020  enants": 2,.    
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2275 7365 7273 5f70 6572 5f74 656e 616e  "users_per_tenan
+00000220: 7422 3a20 330a 2020 2020 2020 2020 2020  t": 3.          
+00000230: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000240: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000250: 2020 2022 736c 6122 3a20 7b0a 2020 2020     "sla": {.    
+00000260: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
+00000270: 6c75 7265 5f72 6174 6522 3a20 7b0a 2020  lure_rate": {.  
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 226d 6178 223a 2030 0a20 2020 2020    "max": 0.     
+000002a0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000002b0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+000002c0: 2020 2020 7d0a 2020 2020 5d0a 7d0a           }.    ].}.
```

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/watcher/create-audit-template-and-delete.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/watcher/list-audit-templates.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/watcher/list-audit-templates.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/watcher/list-audit-templates.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/watcher/list-audit-templates.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/workload/wordpress.json` & `rally-openstack-2.3.0/samples/tasks/scenarios/workload/wordpress.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/scenarios/workload/wordpress.yaml` & `rally-openstack-2.3.0/samples/tasks/scenarios/workload/wordpress.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/sla/create-and-delete-user.json` & `rally-openstack-2.3.0/samples/tasks/sla/create-and-delete-user.json`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/samples/tasks/support/instance_linpack.sh` & `rally-openstack-2.3.0/samples/tasks/support/instance_linpack.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/setup.cfg` & `rally-openstack-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/setup.py` & `rally-openstack-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/README.rst` & `rally-openstack-2.3.0/tasks/openstack/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/macro/macro.yaml` & `rally-openstack-2.3.0/tasks/openstack/macro/macro.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/scenario/cinder.yaml` & `rally-openstack-2.3.0/tasks/openstack/scenario/cinder.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/scenario/glance.yaml` & `rally-openstack-2.3.0/tasks/openstack/scenario/glance.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/scenario/keystone.yaml` & `rally-openstack-2.3.0/tasks/openstack/scenario/keystone.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/scenario/neutron.yaml` & `rally-openstack-2.3.0/tasks/openstack/scenario/neutron.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/scenario/nova.yaml` & `rally-openstack-2.3.0/tasks/openstack/scenario/nova.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tasks/openstack/task.yaml` & `rally-openstack-2.3.0/tasks/openstack/task.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set glance_image_location = glance_image_location|default("https://download.cirros-cloud.net/0.3.5/cirros-0.3.5-i386-disk.img") %}
+{%- set glance_image_location = glance_image_location|default("https://download.cirros-cloud.net/0.5.2/cirros-0.5.2-x86_64-disk.img") %}
 {%- set image_name = image_name|default("^(cirros.*-disk|TestVM)$") %}
 {%- set flavor_name = flavor_name|default("m1.tiny") %}
 {%- set use_existing_users = use_existing_users|default(false) %}
 {%- set service_list = service_list|default(["authentication", "cinder", "keystone", "nova", "glance", "neutron"]) %}
 {%- set smoke = smoke|default(true) %}
 {%- set controllers_amount = controllers_amount|default(1) %}
 {%- if smoke %}
```

### Comparing `rally-openstack-2.2.0/tasks/openstack_metrics/task.yaml` & `rally-openstack-2.3.0/tasks/openstack_metrics/task.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/test-requirements.txt` & `rally-openstack-2.3.0/test-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 hacking>=3.0                                           # Apache Software License
 
 pytest                                                 # MIT
 # py.test plugin for measuring coverage.
-pytest-cov>=2.2.1                                      # MIT
+pytest-cov                                             # MIT
 # py.test plugin for generating HTML reports
 pytest-html                                            # Mozilla Public License 2.0 (MPL 2.0)
 # py.test xdist plugin for distributed testing and loop-on-failing modes
 pytest-xdist                                           # MIT
 
-coverage!=4.4                                          # Apache License, Version 2.0
+coverage!=4.4                                          # Apache-2.0
 ddt                                                    # MIT
 testtools                                              # MIT
 
 # docs
-docutils                                               # public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
-Pygments                                               # BSD
+docutils<0.18                                          # public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
+Pygments                                               # BSD-2-Clause
```

### Comparing `rally-openstack-2.2.0/tests/README.rst` & `rally-openstack-2.3.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/cover.sh` & `rally-openstack-2.3.0/tests/ci/cover.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/pages/task-index.html` & `rally-openstack-2.3.0/tests/ci/pages/task-index.html`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/pages/verify-index.html` & `rally-openstack-2.3.0/tests/ci/pages/verify-index.html`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/post-rally-verify.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/post-rally-verify.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/fetch-rally-task-results/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/library/osresources.py` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/library/osresources.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
 """List and compare most used OpenStack cloud resources."""
 
-import argparse
 import io
 import json
 import subprocess
-import sys
 
 from ansible.module_utils.basic import AnsibleModule
 
 from rally.cli import cliutils
 from rally.common.plugin import discover
 from rally import plugins
 
@@ -489,15 +487,15 @@
             manager = cls(self.clients)
             if manager.is_available():
                 resources.extend(manager.get_resources())
         return resources
 
     def compare(self, with_list):
         def make_uuid(res):
-            return"%s.%s:%s" % (
+            return "%s.%s:%s" % (
                 res["cls"], res["resource_name"],
                 ";".join(["%s=%s" % (k, v)
                           for k, v in sorted(res["id"].items())]))
 
         current_resources = dict((make_uuid(r), r) for r in self.list())
         saved_resources = dict((make_uuid(r), r) for r in with_list)
 
@@ -592,15 +590,15 @@
             f.write(json.dumps(result, indent=4))
 
     rc = 1 if any(changes) else 0
     return rc, result
 
 
 @plugins.ensure_plugins_are_loaded
-def main(json_output, compare_with):
+def do_it(json_output, compare_with):
 
     out = subprocess.check_output(
         ["rally", "env", "show", "--only-spec", "--env", "devstack"])
     config = json.loads(out.decode("utf-8"))
     config = config["existing@openstack"]
     config.update(config.pop("admin"))
     if "users" in config:
@@ -618,49 +616,23 @@
     module = AnsibleModule(
         argument_spec=dict(
             json_output=dict(required=False, type="str"),
             compare_with=dict(required=False, type="path")
         )
     )
 
-    rc, json_result = main(
+    rc, json_result = do_it(
         json_output=module.params.get("json_output"),
         compare_with=module.params.get("compare_with")
     )
     if rc:
         module.fail_json(
             msg="Unexpected changes of resources are detected.",
             rc=1,
             resources=json_result
         )
 
     module.exit_json(rc=0, changed=True, resources=json_result)
 
 
-def cli_main():
-    parser = argparse.ArgumentParser(
-        description=("Save list of OpenStack cloud resources or compare "
-                     "with previously saved list."))
-
-    group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument("--dump-list",
-                       type=str,
-                       metavar="<path/to/output/list.json>",
-                       help="dump resources to given file in JSON format")
-    group.add_argument("--compare-with-list",
-                       type=str,
-                       metavar="<path/to/existent/list.json>",
-                       help=("compare current resources with a list from "
-                             "given JSON file"))
-    args = parser.parse_args()
-
-    rc, _json_result = main(
-        json_output=args.dump_list, compare_with=args.compare_with_list)
-
-    return rc
-
-
 if __name__ == "__main__":
-    if sys.stdin.isatty():
-        cli_main()
-    else:
-        ansible_main()
+    ansible_main()
```

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_and_compare_resources.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/list-os-resources/tasks/list_and_compare_resources.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/make_env_spec_with_existing_users.py` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/library/make_env_spec_with_existing_users.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/main.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -41,41 +41,41 @@
     path: '{{ rally_home_dir }}/plugins'
     state: directory
     owner: stack
     group: stack
 
 - name: Check the existence of custom plugins
   stat:
-    path: '{{ zuul.project.src_dir }}/rally-jobs/plugins'
+    path: '{{ ansible_user_dir }}/{{ zuul.project.src_dir }}/rally-jobs/plugins'
   register: custom_plugins_stat
 
 - name: Copy custom plugins, if they are presented
   become: True
   become_user: stack
-  command: cp -r {{ zuul.project.src_dir }}/rally-jobs/plugins {{ rally_home_dir }}/
+  command: cp -r {{ custom_plugins_stat.stat.path }} {{ rally_home_dir }}/
   when: custom_plugins_stat.stat.exists == True
 
 - name: Create a directory for extra files
   become: True
   become_user: stack
   file:
     path: '{{ rally_home_dir }}/extra'
     state: directory
     owner: stack
     group: stack
 
 - name: Check the existence of extra files
   stat:
-    path: '{{ zuul.project.src_dir }}/rally-jobs/extra'
+    path: '{{ ansible_user_dir }}/{{ zuul.project.src_dir }}/rally-jobs/extra'
   register: extra_files_stat
 
 - name: Copy extra files, if they are presented
   become: True
   become_user: stack
-  command: cp -r {{ zuul.project.src_dir }}/rally-jobs/extra {{ rally_home_dir }}/
+  command: cp -r {{ extra_files_stat.stat.path }} {{ rally_home_dir }}/
   when: extra_files_stat.stat.exists == True
 
 - name: Check the existence of fake image
   stat:
     path: '{{ rally_fake_image_path }}'
   register: fake_image_stat
 
@@ -141,37 +141,37 @@
       if rally deployment check | grep 'nova' | grep 'Available' > /dev/null;
       then
           nova flavor-create m1.nano 42 64 0 1
       fi
 
 - name: Check the existence of rally_task
   stat:
-    path: '{{ zuul.project.src_dir }}/{{ rally_task }}'
+    path: '{{ ansible_user_dir }}/{{ zuul.project.src_dir }}/{{ rally_task }}'
   register: rally_task_file_stat
 
 - name: Fail if Rally task file is missed.
   fail:
     msg: "'{{ rally_task }}' Rally task file is missed."
   when: rally_task_file_stat.stat.exists != True
 
 - name: Copy task file
   become: True
   become_user: stack
-  command: cp "{{ zuul.project.src_dir }}/{{ rally_task }}" "{{ rally_home_dir }}/task.yaml"
+  command: cp "{{ rally_task_file_stat.stat.path }}" "{{ rally_home_dir }}/task.yaml"
   when: rally_task_file_stat.stat.exists == True
 
 - name: Check the existence of task_args_file
   stat:
-    path: '{{ zuul.project.src_dir }}/{{ rally_task_args_file }}'
+    path: '{{ ansible_user_dir }}/{{ zuul.project.src_dir }}/{{ rally_task_args_file }}'
   register: task_args_file_stat
 
 - name: Copy task_args_file
   become: True
   become_user: stack
-  command: cp "{{ zuul.project.src_dir }}/{{ rally_task_args_file }}" "{{ rally_home_dir }}/task_args_file.yaml"
+  command: cp "{{ task_args_file_stat.stat.path }}" "{{ rally_home_dir }}/task_args_file.yaml"
   when: task_args_file_stat.stat.exists == True
 
 - name: Create an empty task_args_file
   become: True
   become_user: stack
   command: echo "{}" > "{{ rally_home_dir }}/task_args_file.yaml"
   when: task_args_file_stat.stat.exists == False
```

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/prepare-env-with-existing-users.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/prepare-for-rally-task/tasks/prepare-env-with-existing-users.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/process-task-results/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/process-task-results/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/roles/run-rally-task/tasks/main.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/roles/run-rally-task/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/run-rally-task.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/run-rally-task.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/playbooks/run-rally-verify.yaml` & `rally-openstack-2.3.0/tests/ci/playbooks/run-rally-verify.yaml`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/pytest_launcher.py` & `rally-openstack-2.3.0/tests/ci/pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/rally_functional_job.sh` & `rally-openstack-2.3.0/tests/ci/rally_functional_job.sh`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/ci/rally_verify.py` & `rally-openstack-2.3.0/tests/ci/rally_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,34 +320,14 @@
             "This test was skipped intentionally",
     }
     XFAIL_TESTS = {
         "tempest.scenario.test_dashboard_basic_ops"
         ".TestDashboardBasicOps.test_basic_scenario"
         "[dashboard,id-4f8851b1-0e69-482b-b63b-84c6e76f6c80,smoke]":
             "Fails for unknown reason",
-
-        "tempest.api.compute.servers.test_attach_interfaces"
-        ".AttachInterfacesUnderV243Test.test_add_remove_fixed_ip"
-        "[id-c7e0e60b-ee45-43d0-abeb-8596fd42a2f9,network,smoke]":
-            "Fails for unknown reason",
-
-        "tempest.scenario.test_network_basic_ops"
-        ".TestNetworkBasicOps.test_network_basic_ops"
-        "[compute,id-f323b3ba-82f8-4db7-8ea6-6a895869ec49,network,smoke]":
-            "Fails for unknown reason",
-
-        "tempest.scenario.test_server_basic_ops"
-        ".TestServerBasicOps.test_server_basic_ops"
-        "[compute,id-7fff3fb3-91d8-4fd0-bd7d-0204f1f180ba,network,smoke]":
-            "Fails for unknown reason",
-
-        "tempest.api.compute.servers.test_server_actions"
-        ".ServerActionsTestJSON.test_reboot_server_hard"
-        "[id-2cb1baf6-ac8d-4429-bf0d-ba8a0ba53e32,smoke]":
-            "Fails for unknown reason"
     }
 
     def setUp(self):
         self.CALL_ARGS["tag"] = "tag-1 tag-2"
         self.CALL_ARGS["set"] = "full" if self.args.mode == "full" else "smoke"
         # Start a verification, show results and generate reports
         skip_tests = json.dumps(self.SKIP_TESTS)
```

### Comparing `rally-openstack-2.2.0/tests/ci/sync_requirements.py` & `rally-openstack-2.3.0/tests/ci/sync_requirements.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
     # NOTE(andreykurilin): global OpenStack upper-constraints file includes
     #   comments which can be unrelated to Rally project, so let's just ignore
     #   them.
     global_uc = parse_data(raw_g_uc,
                            include_comments=False,
                            dependency_cls=UpperConstraint)
 
-    our_uc = [UpperConstraint(package_name=p.project_name)
+    our_uc = [UpperConstraint(package_name=p.project_name, version=p.version)
               for p in pkg_resources.working_set
               # do not include the current package at u-c
               if p.project_name != "rally-openstack"]
 
     for package in our_uc:
         if package.package_name in global_uc:
             # we cannot use whatever we want versions in CI. OpenStack CI
```

### Comparing `rally-openstack-2.2.0/tests/functional/extra/fake_dir/fake_plugin.py` & `rally-openstack-2.3.0/tests/functional/extra/fake_dir/fake_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/functional/test_certification_task.py` & `rally-openstack-2.3.0/tests/functional/test_certification_task.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/functional/test_cli_deployment.py` & `rally-openstack-2.3.0/tests/functional/test_cli_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
-
+import json
 import re
 
 import testtools
 
 from tests.functional import utils
 
 
@@ -42,16 +42,17 @@
         self.assertIn(TEST_ENV["OS_AUTH_URL"],
                       rally("deployment show"))
 
     def test_create_fromfile(self):
         rally = utils.Rally()
         rally.env.update(TEST_ENV)
         rally("deployment create --name t_create_env --fromenv")
+        existing_conf = rally("deployment config", getjson=True)
         with open("/tmp/.tmp.deployment", "w") as f:
-            f.write(rally("deployment config"))
+            f.write(json.dumps(existing_conf))
         rally("deployment create --name t_create_file "
               "--filename /tmp/.tmp.deployment")
         self.assertIn("t_create_file", rally("deployment list"))
 
     def test_destroy(self):
         rally = utils.Rally()
         rally.env.update(TEST_ENV)
```

### Comparing `rally-openstack-2.2.0/tests/functional/test_cli_env.py` & `rally-openstack-2.3.0/tests/functional/test_cli_env.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/functional/test_cli_task.py` & `rally-openstack-2.3.0/tests/functional/test_cli_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import json
 import unittest
 
 from tests.functional import utils
 
 
 class TaskTestCase(unittest.TestCase):
 
     def test_specify_version_by_deployment(self):
         rally = utils.Rally()
-        deployment = json.loads(rally("deployment config"))
+        deployment = rally("deployment config", getjson=True)
         deployment["openstack"]["api_info"] = {
             "fakedummy": {
                 "version": "2",
                 "service_type": "dummyv2"
             }
         }
         deployment = utils.JsonTempFile(deployment)
@@ -48,15 +47,15 @@
         config = utils.TaskConfig(config)
         plugins = "tests/functional/extra/fake_dir/fake_plugin.py"
         rally("--plugin-paths %s task start --task %s" % (
             plugins, config.filename))
 
     def test_specify_version_by_deployment_with_existing_users(self):
         rally = utils.Rally()
-        deployment = json.loads(rally("deployment config"))
+        deployment = rally("deployment config", getjson=True)
         deployment["openstack"]["users"] = [deployment["openstack"]["admin"]]
         deployment["openstack"]["api_info"] = {
             "fakedummy": {
                 "version": "2",
                 "service_type": "dummyv2"
             }
         }
```

### Comparing `rally-openstack-2.2.0/tests/functional/test_task_samples.py` & `rally-openstack-2.3.0/tests/functional/test_task_samples.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/functional/utils.py` & `rally-openstack-2.3.0/tests/functional/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -197,17 +197,18 @@
         """
 
         if not isinstance(cmd, list):
             cmd = cmd.split(" ")
         try:
             if no_logs or getjson:
                 cmd = self.args + ["--log-file", "/dev/null"] + cmd
-                with open(os.devnull, "w") as DEVNULL:
-                    output = encodeutils.safe_decode(subprocess.check_output(
-                        cmd, stderr=DEVNULL, env=self.env))
+                output = encodeutils.safe_decode(
+                    subprocess.check_output(
+                        cmd, stderr=subprocess.DEVNULL, env=self.env)
+                )
             else:
                 cmd = self.args + cmd
                 output = encodeutils.safe_decode(subprocess.check_output(
                     cmd, stderr=subprocess.STDOUT, env=self.env))
 
             if getjson:
                 return json.loads(output)
```

### Comparing `rally-openstack-2.2.0/tests/hacking/checks.py` & `rally-openstack-2.3.0/tests/hacking/checks.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,19 @@
  - Keep the test method code in the source file ordered based
    on the N3xx value.
  - List the new rule in the top level HACKING.rst file
  - Add test cases for each new rule to tests/unit/test_hacking.py
 
 """
 
-import functools
 import re
 import tokenize
 
 from hacking import core
 
-
 re_assert_equal_end_with_true_or_false = re.compile(
     r"assertEqual\(.*?, \s+(True|False)\)$")
 re_assert_equal_start_with_true_or_false = re.compile(
     r"assertEqual\((True|False),")
 re_assert_true_instance = re.compile(
     r"(.)*assertTrue\(isinstance\((\w|\.|\'|\"|\[|\])+, "
     r"(\w|\.|\'|\"|\[|\])+\)\)")
@@ -74,53 +72,38 @@
 re_db_import = re.compile(r"^from rally.common import db")
 re_objects_import = re.compile(r"^from rally.common import objects")
 re_old_type_class = re.compile(r"^\s*class \w+(\(\))?:")
 re_datetime_alias = re.compile(r"^(from|import) datetime(?!\s+as\s+dt$)")
 re_log_warn = re.compile(r"(.)*LOG\.(warn)\(\s*('|\"|_)")
 
 
-def skip_ignored_lines(func):
-
-    @functools.wraps(func)
-    def wrapper(physical_line, logical_line, filename):
-        line = physical_line.strip()
-        if not line or line.startswith("#") or line.endswith("# noqa"):
-            return
-        try:
-            for res in func(physical_line, logical_line, filename):
-                yield res
-        except StopIteration:
-            return
-
-    return wrapper
-
-
 def _parse_assert_mock_str(line):
     point = line.find(".assert_")
 
     if point == -1:
         point = line.find(".called_once_with(")
 
     if point != -1:
         end_pos = line[point:].find("(") + point
         return point, line[point + 1: end_pos], line[: point]
     else:
         return None, None, None
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_assert_methods_from_mock(physical_line, logical_line, filename):
+def check_assert_methods_from_mock(logical_line, filename, noqa=False):
     """Ensure that ``assert_*`` methods from ``mock`` library is used correctly
 
     N301 - base error number
     N302 - related to nonexistent "assert_called"
     N303 - related to nonexistent "assert_called_once"
     N304 - related to nonexistent "called_once_with"
     """
+    if noqa:
+        return
 
     correct_names = ["assert_any_call", "assert_called_once_with",
                      "assert_called_with", "assert_has_calls",
                      "assert_not_called"]
     ignored_files = ["./tests/unit/test_hacking.py"]
 
     if filename.startswith("./tests") and filename not in ignored_files:
@@ -158,23 +141,24 @@
                 yield (pos, msg % {
                     "error_number": error_number,
                     "method": method_name,
                     "custom_msg": custom_msg})
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_import_of_logging(physical_line, logical_line, filename):
+def check_import_of_logging(logical_line, filename, noqa=False):
     """Check correctness import of logging module
 
     N310
     """
+    if noqa:
+        return
 
     excluded_files = ["./rally/common/logging.py",
-                      "./tests/unit/test_logging.py",
+                      "./tests/unit/common/test_logging.py",
                       "./tests/ci/rally_verify.py",
                       "./tests/ci/sync_requirements.py"]
 
     forbidden_imports = ["from oslo_log",
                          "import oslo_log",
                          "import logging"]
 
@@ -182,213 +166,221 @@
         for forbidden_import in forbidden_imports:
             if logical_line.startswith(forbidden_import):
                 yield (0, "N310 Wrong module for logging is imported. Please "
                           "use `rally.common.logging` instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_import_of_config(physical_line, logical_line, filename):
+def check_import_of_config(logical_line, filename, noqa=False):
     """Check correctness import of config module
 
     N311
     """
+    if noqa:
+        return
 
     excluded_files = ["./rally/common/cfg.py"]
 
     forbidden_imports = ["from oslo_config",
                          "import oslo_config"]
 
     if filename not in excluded_files:
         for forbidden_import in forbidden_imports:
             if logical_line.startswith(forbidden_import):
                 yield (0, "N311 Wrong module for config is imported. Please "
                           "use `rally.common.cfg` instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def no_use_conf_debug_check(physical_line, logical_line, filename):
+def no_use_conf_debug_check(logical_line, filename, noqa=False):
     """Check for "cfg.CONF.debug"
 
     Rally has two DEBUG level:
      - Full DEBUG, which include all debug-messages from all OpenStack services
      - Rally DEBUG, which include only Rally debug-messages
     so we should use custom check to know debug-mode, instead of CONF.debug
 
     N312
     """
+    if noqa:
+        return
     excluded_files = ["./rally/common/logging.py"]
 
     point = logical_line.find("CONF.debug")
     if point != -1 and filename not in excluded_files:
         yield (point, "N312 Don't use `CONF.debug`. "
                       "Function `rally.common.logging.is_debug` "
                       "should be used instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_true_instance(physical_line, logical_line, filename):
+def assert_true_instance(logical_line, noqa=False):
     """Check for assertTrue(isinstance(a, b)) sentences
 
     N320
     """
+    if noqa:
+        return
     if re_assert_true_instance.match(logical_line):
         yield (0, "N320 assertTrue(isinstance(a, b)) sentences not allowed, "
                   "you should use assertIsInstance(a, b) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_type(physical_line, logical_line, filename):
+def assert_equal_type(logical_line, noqa=False):
     """Check for assertEqual(type(A), B) sentences
 
     N321
     """
+    if noqa:
+        return
     if re_assert_equal_type.match(logical_line):
         yield (0, "N321 assertEqual(type(A), B) sentences not allowed, "
                   "you should use assertIsInstance(a, b) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_none(physical_line, logical_line, filename):
+def assert_equal_none(logical_line, noqa=False):
     """Check for assertEqual(A, None) or assertEqual(None, A) sentences
 
     N322
     """
+    if noqa:
+        return
     res = (re_assert_equal_start_with_none.search(logical_line)
            or re_assert_equal_end_with_none.search(logical_line))
     if res:
         yield (0, "N322 assertEqual(A, None) or assertEqual(None, A) "
                   "sentences not allowed, you should use assertIsNone(A) "
                   "instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_true_or_false_with_in(physical_line, logical_line, filename):
+def assert_true_or_false_with_in(logical_line, noqa=False):
     """Check assertTrue/False(A in/not in B) with collection contents
 
     Check for assertTrue/False(A in B), assertTrue/False(A not in B),
     assertTrue/False(A in B, message) or assertTrue/False(A not in B, message)
     sentences.
 
     N323
     """
+    if noqa:
+        return
     res = (re_assert_true_false_with_in_or_not_in.search(logical_line)
            or re_assert_true_false_with_in_or_not_in_spaces.search(
                logical_line))
     if res:
         yield (0, "N323 assertTrue/assertFalse(A in/not in B)sentences not "
                   "allowed, you should use assertIn(A, B) or assertNotIn(A, B)"
                   " instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_in(physical_line, logical_line, filename):
+def assert_equal_in(logical_line, noqa=False):
     """Check assertEqual(A in/not in B, True/False) with collection contents
 
     Check for assertEqual(A in B, True/False), assertEqual(True/False, A in B),
     assertEqual(A not in B, True/False) or assertEqual(True/False, A not in B)
     sentences.
 
     N324
     """
+    if noqa:
+        return
     res = (re_assert_equal_in_end_with_true_or_false.search(logical_line)
            or re_assert_equal_in_start_with_true_or_false.search(logical_line))
     if res:
         yield (0, "N324: Use assertIn/NotIn(A, B) rather than "
                   "assertEqual(A in/not in B, True/False) when checking "
                   "collection contents.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_not_equal_none(physical_line, logical_line, filename):
+def assert_not_equal_none(logical_line, noqa=False):
     """Check for assertNotEqual(A, None) or assertEqual(None, A) sentences
 
     N325
     """
+    if noqa:
+        return
     res = (re_assert_not_equal_start_with_none.search(logical_line)
            or re_assert_not_equal_end_with_none.search(logical_line))
     if res:
         yield (0, "N325 assertNotEqual(A, None) or assertNotEqual(None, A) "
                   "sentences not allowed, you should use assertIsNotNone(A) "
                   "instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_true_or_false(physical_line, logical_line, filename):
+def assert_equal_true_or_false(logical_line, noqa=False):
     """Check for assertEqual(A, True/False) sentences
 
     Check for assertEqual(A, True/False) sentences or
     assertEqual(True/False, A)
 
     N326
     """
+    if noqa:
+        return
     res = (re_assert_equal_end_with_true_or_false.search(logical_line)
            or re_assert_equal_start_with_true_or_false.search(logical_line))
     if res:
         yield (0, "N326 assertEqual(A, True/False) or "
                   "assertEqual(True/False, A) sentences not allowed,"
                   "you should use assertTrue(A) or assertFalse(A) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_direct_rally_objects_import(physical_line, logical_line,
-                                         filename):
+def check_no_direct_rally_objects_import(logical_line, filename, noqa=False):
     """Check if rally.common.objects are properly imported.
 
     If you import "from rally.common import objects" you are able to use
     objects directly like objects.Task.
 
     N340
     """
-    if filename == "./rally/common/objects/__init__.py":
+    if noqa:
         return
-
-    if filename == "./rally/common/objects/endpoint.py":
+    if filename == "./rally/common/objects/__init__.py":
         return
 
     if (logical_line.startswith("from rally.common.objects")
        or logical_line.startswith("import rally.common.objects.")):
         yield (0, "N340: Import objects module:"
                   "`from rally.common import objects`. "
                   "After that you can use directly objects e.g. objects.Task")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_oslo_deprecated_import(physical_line, logical_line, filename):
+def check_no_oslo_deprecated_import(logical_line, noqa=False):
     """Check if oslo.foo packages are not imported instead of oslo_foo ones.
 
     Libraries from oslo.foo namespace are deprecated because of namespace
     problems.
 
     N341
     """
+    if noqa:
+        return
     if (logical_line.startswith("from oslo.")
        or logical_line.startswith("import oslo.")):
         yield (0, "N341: Import oslo module: `from oslo_xyz import ...`. "
                   "The oslo.xyz namespace was deprecated, use oslo_xyz "
                   "instead")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_quotes(physical_line, logical_line, filename):
+def check_quotes(logical_line, noqa=False):
     """Check that single quotation marks are not used
 
     N350
     """
+    if noqa:
+        return
 
     in_string = False
     in_multiline_string = False
     single_quotas_are_used = False
 
     check_tripple = (
         lambda line, i, char: (
@@ -429,41 +421,37 @@
         i += 1
 
     if single_quotas_are_used:
         yield i, "N350 Remove Single quotes"
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_constructor_data_struct(physical_line, logical_line, filename):
+def check_no_constructor_data_struct(logical_line, noqa=False):
     """Check that data structs (lists, dicts) are declared using literals
 
     N351
     """
+    if noqa:
+        return
 
     match = re_no_construct_dict.search(logical_line)
     if match:
         yield 0, "N351 Remove dict() construct and use literal {}"
     match = re_no_construct_list.search(logical_line)
     if match:
         yield 0, "N351 Remove list() construct and use literal []"
 
 
 @core.flake8ext
-def check_dict_formatting_in_string(logical_line, tokens):
+def check_dict_formatting_in_string(logical_line, tokens, noqa=False):
     """Check that strings do not use dict-formatting with a single replacement
 
     N352
     """
-    # NOTE(stpierre): Can't use @skip_ignored_lines here because it's
-    # a stupid decorator that only works on functions that take
-    # (logical_line, filename) as arguments.
-    if (not logical_line
-            or logical_line.startswith("#")
-            or logical_line.endswith("# noqa")):
+    if noqa:
         return
 
     current_string = ""
     in_string = False
     for token_type, text, start, end, line in tokens:
         if token_type == tokenize.STRING:
             if not in_string:
@@ -496,15 +484,15 @@
             in_string = False
             if text == "%":
                 format_keys = set()
                 for match in re_str_format.finditer(current_string):
                     format_keys.add(match.group(1))
                 if len(format_keys) == 1:
                     yield (0,
-                           "N353 Do not use mapping key string formatting "
+                           "N352 Do not use mapping key string formatting "
                            "with a single key")
             if text != ")":
                 # NOTE(stpierre): You can have a parenthesized string
                 # followed by %, so a closing paren doesn't obviate
                 # the possibility for a substitution operator like
                 # every other operator does.
                 current_string = ""
@@ -513,114 +501,99 @@
         else:
             in_string = False
             if token_type == tokenize.NEWLINE:
                 current_string = ""
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_using_unicode(physical_line, logical_line, filename):
-    """Check crosspython unicode usage
-
-    N353
-    """
-
-    if re.search(r"\bunicode\(", logical_line):
-        yield (0, "N353 'unicode' function is absent in python3. Please "
-                  "use 'str' instead.")
-
-
-@core.flake8ext
-def check_raises(physical_line, logical_line, filename):
+def check_raises(logical_line, filename, noqa=False):
     """Check raises usage
 
     N354
     """
+    if noqa:
+        return
 
     ignored_files = ["./tests/unit/test_hacking.py",
                      "./tests/hacking/checks.py"]
     if filename not in ignored_files:
-        if re_raises.search(physical_line):
+        if re_raises.search(logical_line):
             yield (0, "N354 ':Please use ':raises Exception: conditions' "
                       "in docstrings.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_old_type_class(physical_line, logical_line, filename):
+def check_old_type_class(logical_line, noqa=False):
     """Use new-style Python classes
 
     N355
     """
+    if noqa:
+        return
 
     if re_old_type_class.search(logical_line):
         yield (0, "N355 This class does not inherit from anything and thus "
                   "will be an old-style class by default. Try to inherit from "
                   "``object`` or another new-style class.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_datetime_alias(physical_line, logical_line, filename):
+def check_datetime_alias(logical_line, noqa=False):
     """Ensure using ``dt`` as alias for ``datetime``
 
     N356
     """
+    if noqa:
+        return
     if re_datetime_alias.search(logical_line):
         yield 0, "N356 Please use ``dt`` as alias for ``datetime``."
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_db_imports_in_cli(physical_line, logical_line, filename):
+def check_db_imports_in_cli(logical_line, filename, noqa=False):
     """Ensure that CLI modules do not use ``rally.common.db``
 
     N360
     """
+    if noqa:
+        return
     if (not filename.startswith("./rally/cli")
             or filename == "./rally/cli/commands/db.py"):
         return
     if re_db_import.search(logical_line):
         yield (0, "N360 CLI modules do not allow to work with "
                   "`rally.common.db``.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_objects_imports_in_cli(physical_line, logical_line, filename):
+def check_objects_imports_in_cli(logical_line, filename):
     """Ensure that CLI modules do not use ``rally.common.objects``
 
     N361
     """
     if not filename.startswith("./rally/cli"):
         return
     if re_objects_import.search(logical_line):
         yield (0, "N361 CLI modules do not allow to work with "
                   "`rally.common.objects``.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_log_warn(physical_line, logical_line, filename):
+def check_log_warn(logical_line):
     if re_log_warn.search(logical_line):
         yield 0, "N313 LOG.warn is deprecated, please use LOG.warning"
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_opts_import_path(physical_line, logical_line, filename):
+def check_opts_import_path(logical_line, noqa=False):
     """Ensure that we load opts from correct paths only
 
-     N342
-     """
-    excluded_files = ["./rally/task/engine.py",
-                      "./rally/task/context.py",
-                      "./rally/task/scenario.py",
-                      "./rally/common/opts.py"]
-    forbidden_methods = [r".register_opts("]
+    N342
+    """
+    if noqa:
+        return
+    forbidden_methods = [".register_opts("]
 
-    if filename not in excluded_files:
-        for forbidden_method in forbidden_methods:
-            if logical_line.find(forbidden_method) != -1:
-                yield (0, "N342 All options should be loaded from correct "
-                          "paths only. For 'openstack' "
-                          "its './rally/plugin/openstack/cfg'")
+    for forbidden_method in forbidden_methods:
+        if logical_line.find(forbidden_method) != -1:
+            yield (0, "N342 All options should be loaded from correct "
+                      "paths only: rally_openstack/common/cfg")
```

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/barbican/test_secrets.py` & `rally-openstack-2.3.0/tests/unit/common/services/barbican/test_secrets.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/gnocchi/test_metric.py` & `rally-openstack-2.3.0/tests/unit/common/services/gnocchi/test_metric.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/heat/test_main.py` & `rally-openstack-2.3.0/tests/unit/common/services/heat/test_main.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/identity/test_identity.py` & `rally-openstack-2.3.0/tests/unit/common/services/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_common.py` & `rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_common.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_v2.py` & `rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/identity/test_keystone_v3.py` & `rally-openstack-2.3.0/tests/unit/common/services/identity/test_keystone_v3.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_common.py` & `rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_common.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_v1.py` & `rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_v1.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/image/test_glance_v2.py` & `rally-openstack-2.3.0/tests/unit/common/services/image/test_glance_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/image/test_image.py` & `rally-openstack-2.3.0/tests/unit/common/services/image/test_image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/loadbalancer/test_octavia.py` & `rally-openstack-2.3.0/tests/unit/common/services/loadbalancer/test_octavia.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/network/test_net_utils.py` & `rally-openstack-2.3.0/tests/unit/common/services/network/test_net_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/network/test_neutron.py` & `rally-openstack-2.3.0/tests/unit/common/services/network/test_neutron.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/storage/test_block.py` & `rally-openstack-2.3.0/tests/unit/common/services/storage/test_block.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_common.py` & `rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,26 +619,47 @@
             [self.service._unify_transfer.return_value],
             self.service.list_transfers(detailed=True, search_opts=None))
         self.service._impl.list_transfers.assert_called_once_with(
             detailed=True, search_opts=None)
         self.service._unify_transfer.assert_called_once_with(
             "transfer")
 
+    def test_update_volume_type(self):
+        self.assertEqual(self.service._impl.update_volume_type.return_value,
+                         self.service.update_volume_type("volume_type"))
+        self.service._impl.update_volume_type.assert_called_once_with(
+            volume_type="volume_type", name=None, description=None,
+            is_public=None
+        )
+
     def test_get_volume_type(self):
         self.assertEqual(self.service._impl.get_volume_type.return_value,
                          self.service.get_volume_type("volume_type"))
         self.service._impl.get_volume_type.assert_called_once_with(
             "volume_type")
 
     def test_delete_volume_type(self):
         self.assertEqual(self.service._impl.delete_volume_type.return_value,
                          self.service.delete_volume_type("volume_type"))
         self.service._impl.delete_volume_type.assert_called_once_with(
             "volume_type")
 
+    def test_add_type_access(self):
+        self.assertEqual(self.service._impl.add_type_access.return_value,
+                         self.service.add_type_access(volume_type="some_type",
+                                                      project="some_project"))
+        self.service._impl.add_type_access.assert_called_once_with(
+            volume_type="some_type", project="some_project")
+
+    def test_list_type_access(self):
+        self.assertEqual(self.service._impl.list_type_access.return_value,
+                         self.service.list_type_access("some_type"))
+        self.service._impl.list_type_access.assert_called_once_with(
+            "some_type")
+
     def test_set_volume_type_keys(self):
         self.assertEqual(self.service._impl.set_volume_type_keys.return_value,
                          self.service.set_volume_type_keys(
                              "volume_type", metadata="metadata"))
         self.service._impl.set_volume_type_keys.assert_called_once_with(
             "volume_type", "metadata")
```

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v1.py` & `rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,7 +361,21 @@
         self.service._unify_volume = mock.MagicMock()
         self.assertEqual(self.service._unify_volume.return_value,
                          self.service.restore_backup(1, volume_id=1))
         self.service._impl.restore_backup.assert_called_once_with(1,
                                                                   volume_id=1)
         self.service._unify_volume.assert_called_once_with(
             self.service._impl.restore_backup.return_value)
+
+    def test_not_implemented_methods(self):
+        self.assertRaises(
+            NotImplementedError,
+            self.service.update_volume_type, "type"
+        )
+        self.assertRaises(
+            NotImplementedError,
+            self.service.list_type_access, "type"
+        )
+        self.assertRaises(
+            NotImplementedError,
+            self.service.add_type_access, "type", project="project"
+        )
```

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v2.py` & `rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,18 +231,20 @@
     def test_update_volume_type(self):
         volume_type = mock.Mock()
         name = "random_name"
         self.service.generate_random_name = mock.MagicMock(
             return_value=name)
         description = "test update"
 
-        result = self.service.update_volume_type(volume_type,
-                                                 description=description,
-                                                 name=None,
-                                                 is_public=None)
+        result = self.service.update_volume_type(
+            volume_type,
+            description=description,
+            name=self.service.generate_random_name(),
+            is_public=None
+        )
         self.assertEqual(
             self.cinder.volume_types.update.return_value,
             result)
         self._test_atomic_action_timer(self.atomic_actions(),
                                        "cinder_v2.update_volume_type")
 
     def test_add_type_access(self):
```

### Comparing `rally-openstack-2.2.0/tests/unit/common/services/storage/test_cinder_v3.py` & `rally-openstack-2.3.0/tests/unit/common/services/storage/test_cinder_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,18 +236,20 @@
     def test_update_volume_type(self):
         volume_type = mock.Mock()
         name = "random_name"
         self.service.generate_random_name = mock.MagicMock(
             return_value=name)
         description = "test update"
 
-        result = self.service.update_volume_type(volume_type,
-                                                 description=description,
-                                                 update_name=True,
-                                                 is_public=None)
+        result = self.service.update_volume_type(
+            volume_type,
+            description=description,
+            name=self.service.generate_random_name(),
+            is_public=None
+        )
         self.assertEqual(
             self.cinder.volume_types.update.return_value,
             result)
         self._test_atomic_action_timer(self.atomic_actions(),
                                        "cinder_v3.update_volume_type")
 
     def test_add_type_access(self):
```

### Comparing `rally-openstack-2.2.0/tests/unit/common/test_credential.py` & `rally-openstack-2.3.0/tests/unit/common/test_credential.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/test_osclients.py` & `rally-openstack-2.3.0/tests/unit/common/test_osclients.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/test_validators.py` & `rally-openstack-2.3.0/tests/unit/common/test_validators.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/common/wrappers/test_network.py` & `rally-openstack-2.3.0/tests/unit/common/wrappers/test_network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/doc/test_docker_readme.py` & `rally-openstack-2.3.0/tests/unit/doc/test_docker_readme.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/doc/test_docstrings.py` & `rally-openstack-2.3.0/tests/unit/doc/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/doc/test_format.py` & `rally-openstack-2.3.0/tests/unit/doc/test_format.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/doc/test_jsonschemas.py` & `rally-openstack-2.3.0/tests/unit/doc/test_jsonschemas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/doc/test_task_samples.py` & `rally-openstack-2.3.0/tests/unit/doc/test_task_samples.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/environment/platforms/test_existing.py` & `rally-openstack-2.3.0/tests/unit/environment/platforms/test_existing.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/fakes.py` & `rally-openstack-2.3.0/tests/unit/fakes.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     :returns: str, MAC address
     """
     rand_str = generate_name(choices="0123456789abcdef", length=12)
     return ":".join(re.findall("..", rand_str))
 
 
 def setup_dict(data, required=None, defaults=None):
-    """Setup and validate dict scenario_base. on mandatory keys and default data.
+    """Setup and validate dict scenario_base on mandatory keys and default data
 
     This function reduces code that constructs dict objects
     with specific schema (e.g. for API data).
 
     :param data: dict, input data
     :param required: list, mandatory keys to check
     :param defaults: dict, default data
```

### Comparing `rally-openstack-2.2.0/tests/unit/rally_jobs/test_jobs.py` & `rally-openstack-2.3.0/tests/unit/rally_jobs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/rally_jobs/test_zuul_jobs.py` & `rally-openstack-2.3.0/tests/unit/rally_jobs/test_zuul_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,25 @@
     def _parse_job(job):
         if isinstance(job, dict):
             job_name = list(job)[0]
             job_cfg = job[job_name]
             return job_name, job_cfg
         return job, None
 
+    @staticmethod
+    def _tox_job_sorter(job_name):
+        python_maj_version = 0
+        python_min_version = 0
+        _rally, _tox, job_name = job_name.split("-", 3)
+        if job_name.startswith("py"):
+            python_maj_version = int(job_name[2])
+            python_min_version = int(job_name[3:])
+            job_name = "py"
+        return job_name, python_maj_version, python_min_version
+
     def _check_order_of_jobs(self, pipeline):
         jobs = self.project_cfg[pipeline]["jobs"]
 
         specific_jobs = ["rally-dsvm-tox-functional",
                          "rally-openstack-docker-build",
                          "rally-task-basic-with-existing-users",
                          "rally-task-simple-job"]
@@ -60,16 +71,18 @@
             f"expected ({', '.join(specific_jobs)}). "
             f"Next - all other jobs in alphabetic order."
         )
         error_message += "\nPlease place '%s' at the position of '%s'."
 
         jobs_names = [self._parse_job(job)[0] for job in jobs]
 
-        tox_jobs = sorted(job for job in jobs_names
-                          if job.startswith("rally-tox"))
+        tox_jobs = sorted(
+            (job for job in jobs_names if job.startswith("rally-tox-")),
+            key=self._tox_job_sorter
+        )
         for i, job in enumerate(tox_jobs):
             if job != jobs[i]:
                 self.fail(error_message % (job, jobs[i]))
 
         for job in specific_jobs:
             if job not in jobs_names:
                 continue
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/cleanup/test_base.py` & `rally-openstack-2.3.0/tests/unit/task/cleanup/test_base.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/cleanup/test_manager.py` & `rally-openstack-2.3.0/tests/unit/task/cleanup/test_manager.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/cleanup/test_resources.py` & `rally-openstack-2.3.0/tests/unit/task/cleanup/test_resources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/cinder/test_volume_types.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/cinder/test_volume_types.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/cinder/test_volumes.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/cinder/test_volumes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/test_admin.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/test_admin.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/cleanup/test_user.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/cleanup/test_user.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/dataplane/test_heat.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/dataplane/test_heat.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/designate/test_zones.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/designate/test_zones.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/glance/test_images.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/glance/test_images.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/heat/test_stacks.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/heat/test_stacks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/keystone/test_roles.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/keystone/test_roles.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/keystone/test_users.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/keystone/test_users.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_ca_certs.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_ca_certs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_cluster_templates.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_cluster_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/magnum/test_clusters.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/magnum/test_clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_security_services.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_security_services.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_share_networks.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_share_networks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/manila/test_manila_shares.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/manila/test_manila_shares.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/monasca/test_metrics.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/monasca/test_metrics.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/murano/test_murano_environments.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/murano/test_murano_environments.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/murano/test_murano_packages.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/murano/test_murano_packages.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/network/test_allow_ssh.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/network/test_allow_ssh.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/network/test_existing_network.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/network/test_existing_network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/network/test_network.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/network/test_network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/network/test_networking_agents.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/network/test_networking_agents.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/network/test_routers.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/network/test_routers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/neutron/test_lbaas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/neutron/test_lbaas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_flavors.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_flavors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_keypairs.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_keypairs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/nova/test_servers.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/nova/test_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                     "users_per_tenant": 5,
                     "concurrent": 10,
                 },
                 "servers": {
                     "auto_assign_nic": True,
                     "servers_per_tenant": 5,
                     "image": {
-                        "name": "cirros-0.3.4-x86_64-uec",
+                        "name": "cirros-0.5.2-x86_64-uec",
                     },
                     "flavor": {
                         "name": "m1.tiny",
                     },
                     "nics": ["foo", "bar"]
                 },
             },
@@ -144,15 +144,15 @@
                     "tenants": 2,
                     "users_per_tenant": 5,
                     "concurrent": 10,
                 },
                 "servers": {
                     "servers_per_tenant": 5,
                     "image": {
-                        "name": "cirros-0.3.4-x86_64-uec",
+                        "name": "cirros-0.5.2-x86_64-uec",
                     },
                     "flavor": {
                         "name": "m1.tiny",
                     },
                 },
             },
             "admin": {
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_cinder_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_cinder_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_designate_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_designate_quotas.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def test_update(self):
         clients = mock.MagicMock()
         quotas = designate_quotas.DesignateQuotas(clients)
         tenant_id = mock.MagicMock()
         quotas_values = {
             "api_export_size": 5,
             "zones": 5,
-            "zones_recordsets": 20,
-            "zones_records": 20,
+            "zone_recordsets": 20,
+            "zone_records": 20,
             "recordset_records": 20,
         }
         quotas.update(tenant_id, **quotas_values)
         clients.designate().quotas.update.assert_called_once_with(
             tenant_id, quotas_values)
 
     def test_delete(self):
@@ -41,15 +41,15 @@
         tenant_id = mock.MagicMock()
         quotas.delete(tenant_id)
         clients.designate().quotas.reset.assert_called_once_with(tenant_id)
 
     def test_get(self):
         tenant_id = "tenant_id"
         quotas = {"api_export_size": -1, "zones": -1,
-                  "zones_recordsets": 2, "zones_records": 3,
+                  "zone_recordsets": 2, "zone_records": 3,
                   "recordset_records": 3}
         clients = mock.MagicMock()
         clients.designate.return_value.quotas.get.return_value = quotas
         designate_quo = designate_quotas.DesignateQuotas(clients)
 
         self.assertEqual(quotas, designate_quo.get(tenant_id))
         clients.designate().quotas.get.assert_called_once_with(tenant_id)
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_manila_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_manila_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_neutron_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_neutron_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_nova_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_nova_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/quotas/test_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/quotas/test_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_cluster.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_cluster.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_image.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_input_data_sources.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_input_data_sources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_job_binaries.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_job_binaries.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/sahara/test_sahara_output_data_sources.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/sahara/test_sahara_output_data_sources.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/senlin/test_profiles.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/senlin/test_profiles.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/swift/test_objects.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/swift/test_objects.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/swift/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/swift/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/test_api_versions.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/vm/test_custom_image.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/vm/test_custom_image.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/vm/test_image_command_customizer.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/vm/test_image_command_customizer.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/contexts/watcher/test_audit_templates.py` & `rally-openstack-2.3.0/tests/unit/task/contexts/watcher/test_audit_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/hooks/test_fault_injection.py` & `rally-openstack-2.3.0/tests/unit/task/hooks/test_fault_injection.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/authenticate/test_authenticate.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/authenticate/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_containers.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_containers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_orders.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_orders.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_secrets.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_secrets.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/barbican/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/barbican/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_qos_specs.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_qos_specs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volume_backups.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volume_backups.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volume_types.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volume_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 from unittest import mock
 
 from rally import exceptions as rally_exceptions
 from rally_openstack.task.scenarios.cinder import volume_types
 from tests.unit import test
 
-CINDER_V2_PATH = ("rally_openstack.common.services.storage"
-                  ".cinder_v2.CinderV2Service")
-
 
 class CinderVolumeTypesTestCase(test.ScenarioTestCase):
 
     def setUp(self):
         super(CinderVolumeTypesTestCase, self).setUp()
         patch = mock.patch(
             "rally_openstack.common.services.storage.block.BlockStorage")
@@ -153,34 +150,35 @@
                           scenario.run,
                           description=description, is_public=is_public)
 
         mock_service.create_volume_type.assert_called_once_with(
             description=description, is_public=is_public)
         mock_service.list_types.assert_called_once_with()
 
-    @mock.patch("%s.create_volume_type" % CINDER_V2_PATH)
-    @mock.patch("%s.update_volume_type" % CINDER_V2_PATH)
-    def test_create_and_update_volume_type(self, mock_update_volume_type,
-                                           mock_create_volume_type):
+    def test_create_and_update_volume_type(self):
+        mock_service = self.mock_cinder.return_value
         scenario = volume_types.CreateAndUpdateVolumeType(self._get_context())
         fake_type = mock.MagicMock()
         fake_type.name = "any"
         create_description = "test create"
         update_description = "test update"
-        mock_create_volume_type.return_value = fake_type
+        mock_service.create_volume_type.return_value = fake_type
         scenario.run(description=create_description,
                      update_description=update_description)
 
-        mock_create_volume_type.assert_called_once_with(
+        mock_service.create_volume_type.assert_called_once_with(
             description=create_description,
             is_public=True)
-        mock_update_volume_type.assert_called_once_with(
-            fake_type, name="any",
+        mock_service.update_volume_type.assert_called_once_with(
+            fake_type,
             description=update_description,
-            is_public=None)
+            # update_is_public and update_name are not specified, so should
+            # not be used
+            is_public=None, name=None
+        )
 
     def test_create_volume_type_and_encryption_type(self):
         mock_service = self.mock_cinder.return_value
         scenario = volume_types.CreateVolumeTypeAndEncryptionType(
             self._get_context())
         description = "rally tests creating types"
         is_public = False
@@ -288,23 +286,20 @@
                      update_key_size="update_ks",
                      update_control_location="update_cl")
         mock_service.create_encryption_type.assert_called_once_with(
             "fake_id", specs=create_specs)
         mock_service.update_encryption_type.assert_called_once_with(
             "fake_id", specs=update_specs)
 
-    @mock.patch("%s.list_type_access" % CINDER_V2_PATH)
-    @mock.patch("%s.add_type_access" % CINDER_V2_PATH)
-    @mock.patch("%s.create_volume_type" % CINDER_V2_PATH)
-    def test_create_volume_type_add_and_list_type_access(
-        self, mock_create_volume_type, mock_add_type_access,
-            mock_list_type_access):
+    def test_create_volume_type_add_and_list_type_access(self):
+        mock_service = self.mock_cinder.return_value
         scenario = volume_types.CreateVolumeTypeAddAndListTypeAccess(
             self._get_context())
         fake_type = mock.Mock()
-        mock_create_volume_type.return_value = fake_type
+        mock_service.create_volume_type.return_value = fake_type
 
         scenario.run(description=None, is_public=False)
-        mock_create_volume_type.assert_called_once_with(
+        mock_service.create_volume_type.assert_called_once_with(
             description=None, is_public=False)
-        mock_add_type_access.assert_called_once_with(fake_type, project="fake")
-        mock_list_type_access.assert_called_once_with(fake_type)
+        mock_service.add_type_access.assert_called_once_with(
+            fake_type, project="fake")
+        mock_service.list_type_access.assert_called_once_with(fake_type)
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/cinder/test_volumes.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/cinder/test_volumes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/designate/test_basic.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/designate/test_basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/designate/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/designate/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/glance/test_images.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/glance/test_images.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_archive_policy.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_archive_policy.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_archive_policy_rule.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_archive_policy_rule.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_capabilities.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_metric.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_metric.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_resource.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_resource.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_resource_type.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_status.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_status.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/gnocchi/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/gnocchi/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/heat/test_stacks.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/heat/test_stacks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/heat/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/heat/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/test_nodes.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/ironic/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/ironic/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/keystone/test_basic.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/keystone/test_basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_loadbalancers.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_loadbalancers.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_pools.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_pools.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/loadbalancer/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/loadbalancer/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_cluster_templates.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_cluster_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_clusters.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_k8s_pods.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_k8s_pods.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/magnum/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/magnum/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/manila/test_shares.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/manila/test_shares.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/manila/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/manila/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
         {"new_size": 10}
     )
     def test__extend_share(self, new_size):
         fake_share = mock.MagicMock()
 
         self.scenario._extend_share(fake_share, new_size)
 
-        fake_share.extend.assert_called_with(new_size)
+        self.clients("manila").shares.extend.assert_called_once_with(
+            fake_share, new_size)
 
         self.mock_wait_for_status.mock.assert_called_once_with(
             fake_share,
             ready_statuses=["available"],
             update_resource=self.mock_get_from_manager.mock.return_value,
             timeout=300, check_interval=3)
         self.mock_get_from_manager.mock.assert_called_once_with()
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_executions.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_executions.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/mistral/test_workbooks.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/mistral/test_workbooks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/test_metrics.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/test_metrics.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/monasca/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/monasca/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_environments.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_environments.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_packages.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_packages.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/murano/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/murano/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_bgpvpn.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v1.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v1.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v2.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_loadbalancer_v2.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_network.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_network.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_security_groups.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_trunk.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_trunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,23 @@
         net = mock.MagicMock()
         scenario = trunk.CreateAndListTrunks(self.context)
         scenario._create_network = mock.Mock(return_value=net)
         scenario._create_port = mock.MagicMock()
         scenario._create_trunk = mock.MagicMock()
         scenario._list_subports_by_trunk = mock.MagicMock()
         scenario._update_port = mock.Mock()
-        scenario._list_ports_by_device_id = mock.Mock()
         scenario.run(network_create_args=network_create_args,
                      subport_count=subport_count)
         scenario._create_network.assert_called_once_with(
             network_create_args)
         scenario._create_port.assert_has_calls(
             [mock.call(net, {})
              for _ in range(subport_count + 1)])
         self.assertEqual(1, scenario._create_trunk.call_count)
-        self.assertEqual(1, scenario._update_port.call_count)
         self.assertEqual(1, scenario._list_subports_by_trunk.call_count)
-        self.assertEqual(1, scenario._list_ports_by_device_id.call_count)
 
     def test_boot_server_with_subports(self):
         img_name = "img"
         flavor_uuid = 0
         subport_count = 10
         network_create_args = {}
         net = mock.MagicMock()
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/neutron/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/neutron/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_agents.py` & `rally-openstack-2.3.0/tests/unit/test_plugins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-# Copyright 2016 IBM Corp.
 # All Rights Reserved.
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from unittest import mock
+import subprocess
 
-from rally_openstack.task.scenarios.nova import agents
 from tests.unit import test
 
 
-class NovaAgentsTestCase(test.TestCase):
+class PluginsLoadingTestCase(test.TestCase):
 
-    def test_list_agents(self):
-        scenario = agents.ListAgents()
-        scenario._list_agents = mock.Mock()
-        scenario.run(hypervisor=None)
-        scenario._list_agents.assert_called_once_with(None)
+    def test_plugins_loaded(self):
+        subprocess.check_output(
+            ["rally", "--debug", "plugin", "show", "Dummy.openstack"]
+        )
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_aggregates.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_availability_zones.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_flavors.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_flavors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_hypervisors.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_hypervisors.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_keypairs.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_keypairs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_server_groups.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_server_groups.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_servers.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,14 +564,54 @@
             scenario._detach_volume.assert_called_once_with(fake_server,
                                                             fake_volume)
             cinder.delete_volume.assert_called_once_with(fake_volume)
             scenario._delete_server.assert_called_once_with(fake_server,
                                                             force=False)
 
     @mock.patch("rally_openstack.common.services.storage.block.BlockStorage")
+    def test_boot_server_attach_created_volume_and_extend(
+            self, mock_block_storage, do_delete=False):
+        fake_volume = mock.MagicMock()
+        fake_server = mock.MagicMock()
+        flavor = mock.MagicMock()
+        fake_attachment = mock.MagicMock()
+
+        cinder = mock_block_storage.return_value
+        cinder.create_volume.return_value = fake_volume
+
+        scenario = servers.BootServerAttachCreatedVolumeAndExtend(
+            self.context, clients=mock.Mock())
+        scenario.generate_random_name = mock.MagicMock(return_value="name")
+        scenario._boot_server = mock.MagicMock(return_value=fake_server)
+        scenario._attach_volume = mock.MagicMock(return_value=fake_attachment)
+        scenario._detach_volume = mock.MagicMock()
+        scenario._delete_server = mock.MagicMock()
+        scenario.sleep_between = mock.MagicMock()
+
+        volume_size = 10
+        new_volume_size = 20
+        scenario.run("img", flavor, volume_size, new_volume_size,
+                     min_sleep=10, max_sleep=20, do_delete=do_delete)
+
+        scenario._boot_server.assert_called_once_with("img", flavor)
+        cinder.create_volume.assert_called_once_with(volume_size)
+        scenario._attach_volume.assert_called_once_with(fake_server,
+                                                        fake_volume)
+        scenario.sleep_between.assert_called_once_with(10, 20)
+        cinder.extend_volume.assert_called_once_with(
+            fake_volume, new_size=new_volume_size)
+
+        if do_delete:
+            scenario._detach_volume.assert_called_once_with(fake_server,
+                                                            fake_volume)
+            cinder.delete_volume.assert_called_once_with(fake_volume)
+            scenario._delete_server.assert_called_once_with(fake_server,
+                                                            force=False)
+
+    @mock.patch("rally_openstack.common.services.storage.block.BlockStorage")
     def test_list_attachments(self, mock_block_storage):
         mock_volume_service = mock_block_storage.return_value
         fake_volume = mock.MagicMock()
         fake_server = mock.MagicMock()
         flavor = mock.MagicMock()
         fake_attachment = mock.MagicMock()
         list_attachments = [mock.MagicMock(),
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_services.py` & `rally-openstack-2.3.0/tests/unit/task/test_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,47 @@
-# Copyright 2016 IBM Corp.
+# Copyright 2013: Mirantis Inc.
 # All Rights Reserved.
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
-#         http://www.apache.org/licenses/LICENSE-2.0
-#
+#         http://www.apache.org/licenses/LICENSE-2.0#
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from unittest import mock
-
-from rally_openstack.task.scenarios.nova import services
+from rally_openstack.task import context
 from tests.unit import test
 
 
-class NovaServicesTestCase(test.TestCase):
+class TenantIteratorTestCase(test.TestCase):
+
+    def test__iterate_per_tenant(self):
+
+        class DummyContext(context.OpenStackContext):
+            def __init__(self, ctx):
+                self.context = ctx
+
+            def setup(self):
+                pass
+
+            def cleanup(self):
+                pass
+
+        users = []
+        tenants_count = 2
+        users_per_tenant = 5
+        for tenant_id in range(tenants_count):
+            for user_id in range(users_per_tenant):
+                users.append({"id": str(user_id),
+                              "tenant_id": str(tenant_id)})
+
+        expected_result = [
+            ({"id": "0", "tenant_id": str(i)}, str(i)) for i in range(
+                tenants_count)]
+        real_result = [
+            i for i in DummyContext({"users": users})._iterate_per_tenants()]
 
-    def test_list_services(self):
-        scenario = services.ListServices()
-        scenario._list_services = mock.Mock()
-        scenario.run(host="foo_host", binary="foo_hypervisor")
-        scenario._list_services.assert_called_once_with("foo_host",
-                                                        "foo_hypervisor")
+        self.assertEqual(expected_result, real_result)
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/nova/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/nova/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,21 +219,31 @@
         self._test_atomic_action_timer(nova_scenario.atomic_actions(),
                                        "nova.unpause_server")
 
     def test__shelve_server(self):
         nova_scenario = utils.NovaScenario(context=self.context)
         nova_scenario._shelve_server(self.server)
         self.server.shelve.assert_called_once_with()
-        self.mock_wait_for_status.mock.assert_called_once_with(
-            self.server,
-            ready_statuses=["SHELVED_OFFLOADED"],
-            update_resource=self.mock_get_from_manager.mock.return_value,
-            check_interval=CONF.openstack.nova_server_shelve_poll_interval,
-            timeout=CONF.openstack.nova_server_shelve_timeout)
-        self.mock_get_from_manager.mock.assert_called_once_with()
+        self.mock_wait_for_status.mock.assert_has_calls([
+            mock.call(
+                self.server,
+                ready_statuses=["SHELVED_OFFLOADED"],
+                update_resource=self.mock_get_from_manager.mock.return_value,
+                check_interval=CONF.openstack.nova_server_shelve_poll_interval,
+                timeout=CONF.openstack.nova_server_shelve_timeout
+            ),
+            mock.call(
+                self.server,
+                ready_statuses=["None"],
+                status_attr="OS-EXT-STS:task_state",
+                update_resource=self.mock_get_from_manager.mock.return_value,
+                check_interval=CONF.openstack.nova_server_shelve_poll_interval,
+                timeout=CONF.openstack.nova_server_shelve_timeout)]
+        )
+        self.assertEqual(2, self.mock_get_from_manager.mock.call_count)
         self._test_atomic_action_timer(nova_scenario.atomic_actions(),
                                        "nova.shelve_server")
 
     def test__unshelve_server(self):
         nova_scenario = utils.NovaScenario(context=self.context)
         nova_scenario._unshelve_server(self.server)
         self.server.unshelve.assert_called_once_with()
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/test_quotas.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/test_quotas.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/quotas/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/quotas/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_clusters.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_jobs.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_jobs.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_node_group_templates.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_node_group_templates.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/sahara/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/sahara/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/test_clusters.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/test_clusters.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/senlin/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/senlin/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/swift/test_objects.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/swift/test_objects.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/swift/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/swift/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/vm/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/vm/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/vm/test_vmtasks.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/vm/test_vmtasks.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/vm/workloads/test_siege.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/vm/workloads/test_siege.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/test_basic.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/test_basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/watcher/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/watcher/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/test_basic.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/test_basic.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/scenarios/zaqar/test_utils.py` & `rally-openstack-2.3.0/tests/unit/task/scenarios/zaqar/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/test_scenario.py` & `rally-openstack-2.3.0/tests/unit/task/test_scenario.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/task/test_types.py` & `rally-openstack-2.3.0/tests/unit/task/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,48 +173,48 @@
 
 
 class GlanceImageTestCase(test.TestCase):
 
     def setUp(self):
         super(GlanceImageTestCase, self).setUp()
         self.clients = fakes.FakeClients()
-        image1 = fakes.FakeResource(name="cirros-0.3.4-uec", id="100")
+        image1 = fakes.FakeResource(name="cirros-0.5.2-uec", id="100")
         self.clients.glance().images._cache(image1)
-        image2 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk", id="101")
+        image2 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk", id="101")
         self.clients.glance().images._cache(image2)
-        image3 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        image3 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                     id="102")
         self.clients.glance().images._cache(image3)
-        image4 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        image4 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                     id="103")
         self.clients.glance().images._cache(image4)
         self.type_cls = types.GlanceImage(
             context={"admin": {"credential": mock.Mock()}})
         self.type_cls._clients = self.clients
 
     def test_preprocess_by_id(self):
         resource_spec = {"id": "100"}
         image_id = self.type_cls.pre_process(
             resource_spec=resource_spec, config={})
         self.assertEqual("100", image_id)
 
     def test_preprocess_by_name(self):
-        resource_spec = {"name": "^cirros-0.3.4-uec$"}
+        resource_spec = {"name": "^cirros-0.5.2-uec$"}
         image_id = self.type_cls.pre_process(
             resource_spec=resource_spec, config={})
         self.assertEqual("100", image_id)
 
     def test_preprocess_by_name_no_match(self):
-        resource_spec = {"name": "cirros-0.3.4-uec-boot"}
+        resource_spec = {"name": "cirros-0.5.2-uec-boot"}
         self.assertRaises(exceptions.InvalidScenarioArgument,
                           self.type_cls.pre_process,
                           resource_spec=resource_spec, config={})
 
     def test_preprocess_by_name_match_multiple(self):
-        resource_spec = {"name": "cirros-0.3.4-uec-ramdisk-copy"}
+        resource_spec = {"name": "cirros-0.5.2-uec-ramdisk-copy"}
         self.assertRaises(exceptions.InvalidScenarioArgument,
                           self.type_cls.pre_process,
                           resource_spec=resource_spec, config={})
 
     def test_preprocess_by_regex(self):
         resource_spec = {"regex": "-uec$"}
         image_id = self.type_cls.pre_process(
@@ -259,42 +259,42 @@
 
 
 class EC2ImageTestCase(test.TestCase):
 
     def setUp(self):
         super(EC2ImageTestCase, self).setUp()
         self.clients = fakes.FakeClients()
-        image1 = fakes.FakeResource(name="cirros-0.3.4-uec", id="100")
+        image1 = fakes.FakeResource(name="cirros-0.5.2-uec", id="100")
         self.clients.glance().images._cache(image1)
-        image2 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk", id="102")
+        image2 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk", id="102")
         self.clients.glance().images._cache(image2)
-        image3 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        image3 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                     id="102")
         self.clients.glance().images._cache(image3)
-        image4 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        image4 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                     id="103")
         self.clients.glance().images._cache(image4)
 
-        ec2_image1 = fakes.FakeResource(name="cirros-0.3.4-uec", id="200")
-        ec2_image2 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk",
+        ec2_image1 = fakes.FakeResource(name="cirros-0.5.2-uec", id="200")
+        ec2_image2 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk",
                                         id="201")
-        ec2_image3 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        ec2_image3 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                         id="202")
-        ec2_image4 = fakes.FakeResource(name="cirros-0.3.4-uec-ramdisk-copy",
+        ec2_image4 = fakes.FakeResource(name="cirros-0.5.2-uec-ramdisk-copy",
                                         id="203")
 
         self.clients.ec2().get_all_images = mock.Mock(
             return_value=[ec2_image1, ec2_image2, ec2_image3, ec2_image4])
 
         self.type_cls = types.EC2Image(
             context={"admin": {"credential": mock.Mock()}})
         self.type_cls._clients = self.clients
 
     def test_preprocess_by_name(self):
-        resource_spec = {"name": "^cirros-0.3.4-uec$"}
+        resource_spec = {"name": "^cirros-0.5.2-uec$"}
         ec2_image_id = self.type_cls.pre_process(resource_spec=resource_spec,
                                                  config={})
         self.assertEqual("200", ec2_image_id)
 
     def test_preprocess_by_id(self):
         resource_spec = {"id": "100"}
         ec2_image_id = self.type_cls.pre_process(resource_spec=resource_spec,
@@ -304,21 +304,21 @@
     def test_preprocess_by_id_no_match(self):
         resource_spec = {"id": "101"}
         self.assertRaises(exceptions.InvalidScenarioArgument,
                           self.type_cls.pre_process,
                           resource_spec=resource_spec, config={})
 
     def test_preprocess_by_name_no_match(self):
-        resource_spec = {"name": "cirros-0.3.4-uec-boot"}
+        resource_spec = {"name": "cirros-0.5.2-uec-boot"}
         self.assertRaises(exceptions.InvalidScenarioArgument,
                           self.type_cls.pre_process,
                           resource_spec=resource_spec, config={})
 
     def test_preprocess_by_name_match_multiple(self):
-        resource_spec = {"name": "cirros-0.3.4-uec-ramdisk-copy"}
+        resource_spec = {"name": "cirros-0.5.2-uec-ramdisk-copy"}
         self.assertRaises(exceptions.InvalidScenarioArgument,
                           self.type_cls.pre_process,
                           resource_spec=resource_spec, config={})
 
     def test_preprocess_by_regex(self):
         resource_spec = {"regex": "-uec$"}
         ec2_image_id = self.type_cls.pre_process(resource_spec=resource_spec,
```

### Comparing `rally-openstack-2.2.0/tests/unit/task/ui/charts/test_osprofilerchart.py` & `rally-openstack-2.3.0/tests/unit/task/ui/charts/test_osprofilerchart.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test.py` & `rally-openstack-2.3.0/tests/unit/test.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test__compat.py` & `rally-openstack-2.3.0/tests/unit/test__compat.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_ddt.py` & `rally-openstack-2.3.0/tests/unit/test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_hacking.py` & `rally-openstack-2.3.0/tests/unit/test_hacking.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,114 +6,111 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import inspect
 import io
 import tokenize
 
 import ddt
 
 from tests.hacking import checks
 from tests.unit import test
 
 
 @ddt.ddt
 class HackingTestCase(test.TestCase):
 
     def _assert_good_samples(self, checker, samples, module_file="f"):
+        spec = inspect.getfullargspec(checker)
+        base_args = {}
+        if "filename" in spec.args:
+            base_args["filename"] = module_file
         for s in samples:
-            self.assertEqual([], list(checker(s, s, module_file)), s)
+            args = {"logical_line": s, **base_args}
+            self.assertEqual([], list(checker(*args)), s)
 
     def _assert_bad_samples(self, checker, samples, module_file="f"):
+        spec = inspect.getfullargspec(checker)
+        base_args = {}
+        if "filename" in spec.args:
+            base_args["filename"] = module_file
+
         for s in samples:
-            self.assertEqual(1, len(list(checker(s, s, module_file))), s)
+            args = {"logical_line": s, **base_args}
+            self.assertEqual(1, len(list(checker(**args))), s)
 
     def test__parse_assert_mock_str(self):
         pos, method, obj = checks._parse_assert_mock_str(
             "mock_clients.fake().quotas.delete.assert_called_once()")
         self.assertEqual("assert_called_once", method)
         self.assertEqual("mock_clients.fake().quotas.delete", obj)
 
     def test__parse_assert_mock_str_no_assert(self):
         pos, method, obj = checks._parse_assert_mock_str(
             "mock_clients.fake().quotas.delete.")
         self.assertIsNone(pos)
         self.assertIsNone(method)
         self.assertIsNone(obj)
 
-    @ddt.data(
-        {"line": "fdafadfdas  # noqa", "result": []},
-        {"line": "  # fdafadfdas", "result": []},
-        {"line": "  ", "result": []},
-        {"line": "otherstuff", "result": [42]}
-    )
-    @ddt.unpack
-    def test_skip_ignored_lines(self, line, result):
-
-        @checks.skip_ignored_lines
-        def any_gen(physical_line, logical_line, file_name):
-            yield 42
-
-        self.assertEqual(result, list(any_gen(line, line, "f")))
-
     def test_correct_usage_of_assert_from_mock(self):
         correct_method_names = ["assert_any_call", "assert_called_once_with",
                                 "assert_called_with", "assert_has_calls"]
         for name in correct_method_names:
             line = "some_mock.%s(asd)" % name
             self.assertEqual(0, len(
                 list(checks.check_assert_methods_from_mock(
                     line, line, "./tests/fake/test"))))
 
     def test_wrong_usage_of_broad_assert_from_mock(self):
         fake_method = "rtfm.assert_something()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test"))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N301"))
 
     def test_wrong_usage_of_assert_called_from_mock(self):
         fake_method = "rtfm.assert_called()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test", False))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N302"))
 
     def test_wrong_usage_of_assert_called_once_from_mock(self):
         fake_method = "rtfm.assert_called_once()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test", False))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N303"))
 
     def test_check_wrong_logging_import(self):
         bad_imports = ["from oslo_log import log",
                        "import oslo_log",
                        "import logging"]
         good_imports = ["from rally.common import logging",
                         "from rally.common.logging",
                         "import rally.common.logging"]
 
         for bad in bad_imports:
-            checkres = checks.check_import_of_logging(bad, bad, "fakefile")
+            checkres = checks.check_import_of_logging(bad, "fakefile")
             self.assertIsNotNone(next(checkres))
 
         for bad in bad_imports:
             checkres = checks.check_import_of_logging(
-                bad, bad, "./rally/common/logging.py")
+                bad, "./rally/common/logging.py")
             self.assertEqual([], list(checkres))
 
         for good in good_imports:
-            checkres = checks.check_import_of_logging(good, good, "fakefile")
+            checkres = checks.check_import_of_logging(good, "fakefile")
             self.assertEqual([], list(checkres))
 
     def test_no_use_conf_debug_check(self):
         bad_samples = [
             "if CONF.debug:",
             "if cfg.CONF.debug"
         ]
@@ -130,54 +127,49 @@
         {
             "line": "self.assertTrue()",
             "result": 0
         }
     )
     @ddt.unpack
     def test_assert_true_instance(self, line, result):
-        self.assertEqual(
-            result, len(list(checks.assert_true_instance(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_true_instance(line))))
 
     @ddt.data(
         {
             "line": "self.assertEqual(type(als['QuicAssist']), list)",
             "result": 1
         },
         {
             "line": "self.assertTrue()",
             "result": 0
         }
     )
     @ddt.unpack
     def test_assert_equal_type(self, line, result):
-        self.assertEqual(result,
-                         len(list(checks.assert_equal_type(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_equal_type(line))))
 
     @ddt.data(
         {"line": "self.assertEqual(A, None)", "result": 1},
         {"line": "self.assertEqual(None, A)", "result": 1},
         {"line": "self.assertIsNone()", "result": 0}
     )
     @ddt.unpack
     def test_assert_equal_none(self, line, result):
 
-        self.assertEqual(result,
-                         len(list(checks.assert_equal_none(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_equal_none(line))))
 
     @ddt.data(
         {"line": "self.assertNotEqual(A, None)", "result": 1},
         {"line": "self.assertNotEqual(None, A)", "result": 1},
         {"line": "self.assertIsNotNone()", "result": 0}
     )
     @ddt.unpack
     def test_assert_not_equal_none(self, line, result):
 
-        self.assertEqual(result,
-                         len(list(checks.assert_not_equal_none(line,
-                                                               line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_not_equal_none(line))))
 
     def test_assert_true_or_false_with_in_or_not_in(self):
         good_lines = [
             "self.assertTrue(any(A > 5 for A in B))",
             "self.assertTrue(any(A > 5 for A in B), 'some message')",
             "self.assertFalse(some in list1 and some2 in list2)"
         ]
@@ -330,75 +322,61 @@
             sample = "print(%s)" % sample
             tokens = tokenize.generate_tokens(
                 io.StringIO(sample).readline)
             self.assertEqual(
                 [],
                 list(checks.check_dict_formatting_in_string(sample, tokens)))
 
-    @ddt.data(
-        "text = unicode('sometext')",
-        "text = process(unicode('sometext'))"
-    )
-    def test_check_using_unicode(self, line):
-
-        checkres = checks.check_using_unicode(line, line, "fakefile")
-        self.assertIsNotNone(next(checkres))
-        self.assertEqual([], list(checkres))
-
     def test_check_raises(self):
         self._assert_bad_samples(
             checks.check_raises,
             ["text = :raises: Exception if conditions"])
 
         self._assert_good_samples(
             checks.check_raises,
             ["text = :raises Exception: if conditions"]
         )
 
     def test_check_db_imports_of_cli(self):
         line = "from rally.common import db"
 
-        next(checks.check_db_imports_in_cli(
-            line, line, "./rally/cli/filename"))
+        next(checks.check_db_imports_in_cli(line, "./rally/cli/filename"))
 
-        checkres = checks.check_db_imports_in_cli(
-            line, line, "./filename")
+        checkres = checks.check_db_imports_in_cli(line, "./filename")
         self.assertRaises(StopIteration, next, checkres)
 
     def test_check_objects_imports_of_cli(self):
         line = "from rally.common import objects"
 
-        next(checks.check_objects_imports_in_cli(
-            line, line, "./rally/cli/filename"))
+        next(checks.check_objects_imports_in_cli(line, "./rally/cli/filename"))
 
-        checkres = checks.check_objects_imports_in_cli(
-            line, line, "./filename")
+        checkres = checks.check_objects_imports_in_cli(line, "./filename")
         self.assertRaises(StopIteration, next, checkres)
 
     @ddt.data(
         "class Oldstype():",
         "class Oldstyle:"
     )
     def test_check_old_type_class(self, line):
-        checkres = checks.check_old_type_class(line, line, "fakefile")
+        checkres = checks.check_old_type_class(line)
         self.assertIsNotNone(next(checkres))
         self.assertEqual([], list(checkres))
 
     def test_check_datetime_alias(self):
         lines = ["import datetime as date",
                  "import datetime",
                  "import datetime as dto",
                  "from datetime import datetime as dtime"]
 
         for line in lines:
-            checkres = checks.check_datetime_alias(line, line, "fakefile")
+            checkres = checks.check_datetime_alias(line)
             self.assertIsNotNone(next(checkres))
             self.assertEqual([], list(checkres))
 
         line = "import datetime as dt"
-        checkres = checks.check_datetime_alias(line, line, "fakefile")
+        checks.check_datetime_alias(line)
 
     def test_check_log_warn(self):
         bad_samples = ["LOG.warn('foo')", "LOG.warn(_('bar'))"]
         self._assert_bad_samples(checks.check_log_warn, bad_samples)
         good_samples = ["LOG.warning('foo')", "LOG.warning(_('bar'))"]
         self._assert_good_samples(checks.check_log_warn, good_samples)
```

### Comparing `rally-openstack-2.2.0/tests/unit/test_mock.py` & `rally-openstack-2.3.0/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_pytest_launcher.py` & `rally-openstack-2.3.0/tests/unit/test_pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_test_ddt.py` & `rally-openstack-2.3.0/tests/unit/test_test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_test_mock.py` & `rally-openstack-2.3.0/tests/unit/test_test_mock.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/test_workarounds.py` & `rally-openstack-2.3.0/tests/unit/test_workarounds.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/verification/tempest/test_config.py` & `rally-openstack-2.3.0/tests/unit/verification/tempest/test_config.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/verification/tempest/test_context.py` & `rally-openstack-2.3.0/tests/unit/verification/tempest/test_context.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tests/unit/verification/tempest/test_manager.py` & `rally-openstack-2.3.0/tests/unit/verification/tempest/test_manager.py`

 * *Files identical despite different names*

### Comparing `rally-openstack-2.2.0/tox.ini` & `rally-openstack-2.3.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 [tox]
 minversion = 3.1.1
-skipsdist = True
 ignore_basepython_conflict = true
 envlist = py36,py37,py38,pep8
 
 [testenv]
 extras = {env:RALLY_EXTRAS:}
 setenv = VIRTUAL_ENV={envdir}
-         HOME={homedir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
          PYTHONHASHSEED=0
          TOX_ENV_NAME={envname}
-whitelist_externals = find
+allowlist_externals = find
                       rm
                       make
 deps =
   -c ./upper-constraints.txt
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 usedevelop = True
 commands =
   find . -type f -name "*.pyc" -delete
-  python {toxinidir}/tests/ci/pytest_launcher.py tests/unit --posargs={posargs}
+  python3 {toxinidir}/tests/ci/pytest_launcher.py tests/unit --posargs={posargs}
 distribute = false
 basepython = python3
-passenv = http_proxy HTTP_PROXY https_proxy HTTPS_PROXY no_proxy NO_PROXY REQUESTS_CA_BUNDLE
+passenv =
+  http_proxy
+  HTTP_PROXY
+  https_proxy
+  HTTPS_PROXY
+  no_proxy
+  NO_PROXY
+  REQUESTS_CA_BUNDLE
+  HOME
 
 [testenv:pep8]
 commands = flake8
 distribute = false
 
 [testenv:py36]
 basepython = python3.6
 
 [testenv:py37]
 basepython = python3.7
 
 [testenv:py38]
 basepython = python3.8
 
+[testenv:py39]
+basepython = python3.9
 
 [testenv:venv]
 basepython = python3
 commands = {posargs}
 
 [testenv:debug]
 commands = oslo_debug_helper -t tests {posargs}
 
 [testenv:functional]
 basepython = python3
 sitepackages = True
 commands =
   find . -type f -name "*.pyc" -delete
   {toxinidir}/tests/ci/rally_functional_job.sh {posargs}
+allowlist_externals = find
+                      rm
+                      make
+                      {toxinidir}/tests/ci/rally_functional_job.sh
 
 [testenv:cover]
 commands = {toxinidir}/tests/ci/cover.sh {posargs}
-
+allowlist_externals = {toxinidir}/tests/ci/cover.sh
 
 [testenv:genconfig]
 basepython = python3
 commands =
     oslo-config-generator --config-file etc/rally/rally-config-generator.conf
 
 [testenv:requirements]
 deps =
   # do not use upper-constraints file
-  --no-cache-dir
   requests[security]
   -r{toxinidir}/requirements.txt
 commands = python {toxinidir}/tests/ci/sync_requirements.py {posargs}
 
 [flake8]
 # H105  Don't use author tags
 # E731 do not assign a lambda expression, use a def
@@ -96,15 +107,14 @@
    N326 = checks:assert_equal_true_or_false
    N340 = checks:check_no_direct_rally_objects_import
    N341 = checks:check_no_oslo_deprecated_import
    N342 = checks:check_opts_import_path
    N350 = checks:check_quotes
    N351 = checks:check_no_constructor_data_struct
    N352 = checks:check_dict_formatting_in_string
-   N353 = checks:check_using_unicode
    N354 = checks:check_raises
    N355 = checks:check_old_type_class
    N356 = checks:check_datetime_alias
    N360 = checks:check_db_imports_in_cli
    N361 = checks:check_objects_imports_in_cli
 paths = ./tests/hacking
 
@@ -121,12 +131,29 @@
 
 [pytest]
 filterwarnings =
     error
     ignore:invalid escape sequence:DeprecationWarning:.*subunit.*
     ignore:::.*netaddr.strategy.*
     ignore:the imp module is deprecated in favour of importlib.*:DeprecationWarning
+    # we do not use anything inner from OptionParser, so we do not care about it's parent
+    ignore:The frontend.OptionParser class will be replaced by a subclass of argparse.ArgumentParser in Docutils 0.21 or later.:DeprecationWarning:
+    # we do not use Option directly, it is initialized by OptionParser by itself.
+    # as soon as docutils team get rid of frontend.Option, they will also fix OptionParser
+    ignore: The frontend.Option class will be removed in Docutils 0.21 or later.:DeprecationWarning:
     # raised by designateclient?!
     ignore:dns.hash module will be removed in future versions. Please use hashlib instead.:DeprecationWarning
     # should be fixed at rally framework (raised by functional job)
     ignore:.*EngineFacade is deprecated; please use oslo_db.sqlalchemy.enginefacade*:
     ignore:.*unclosed file <_io.TextIOWrapper name='/tmp/rally.log'::
+    ignore:.*mysql_enable_ndb.*::
+    ignore:.*distutils Version classes are deprecated.*::
+    # pytest-cov
+    ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning:
+    ignore:::.*requests.*
+    # python 3.10
+    ignore:The distutils package is deprecated and slated for removal in Python 3.12. Use setuptools or check PEP 632 for potential alternatives:DeprecationWarning:
+    ignore:pkg_resources is deprecated as an API:DeprecationWarning:
+    # python 3.8
+    ignore:Deprecated call to `pkg_resources.declare_namespace*:DeprecationWarning:
+    # python 3.7
+    ignore:invalid escape sequence:DeprecationWarning:.*prettytable.*
```

