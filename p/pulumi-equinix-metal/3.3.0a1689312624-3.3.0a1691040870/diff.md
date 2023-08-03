# Comparing `tmp/pulumi_equinix_metal-3.3.0a1689312624.tar.gz` & `tmp/pulumi_equinix_metal-3.3.0a1691040870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix_metal-3.3.0a1689312624.tar", last modified: Fri Jul 14 05:42:06 2023, max compression
+gzip compressed data, was "pulumi_equinix_metal-3.3.0a1691040870.tar", last modified: Thu Aug  3 05:45:01 2023, max compression
```

## Comparing `pulumi_equinix_metal-3.3.0a1689312624.tar` & `pulumi_equinix_metal-3.3.0a1691040870.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27747 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/bgp_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28398 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    91992 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    38360 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    23360 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:42:06.547479 pulumi_equinix_metal-3.3.0a1689312624/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 05:42:06.000000 pulumi_equinix_metal-3.3.0a1689312624/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27747 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/bgp_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28398 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91992 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38360 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23360 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 05:45:01.634964 pulumi_equinix_metal-3.3.0a1691040870/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-03 05:45:01.000000 pulumi_equinix_metal-3.3.0a1691040870/setup.py
```

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/PKG-INFO` & `pulumi_equinix_metal-3.3.0a1691040870/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_equinix_metal
-Version: 3.3.0a1689312624
-Summary: A Pulumi package for creating and managing equinix-metal cloud resources.
-Home-page: https://pulumi.io
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-equinix-metal
-Keywords: pulumi equinix-metal
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 [![Actions Status](https://github.com/pulumi/pulumi-equinix-metal/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-equinix-metal/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fequinix-metal.svg)](https://www.npmjs.com/package/@pulumi/equinix-metal)
 [![Python version](https://badge.fury.io/py/pulumi-equinix-metal.svg)](https://pypi.org/project/pulumi-equinix-metal)
 [![NuGet version](https://badge.fury.io/nu/pulumi.equinixmetal.svg)](https://badge.fury.io/nu/pulumi.equinixmetal)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-equinix-metal/sdk/v2/go)](https://pkg.go.dev/github.com/pulumi/pulumi-equinix-metal/sdk/v2/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-equinix-metal/blob/master/LICENSE)
@@ -64,9 +53,7 @@
 
 - `equinix-metal:authToken` - (Required) This is your Equinix Metal API Auth token. This can also be specified with the
   `PACKET_AUTH_TOKEN` or `METAL_AUTH_TOKEN` shell environment variable.
 
 ## Reference
 
 For further information, please visit [the Equinix Metal provider docs](https://www.pulumi.com/docs/intro/cloud-providers/equinix-metal) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/equinix-metal).
-
-
```

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/README.md` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pulumi-equinix-metal
+Version: 3.3.0a1691040870
+Summary: A Pulumi package for creating and managing equinix-metal cloud resources.
+Home-page: https://pulumi.io
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-equinix-metal
+Keywords: pulumi equinix-metal
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 [![Actions Status](https://github.com/pulumi/pulumi-equinix-metal/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-equinix-metal/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fequinix-metal.svg)](https://www.npmjs.com/package/@pulumi/equinix-metal)
 [![Python version](https://badge.fury.io/py/pulumi-equinix-metal.svg)](https://pypi.org/project/pulumi-equinix-metal)
 [![NuGet version](https://badge.fury.io/nu/pulumi.equinixmetal.svg)](https://badge.fury.io/nu/pulumi.equinixmetal)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-equinix-metal/sdk/v2/go)](https://pkg.go.dev/github.com/pulumi/pulumi-equinix-metal/sdk/v2/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-equinix-metal/blob/master/LICENSE)
@@ -53,7 +64,9 @@
 
 - `equinix-metal:authToken` - (Required) This is your Equinix Metal API Auth token. This can also be specified with the
   `PACKET_AUTH_TOKEN` or `METAL_AUTH_TOKEN` shell environment variable.
 
 ## Reference
 
 For further information, please visit [the Equinix Metal provider docs](https://www.pulumi.com/docs/intro/cloud-providers/equinix-metal) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/equinix-metal).
+
+
```

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/__init__.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_enums.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_inputs.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_tables.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/_utilities.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/bgp_session.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/config/vars.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/connection.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/device.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/device_network_type.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/device_network_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/gateway.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_connection.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_device.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_device_bgp_neighbors.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_device_bgp_neighbors.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_facility.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_facility.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_gateway.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_hardware_reservation.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_hardware_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_ip_block_ranges.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_ip_block_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_metro.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_metro.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_operating_system.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_operating_system.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_organization.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_port.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_precreated_ip_block.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_precreated_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_project.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_project_ssh_key.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_reserved_ip_block.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_spot_market_price.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_spot_market_price.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_spot_market_request.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_virtual_circuit.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_vlan.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/get_volume.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/ip_attachment.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/ip_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/organization.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/outputs.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/port.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/port_vlan_attachment.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/port_vlan_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project_api_key.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/project_ssh_key.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/provider.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/reserved_ip_block.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/spot_market_request.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/ssh_key.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/user_api_key.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/virtual_circuit.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/vlan.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/volume.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal/volume_attachment.py` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/PKG-INFO` & `pulumi_equinix_metal-3.3.0a1691040870/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-equinix-metal
-Version: 3.3.0a1689312624
+Name: pulumi_equinix_metal
+Version: 3.3.0a1691040870
 Summary: A Pulumi package for creating and managing equinix-metal cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-equinix-metal
 Keywords: pulumi equinix-metal
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/pulumi_equinix_metal.egg-info/SOURCES.txt` & `pulumi_equinix_metal-3.3.0a1691040870/pulumi_equinix_metal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix_metal-3.3.0a1689312624/setup.py` & `pulumi_equinix_metal-3.3.0a1691040870/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.3.0a1689312624"
-PLUGIN_VERSION = "3.3.0-alpha.1689312624+1b0c6171"
+VERSION = "3.3.0a1691040870"
+PLUGIN_VERSION = "3.3.0-alpha.1691040870+9cf1161e"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'equinix-metal', PLUGIN_VERSION])
         except OSError as error:
```

