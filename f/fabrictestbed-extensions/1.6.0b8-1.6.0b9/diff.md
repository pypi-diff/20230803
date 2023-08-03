# Comparing `tmp/fabrictestbed-extensions-1.6.0b8.tar.gz` & `tmp/fabrictestbed-extensions-1.6.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.6.0b8.tar", last modified: Wed Jul 26 18:52:58 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.6.0b9.tar", last modified: Wed Jul 26 20:21:06 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.6.0b8.tar` & `fabrictestbed-extensions-1.6.0b9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b8/.github/workflows/build.yml
--rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b8/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b8/.github/workflows/test.yml
--rw-r--r--   0        0        0     1839 2023-07-26 18:51:56.402517 fabrictestbed-extensions-1.6.0b8/.gitignore
--rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b8/.readthedocs.yaml
--rw-r--r--   0        0        0     3918 2023-07-26 18:51:56.402734 fabrictestbed-extensions-1.6.0b8/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b8/LICENSE
--rw-r--r--   0        0        0     4509 2023-07-26 18:51:56.402940 fabrictestbed-extensions-1.6.0b8/README.md
--rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b8/docs/Makefile
--rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b8/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b8/docs/source/conf.py
--rw-r--r--   0        0        0     9045 2023-07-26 18:51:56.403389 fabrictestbed-extensions-1.6.0b8/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b8/docs/source/index.rst
--rw-r--r--   0        0        0      149 2023-07-26 18:52:18.640526 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    78005 2023-07-26 18:51:56.405727 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    26951 2023-07-26 18:51:56.406253 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    97080 2023-07-26 18:51:56.406552 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    82338 2023-07-26 18:51:56.407041 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1875 2023-07-26 18:52:31.086467 fabrictestbed-extensions-1.6.0b8/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b8/sphinx.sh
--rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/link_benchmark.py
--rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/local_network_benchmark.py
--rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/network_benchmark_tests.py
--rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/nvme_benchmark.py
--rw-r--r--   0        0        0     6207 2023-07-26 18:51:56.407212 fabrictestbed-extensions-1.6.0b8/tests/integration/L2_reconfig_post_reboot_tests.py
--rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b8/tests/integration/abc_test.py
--rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b8/tests/integration/component_tests.py
--rw-r--r--   0        0        0     2106 2023-07-26 18:51:56.407324 fabrictestbed-extensions-1.6.0b8/tests/integration/test_hello_fabric.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b8/tests/unit/__init__.py
--rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b8/tests/unit/data/dummy-token.json
--rw-r--r--   0        0        0     5522 2023-07-26 18:51:56.407569 fabrictestbed-extensions-1.6.0b8/tests/unit/test_basic.py
--rw-r--r--   0        0        0      397 2023-07-26 18:51:56.407797 fabrictestbed-extensions-1.6.0b8/tox.ini
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b9/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b9/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1839 2023-07-26 18:51:56.402517 fabrictestbed-extensions-1.6.0b9/.gitignore
+-rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b9/.readthedocs.yaml
+-rw-r--r--   0        0        0     3918 2023-07-26 18:51:56.402734 fabrictestbed-extensions-1.6.0b9/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b9/LICENSE
+-rw-r--r--   0        0        0     4509 2023-07-26 18:51:56.402940 fabrictestbed-extensions-1.6.0b9/README.md
+-rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b9/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b9/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b9/docs/source/conf.py
+-rw-r--r--   0        0        0     9045 2023-07-26 18:51:56.403389 fabrictestbed-extensions-1.6.0b9/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b9/docs/source/index.rst
+-rw-r--r--   0        0        0      149 2023-07-26 20:21:01.771735 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    78005 2023-07-26 18:51:56.405727 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26951 2023-07-26 18:51:56.406253 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    97080 2023-07-26 18:51:56.406552 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    82338 2023-07-26 18:51:56.407041 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1875 2023-07-26 20:20:56.523842 fabrictestbed-extensions-1.6.0b9/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b9/sphinx.sh
+-rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b9/tests/benchmarks/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b9/tests/benchmarks/link_benchmark.py
+-rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b9/tests/benchmarks/local_network_benchmark.py
+-rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b9/tests/benchmarks/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b9/tests/benchmarks/nvme_benchmark.py
+-rw-r--r--   0        0        0     6207 2023-07-26 18:51:56.407212 fabrictestbed-extensions-1.6.0b9/tests/integration/L2_reconfig_post_reboot_tests.py
+-rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b9/tests/integration/abc_test.py
+-rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b9/tests/integration/component_tests.py
+-rw-r--r--   0        0        0     2106 2023-07-26 18:51:56.407324 fabrictestbed-extensions-1.6.0b9/tests/integration/test_hello_fabric.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b9/tests/unit/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b9/tests/unit/data/dummy-token.json
+-rw-r--r--   0        0        0     5522 2023-07-26 18:51:56.407569 fabrictestbed-extensions-1.6.0b9/tests/unit/test_basic.py
+-rw-r--r--   0        0        0      397 2023-07-26 18:51:56.407797 fabrictestbed-extensions-1.6.0b9/tox.ini
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b9/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.6.0b8/.github/workflows/build.yml` & `fabrictestbed-extensions-1.6.0b9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.6.0b9/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/.github/workflows/test.yml` & `fabrictestbed-extensions-1.6.0b9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/.gitignore` & `fabrictestbed-extensions-1.6.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/.readthedocs.yaml` & `fabrictestbed-extensions-1.6.0b9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/CHANGELOG.md` & `fabrictestbed-extensions-1.6.0b9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/LICENSE` & `fabrictestbed-extensions-1.6.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/README.md` & `fabrictestbed-extensions-1.6.0b9/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/docs/Makefile` & `fabrictestbed-extensions-1.6.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/docs/make.bat` & `fabrictestbed-extensions-1.6.0b9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/docs/source/conf.py` & `fabrictestbed-extensions-1.6.0b9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/docs/source/fablib.rst` & `fabrictestbed-extensions-1.6.0b9/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/docs/source/index.rst` & `fabrictestbed-extensions-1.6.0b9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/interface.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.6.0b9/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/pyproject.toml` & `fabrictestbed-extensions-1.6.0b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.6.0b7",
+    "fabrictestbed==1.6.0b8",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
     ]
```

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.6.0b9/tests/benchmarks/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/link_benchmark.py` & `fabrictestbed-extensions-1.6.0b9/tests/benchmarks/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/local_network_benchmark.py` & `fabrictestbed-extensions-1.6.0b9/tests/benchmarks/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/network_benchmark_tests.py` & `fabrictestbed-extensions-1.6.0b9/tests/benchmarks/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/nvme_benchmark.py` & `fabrictestbed-extensions-1.6.0b9/tests/benchmarks/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/integration/L2_reconfig_post_reboot_tests.py` & `fabrictestbed-extensions-1.6.0b9/tests/integration/L2_reconfig_post_reboot_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/integration/abc_test.py` & `fabrictestbed-extensions-1.6.0b9/tests/integration/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/integration/component_tests.py` & `fabrictestbed-extensions-1.6.0b9/tests/integration/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/integration/test_hello_fabric.py` & `fabrictestbed-extensions-1.6.0b9/tests/integration/test_hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/tests/unit/test_basic.py` & `fabrictestbed-extensions-1.6.0b9/tests/unit/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b8/PKG-INFO` & `fabrictestbed-extensions-1.6.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.6.0b8
+Version: 1.6.0b9
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.6.0b7
+Requires-Dist: fabrictestbed==1.6.0b8
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
```

