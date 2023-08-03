# Comparing `tmp/aerleon-1.5.0.tar.gz` & `tmp/aerleon-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerleon-1.5.0.tar", max compression
+gzip compressed data, was "aerleon-1.6.0.tar", max compression
```

## Comparing `aerleon-1.5.0.tar` & `aerleon-1.6.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11358 2023-07-20 05:44:09.349471 aerleon-1.5.0/LICENSE
--rw-r--r--   0        0        0     6934 2023-07-20 05:44:09.353472 aerleon-1.5.0/README.md
--rw-r--r--   0        0        0       15 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/__init__.py
--rw-r--r--   0        0        0      167 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/__main__.py
--rw-r--r--   0        0        0     4399 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/aclcheck_cmdline.py
--rw-r--r--   0        0        0    17930 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/aclgen.py
--rw-r--r--   0        0        0    13124 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/api.py
--rw-r--r--   0        0        0    11358 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/COPYING
--rw-r--r--   0        0        0       29 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/__init__.py
--rwxr-xr-x   0        0        0    11008 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/aclcheck.py
--rw-r--r--   0        0        0    24716 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/aclgenerator.py
--rw-r--r--   0        0        0     4517 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/addressbook.py
--rw-r--r--   0        0        0     2792 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/arista.py
--rw-r--r--   0        0        0    36176 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/arista_tp.py
--rw-r--r--   0        0        0    10035 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/aruba.py
--rw-r--r--   0        0        0     1116 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/brocade.py
--rw-r--r--   0        0        0    39710 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/cisco.py
--rw-r--r--   0        0        0    14390 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/ciscoasa.py
--rw-r--r--   0        0        0     2754 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/cisconx.py
--rw-r--r--   0        0        0     2428 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/ciscoxr.py
--rw-r--r--   0        0        0     9968 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/cloudarmor.py
--rw-r--r--   0        0        0     7737 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/demo.py
--rw-r--r--   0        0        0      691 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/fqdn.py
--rw-r--r--   0        0        0    24978 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/gce.py
--rw-r--r--   0        0        0     4759 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/gcp.py
--rw-r--r--   0        0        0    24295 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/gcp_hf.py
--rw-r--r--   0        0        0     9076 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/ipset.py
--rw-r--r--   0        0        0    38752 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/iptables.py
--rw-r--r--   0        0        0    44422 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/juniper.py
--rw-r--r--   0        0        0     5090 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/juniperevo.py
--rw-r--r--   0        0        0    32101 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/junipermsmpc.py
--rw-r--r--   0        0        0    37947 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/junipersrx.py
--rw-r--r--   0        0        0    14344 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/k8s.py
--rw-r--r--   0        0        0    17897 2023-07-20 05:44:09.353472 aerleon-1.5.0/aerleon/lib/nacaddr.py
--rw-r--r--   0        0        0    39850 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/naming.py
--rw-r--r--   0        0        0    33371 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/nftables.py
--rw-r--r--   0        0        0    12419 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/nsxt.py
--rw-r--r--   0        0        0    24741 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/nsxv.py
--rw-r--r--   0        0        0    10014 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/openconfig.py
--rw-r--r--   0        0        0    23249 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/packetfilter.py
--rw-r--r--   0        0        0    49360 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/paloaltofw.py
--rw-r--r--   0        0        0    17077 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/pcap.py
--rw-r--r--   0        0        0     3411 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/plugin.py
--rw-r--r--   0        0        0    13357 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/plugin_supervisor.py
--rw-r--r--   0        0        0    97865 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/policy.py
--rw-r--r--   0        0        0    39619 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/policy_builder.py
--rw-r--r--   0        0        0    21391 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/policy_simple.py
--rw-r--r--   0        0        0     9162 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/policyreader.py
--rw-r--r--   0        0        0     4948 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/port.py
--rw-r--r--   0        0        0    14617 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/recognizers.py
--rw-r--r--   0        0        0     1316 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/speedway.py
--rw-r--r--   0        0        0     2405 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/srxlo.py
--rw-r--r--   0        0        0     9069 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/summarizer.py
--rw-r--r--   0        0        0    14092 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/windows.py
--rw-r--r--   0        0        0     6118 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/windows_advfirewall.py
--rw-r--r--   0        0        0     9096 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/windows_ipsec.py
--rw-r--r--   0        0        0    12540 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/yaml.py
--rw-r--r--   0        0        0     1140 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/lib/yaml_loader.py
--rw-r--r--   0        0        0        0 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/utils/__init__.py
--rw-r--r--   0        0        0     3240 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/utils/config.py
--rw-r--r--   0        0        0     3592 2023-07-20 05:44:09.357472 aerleon-1.5.0/aerleon/utils/iputils.py
--rw-r--r--   0        0        0     2712 2023-07-20 05:44:09.365472 aerleon-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 05:44:09.417472 aerleon-1.5.0/tools/__init__.py
--rw-r--r--   0        0        0    16269 2023-07-20 05:44:09.417472 aerleon-1.5.0/tools/cgrep.py
--rw-r--r--   0        0        0     1794 2023-07-20 05:44:09.417472 aerleon-1.5.0/tools/iputilstools.py
--rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 aerleon-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-03 06:54:51.986266 aerleon-1.6.0/LICENSE
+-rw-r--r--   0        0        0     6934 2023-08-03 06:54:51.986266 aerleon-1.6.0/README.md
+-rw-r--r--   0        0        0       15 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/__init__.py
+-rw-r--r--   0        0        0      167 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/__main__.py
+-rw-r--r--   0        0        0     4399 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/aclcheck_cmdline.py
+-rw-r--r--   0        0        0    17930 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/aclgen.py
+-rw-r--r--   0        0        0    13124 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/api.py
+-rw-r--r--   0        0        0    11358 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/COPYING
+-rw-r--r--   0        0        0       29 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/__init__.py
+-rwxr-xr-x   0        0        0    11008 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/aclcheck.py
+-rw-r--r--   0        0        0    24716 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/aclgenerator.py
+-rw-r--r--   0        0        0     7802 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/addressbook.py
+-rw-r--r--   0        0        0     2792 2023-08-03 06:54:51.986266 aerleon-1.6.0/aerleon/lib/arista.py
+-rw-r--r--   0        0        0    36415 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/arista_tp.py
+-rw-r--r--   0        0        0    10035 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/aruba.py
+-rw-r--r--   0        0        0     1116 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/brocade.py
+-rw-r--r--   0        0        0    40020 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/cisco.py
+-rw-r--r--   0        0        0    14390 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/ciscoasa.py
+-rw-r--r--   0        0        0     2754 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/cisconx.py
+-rw-r--r--   0        0        0     2428 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/ciscoxr.py
+-rw-r--r--   0        0        0     9968 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/cloudarmor.py
+-rw-r--r--   0        0        0     7737 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/demo.py
+-rw-r--r--   0        0        0      691 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/fqdn.py
+-rw-r--r--   0        0        0    24978 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/gce.py
+-rw-r--r--   0        0        0     4759 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/gcp.py
+-rw-r--r--   0        0        0    24295 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/gcp_hf.py
+-rw-r--r--   0        0        0     9076 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/ipset.py
+-rw-r--r--   0        0        0    38752 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/iptables.py
+-rw-r--r--   0        0        0    44864 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/juniper.py
+-rw-r--r--   0        0        0     5090 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/juniperevo.py
+-rw-r--r--   0        0        0    32101 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/junipermsmpc.py
+-rw-r--r--   0        0        0    37939 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/junipersrx.py
+-rw-r--r--   0        0        0    14344 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/k8s.py
+-rw-r--r--   0        0        0    17897 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/nacaddr.py
+-rw-r--r--   0        0        0    39850 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/naming.py
+-rw-r--r--   0        0        0    33371 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/nftables.py
+-rw-r--r--   0        0        0    12419 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/nsxt.py
+-rw-r--r--   0        0        0    24741 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/nsxv.py
+-rw-r--r--   0        0        0    10742 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/openconfig.py
+-rw-r--r--   0        0        0    23397 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/packetfilter.py
+-rw-r--r--   0        0        0    48254 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/paloaltofw.py
+-rw-r--r--   0        0        0    17225 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/pcap.py
+-rw-r--r--   0        0        0     3411 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/plugin.py
+-rw-r--r--   0        0        0    13357 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/plugin_supervisor.py
+-rw-r--r--   0        0        0    97865 2023-08-03 06:54:51.990266 aerleon-1.6.0/aerleon/lib/policy.py
+-rw-r--r--   0        0        0    39619 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/policy_builder.py
+-rw-r--r--   0        0        0    21391 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/policy_simple.py
+-rw-r--r--   0        0        0     9162 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/policyreader.py
+-rw-r--r--   0        0        0     4948 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/port.py
+-rw-r--r--   0        0        0    14617 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/recognizers.py
+-rw-r--r--   0        0        0     1316 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/speedway.py
+-rw-r--r--   0        0        0     2405 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/srxlo.py
+-rw-r--r--   0        0        0     9069 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/summarizer.py
+-rw-r--r--   0        0        0    14092 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/windows.py
+-rw-r--r--   0        0        0     6118 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/windows_advfirewall.py
+-rw-r--r--   0        0        0     9096 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/windows_ipsec.py
+-rw-r--r--   0        0        0    16148 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/yaml.py
+-rw-r--r--   0        0        0     1140 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/lib/yaml_loader.py
+-rw-r--r--   0        0        0        0 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/utils/__init__.py
+-rw-r--r--   0        0        0     3240 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/utils/config.py
+-rw-r--r--   0        0        0     3592 2023-08-03 06:54:51.994266 aerleon-1.6.0/aerleon/utils/iputils.py
+-rw-r--r--   0        0        0     2712 2023-08-03 06:54:51.998266 aerleon-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 06:54:52.038266 aerleon-1.6.0/tools/__init__.py
+-rw-r--r--   0        0        0    16269 2023-08-03 06:54:52.038266 aerleon-1.6.0/tools/cgrep.py
+-rw-r--r--   0        0        0     1794 2023-08-03 06:54:52.038266 aerleon-1.6.0/tools/iputilstools.py
+-rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 aerleon-1.6.0/PKG-INFO
```

### Comparing `aerleon-1.5.0/LICENSE` & `aerleon-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/README.md` & `aerleon-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/aclcheck_cmdline.py` & `aerleon-1.6.0/aerleon/aclcheck_cmdline.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/aclgen.py` & `aerleon-1.6.0/aerleon/aclgen.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/api.py` & `aerleon-1.6.0/aerleon/api.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/COPYING` & `aerleon-1.6.0/aerleon/lib/COPYING`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/aclcheck.py` & `aerleon-1.6.0/aerleon/lib/aclcheck.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/aclgenerator.py` & `aerleon-1.6.0/aerleon/lib/aclgenerator.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/arista.py` & `aerleon-1.6.0/aerleon/lib/arista.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/arista_tp.py` & `aerleon-1.6.0/aerleon/lib/arista_tp.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,22 @@
             "addr_fam": "ipv4",
         },
         "inet6": {
             "addr_fam": "ipv6",
         },
     }
 
-    def __init__(self, term: policy.Term, term_type: str, noverbose: bool) -> None:
+    def __init__(
+        self, term: policy.Term, term_type: str, noverbose: bool, filter_type: str = None
+    ) -> None:
         super().__init__(term)
         self.term = term
         self.term_type = term_type  # drives the address-family
         self.noverbose = noverbose
+        self.filter_type = filter_type
 
         if term_type not in self._TERM_TYPE:
             raise ValueError("unknown filter type: %s" % term_type)
 
     def __str__(self) -> str:
         config = Config()
 
@@ -256,19 +259,20 @@
                     src_str += " field-set src-%s" % self.term.name
                 else:
                     for addr in src_addr:
                         src_str += " %s" % addr
 
                 term_block.append([MATCH_INDENT, src_str, False])
             elif self.term.source_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction="source", af=self.term_type
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction="source", af=self.term_type
+                        )
                     )
-                )
                 return ""
 
             # destination address
             dst_addr = self.term.GetAddressOfVersion("destination_address", term_af)
             dst_addr_ex = self.term.GetAddressOfVersion("destination_address_exclude", term_af)
 
             if dst_addr:
@@ -279,19 +283,20 @@
                 else:
                     for addr in dst_addr:
                         dst_str += " %s" % addr
 
                 term_block.append([MATCH_INDENT, dst_str, False])
 
             elif self.term.destination_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction="destination", af=self.term_type
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction="destination", af=self.term_type
+                        )
                     )
-                )
                 return ""
 
             if self.term.source_prefix:
                 src_pfx_str = "source prefix field-set"
                 for pfx in self.term.source_prefix:
                     src_pfx_str += " %s" % pfx
 
@@ -901,15 +906,15 @@
 
                     # generate the unique list of named counters
                     if term.counter:
                         # we can't have '.' in counter names
                         term.counter = re.sub(r"\.", "-", str(term.counter))
                         policy_counters.add(term.counter)
 
-                    new_terms.append(self._TERM(term, ft, noverbose))
+                    new_terms.append(self._TERM(term, ft, noverbose, filter_type=filter_type))
 
             self.arista_traffic_policies.append(
                 (
                     header,
                     filter_name,
                     filter_type,
                     new_terms,
```

### Comparing `aerleon-1.5.0/aerleon/lib/aruba.py` & `aerleon-1.6.0/aerleon/lib/aruba.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/brocade.py` & `aerleon-1.6.0/aerleon/lib/brocade.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/cisco.py` & `aerleon-1.6.0/aerleon/lib/cisco.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         # w/o reading the pol file twice (with some other library) or doing
         # some other ugly hackery. Instead, the entire block of source and dest
         # addresses for a given term is given a unique, computable name which
         # is not related to the NETWORK.net token name.  that's what you get
         # for using cisco, which has decided to implement its own meta language.
 
         # Create network object-groups
-        for name, ips in self.addressbook.addressbook[''].items():
+        for zone, name, ips, _ in self.addressbook.Walk():
             for version in (4, 6):
                 vips = [i for i in ips if i.version == version]
                 if vips:
 
                     ret_str.append(f'object-group network ipv{version} {name}')
                     for ip in vips:
                         ret_str.append(f' {ip.network_address}/{ip.prefixlen}')
@@ -422,22 +422,24 @@
         term: Term,
         af: int = 4,
         proto_int: bool = True,
         enable_dsmo: bool = False,
         term_remark: bool = True,
         platform: str = 'cisco',
         verbose: bool = True,
+        filter_type: str = None,
     ) -> None:
         self.term = term
         self.proto_int = proto_int
         self.options = []
         self.enable_dsmo = enable_dsmo
         self.term_remark = term_remark
         self.platform = platform
         self.verbose = verbose
+        self.filter_type = filter_type
         # Our caller should have already verified the address family.
         assert af in (4, 6)
         self.af = af
         if af == 4:
             self.text_af = 'inet'
         else:
             self.text_af = 'inet6'
@@ -514,19 +516,20 @@
             source_address = self.term.GetAddressOfVersion('source_address', self.af)
             source_address_exclude = self.term.GetAddressOfVersion(
                 'source_address_exclude', self.af
             )
             if source_address_exclude:
                 source_address = nacaddr.ExcludeAddrs(source_address, source_address_exclude)
             if not source_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction='source', af=self.text_af
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction='source', af=self.text_af
+                        )
                     )
-                )
                 return ''
             if self.enable_dsmo:
                 source_address = summarizer.Summarize(source_address)
         else:
             # source address not set
             source_address = [nacaddr.IPv4('0.0.0.0/0', token='any')]
         fixed_src_addresses = set([x for x in source_address])
@@ -538,19 +541,20 @@
                 'destination_address_exclude', self.af
             )
             if destination_address_exclude:
                 destination_address = nacaddr.ExcludeAddrs(
                     destination_address, destination_address_exclude
                 )
             if not destination_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction='destination', af=self.text_af
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction='destination', af=self.text_af
+                        )
                     )
-                )
                 return ''
             if self.enable_dsmo:
                 destination_address = summarizer.Summarize(destination_address)
         else:
             # destination address not set
             destination_address = [nacaddr.IPv4('0.0.0.0/0', token='any')]
 
@@ -967,27 +971,29 @@
                             ExtendedTerm(
                                 term,
                                 proto_int=self._PROTO_INT,
                                 enable_dsmo=enable_dsmo,
                                 term_remark=self._TERM_REMARK,
                                 platform=self._PLATFORM,
                                 verbose=self.verbose,
+                                filter_type=filter_type,
                             )
                         )
                     elif next_filter == 'object-group':
                         obj_target.AddTerm(term)
                         new_terms.append(self._GetObjectGroupTerm(term, verbose=self.verbose))
                     elif next_filter == 'inet6':
                         new_terms.append(
                             ExtendedTerm(
                                 term,
                                 6,
                                 proto_int=self._PROTO_INT,
                                 platform=self._PLATFORM,
                                 verbose=self.verbose,
+                                filter_type=filter_type,
                             )
                         )
 
                 # cisco requires different name for the v4 and v6 acls
                 if filter_type == 'mixed' and next_filter == 'inet6':
                     filter_name = 'ipv6-%s' % filter_name
                 self.cisco_policies.append(
@@ -1081,13 +1087,13 @@
 
                 # now add the terms
                 for term in terms:
                     term_str = str(term)
                     if term_str:
                         target.append(term_str)
 
-            if obj_target.addressbook.addressbook.keys():
+            if obj_target.addressbook.GetZoneNames():
                 target = [str(obj_target)] + target
             # ensure that the header is always first
             target = target_header + target
             target += ['', 'exit', '']
         return '\n'.join(target)
```

### Comparing `aerleon-1.5.0/aerleon/lib/ciscoasa.py` & `aerleon-1.6.0/aerleon/lib/ciscoasa.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/cisconx.py` & `aerleon-1.6.0/aerleon/lib/cisconx.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/ciscoxr.py` & `aerleon-1.6.0/aerleon/lib/ciscoxr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/cloudarmor.py` & `aerleon-1.6.0/aerleon/lib/cloudarmor.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/demo.py` & `aerleon-1.6.0/aerleon/lib/demo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/fqdn.py` & `aerleon-1.6.0/aerleon/lib/fqdn.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/gce.py` & `aerleon-1.6.0/aerleon/lib/gce.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/gcp.py` & `aerleon-1.6.0/aerleon/lib/gcp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/gcp_hf.py` & `aerleon-1.6.0/aerleon/lib/gcp_hf.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/ipset.py` & `aerleon-1.6.0/aerleon/lib/ipset.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/iptables.py` & `aerleon-1.6.0/aerleon/lib/iptables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/juniper.py` & `aerleon-1.6.0/aerleon/lib/juniper.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
       term_type: String indicating type of term, inet, inet6 icmp etc.
       enable_dsmo: Boolean to enable dsmo.
       noverbose: Boolean to disable verbosity.
       filter_direction: Enum indicating the direction of the filter on an
         interface e.g. INGRESS.
       interface_type: Enum indicating the type of interface filter will be applied
         e.g. LOOPBACK.
+      filter_type: String indicating the type of the filter, which may be mixed.
     """
 
     _PLATFORM = 'juniper'
     _DEFAULT_INDENT = 12
     ACTIONS = {
         'accept': 'accept',
         'deny': 'discard',
@@ -195,23 +196,25 @@
         self,
         term: policy.Term,
         term_type: str,
         enable_dsmo: bool,
         noverbose: bool,
         filter_direction: str = None,
         interface_type: str = None,
+        filter_type: str = None,
     ):
         super().__init__(term)
         self.term = term
         self.term_type = term_type
         self.enable_dsmo = enable_dsmo
         self.noverbose = noverbose
         # Filter direction and interface type are needed in juniperevo sub-class for IPv6 filters.
         self.filter_direction = filter_direction
         self.interface_type = interface_type
+        self.filter_type = filter_type
 
         if self._PLATFORM != 'msmpc':
             if term_type not in self._TERM_TYPE:
                 raise ValueError('Unknown Filter Type: %s' % term_type)
             if 'hopopt' in self.term.protocol:
                 loc = self.term.protocol.index('hopopt')
                 self.term.protocol[loc] = 'hop-by-hop'
@@ -365,17 +368,18 @@
                         config.Append('%s' % comment)
                     if self.enable_dsmo:
                         config.Append('%s/%s;' % summarizer.ToDottedQuad(addr, nondsm=True))
                     else:
                         config.Append('%s;' % addr)
                 config.Append('}')
             elif self.term.address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(term=self.term.name, af=self.term_type)
-                )
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(term=self.term.name, af=self.term_type)
+                    )
                 return ''
 
             # source address
 
             src_addr = self.term.GetAddressOfVersion('source_address', term_af)
             src_addr_ex = self.term.GetAddressOfVersion('source_address_exclude', term_af)
             if self.enable_dsmo:
@@ -398,19 +402,20 @@
                         config.Append('%s' % comment)
                     if self.enable_dsmo:
                         config.Append('%s/%s except;' % summarizer.ToDottedQuad(addr, nondsm=True))
                     else:
                         config.Append('%s except;' % addr)
                 config.Append('}')
             elif self.term.source_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction='source', af=self.term_type
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction='source', af=self.term_type
+                        )
                     )
-                )
                 return ''
 
             # destination address
             dst_addr = self.term.GetAddressOfVersion('destination_address', term_af)
             dst_addr_ex = self.term.GetAddressOfVersion('destination_address_exclude', term_af)
             if self.enable_dsmo:
                 dst_addr = summarizer.Summarize(dst_addr)
@@ -432,19 +437,20 @@
                         config.Append('%s' % comment)
                     if self.enable_dsmo:
                         config.Append('%s/%s except;' % summarizer.ToDottedQuad(addr, nondsm=True))
                     else:
                         config.Append('%s except;' % addr)
                 config.Append('}')
             elif self.term.destination_address:
-                logging.warning(
-                    self.NO_AF_LOG_ADDR.substitute(
-                        term=self.term.name, direction='destination', af=self.term_type
+                if self.filter_type != 'mixed':
+                    logging.warning(
+                        self.NO_AF_LOG_ADDR.substitute(
+                            term=self.term.name, direction='destination', af=self.term_type
+                        )
                     )
-                )
                 return ''
 
             # forwarding-class
             if self.term.forwarding_class:
                 config.Append(
                     'forwarding-class %s' % self._Group(self.term.forwarding_class, lc=False)
                 )
@@ -1031,32 +1037,32 @@
                 filter_type = filter_options[1]
 
             if filter_type == 'mixed':
                 filter_types_to_process = ['inet', 'inet6']
             else:
                 filter_types_to_process = [filter_type]
 
-            for filter_type in filter_types_to_process:
+            for term_filter_type in filter_types_to_process:
 
                 filter_name_suffix = ''
                 # If mixed filter_type, will append 4 or 6 to the filter name
                 if len(filter_types_to_process) > 1:
-                    if filter_type == 'inet':
+                    if term_filter_type == 'inet':
                         filter_name_suffix = '4'
-                    if filter_type == 'inet6':
+                    if term_filter_type == 'inet6':
                         filter_name_suffix = '6'
 
                 term_names = set()
                 new_terms = []
                 for term in terms:
 
                     # Ignore if the term is for a different AF
                     if (
                         term.restrict_address_family
-                        and term.restrict_address_family != filter_type
+                        and term.restrict_address_family != term_filter_type
                     ):
                         continue
 
                     # if inactive is set, deactivate the term and remove the option.
                     if 'inactive' in term.option:
                         term.inactive = True
                         term.option.remove('inactive')
@@ -1065,39 +1071,40 @@
 
                     if term.name in term_names:
                         raise JuniperDuplicateTermError(
                             'You have multiple terms named: %s' % term.name
                         )
                     term_names.add(term.name)
 
-                    term = self.FixHighPorts(term, af=filter_type)
+                    term = self.FixHighPorts(term, af=term_filter_type)
                     if not term:
                         continue
 
-                    if 'is-fragment' in term.option and filter_type == 'inet6':
+                    if 'is-fragment' in term.option and term_filter_type == 'inet6':
                         raise JuniperFragmentInV6Error(
                             'The term %s uses "is-fragment" but ' 'is a v6 policy.' % term.name
                         )
 
                     new_terms.append(
                         self._TERM(
                             term,
-                            filter_type,
+                            term_filter_type,
                             enable_dsmo,
                             noverbose,
                             filter_direction,
                             interface_type,
+                            filter_type=filter_type,
                         )
                     )
 
                 self.juniper_policies.append(
                     (
                         header,
                         filter_name + filter_name_suffix,
-                        filter_type,
+                        term_filter_type,
                         interface_specific,
                         filter_enhanced_mode,
                         new_terms,
                     )
                 )
 
     def __str__(self):
```

### Comparing `aerleon-1.5.0/aerleon/lib/juniperevo.py` & `aerleon-1.6.0/aerleon/lib/juniperevo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/junipermsmpc.py` & `aerleon-1.6.0/aerleon/lib/junipermsmpc.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/junipersrx.py` & `aerleon-1.6.0/aerleon/lib/junipersrx.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
 from aerleon.lib import aclgenerator, addressbook, nacaddr, policy
 
 ICMP_TERM_LIMIT = 8
+FQDNSUFFIX = '_FQDN'
 
 
 def JunipersrxList(name, data):
     return '%s [ %s ];' % (name, ' '.join(data))
 
 
 class Error(aclgenerator.Error):
@@ -129,32 +130,26 @@
             for line in comments:
                 ret_str.IndentAppend(3, line)
             ret_str.IndentAppend(3, '*/')
 
         ret_str.IndentAppend(3, 'policy ' + self.term.name + ' {')
         ret_str.IndentAppend(4, 'match {')
         # SOURCE-ADDRESS
-        if self.term.source_address:
-            saddr_check = set()
-            for saddr in self.term.source_address:
-                saddr_check.add(saddr.parent_token)
-            saddr_check = sorted(saddr_check)
-            ret_str.IndentAppend(5, JunipersrxList('source-address', saddr_check))
+        saddrs = {i.parent_token for i in self.term.source_address}
+        saddrs.update({i.parent_token + FQDNSUFFIX for i in self.term.source_fqdn})
+        if saddrs:
+            ret_str.IndentAppend(5, JunipersrxList('source-address', sorted(saddrs)))
         else:
             ret_str.IndentAppend(5, 'source-address any;')
 
         # DESTINATION-ADDRESS
-        if self.term.destination_address:
-            daddr_check = []
-            for daddr in self.term.destination_address:
-                daddr_check.append(daddr.parent_token)
-            daddr_check = set(daddr_check)
-            daddr_check = list(daddr_check)
-            daddr_check.sort()
-            ret_str.IndentAppend(5, JunipersrxList('destination-address', daddr_check))
+        daddrs = {i.parent_token for i in self.term.destination_address}
+        daddrs.update({i.parent_token + FQDNSUFFIX for i in self.term.destination_fqdn})
+        if daddrs:
+            ret_str.IndentAppend(5, JunipersrxList('destination-address', sorted(daddrs)))
         else:
             ret_str.IndentAppend(5, 'destination-address any;')
 
         # APPLICATION
         if (
             not self.term.source_port
             and not self.term.destination_port
@@ -324,18 +319,20 @@
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
 
         supported_tokens |= {
             'dscp_except',
             'dscp_match',
             'dscp_set',
+            'destination_fqdn',
             'destination_zone',
             'logging',
             'option',
             'owner',
+            'source_fqdn',
             'source_zone',
             'timeout',
             'verbatim',
             'vpn',
         }
 
         supported_sub_tokens.update(
@@ -525,16 +522,16 @@
                         for j in term.destination_address:
                             j.token = new_dst_token
                             j.parent_token = new_dst_parent_token
 
                 # SRX policies are controlled by addresses that are used within, so
                 # policy can be at the same time inet and inet6.
                 if self._GLOBAL_ADDR_BOOK in self.addr_book_type:
-                    for zone in self.addressbook.addressbook:
-                        for _, ips in sorted(self.addressbook.addressbook[zone].items()):
+                    for zone in self.addressbook._ip_addressbook:
+                        for _, ips in sorted(self.addressbook._ip_addressbook[zone].items()):
                             ips = [i for i in ips]
                             if term.source_address == ips:
                                 term.source_address = ips
                             if term.destination_address == ips:
                                 term.destination_address = ips
 
                 # Filter source_address based on filter_type & add to address book
@@ -547,14 +544,16 @@
                         logging.warning(
                             'WARNING: Term %s has 0 valid source IPs, skipping.', term.name
                         )
                         continue
                     term.source_address = valid_addrs
                     if term.source_address:
                         self.addressbook.AddAddresses(self.from_zone, term.source_address)
+                if term.source_fqdn:
+                    self.addressbook.AddFQDNs(self.from_zone, term.source_fqdn, suffix=FQDNSUFFIX)
 
                 # Filter destination_address based on filter_type & add to address book
                 if term.destination_address:
                     valid_addrs = []
                     for addr in term.destination_address:
                         if addr.version in self._AF_MAP[filter_type]:
                             valid_addrs.append(addr)
@@ -562,15 +561,18 @@
                         logging.warning(
                             'WARNING: Term %s has 0 valid destination IPs, skipping.', term.name
                         )
                         continue
                     term.destination_address = valid_addrs
                     if term.destination_address:
                         self.addressbook.AddAddresses(self.to_zone, term.destination_address)
-
+                if term.destination_fqdn:
+                    self.addressbook.AddFQDNs(
+                        self.to_zone, term.destination_fqdn, suffix=FQDNSUFFIX
+                    )
                 new_term = Term(term, self.from_zone, self.to_zone, self.expresspath, verbose)
                 new_terms.append(new_term)
 
                 # Because SRX terms can contain inet and inet6 addresses. We have to
                 # have ability to recover proper AF for ICMP type we need.
                 # If protocol is empty or we cannot map to inet or inet6 we insert bogus
                 # af_type name which will cause new_term.NormalizeIcmpTypes to fail.
@@ -694,79 +696,75 @@
         for i in ports:
             if i[0] == i[1]:
                 port_list.append(str(i[0]))
             else:
                 port_list.append('%s-%s' % (str(i[0]), str(i[1])))
         return port_list
 
+    def _GenerateAddresses(self, token: str, ips, fqdns):
+        target = IndentList(self.INDENT)
+        counter = 0
+        ips = nacaddr.SortAddrList(ips)
+        ips = nacaddr.CollapseAddrList(ips)
+        for ip in ips:
+            target.IndentAppend(4, 'address ' + token + '_' + str(counter) + ' ' + str(ip) + ';')
+            counter += 1
+        for fqdn in fqdns:
+            target.IndentAppend(4, f'address {token}_{counter} {{')
+            target.IndentAppend(5, f'dns-name {fqdn.fqdn};')
+            target.IndentAppend(4, f'}}')
+        return target
+
+    def _GenerateAddressSets(self, group, ips, fqdns) -> IndentList:
+        target = IndentList(self.INDENT)
+        target.IndentAppend(4, 'address-set ' + group + ' {')
+        counter = 0
+        for _ in nacaddr.CollapseAddrList(ips):
+            target.IndentAppend(5, 'address ' + group + '_' + str(counter) + ';')
+            counter += 1
+        for _ in fqdns:
+            target.IndentAppend(5, 'address ' + group + '_' + str(counter) + ';')
+            counter += 1
+        target.IndentAppend(4, '}')
+        return target
+
     def _GenerateAddressBook(self) -> IndentList:
         """Creates address book."""
         target = IndentList(self.INDENT)
 
         # create address books if address-book-type set to global
         if self._GLOBAL_ADDR_BOOK in self.addr_book_type:
-            global_address_book = collections.defaultdict(list)
 
             target.IndentAppend(1, 'replace: address-book {')
             target.IndentAppend(2, 'global {')
-            for zone in self.addressbook.addressbook:
-                for group in self.addressbook.addressbook[zone]:
-                    for address in self.addressbook.addressbook[zone][group]:
-                        global_address_book[group].append(address)
-            names = sorted(global_address_book.keys())
-            for name in names:
-                counter = 0
-                ips = nacaddr.SortAddrList(global_address_book[name])
-                ips = nacaddr.CollapseAddrList(ips)
-                global_address_book[name] = ips
-                for ip in ips:
-                    target.IndentAppend(
-                        4, 'address ' + name + '_' + str(counter) + ' ' + str(ip) + ';'
-                    )
-                    counter += 1
-
-            for group in sorted(global_address_book.keys()):
-                target.IndentAppend(4, 'address-set ' + group + ' {')
-                counter = 0
-                for unused_addr in global_address_book[group]:
-                    target.IndentAppend(5, 'address ' + group + '_' + str(counter) + ';')
-                    counter += 1
-                target.IndentAppend(4, '}')
+            global_addressbook = addressbook.Addressbook()
+            for zone, _, ips, fqdns in self.addressbook.Walk():
+                global_addressbook.AddAddresses('global', ips)
+                global_addressbook.AddFQDNs('global', fqdns, suffix=FQDNSUFFIX)
+            if 'global' in global_addressbook.GetZoneNames():
+                addrs = []
+                addr_sets = []
+                for _, group, ips, fqdns in global_addressbook.Walk('global'):
+                    addrs.extend(self._GenerateAddresses(group, ips, fqdns))
+                    addr_sets.extend(self._GenerateAddressSets(group, ips, fqdns))
+                target.extend(addrs)
+                target.extend(addr_sets)
 
             target.IndentAppend(2, '}')
             target.IndentAppend(1, '}')
 
         else:
             target.IndentAppend(1, 'zones {')
-            for zone in self.addressbook.addressbook:
+            zones = self.addressbook.GetZoneNames()
+            for zone in zones:
                 target.IndentAppend(2, 'security-zone ' + zone + ' {')
                 target.IndentAppend(3, 'replace: address-book {')
-
-                # building individual addresses
-                groups = sorted(self.addressbook.addressbook[zone])
-                for group in groups:
-                    ips = nacaddr.SortAddrList(self.addressbook.addressbook[zone][group])
-                    ips = nacaddr.CollapseAddrList(ips)
-                    self.addressbook.addressbook[zone][group] = ips
-                    count = 0
-                    for address in self.addressbook.addressbook[zone][group]:
-                        target.IndentAppend(
-                            4, 'address ' + group + '_' + str(count) + ' ' + str(address) + ';'
-                        )
-                        count += 1
-
-                # building address-sets
-                for group in groups:
-                    target.IndentAppend(4, 'address-set ' + group + ' {')
-                    count = 0
-                    for address in self.addressbook.addressbook[zone][group]:
-                        target.IndentAppend(5, 'address ' + group + '_' + str(count) + ';')
-                        count += 1
-
-                    target.IndentAppend(4, '}')
+                for _, group, ips, fqdns in self.addressbook.Walk(zone):
+                    target.extend(self._GenerateAddresses(group, ips, fqdns))
+                    target.extend(self._GenerateAddressSets(group, ips, fqdns))
                 target.IndentAppend(3, '}')
                 target.IndentAppend(2, '}')
             target.IndentAppend(1, '}')
 
         return target
 
     def _GenerateApplications(self) -> IndentList:
```

### Comparing `aerleon-1.5.0/aerleon/lib/k8s.py` & `aerleon-1.6.0/aerleon/lib/k8s.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/nacaddr.py` & `aerleon-1.6.0/aerleon/lib/nacaddr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/naming.py` & `aerleon-1.6.0/aerleon/lib/naming.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/nftables.py` & `aerleon-1.6.0/aerleon/lib/nftables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/nsxt.py` & `aerleon-1.6.0/aerleon/lib/nsxt.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/nsxv.py` & `aerleon-1.6.0/aerleon/lib/nsxv.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/openconfig.py` & `aerleon-1.6.0/aerleon/lib/openconfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 IP = TypedDict("IP", {"config": IPConfig})
 ActionConfig = TypedDict("ActionConfig", {"forwarding-action": str})
 Action = TypedDict("Action", {"config": ActionConfig})
 ACLEntry = TypedDict(
     "ACLEntry",
     {"sequence-id": int, "actions": Action, "ipv4": IP, "ipv6": IP, "transport": Transport},
 )
+aclEntries = TypedDict("aclEntries", {"acl-entry": List[ACLEntry]})
+ACLSetConfig = TypedDict("ACLSetConfig", {"name": str, "type": str})
+ACLSet = TypedDict(
+    "ACLSet", {"acl-entries": aclEntries, "config": ACLSetConfig, "name": str, "type": str}
+)
 
 
 class Term(aclgenerator.Term):
     """Creates the term for the OpenConfig firewall."""
 
     ACTION_MAP = {'accept': 'ACCEPT', 'deny': 'DROP', 'reject': 'REJECT'}
 
@@ -205,14 +210,15 @@
 
 class OpenConfig(aclgenerator.ACLGenerator):
     """A OpenConfig firewall policy object."""
 
     _PLATFORM = 'openconfig'
     SUFFIX = '.oacl'
     _SUPPORTED_AF = frozenset(('inet', 'inet6', 'mixed'))
+    FAMILY_MAP = {'mixed': 'ACL_MIXED', 'inet6': 'ACL_IPV6', 'inet': 'ACL_IPV4'}
 
     def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
@@ -223,16 +229,16 @@
 
         # OpenConfig ACL model only supports these three forwarding actions.
         supported_sub_tokens['action'] = {'accept', 'deny', 'reject'}
 
         return supported_tokens, supported_sub_tokens
 
     def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
-        self.oc_policies = []
         total_rule_count = 0
+        self.acl_sets: List[ACLSet] = []
 
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
             filter_name = header.FilterName(self._PLATFORM)
 
             # Options are anything after the platform name in the target message of
             # the policy header, [1:].
@@ -240,14 +246,16 @@
             # Get the address family if set.
             address_family = 'inet'
             for i in self._SUPPORTED_AF:
                 if i in filter_options:
                     address_family = i
                     filter_options.remove(i)
 
+            oc_acl_entries: List[ACLEntry] = []
+
             for term in terms:
                 # TODO(b/196430344): Add support for options such as
                 # established/rst/first-fragment
                 if term.option:
                     raise OcFirewallError('OpenConfig firewall does not support term options.')
 
                 # Handle mixed for each indvidual term as inet and inet6.
@@ -255,20 +263,31 @@
                 term_address_families = []
                 if address_family == 'mixed':
                     term_address_families = ['inet', 'inet6']
                 else:
                     term_address_families = [address_family]
                 for term_af in term_address_families:
                     t = Term(term, term_af)
+
                     for rule in t.ConvertToDict():
                         total_rule_count += 1
                         rule['sequence-id'] = total_rule_count * 5
-                        self.oc_policies.append(rule)
+                        oc_acl_entries.append(rule)
+
+            oc_type = self.FAMILY_MAP[address_family]
+
+            oc_acl_set = {
+                "acl-entries": {"acl-entry": oc_acl_entries},
+                "config": {"name": filter_name, "type": oc_type},
+                "name": filter_name,
+                "type": oc_type,
+            }
+            self.acl_sets.append(oc_acl_set)
 
         logging.info('Total rule count of policy %s is: %d', filter_name, total_rule_count)
 
     def __str__(self) -> str:
         out = '%s\n\n' % (
-            json.dumps(self.oc_policies, indent=2, separators=(',', ': '), sort_keys=True)
+            json.dumps(self.acl_sets, indent=2, separators=(',', ': '), sort_keys=True)
         )
 
         return out
```

### Comparing `aerleon-1.5.0/aerleon/lib/packetfilter.py` & `aerleon-1.6.0/aerleon/lib/packetfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,28 +151,32 @@
             protocol = self.term.protocol
         else:
             protocol = []
 
         # source address
         term_saddrs = self._CheckAddressAf(self.term.source_address)
         if not term_saddrs:
-            logging.warning(
-                self.NO_AF_LOG_ADDR.substitute(term=self.term.name, direction='source', af=self.af)
-            )
+            if self.af != 'mixed':
+                logging.warning(
+                    self.NO_AF_LOG_ADDR.substitute(
+                        term=self.term.name, direction='source', af=self.af
+                    )
+                )
             return ''
         term_saddr = self._GenerateAddrStatement(term_saddrs, self.term.source_address_exclude)
 
         # destination address
         term_daddrs = self._CheckAddressAf(self.term.destination_address)
         if not term_daddrs:
-            logging.warning(
-                self.NO_AF_LOG_ADDR.substitute(
-                    term=self.term.name, direction='destination', af=self.af
+            if self.af != 'mixed':
+                logging.warning(
+                    self.NO_AF_LOG_ADDR.substitute(
+                        term=self.term.name, direction='destination', af=self.af
+                    )
                 )
-            )
             return ''
         term_daddr = self._GenerateAddrStatement(
             term_daddrs, self.term.destination_address_exclude
         )
 
         # ports
         source_port = []
```

### Comparing `aerleon-1.5.0/aerleon/lib/paloaltofw.py` & `aerleon-1.6.0/aerleon/lib/paloaltofw.py`

 * *Files 2% similar despite different names*

```diff
@@ -858,45 +858,14 @@
         # using ::<ipv4-address>.  The 0.0.0.0-255.255.255.255 range is
         # equivalent to ::0/96 which will only match IPv4 addresses; when
         # negated it will match only IPv6 addresses.
         # Used for address families inet and inet6 when source and
         # destination address are not specified (any any).
         ANY_IPV4_RANGE = "0.0.0.0-255.255.255.255"
         add_any_ipv4 = False
-        # Name to IP addresses
-        address_book_names_dict = {}
-        address_book_groups_dict = {}
-        try:
-            groups = sorted(self.addressbook.addressbook[''].keys())
-        except:
-            groups = []
-        for group in groups:
-            count = 0
-            for ip in self.addressbook.addressbook[''][group]:
-                name = f'{ip.parent_token}_{count}'
-                count = count + 1
-                address = ip.with_prefixlen
-                if name in address_book_names_dict:
-                    if address_book_names_dict[name].supernet_of(address):
-                        continue
-                address_book_names_dict[name] = address
-
-            # building individual address-group dictionary
-            for nested_group in groups:
-                group_names = [i for i in address_book_names_dict.keys() if nested_group in i]
-
-                address_book_groups_dict[nested_group] = group_names
-
-        # sort address books and address sets
-        address_book_groups_dict = collections.OrderedDict(
-            sorted(address_book_groups_dict.items())
-        )
-        address_book_keys = sorted(
-            list(address_book_names_dict.keys()), key=self._SortAddressBookNumCheck
-        )
 
         # INITAL CONFIG
         config = etree.Element("config", {"urldb": "paloaltonetworks", "version": "8.1.0"})
         devices = etree.SubElement(config, "devices")
         device_entry = etree.SubElement(devices, "entry", {"name": "localhost.localdomain"})
         vsys = etree.SubElement(device_entry, "vsys")
         vsys_entry = etree.SubElement(vsys, "entry", {"name": "vsys1"})
@@ -1022,17 +991,17 @@
                         member.text = "any-ipv4"
                         add_any_ipv4 = True
                     else:
                         member.text = "any"
                 else:
                     for x in options["source"]:
                         if no_addr_obj:
-                            for group in address_book_groups_dict[x]:
+                            for ip in self.addressbook.GetAddress('', x):
                                 member = etree.SubElement(source, "member")
-                                member.text = str(address_book_names_dict[group])
+                                member.text = str(ip)
                                 max_src_dst += 1
                         else:
                             member = etree.SubElement(source, "member")
                             member.text = x
                             max_src_dst += 1
 
                 if max_src_dst > self._MAX_RULE_SRC_DST_MEMBERS:
@@ -1056,17 +1025,17 @@
                                     negate = etree.SubElement(entry, x)
                                     negate.text = "yes"
                         else:
                             member.text = "any"
                 else:
                     for x in options["destination"]:
                         if no_addr_obj:
-                            for group in address_book_groups_dict[x]:
+                            for ip in self.addressbook.GetAddress('', x):
                                 member = etree.SubElement(dest, "member")
-                                member.text = str(address_book_names_dict[group])
+                                member.text = str(ip)
                                 max_src_dst += 1
                         else:
                             member = etree.SubElement(dest, "member")
                             member.text = x
                             max_src_dst += 1
 
                 if max_src_dst > self._MAX_RULE_SRC_DST_MEMBERS:
@@ -1129,38 +1098,41 @@
                         log.text = "yes"
                     if "log-end" in options["logging"]:
                         log = etree.SubElement(entry, "log-end")
                         log.text = "yes"
 
         # pytype: enable=key-error
 
-        if no_addr_obj:
-            address_book_groups_dict = {}
-            address_book_keys = {}
-
         # ADDRESS
         vsys_entry.append(etree.Comment(" Address Groups "))
         addr_group = etree.SubElement(vsys_entry, "address-group")
 
-        for group, address_list in address_book_groups_dict.items():
-            entry = etree.SubElement(addr_group, "entry", {"name": group})
-            static = etree.SubElement(entry, "static")
-            for name in address_list:
-                member = etree.SubElement(static, "member")
-                member.text = name
+        if not no_addr_obj:
+            for _, token, ips, _ in self.addressbook.Walk(''):
+                entry = etree.SubElement(addr_group, "entry", {"name": token})
+                static = etree.SubElement(entry, "static")
+                count = 0
+                for ip in ips:
+                    member = etree.SubElement(static, "member")
+                    member.text = f'{ip.parent_token}_{count}'
+                    count += 1
 
         vsys_entry.append(etree.Comment(" Addresses "))
         addr = etree.SubElement(vsys_entry, "address")
+        if not no_addr_obj:
 
-        for name in address_book_keys:
-            entry = etree.SubElement(addr, "entry", {"name": name})
-            desc = etree.SubElement(entry, "description")
-            desc.text = name
-            ip = etree.SubElement(entry, "ip-netmask")
-            ip.text = str(address_book_names_dict[name])
+            for _, token, ips, _ in self.addressbook.Walk(''):
+                count = 0
+                for ip in ips:
+                    entry = etree.SubElement(addr, "entry", {"name": f'{token}_{count}'})
+                    desc = etree.SubElement(entry, "description")
+                    desc.text = f'{token}_{count}'
+                    elem = etree.SubElement(entry, "ip-netmask")
+                    elem.text = str(ip)
+                    count += 1
 
         if add_any_ipv4:
             entry = etree.SubElement(addr, "entry", {"name": "any-ipv4"})
             desc = etree.SubElement(entry, "description")
             desc.text = (
                 "Object to match all IPv4 addresses; " "negate to match all IPv6 addresses."
             )
```

### Comparing `aerleon-1.5.0/aerleon/lib/pcap.py` & `aerleon-1.6.0/aerleon/lib/pcap.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,31 +124,35 @@
                 '%s %s %s %s'
                 % ('\n', self.term.name, self.term.action[0], 'action not currently supported.')
             )
 
         # source address
         term_saddrs = self._CheckAddressAf(self.term.source_address)
         if not term_saddrs:
-            logging.warning(
-                self.NO_AF_LOG_ADDR.substitute(term=self.term.name, direction='source', af=self.af)
-            )
+            if self.af != 'mixed':
+                logging.warning(
+                    self.NO_AF_LOG_ADDR.substitute(
+                        term=self.term.name, direction='source', af=self.af
+                    )
+                )
             return ''
 
         conditions.append(
             self._GenerateAddrStatement(term_saddrs, self.term.source_address_exclude)
         )
 
         # destination address
         term_daddrs = self._CheckAddressAf(self.term.destination_address)
         if not term_daddrs:
-            logging.warning(
-                self.NO_AF_LOG_ADDR.substitute(
-                    term=self.term.name, direction='destination', af=self.af
+            if self.af != 'mixed':
+                logging.warning(
+                    self.NO_AF_LOG_ADDR.substitute(
+                        term=self.term.name, direction='destination', af=self.af
+                    )
                 )
-            )
             return ''
 
         conditions.append(
             self._GenerateAddrStatement(term_daddrs, self.term.destination_address_exclude)
         )
 
         # protocol
```

### Comparing `aerleon-1.5.0/aerleon/lib/plugin.py` & `aerleon-1.6.0/aerleon/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/plugin_supervisor.py` & `aerleon-1.6.0/aerleon/lib/plugin_supervisor.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/policy.py` & `aerleon-1.6.0/aerleon/lib/policy.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/policy_builder.py` & `aerleon-1.6.0/aerleon/lib/policy_builder.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/policy_simple.py` & `aerleon-1.6.0/aerleon/lib/policy_simple.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/policyreader.py` & `aerleon-1.6.0/aerleon/lib/policyreader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/port.py` & `aerleon-1.6.0/aerleon/lib/port.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/recognizers.py` & `aerleon-1.6.0/aerleon/lib/recognizers.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/speedway.py` & `aerleon-1.6.0/aerleon/lib/speedway.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/srxlo.py` & `aerleon-1.6.0/aerleon/lib/srxlo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/summarizer.py` & `aerleon-1.6.0/aerleon/lib/summarizer.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/windows.py` & `aerleon-1.6.0/aerleon/lib/windows.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/windows_advfirewall.py` & `aerleon-1.6.0/aerleon/lib/windows_advfirewall.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/windows_ipsec.py` & `aerleon-1.6.0/aerleon/lib/windows_ipsec.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/lib/yaml.py` & `aerleon-1.6.0/aerleon/lib/yaml.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 
 import yaml
 from absl import logging
 from yaml.error import YAMLError
 
 from aerleon.lib import policy
 from aerleon.lib.policy import BadIncludePath, Policy, _SubpathOf
-from aerleon.lib.policy_builder import (
-    PolicyBuilder,
-    PolicyDict,
-    RawFilter,
-    RawFilterHeader,
-    RawPolicy,
-    RawTerm,
-)
+from aerleon.lib.policy_builder import PolicyBuilder, PolicyDict
 from aerleon.lib.yaml_loader import SpanSafeYamlLoader
 
+MAX_INCLUDE_DEPTH = 5
+
 
 class PolicyTypeError(Exception):
     """Invalid policy."""
 
 
 class ExcessiveRecursionError(Exception):
     """Include depth limit exceeded."""
@@ -104,17 +99,19 @@
     with open(pathlib.Path(base_dir).joinpath(filename), 'r') as file:
         try:
             policy_dict = yaml.load(file, Loader=SpanSafeYamlLoader(filename=filename))
         except YAMLError as yaml_error:
             raise PolicyTypeError(
                 UserMessage("Unable to read file as YAML.", filename=filename)
             ) from yaml_error
-    policy_dict = PreprocessYAMLPolicy(filename, base_dir, policy_dict)
+    policy_dict = _preprocessYAMLPolicy(filename, base_dir, policy_dict)
     if not policy_dict:
         return
+    if not policy_dict['filters']:
+        return
     return policy.FromBuilder(PolicyBuilder(policy_dict, definitions, optimize, shade_check))
 
 
 def ParsePolicy(
     file: str, *, filename, base_dir='', definitions=None, optimize=False, shade_check=False
 ) -> Optional[Union[MagicMock, Policy]]:
     """Load a policy yaml file (provided as a string) and return a Policy data model.
@@ -136,53 +133,147 @@
     try:
         policy_dict = yaml.load(file, Loader=SpanSafeYamlLoader(filename=filename))
     except YAMLError as yaml_error:
         raise PolicyTypeError(
             UserMessage("Unable to read file as YAML.", filename=filename)
         ) from yaml_error
 
-    policy_dict = PreprocessYAMLPolicy(filename, base_dir, policy_dict)
+    policy_dict = _preprocessYAMLPolicy(filename, base_dir, policy_dict)
     if not policy_dict:
         return
+    if not policy_dict['filters']:
+        return
     return policy.FromBuilder(PolicyBuilder(policy_dict, definitions, optimize, shade_check))
 
 
-def PreprocessYAMLPolicy(
+def suffix_is_yaml(filename):
+    return filename[-5:] == '.yaml' or filename[-4:] == '.yml'
+
+
+def _preprocessYAMLPolicy(
     filename: str, base_dir: str, policy_dict: Optional[PolicyDict]
 ) -> Optional[Dict[str, List[Dict[str, Union[Dict[str, Dict[str, str]], List[Dict[str, str]]]]]]]:
     """Process includes and validate the file data as a PolicyDict."""
+    debug_stack = []
+    return _preprocessYAMLPolicyInner(
+        MAX_INCLUDE_DEPTH,
+        debug_stack,
+        filename=filename,
+        base_dir=base_dir,
+        policy_dict=policy_dict,
+    )
+
+
+def _preprocessYAMLPolicyInner(
+    depth: int, debug_stack: list, filename: str, base_dir: str, policy_dict: Optional[PolicyDict]
+) -> Optional[Dict[str, List[Dict[str, Union[Dict[str, Dict[str, str]], List[Dict[str, str]]]]]]]:
 
     # Empty files are ignored with a warning
     if policy_dict is None or not policy_dict:
         logging.warning(UserMessage("Ignoring empty policy file.", filename=filename))
         return
 
     # Malformed policy files should generate a PolicyTypeError (unless this is an include file)
-    if 'filters' not in policy_dict or not isinstance(policy_dict['filters'], list):
-
-        if 'terms' in policy_dict:
-            # In this case we are looking at an include file and need to quietly ignore it.
-            return
-
+    if 'filters' in policy_dict and isinstance(policy_dict['filters'], list):
+        pass  # Normal case.
+    elif (
+        depth < MAX_INCLUDE_DEPTH
+        and 'filters_include_only' in policy_dict
+        and isinstance(policy_dict['filters_include_only'], list)
+    ):
+        # Policy files with filters_include_only: are ignored by ParsePolicy but can be included.
+        policy_dict['filters'] = policy_dict['filters_include_only']
+        del policy_dict['filters_include_only']
+    elif 'terms' in policy_dict or 'filters_include_only' in policy_dict:
+        # We are looking at an include file outside of an include and should quietly ignore it.
+        return
+    else:
         raise PolicyTypeError(
             UserMessage("Policy file must contain one or more filter sections.", filename=filename)
         )
 
+    found_filters = []
+
     for filter in policy_dict['filters']:
         # Malformed filters should generate a PolicyTypeError
         if not isinstance(filter, dict):
             raise PolicyTypeError(UserMessage("Filter must be a mapping.", filename=filename))
+
+        def expand_filter(filter):
+            stack = debug_stack.copy()
+            stack.append((filter['__filename__'], filter['__line__']))
+
+            if depth <= 0:
+                raise ExcessiveRecursionError(
+                    UserMessage(
+                        f"Excessive recursion: include depth limit of {MAX_INCLUDE_DEPTH} reached.",  # noqa: E501
+                        filename=filter['__filename__'],
+                        line=filter['__line__'],
+                        include_chain=stack,
+                    )
+                )
+            if not suffix_is_yaml(filter['include']):
+                raise PolicyTypeError(
+                    UserMessage(
+                        f"Policy include source {filter['include']} must end in \".yaml\".",  # noqa: E501
+                        filename=filter['__filename__'],
+                        line=filter['__line__'],
+                        include_chain=stack,
+                    )
+                )
+            include_path = pathlib.Path(base_dir).joinpath(filter['include'])
+            if not _SubpathOf(base_dir, include_path):
+                raise BadIncludePath(
+                    f"Include file cannot be loaded from outside the base directory. File={include_path} base_directory={base_dir}"
+                )
+            try:
+                include_file = _LoadIncludeFile(include_path)
+                include_data = yaml.load(
+                    include_file, Loader=SpanSafeYamlLoader(filename=str(include_path))
+                )
+            except YAMLError as yaml_error:
+                raise PolicyTypeError(
+                    UserMessage(
+                        "Unable to read file as YAML.",
+                        filename=str(include_path),
+                        include_chain=stack,
+                    )
+                ) from yaml_error
+            data = _preprocessYAMLPolicyInner(
+                depth - 1,
+                stack,
+                filename=include_path.name,
+                base_dir=base_dir,
+                policy_dict=include_data,
+            )
+            if not (data and data['filters']):
+                logging.warning(
+                    UserMessage(
+                        "Ignoring empty policy include source.",
+                        filename=str(include_path),
+                        include_chain=stack,
+                    )
+                )
+                return
+            found_filters.extend(data['filters'])
+
+        if 'include' in filter:
+            # This is an include directive
+            expand_filter(filter)
+            continue
+
         if 'header' not in filter or not isinstance(filter['header'], dict):
             raise PolicyTypeError(
                 UserMessage(
                     "Filter must contain a header section.",
                     filename=filename,
                     line=filter['__line__'],
                 )
             )
+
         if 'terms' not in filter or not filter['terms'] or not isinstance(filter['terms'], list):
             raise PolicyTypeError(
                 UserMessage(
                     "Filter must contain a terms section.",
                     filename=filename,
                     line=filter['__line__'],
                 )
@@ -195,89 +286,84 @@
             raise PolicyTypeError(
                 UserMessage(
                     "Filter header must contain a targets section.",
                     filename=filename,
                     line=header['__line__'],
                 )
             )
+
         # Filters with an empty target list can be ignored with a warning
         elif not header['targets']:
             raise PolicyTypeError(
                 UserMessage(
                     "Filter header cannot be empty.",
                     filename=filename,
                     line=filter['__line__'],
                 )
             )
 
         found_terms = []
-        max_include_depth = 5
 
-        def process_include(depth, stack, include_filename):
-            include_path = pathlib.Path(base_dir).joinpath(include_filename)
-            if not _SubpathOf(base_dir, include_path):
-                raise BadIncludePath(
-                    f"Include file cannot be loaded from outside the base directory. File={include_path} base_directory={base_dir}"
-                )
-
-            try:
-                include_file = _LoadIncludeFile(include_path)
-                include_data = yaml.load(
-                    include_file, Loader=SpanSafeYamlLoader(filename=str(include_path))
-                )
-            except YAMLError as yaml_error:
-                raise PolicyTypeError(
-                    UserMessage(
-                        "Unable to read file as YAML.",
-                        filename=str(include_path),
-                        include_chain=stack,
+        def process_terms(depth, stack, term_items):
+            for term_item in term_items:
+                if 'include' not in term_item:
+                    found_terms.append(term_item)
+                    continue
+                new_stack = stack.copy()
+                new_stack.append((term_item['__filename__'], term_item['__line__']))
+                if depth <= 0:
+                    raise ExcessiveRecursionError(
+                        UserMessage(
+                            f"Excessive recursion: include depth limit of {MAX_INCLUDE_DEPTH} reached.",  # noqa: E501
+                            filename=term_item['__filename__'],
+                            line=term_item['__line__'],
+                            include_chain=new_stack,
+                        )
                     )
-                ) from yaml_error
-            if not include_data or 'terms' not in include_data or not include_data['terms']:
-                logging.warning(
-                    UserMessage(
-                        "Ignoring empty policy include source.",
-                        filename=str(include_path),
-                        include_chain=stack,
+                if not suffix_is_yaml(term_item['include']):
+                    raise PolicyTypeError(
+                        UserMessage(
+                            f"Policy include source {term_item['include']} must end in \".yaml\".",  # noqa: E501
+                            filename=term_item['__filename__'],
+                            line=term_item['__line__'],
+                            include_chain=new_stack,
+                        )
+                    )
+                # process_include(depth - 1, new_stack, term_item['include'])
+                include_path = pathlib.Path(base_dir).joinpath(term_item['include'])
+                if not _SubpathOf(base_dir, include_path):
+                    raise BadIncludePath(
+                        f"Include file cannot be loaded from outside the base directory. File={include_path} base_directory={base_dir}"
                     )
-                )
-                return
-            process_terms(depth, stack, include_data['terms'])
 
-        def process_terms(depth, stack, term_items):
-            for term_item in term_items:
-                if 'include' in term_item:
-                    new_stack = stack.copy()
-                    new_stack.append((term_item['__filename__'], term_item['__line__']))
-                    if depth <= 0:
-                        raise ExcessiveRecursionError(
-                            UserMessage(
-                                f"Excessive recursion: include depth limit of {max_include_depth} reached.",  # noqa: E501
-                                filename=term_item['__filename__'],
-                                line=term_item['__line__'],
-                                include_chain=new_stack,
-                            )
+                try:
+                    include_file = _LoadIncludeFile(include_path)
+                    include_data = yaml.load(
+                        include_file, Loader=SpanSafeYamlLoader(filename=str(include_path))
+                    )
+                except YAMLError as yaml_error:
+                    raise PolicyTypeError(
+                        UserMessage(
+                            "Unable to read file as YAML.",
+                            filename=str(include_path),
+                            include_chain=new_stack,
                         )
-                    if (
-                        term_item['include'][-5:] != '.yaml'
-                        and term_item['include'][-4:] != '.yml'
-                    ):
-                        raise PolicyTypeError(
-                            UserMessage(
-                                f"Policy include source {term_item['include']} must end in \".yaml\".",  # noqa: E501
-                                filename=term_item['__filename__'],
-                                line=term_item['__line__'],
-                                include_chain=new_stack,
-                            )
+                    ) from yaml_error
+                if not include_data or 'terms' not in include_data or not include_data['terms']:
+                    logging.warning(
+                        UserMessage(
+                            "Ignoring empty policy include source.",
+                            filename=str(include_path),
+                            include_chain=new_stack,
                         )
-                    process_include(depth - 1, new_stack, term_item['include'])
-                else:
-                    found_terms.append(term_item)
+                    )
+                    continue
+                process_terms(depth - 1, new_stack, include_data['terms'])
 
-        process_terms(max_include_depth, [], filter['terms'])
+        process_terms(MAX_INCLUDE_DEPTH, [], filter['terms'])
 
         if not found_terms:
             logging.warning(
                 UserMessage(
                     "Ignoring filter with zero terms.",
                     filename=filename,
                     line=filter['__line__'],
@@ -292,14 +378,17 @@
                         "Term must have a name.",
                         filename=term_item['__filename__'],
                         line=term_item['__line__'],
                     )
                 )
 
         filter['terms'] = found_terms
+        found_filters.append(filter)
+
+    policy_dict['filters'] = found_filters
 
     def StripDebuggingData(data):
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, list) or isinstance(item, dict):
                     StripDebuggingData(item)
         elif isinstance(data, dict):
```

### Comparing `aerleon-1.5.0/aerleon/lib/yaml_loader.py` & `aerleon-1.6.0/aerleon/lib/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/utils/config.py` & `aerleon-1.6.0/aerleon/utils/config.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/aerleon/utils/iputils.py` & `aerleon-1.6.0/aerleon/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/pyproject.toml` & `aerleon-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerleon"
-version = "1.5.0"
+version = "1.6.0"
 description = "A firewall generation tool"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aerleon/aerleon"
 repository = "https://github.com/aerleon/aerleon"
 keywords = ["firewall", "networking", "security"]
```

### Comparing `aerleon-1.5.0/tools/cgrep.py` & `aerleon-1.6.0/tools/cgrep.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/tools/iputilstools.py` & `aerleon-1.6.0/tools/iputilstools.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.5.0/PKG-INFO` & `aerleon-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerleon
-Version: 1.5.0
+Version: 1.6.0
 Summary: A firewall generation tool
 Home-page: https://github.com/aerleon/aerleon
 License: Apache-2.0
 Keywords: firewall,networking,security
 Author: Rob Ankeny
 Author-email: ankenyr@gmail.com
 Requires-Python: >=3.7,<4.0
```

