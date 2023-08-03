# Comparing `tmp/ansys_dpf_composites-0.2b2.tar.gz` & `tmp/ansys_dpf_composites-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_dpf_composites-0.2b2.tar", max compression
+gzip compressed data, was "ansys_dpf_composites-0.3.0.tar", max compression
```

## Comparing `ansys_dpf_composites-0.2b2.tar` & `ansys_dpf_composites-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,52 @@
--rw-r--r--   0        0        0     1089 2023-04-04 09:31:11.035109 ansys_dpf_composites-0.2b2/LICENSE
--rw-r--r--   0        0        0     5800 2023-04-04 09:31:11.035109 ansys_dpf_composites-0.2b2/README.rst
--rw-r--r--   0        0        0     3711 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/pyproject.toml
--rw-r--r--   0        0        0      666 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/__init__.py
--rw-r--r--   0        0        0     7464 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_indexer.py
--rw-r--r--   0        0        0      132 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_typing_helper.py
--rw-r--r--   0        0        0    25401 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/composite_model.py
--rw-r--r--   0        0        0      726 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/constants.py
--rw-r--r--   0        0        0    11041 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/data_sources.py
--rw-r--r--   0        0        0     8001 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/example_helper/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/__init__.py
--rw-r--r--   0        0        0     4276 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
--rw-r--r--   0        0        0     1355 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_core_failure.py
--rw-r--r--   0        0        0     6866 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_cuntze.py
--rw-r--r--   0        0        0     2461 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
--rw-r--r--   0        0        0     2094 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
--rw-r--r--   0        0        0     3247 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hashin.py
--rw-r--r--   0        0        0      630 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hoffman.py
--rw-r--r--   0        0        0     4053 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_larc.py
--rw-r--r--   0        0        0     8874 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_strain.py
--rw-r--r--   0        0        0     4705 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_stress.py
--rw-r--r--   0        0        0     9183 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_puck.py
--rw-r--r--   0        0        0     1192 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
--rw-r--r--   0        0        0     1901 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
--rw-r--r--   0        0        0      641 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
--rw-r--r--   0        0        0      629 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
--rw-r--r--   0        0        0     2324 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_von_mises.py
--rw-r--r--   0        0        0      912 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/__init__.py
--rw-r--r--   0        0        0     2879 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
--rw-r--r--   0        0        0      398 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_enums.py
--rw-r--r--   0        0        0    19828 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_layup_info.py
--rw-r--r--   0        0        0     4071 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_operators.py
--rw-r--r--   0        0        0     8676 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_properties.py
--rw-r--r--   0        0        0        0 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/py.typed
--rw-r--r--   0        0        0    10613 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/result_definition.py
--rw-r--r--   0        0        0    29595 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/sampling_point.py
--rw-r--r--   0        0        0     6039 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/select_indices.py
--rw-r--r--   0        0        0      332 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/__init__.py
--rw-r--r--   0        0        0     3586 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
--rw-r--r--   0        0        0     2801 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_load_plugin.py
--rw-r--r--   0        0        0     1944 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/unit_system.py
--rw-r--r--   0        0        0     8556 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.2b2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-08-03 07:51:20.243823 ansys_dpf_composites-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5939 2023-08-03 07:51:20.243823 ansys_dpf_composites-0.3.0/README.rst
+-rw-r--r--   0        0        0     3707 2023-08-03 07:51:20.247823 ansys_dpf_composites-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-08-03 07:51:20.247823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/__init__.py
+-rw-r--r--   0        0        0      754 2023-08-03 07:51:20.247823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_composite_model_factory.py
+-rw-r--r--   0        0        0    25833 2023-08-03 07:51:20.247823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_composite_model_impl.py
+-rw-r--r--   0        0        0    26121 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_composite_model_impl_2023r2.py
+-rw-r--r--   0        0        0     7276 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_indexer.py
+-rw-r--r--   0        0        0    12592 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_sampling_point_helpers.py
+-rw-r--r--   0        0        0      132 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_typing_helper.py
+-rw-r--r--   0        0        0    16724 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/composite_model.py
+-rw-r--r--   0        0        0     1107 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/composite_scope.py
+-rw-r--r--   0        0        0      726 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/constants.py
+-rw-r--r--   0        0        0    21051 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/data_sources.py
+-rw-r--r--   0        0        0     6702 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/example_helper/__init__.py
+-rw-r--r--   0        0        0     1101 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/__init__.py
+-rw-r--r--   0        0        0     4276 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
+-rw-r--r--   0        0        0     1355 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_core_failure.py
+-rw-r--r--   0        0        0     6866 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_cuntze.py
+-rw-r--r--   0        0        0     2461 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
+-rw-r--r--   0        0        0     2094 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
+-rw-r--r--   0        0        0     3072 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_failure_mode_enum.py
+-rw-r--r--   0        0        0     3247 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_hashin.py
+-rw-r--r--   0        0        0      630 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_hoffman.py
+-rw-r--r--   0        0        0     4053 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_larc.py
+-rw-r--r--   0        0        0     8874 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_max_strain.py
+-rw-r--r--   0        0        0     4705 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_max_stress.py
+-rw-r--r--   0        0        0     9183 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_puck.py
+-rw-r--r--   0        0        0     1192 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
+-rw-r--r--   0        0        0     1901 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
+-rw-r--r--   0        0        0      641 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
+-rw-r--r--   0        0        0      629 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
+-rw-r--r--   0        0        0     2324 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_von_mises.py
+-rw-r--r--   0        0        0      912 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/__init__.py
+-rw-r--r--   0        0        0     3983 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
+-rw-r--r--   0        0        0      398 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/_enums.py
+-rw-r--r--   0        0        0    20803 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/_layup_info.py
+-rw-r--r--   0        0        0     4141 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/material_operators.py
+-rw-r--r--   0        0        0     8676 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/material_properties.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/py.typed
+-rw-r--r--   0        0        0    10966 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/result_definition.py
+-rw-r--r--   0        0        0    23474 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/sampling_point.py
+-rw-r--r--   0        0        0    21184 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/sampling_point_2023r2.py
+-rw-r--r--   0        0        0    12720 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/sampling_point_types.py
+-rw-r--r--   0        0        0     5995 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/select_indices.py
+-rw-r--r--   0        0        0      720 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/__init__.py
+-rw-r--r--   0        0        0     3639 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
+-rw-r--r--   0        0        0     4120 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_load_plugin.py
+-rw-r--r--   0        0        0     2452 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_upload_files_to_server.py
+-rw-r--r--   0        0        0     1299 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_versions.py
+-rw-r--r--   0        0        0     1944 2023-08-03 07:51:20.251823 ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/unit_system.py
+-rw-r--r--   0        0        0     8610 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.3.0/PKG-INFO
```

### Comparing `ansys_dpf_composites-0.2b2/LICENSE` & `ansys_dpf_composites-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/README.rst` & `ansys_dpf_composites-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
+.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.8-blue
    :target: https://pypi.org/project/ansys-dpf-composites/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-dpf-composites.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-dpf-composites
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pydpf-composites/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pydpf-composites
+.. |codecov| image:: https://codecov.io/gh/ansys/pydpf-composites/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pydpf-composites
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pydpf-composites/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pydpf-composites/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pydpf-composites/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pydpf-composites/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -33,16 +33,17 @@
    :alt: Black
 
 
 PyDPF Composites is a Python wrapper for Ansys DPF composites. It implements
 classes on top of DPF Composites operators and data accessors for short
 fiber and layered composites (layered shell and solid elements). This module
 can be used to postprocess fiber reinforced plastics and layered composites and
-to implement custom failure criteria and computation. For examples demonstrating
-the behavior and usage of PyDPF Composites, see `PyDPF Composites - Examples`_.
+to implement custom failure criteria and computation. For information demonstrating
+the behavior and usage of PyDPF Composites, see `Examples`_ in the DPF Composite
+documentation.
 
 .. START_MARKER_FOR_SPHINX_DOCS
 
 ----------
 Contribute
 ----------
 
@@ -55,15 +56,15 @@
 Before attempting to contribute to PyDPF Composites, ensure that you are thoroughly
 familiar with the `PyAnsys Developer's Guide`_.
 
 #.  Clone the repository:
 
     .. code:: bash
 
-        git clone https://github.com/pyansys/pydpf-composites
+        git clone https://github.com/ansys/pydpf-composites
         cd pydpf-composites
 
 
 #.  Install dependencies:
 
     .. code:: bash
 
@@ -71,18 +72,20 @@
         pipx ensurepath
         # Minimum required poetry version is 1.2.0
         pipx install poetry
         pipx install pip
         pipx install tox
 
 
-#.  Create a virtual environment and install the package with development
-    dependencies. PyDPF Composites uses `Poetry <https://python-poetry.org>`_
+    PyDPF Composites uses `Poetry <https://python-poetry.org>`_
     to manage the development environment.
 
+#.  Create a virtual environment and install the package with the
+    development dependencies:
+
     .. code:: bash
 
         poetry install --all-extras
 
 
 #.  Activate the virtual environment:
 
@@ -90,77 +93,71 @@
 
         poetry shell
 
 
 Test
 ====
 
-.. note::
-
-   The Docker container referenced in the first option is not yet publicly available.
-
-Set the environment variable `ANSYSLMD_LICENSE_FILE` to configure the licensing or pass it
-as argument (`--license-server=1055@mylicenseserver`) to the pytest call.
-
-There are three ways to run the PyDPF Composites tests, depending on how the DPF
+There are different ways to run the PyDPF Composites tests, depending on how the DPF
 server is started.
 
-#.  Run tests with a Docker container.
+#.  Run tests with a Docker container:
+
+    Follow the steps in `Getting The DPF Server Docker Image`_ to get
+    and run the DPF docker image. Run the tests with the following command
 
     .. code:: bash
 
-        docker pull ghcr.io/pyansys/pydpf-composites:latest
-        pytest .
+        pytest . --port 50052
 
 
 #.  Run tests with a DPF server started from the Ansys installer. The Ansys version must
     be 2023 R2 or later.
 
     .. code:: bash
 
         pytest . --ansys-path "C:\Program Files\Ansys Inc\v232"
 
 
-#.  Run tests with a local gRPC server executable:
+#.  Run tests with a Docker container from Github (Ansys Internal only):
 
     .. code:: bash
 
-        pytest . --server-bin dpf_composites/bin/lib/deps/Ans.Dpf.Grpc.exe
-
-
-    This currently works only on Windows and with the directory structure of the Ansys internal
-    ``dpf_composites`` package. The runtime dependencies of the ``Ans.Dpf.Grpc.exe`` file must be
-    in its folder and the parent folder.
+        docker pull ghcr.io/ansys/pydpf-composites:latest
+        pytest .
 
 
 Build documentation
 ===================
 
-.. note::
-
-    The Docker container referenced in this section is not yet publicly available.
+Follow the description in `Getting The DPF Server Docker Image`_ image to get
+and run the dpf docker image.
 
-
-On Windows, build documentation with this code:
+On Windows, build the documentation with:
 
 .. code:: bash
 
-    docker pull ghcr.io/pyansys/pydpf-composites:latest
-    docker run -d -p 21002:50052 -e ANSYSLMD_LICENSE_FILE=10555@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/pyansys/pydpf-composites:latest
     tox -e doc-windows
 
 
-On Linux, build documentation with this code:
+On Linux, build the documentation with:
 
 .. code:: bash
 
-    docker pull ghcr.io/pyansys/pydpf-composites:latest
-    docker run -d -p 21002:50052 -e ANSYSLMD_LICENSE_FILE=10555@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/pyansys/pydpf-composites:latest
     tox -e doc-linux
 
+Ansys internal only: Build the docs with the latest container from Github:
+
+.. code:: bash
+
+    docker pull ghcr.io/ansys/pydpf-composites:latest
+    docker run -d -p 50052:50052 -e ANSYSLMD_LICENSE_FILE=1055@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/ansys/pydpf-composites:latest
+    tox -e doc-windows
+
+
 
 Run style checks
 ================
 
 The style checks use `pre-commit`_ and can be run through `tox`_:
 
 .. code:: bash
@@ -171,18 +168,31 @@
 The style checks can also be configured to run automatically before each ``git commit``:
 
 .. code:: bash
 
     pre-commit install
 
 
+View documentation
+-------------------
+Documentation for the latest stable release of PyDPF Composites is hosted at
+`PyDPF Composites Documentation <https://composites.dpf.docs.pyansys.com/version/stable/>`_.
+
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
+
+
+
 .. LINKS AND REFERENCES
 .. _black: https://github.com/psf/black
 .. _flake8: https://flake8.pycqa.org/en/latest/
 .. _isort: https://github.com/PyCQA/isort
 .. _pip: https://pypi.org/project/pip/
 .. _pre-commit: https://pre-commit.com/
 .. _PyAnsys Developer's Guide: https://dev.docs.pyansys.com/
 .. _pytest: https://docs.pytest.org/en/stable/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _tox: https://tox.wiki/
-.. _PyDPF Composites - Examples: https://composites.dpf.docs.pyansys.com/dev/examples/index.html
+.. _Examples: https://composites.dpf.docs.pyansys.com/dev/examples/index.html
+.. _Getting The DPF Server Docker Image: https://composites.dpf.docs.pyansys.com/version/stable/intro.html#getting-the-dpf-server-docker-image
```

### Comparing `ansys_dpf_composites-0.2b2/pyproject.toml` & `ansys_dpf_composites-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-dpf-composites"
-version = "0.2b2"
+version = "0.3.0"
 description = "A python wrapper for ansys dpf composites"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
-repository = "https://github.com/pyansys/pydpf-composites"
+repository = "https://github.com/ansys/pydpf-composites"
 documentation = "https://composites.dpf.docs.pyansys.com"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-numpy = [
-    {version = ">=1.19,<1.22", python = ">=3.7,<3.8"},
-    {version = "^1.22", python = ">=3.8"}
-]
-importlib-metadata = {version = "^4.0", python = "<3.8"}
+python = ">=3.8,<4.0"
+packaging = "*"
+numpy = "^1.22"
 build = {version = "^0.8.0", optional = true}
 twine = {version = "^4.0.1", optional = true}
 Sphinx =  {version = "^5.0.1", optional = true}
 numpydoc = {version = "^1.5", optional = true}
 ansys-sphinx-theme = {version = "^0", optional = true}
 sphinx-copybutton =  {version = "^0.4", optional = true}
 sphinx_gallery = {version = "^0.11.0", optional = true}
 sphinx-design = {version = "^0.3.0", optional = true}
 pypandoc = {version = "^1.8.1", optional = true}
 pytest = {version = "^7.1.2", optional = true}
 pytest-cov = {version = "^3.0.0", optional = true}
-mypy = {version = "^0.931", optional = true}
-mypy-extensions = {version = "^0.4.3", optional = true}
-# If this version changes also the link in doc/src/conf.py intersphinx-mapping has to change
+mypy = {version = "^1.2.0", optional = true}
+mypy-extensions = {version = "^1.0.0", optional = true}
 ansys-dpf-core = ">=0.8,<1"
-vtk = {version = "*"}
 matplotlib = {version = "^3.5.0"}
-pyvista = {version = "^0.36.1"}
+pyvista = {version = ">=0.36.1,<1", extras=["jupyter"], optional=true}
 pre-commit = {version = "*", optional = true}
 # Upper bound because there is a problem with examples in versions > 1.20.1
 sphinx-autodoc-typehints = {version = "^1.19,<1.20.2", optional = true}
 pylint = {version = "^2.13", optional = true}
-
+scipy = {version = ">=1.9.0", optional = true}
+pytest-rerunfailures = {version = "^11.1.2", optional = true}
 
 [tool.poetry.extras]
 all = [
     "Sphinx",
     "ansys-sphinx-theme",
     "sphinx-copybutton",
     "sphinx_gallery",
     "sphinx-design",
     "numpydoc",
+    "pyvista",
     "pytest",
     "pytest-cov",
+    "pytest-rerunfailures",
     "twine",
     "build",
     "mypy",
     "mypy-extensions",
     "pylint",
     "pre-commit",
     "pypandoc",
+    "scipy",
     "sphinx-autodoc-typehints",
 ]
 docs = ["Sphinx", "ansys-sphinx-theme", "sphinx-copybutton", "numpydoc", "sphinx_gallery",
-    "pypandoc", "sphinx-autodoc-typehints", "sphinx-design"]
-test = ["pytest", "pytest-cov"]
+    "pypandoc", "sphinx-autodoc-typehints", "sphinx-design", "scipy", "pyvista"]
+test = ["pytest", "pytest-cov", "pytest-rerunfailures"]
 build = ["build", "twine"]
 pre-commit = ["pre-commit", "mypy", "mypy-extensions", "pylint"]
 
 
 [tool.black]
 line-length = 100
 
@@ -116,10 +115,10 @@
 [tool.pylint.typecheck]
 ignored-classes = [
     "ansys.dpf.core.inputs.Inputs",
     "ansys.dpf.core.outputs.Outputs"
 ]
 
 [tool.mypy]
-python_version = 3.7
+python_version = 3.8
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src:$MYPY_CONFIG_FILE_DIR/tests"
 ignore_missing_imports = true
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/__init__.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 except ModuleNotFoundError:
     import importlib_metadata  # type: ignore
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 from . import (
     composite_model,
+    composite_scope,
     constants,
     data_sources,
     failure_criteria,
     layup_info,
     result_definition,
     sampling_point,
     select_indices,
     server_helpers,
 )
 
 __all__ = (
     "composite_model",
+    "composite_scope",
     "constants",
     "data_sources",
     "failure_criteria",
     "layup_info",
     "result_definition",
     "sampling_point",
     "server_helpers",
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_indexer.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_indexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 """Indexer helper classes."""
 from dataclasses import dataclass
-import sys
-from typing import TYPE_CHECKING, Optional, cast
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
+from typing import Optional, Protocol, cast
 
 from ansys.dpf.core import Field, PropertyField, Scoping
 import numpy as np
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
+from numpy.typing import NDArray
 
 
 @dataclass(frozen=True)
 class IndexToId:
     """Mapping maps id to index."""
 
-    mapping: "NDArray[np.int64]"
+    mapping: NDArray[np.int64]
     max_id: int
 
 
 def setup_index_by_id(scoping: Scoping) -> IndexToId:
     """Create array that can be indexed by id to get the index.
 
     For ids which are not present in the scoping the array has a value of -1
 
     Parameters
     ----------
     scoping:
         DPF scoping
     """
-    indices: "NDArray[np.int64]" = np.full(max(scoping.ids) + 1, -1, dtype=np.int64)
+    indices: NDArray[np.int64] = np.full(max(scoping.ids) + 1, -1, dtype=np.int64)
     indices[scoping.ids] = np.arange(len(scoping.ids))
     return IndexToId(mapping=indices, max_id=len(indices) - 1)
 
 
 class PropertyFieldIndexerSingleValue(Protocol):
     """Protocol for single value property field indexer."""
 
     def by_id(self, entity_id: int) -> Optional[np.int64]:
         """Get index by id."""
 
 
 class PropertyFieldIndexerArrayValue(Protocol):
     """Protocol for array valued property field indexer."""
 
-    def by_id(self, entity_id: int) -> Optional["NDArray[np.int64]"]:
+    def by_id(self, entity_id: int) -> Optional[NDArray[np.int64]]:
         """Get index by id."""
 
 
 # General comment for all Indexer:
 # The .data call accesses the actual data. This sends the data over grpc which takes some time
 # It looks like it returns a DpfArray for non-local fields and an numpy array for local fields.
 # Without converting the DpfArray to a numpy array,
@@ -66,15 +58,15 @@
     """Indexer for a property field with no data pointer."""
 
     def __init__(self, field: PropertyField):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
         self._max_id = index_by_id.max_id
-        self._data: "NDArray[np.int64]" = np.array(field.data, dtype=np.int64)
+        self._data: NDArray[np.int64] = np.array(field.data, dtype=np.int64)
 
     def by_id(self, entity_id: int) -> Optional[np.int64]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
@@ -92,15 +84,15 @@
     """Indexer for a dpf field with no data pointer."""
 
     def __init__(self, field: Field):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
         self._max_id = index_by_id.max_id
-        self._data: "NDArray[np.double]" = np.array(field.data, dtype=np.double)
+        self._data: NDArray[np.double] = np.array(field.data, dtype=np.double)
 
     def by_id(self, entity_id: int) -> Optional[np.double]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
@@ -116,15 +108,15 @@
 class PropertyFieldIndexerNoDataPointerNoBoundsCheck:
     """Indexer for a property field with no data pointer and no bounds checks."""
 
     def __init__(self, field: PropertyField):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
-        self._data: "NDArray[np.int64]" = np.array(field.data, dtype=np.int64)
+        self._data: NDArray[np.int64] = np.array(field.data, dtype=np.int64)
 
     def by_id(self, entity_id: int) -> Optional[np.int64]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
@@ -137,36 +129,36 @@
 
     def __init__(self, field: PropertyField):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
         self._max_id = index_by_id.max_id
 
-        self._data: "NDArray[np.int64]" = np.array(field.data, dtype=np.int64)
+        self._data: NDArray[np.int64] = np.array(field.data, dtype=np.int64)
         self._n_components = field.component_count
 
-        self._data_pointer: "NDArray[np.int64]" = np.append(
+        self._data_pointer: NDArray[np.int64] = np.append(
             field._data_pointer, len(self._data) * self._n_components
         )
 
-    def by_id(self, entity_id: int) -> Optional["NDArray[np.int64]"]:
+    def by_id(self, entity_id: int) -> Optional[NDArray[np.int64]]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
         """
         if entity_id > self._max_id:
             return None
 
         idx = self._indices[entity_id]
         if idx < 0:
             return None
         return cast(
-            "NDArray[np.int64]",
+            NDArray[np.int64],
             self._data[
                 self._data_pointer[idx]
                 // self._n_components : self._data_pointer[idx + 1]
                 // self._n_components
             ],
         )
 
@@ -176,36 +168,36 @@
 
     def __init__(self, field: Field):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
         self._max_id = index_by_id.max_id
 
-        self._data: "NDArray[np.double]" = np.array(field.data, dtype=np.double)
+        self._data: NDArray[np.double] = np.array(field.data, dtype=np.double)
         self._n_components = field.component_count
 
-        self._data_pointer: "NDArray[np.int64]" = np.append(
+        self._data_pointer: NDArray[np.int64] = np.append(
             field._data_pointer, len(self._data) * self._n_components
         )
 
-    def by_id(self, entity_id: int) -> Optional["NDArray[np.double]"]:
+    def by_id(self, entity_id: int) -> Optional[NDArray[np.double]]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
         """
         if entity_id > self._max_id:
             return None
 
         idx = self._indices[entity_id]
         if idx < 0:
             return None
         return cast(
-            "NDArray[np.double]",
+            NDArray[np.double],
             self._data[
                 self._data_pointer[idx]
                 // self._n_components : self._data_pointer[idx + 1]
                 // self._n_components
             ],
         )
 
@@ -214,33 +206,33 @@
     """Indexer for a property field with data pointer and no bounds checks."""
 
     def __init__(self, field: PropertyField):
         """Create indexer and get data."""
         index_by_id = setup_index_by_id(field.scoping)
         self._indices = index_by_id.mapping
 
-        self._data: "NDArray[np.int64]" = np.array(field.data, dtype=np.int64)
+        self._data: NDArray[np.int64] = np.array(field.data, dtype=np.int64)
 
         self._n_components = field.component_count
 
-        self._data_pointer: "NDArray[np.int64]" = np.append(
+        self._data_pointer: NDArray[np.int64] = np.append(
             field._data_pointer, len(self._data) * self._n_components
         )
 
-    def by_id(self, entity_id: int) -> Optional["NDArray[np.int64]"]:
+    def by_id(self, entity_id: int) -> Optional[NDArray[np.int64]]:
         """Get index by id.
 
         Parameters
         ----------
         entity_id
         """
         idx = self._indices[entity_id]
         if idx < 0:
             return None
         return cast(
-            "NDArray[np.int64]",
+            NDArray[np.int64],
             self._data[
                 self._data_pointer[idx]
                 // self._n_components : self._data_pointer[idx + 1]
                 // self._n_components
             ],
         )
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/composite_model.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/_composite_model_impl_2023r2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-"""Composite Model."""
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Collection, Dict, List, Optional, Sequence, cast
+"""Composite Model Interface 2023R2."""
+from typing import Collection, Dict, List, Optional, Sequence, cast
+from warnings import warn
 
 import ansys.dpf.core as dpf
 from ansys.dpf.core import FieldsContainer, MeshedRegion, Operator, UnitSystem
 from ansys.dpf.core.server_types import BaseServer
 import numpy as np
+from numpy.typing import NDArray
 
-from .unit_system import UnitSystemProvider, get_unit_system
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
-
+from .composite_scope import CompositeScope
 from .data_sources import (
     CompositeDataSources,
     ContinuousFiberCompositesFiles,
     get_composites_data_sources,
 )
 from .failure_criteria import CombinedFailureCriterion
 from .layup_info import (
@@ -23,53 +20,19 @@
     LayerProperty,
     LayupPropertiesProvider,
     add_layup_info_to_mesh,
     get_element_info_provider,
 )
 from .layup_info.material_operators import MaterialOperators, get_material_operators
 from .layup_info.material_properties import MaterialProperty, get_constant_property_dict
-from .result_definition import FailureMeasure, ResultDefinition, ResultDefinitionScope
-from .sampling_point import SamplingPoint
-
-__all__ = ("CompositeScope", "CompositeInfo", "CompositeModel")
-
-
-@dataclass(frozen=True)
-class CompositeScope:
-    """Provides the composite scope.
-
-    This class defines which part of the model and solution step are selected.
-
-    Parameters
-    ----------
-    elements:
-        List of elements.
-    plies:
-        List of plies.
-    time:
-        Time or frequency. You can use the
-        :func:`CompositeModel.get_result_times_or_frequencies` method
-        to list the solution steps.
-    named_selections:
-        List of element sets.
-        Use `composite_model.get_mesh().available_named_selections` to list
-        all named selections.
-
-    Notes
-    -----
-    If more than one scope (``elements``, ``named_selections`` and ``plies``)
-    is set, then the final element scope is the intersection
-    of the defined parameters. All elements are selected if no parameter is set.
-
-    """
-
-    elements: Optional[Sequence[int]] = None
-    plies: Optional[Sequence[str]] = None
-    time: Optional[float] = None
-    named_selections: Optional[Sequence[str]] = None
+from .result_definition import FailureMeasureEnum, ResultDefinition, ResultDefinitionScope
+from .sampling_point_2023r2 import SamplingPoint2023R2
+from .sampling_point_types import SamplingPoint
+from .server_helpers import upload_continuous_fiber_composite_files_to_server
+from .unit_system import UnitSystemProvider, get_unit_system
 
 
 class CompositeInfo:
     """Contains composite data providers for a composite definition."""
 
     def __init__(
         self,
@@ -97,20 +60,22 @@
             stream_provider_or_data_source=streams_provider,
         )
         self.layup_properties_provider = LayupPropertiesProvider(
             layup_provider=self.layup_provider, mesh=self.mesh
         )
 
 
-class CompositeModel:
+class CompositeModelImpl2023R2:
     """Provides access to the basic composite postprocessing functionality.
 
+    This class supports DPF Server version 6.1 (2-23 R2) and earlier.
     On initialization, the ``CompositeModel`` class automatically adds composite lay-up
-    information to the meshed regions. It prepares the providers for different lay-up properties
-    so that they can be efficiently evaluated.
+    information to the meshed regions. It prepares the providers for different lay-up
+    properties so that they can be efficiently evaluated. The composite_files provided
+    are automatically uploaded to the server if needed.
 
     .. note::
 
         When creating a ``CompositeModel`` instance, several providers are created and
         lay-up information is added to the DPF meshed regions. Depending on the use
         case, it can be more efficient to create the providers separately.
 
@@ -122,15 +87,15 @@
         parameter. The layered elements that get information from a given
         composite definition label can be determined by calling
         ``self.get_all_layered_element_ids_for_composite_definition_label``.
         All the elements that are not part of a composite definition are either homogeneous
         solids or layered models defined outside of an ACP model. The
         ``self.composite_definition_labels`` command returns all available composite
         definition labels. For more information, see
-        :ref:`sphx_glr_examples_gallery_examples_8_assembly_example.py`.
+        :ref:`sphx_glr_examples_gallery_examples_008_assembly_example.py`.
 
     Parameters
     ----------
     composite_files:
         Use the :func:`.get_composite_files_from_workbench_result_folder` function to obtain
         the :class:`.ContinuousFiberCompositesFiles` object.
     server:
@@ -144,46 +109,62 @@
     def __init__(
         self,
         composite_files: ContinuousFiberCompositesFiles,
         server: BaseServer,
         default_unit_system: Optional[UnitSystem] = None,
     ):
         """Initialize data providers and add composite information to meshed region."""
-        self._core_model = dpf.Model(composite_files.rst, server=server)
-        self._server = server
+        self._composite_files = upload_continuous_fiber_composite_files_to_server(
+            composite_files, server
+        )
+        self._data_sources = get_composites_data_sources(self._composite_files)
 
-        self._composite_files = composite_files
-        self._data_sources = get_composites_data_sources(composite_files)
+        self._core_model = dpf.Model(self._data_sources.rst, server=server)
+        self._server = server
 
         self._unit_system = get_unit_system(self._data_sources.rst, default_unit_system)
 
         self._material_operators = get_material_operators(
-            rst_data_source=self._data_sources.rst,
+            rst_data_source=self._data_sources.material_support,
             unit_system=self._unit_system,
             engineering_data_source=self._data_sources.engineering_data,
         )
 
         self._composite_infos: Dict[str, CompositeInfo] = {}
-        for composite_definition_label in self._data_sources.composite:
+        for composite_definition_label in self._data_sources.old_composite_sources:
             self._composite_infos[composite_definition_label] = CompositeInfo(
-                self._data_sources,
-                composite_definition_label,
-                self._core_model.metadata.streams_provider,
+                data_sources=self._data_sources,
+                composite_definition_label=composite_definition_label,
+                streams_provider=self._core_model.metadata.streams_provider,
                 material_operators=self._material_operators,
                 unit_system=self._unit_system,
             )
 
+        if len(self._composite_infos) > 1:
+            warn(
+                "The post-processing of composite models with multiple lay-up"
+                " definitions (assemblies) is deprecated with DPF servers older than 7.0"
+                " (2024 R1). Please use DPF server 7.0 or later.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
     @property
     def composite_definition_labels(self) -> Sequence[str]:
         """All composite definition labels in the model.
 
         This property is only relevant for assemblies.
         """
         return list(self._composite_infos.keys())
 
+    @property
+    def composite_files(self) -> ContinuousFiberCompositesFiles:
+        """Get the composite file paths on the server."""
+        return self._composite_files
+
     def get_mesh(self, composite_definition_label: Optional[str] = None) -> MeshedRegion:
         """Get the underlying DPF meshed region.
 
         The meshed region contains the lay-up information.
 
         Parameters
         ----------
@@ -209,15 +190,15 @@
 
     @property
     def material_operators(self) -> MaterialOperators:
         """Material operators."""
         return self._material_operators
 
     def get_layup_operator(self, composite_definition_label: Optional[str] = None) -> Operator:
-        """Get the lay-up operators.
+        """Get the lay-up operator.
 
         Parameters
         ----------
         composite_definition_label :
             Label of the composite definition, which is the
             dictionary key in the :attr:`.ContinuousFiberCompositesFiles.composite`
             attribute. This parameter is only required for assemblies.
@@ -228,23 +209,23 @@
             composite_definition_label = self._first_composite_definition_label_if_only_one()
         return self._composite_infos[composite_definition_label].layup_provider
 
     def evaluate_failure_criteria(
         self,
         combined_criterion: CombinedFailureCriterion,
         composite_scope: Optional[CompositeScope] = None,
-        measure: FailureMeasure = FailureMeasure.INVERSE_RESERVE_FACTOR,
+        measure: FailureMeasureEnum = FailureMeasureEnum.INVERSE_RESERVE_FACTOR,
         write_data_for_full_element_scope: bool = True,
     ) -> FieldsContainer:
         """Get a fields container with the evaluated failure criteria.
 
         The fields container contains the maximum per element if the measure
-        is :attr:`.FailureMeasure.INVERSE_RESERVE_FACTOR` and the minimum per element
-        if the measure is :attr:`.FailureMeasure.MARGIN_OF_SAFETY` or
-        :attr:`.FailureMeasure.RESERVE_FACTOR`.
+        is :attr:`.FailureMeasureEnum.INVERSE_RESERVE_FACTOR` and the minimum per element
+        if the measure is :attr:`.FailureMeasureEnum.MARGIN_OF_SAFETY` or
+        :attr:`.FailureMeasureEnum.RESERVE_FACTOR`.
 
         Parameters
         ----------
         combined_criterion :
             Combined failure criterion to evaluate.
         composite_scope :
             Composite scope on which to evaluate the failure criteria. If empty, the criteria
@@ -278,14 +259,15 @@
             # write_data_for_full_element_scope flag to True can lead to
             # problems with 2023 R1 if non-composite elements such as
             # beams exist in the solution. Because the flag
             # is irrelevant for cases without a ply scope, we set it to False here.
             write_data_for_full_element_scope = False
 
         scopes = []
+
         for composite_definition_label in self.composite_definition_labels:
             composite_files = self._composite_files.composite[composite_definition_label]
             scopes.append(
                 ResultDefinitionScope(
                     composite_definition=composite_files.definition,
                     mapping_file=composite_files.mapping,
                     element_scope=element_scope_in,
@@ -293,26 +275,27 @@
                     named_selection_scope=ns_in,
                     write_data_for_full_element_scope=write_data_for_full_element_scope,
                 )
             )
 
         rd = ResultDefinition(
             name="combined failure criteria",
-            rst_file=self._composite_files.rst,
+            rst_files=self._composite_files.rst,
             material_file=self._composite_files.engineering_data,
             combined_failure_criterion=combined_criterion,
             composite_scopes=scopes,
             time=time_in,
             measure=measure.value,
         )
         failure_operator = dpf.Operator("composite::composite_failure_operator")
+        failure_operator.inputs.unit_system(self._unit_system)
 
         failure_operator.inputs.result_definition(rd.to_json())
 
-        if measure == FailureMeasure.INVERSE_RESERVE_FACTOR:
+        if measure == FailureMeasureEnum.INVERSE_RESERVE_FACTOR:
             return failure_operator.outputs.fields_containerMax()
         else:
             return failure_operator.outputs.fields_containerMin()
 
     def get_sampling_point(
         self,
         combined_criterion: CombinedFailureCriterion,
@@ -356,22 +339,22 @@
             mapping_file=self._composite_files.composite[composite_definition_label].mapping,
             element_scope=[element_id],
             ply_scope=[],
             named_selection_scope=[],
         )
         rd = ResultDefinition(
             name="combined failure criteria",
-            rst_file=self._composite_files.rst,
+            rst_files=self._composite_files.rst,
             material_file=self._composite_files.engineering_data,
             combined_failure_criterion=combined_criterion,
             time=time_in,
             composite_scopes=[scope],
         )
 
-        return SamplingPoint("Sampling Point", rd, server=self._server)
+        return SamplingPoint2023R2("Sampling Point", rd, self._unit_system, server=self._server)
 
     def get_element_info(
         self, element_id: int, composite_definition_label: Optional[str] = None
     ) -> Optional[ElementInfo]:
         """Get element information for an element ID.
 
         This method returns ``None`` if the element type is not supported.
@@ -393,15 +376,15 @@
         ].element_info_provider.get_element_info(element_id)
 
     def get_property_for_all_layers(
         self,
         layup_property: LayerProperty,
         element_id: int,
         composite_definition_label: Optional[str] = None,
-    ) -> Optional["NDArray[np.double]"]:
+    ) -> Optional[NDArray[np.double]]:
         """Get a layer property for an element ID.
 
         Returns a numpy array with the values of the property for all the layers.
         Values are ordered from bottom to top.
 
         This method returns ``None`` if the element is not layered.
 
@@ -428,15 +411,15 @@
             return layup_properties_provider.get_layer_thicknesses(element_id)
         if layup_property == LayerProperty.SHEAR_ANGLES:
             return layup_properties_provider.get_layer_shear_angles(element_id)
         raise RuntimeError(f"Invalid property {layup_property}")
 
     def get_analysis_plies(
         self, element_id: int, composite_definition_label: Optional[str] = None
-    ) -> Optional[Collection[str]]:
+    ) -> Optional[Sequence[str]]:
         """Get analysis ply names.
 
         This method returns ``None`` if the element is not layered.
 
         Parameters
         ----------
         element_id:
@@ -512,30 +495,30 @@
         return get_constant_property_dict(
             material_properties=material_properties,
             materials_provider=self.material_operators.material_provider,
             data_source_or_streams_provider=self.core_model.metadata.streams_provider,
             mesh=self.get_mesh(composite_definition_label),
         )
 
-    def get_result_times_or_frequencies(self) -> "NDArray[np.double]":
+    def get_result_times_or_frequencies(self) -> NDArray[np.double]:
         """Get the times or frequencies in the result file."""
         return cast(
-            "NDArray[np.double]", self._core_model.metadata.time_freq_support.time_frequencies.data
+            NDArray[np.double], self._core_model.metadata.time_freq_support.time_frequencies.data
         )
 
     def add_interlaminar_normal_stresses(
         self,
         stresses: FieldsContainer,
         strains: FieldsContainer,
         composite_definition_label: Optional[str] = None,
     ) -> None:
         """Add interlaminar normal stresses to the stresses fields container.
 
         For a usage example, see
-        :ref:`sphx_glr_examples_gallery_examples_7_interlaminar_normal_stress_example.py`.
+        :ref:`sphx_glr_examples_gallery_examples_007_interlaminar_normal_stress_example.py`.
 
         Parameters
         ----------
         stresses:
             Stresses fields container to add interlaminar normal stresses to.
         strains:
         composite_definition_label:
@@ -559,27 +542,41 @@
         ins_operator.inputs.section_data_container(layup_provider.outputs.section_data_container)
         ins_operator.inputs.strains_container(strains)
         ins_operator.inputs.stresses_container(stresses)
 
         # call run because ins operator has not output
         ins_operator.run()
 
+    def get_all_layered_element_ids(self) -> Sequence[int]:
+        """Get all layered element IDs."""
+        raise NotImplementedError(
+            "get_all_layered_element_ids is not implemented"
+            " for this version of DPF. Please upgrade to 7.0 (2024 R1)"
+            " or later. Use get_all_layered_element_ids_for_composite_definition_label"
+            " instead."
+        )
+
     def get_all_layered_element_ids_for_composite_definition_label(
-        self, composite_definition_label: str
+        self, composite_definition_label: Optional[str]
     ) -> Sequence[int]:
         """Get all layered element IDs that belong to a composite definition label.
 
         Parameters
         ----------
         composite_definition_label:
             Label of the composite definition, which is the
             dictionary key in the :attr:`.ContinuousFiberCompositesFiles.composite`
             attribute. This parameter is only required for assemblies.
             See the note about assemblies in the description for the :class:`CompositeModel` class.
         """
+        if not composite_definition_label:
+            raise RuntimeError(
+                "The composite_definition_label must be set for this version of DPF server."
+                " Or update the the latest version."
+            )
         return cast(
             List[int],
             self.get_mesh(composite_definition_label)
             .property_field("element_layer_indices")
             .scoping.ids,
         )
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/constants.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/example_helper/__init__.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/example_helper/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,42 @@
 """Helper to get example files."""
 
 from dataclasses import dataclass
 import os
 import tempfile
-from typing import Dict, Optional, cast
+from typing import Dict, List, Optional, cast
 import urllib.request
 
 import ansys.dpf.core as dpf
 
-from .._typing_helper import PATH as _PATH
 from ..data_sources import (
     CompositeDefinitionFiles,
     ContinuousFiberCompositesFiles,
     ShortFiberCompositesFiles,
 )
 
-EXAMPLE_REPO = "https://github.com/pyansys/example-data/raw/master/pydpf-composites/"
-
-
-def upload_short_fiber_composite_files_to_server(
-    data_files: ShortFiberCompositesFiles, server: dpf.server
-) -> ShortFiberCompositesFiles:
-    """Upload short fiber composites files to server.
-
-    Parameters
-    ----------
-    data_files
-    server
-    """
-
-    def upload(filename: _PATH) -> str:
-        return cast(str, dpf.upload_file_in_tmp_folder(filename, server=server))
-
-    return ShortFiberCompositesFiles(
-        rst=upload(data_files.engineering_data),
-        dsdat=upload(data_files.dsdat),
-        engineering_data=upload(data_files.engineering_data),
-    )
-
-
-def upload_continuous_fiber_composite_files_to_server(
-    data_files: ContinuousFiberCompositesFiles, server: dpf.server
-) -> ContinuousFiberCompositesFiles:
-    """Upload continuous fiber composites files to server.
-
-    Note: If server.local_server == True the data_files are returned unmodified.
-
-    Parameters
-    ----------
-    data_files
-    server
-    """
-    if server.local_server:
-        return data_files
-
-    def upload(filename: _PATH) -> _PATH:
-        return cast(str, dpf.upload_file_in_tmp_folder(filename, server=server))
-
-    all_composite_files = {}
-    for key, composite_files_by_scope in data_files.composite.items():
-        composite_definition_files = CompositeDefinitionFiles(
-            definition=upload(composite_files_by_scope.definition),
-        )
-
-        if composite_files_by_scope.mapping is not None:
-            composite_definition_files.mapping = upload(composite_files_by_scope.mapping)
-
-        all_composite_files[key] = composite_definition_files
-
-    return ContinuousFiberCompositesFiles(
-        rst=upload(data_files.rst),
-        engineering_data=upload(data_files.engineering_data),
-        composite=all_composite_files,
-    )
+EXAMPLE_REPO = "https://github.com/ansys/example-data/raw/master/pydpf-composites/"
 
 
 @dataclass
 class _ContinuousFiberCompositeFiles:
     definition: str
     mapping: Optional[str] = None
 
 
 @dataclass
 class _ContinuousFiberCompositesExampleFilenames:
-    rst: str
+    rst: List[str]
     composite: Dict[str, _ContinuousFiberCompositeFiles]
     engineering_data: str
 
 
 @dataclass
 class _ShortFiberCompositesExampleFilenames:
-    rst: str
+    rst: List[str]
     dsdat: str
     engineering_data: str
 
 
 @dataclass
 class _ContinuousFiberExampleLocation:
     """Location of the a given continuous fiber example in the example_data repo.
@@ -127,56 +69,66 @@
     files: _ShortFiberCompositesExampleFilenames
 
 
 _continuous_fiber_examples: Dict[str, _ContinuousFiberExampleLocation] = {
     "shell": _ContinuousFiberExampleLocation(
         directory="shell",
         files=_ContinuousFiberCompositesExampleFilenames(
-            rst="shell.rst",
+            rst=["shell.rst"],
             engineering_data="material.engd",
             composite={
                 "shell": _ContinuousFiberCompositeFiles(
                     definition="ACPCompositeDefinitions.h5",
                 )
             },
         ),
     ),
     "ins": _ContinuousFiberExampleLocation(
         directory="ins",
         files=_ContinuousFiberCompositesExampleFilenames(
-            rst="beam_181_analysis_model.rst",
+            rst=["beam_181_analysis_model.rst"],
             engineering_data="materials.xml",
             composite={
                 "shell": _ContinuousFiberCompositeFiles(definition="ACPCompositeDefinitions.h5")
             },
         ),
     ),
     "assembly": _ContinuousFiberExampleLocation(
         directory="assembly",
         files=_ContinuousFiberCompositesExampleFilenames(
-            rst="file.rst",
+            rst=["file.rst"],
             engineering_data="material.engd",
             composite={
                 "solid": _ContinuousFiberCompositeFiles(
                     definition="ACPSolidModel_SM.h5", mapping="ACPSolidModel_SM.mapping"
                 ),
                 "shell": _ContinuousFiberCompositeFiles(
                     definition="ACPCompositeDefinitions.h5",
                     mapping="ACPCompositeDefinitions.mapping",
                 ),
             },
         ),
     ),
+    "harmonic": _ContinuousFiberExampleLocation(
+        directory="harmonic",
+        files=_ContinuousFiberCompositesExampleFilenames(
+            rst=["file.rst"],
+            engineering_data="MatML.xml",
+            composite={
+                "shell": _ContinuousFiberCompositeFiles(definition="ACPCompositeDefinitions.h5"),
+            },
+        ),
+    ),
 }
 
 _short_fiber_examples: Dict[str, _ShortFiberExampleLocation] = {
     "short_fiber": _ShortFiberExampleLocation(
         directory="short_fiber",
         files=_ShortFiberCompositesExampleFilenames(
-            rst="file.rst", engineering_data="MatML.xml", dsdat="ds.dat"
+            rst=["file.rst"], engineering_data="MatML.xml", dsdat="ds.dat"
         ),
     )
 }
 
 
 def _get_file_url(directory: str, filename: str) -> str:
     return EXAMPLE_REPO + "/".join([directory, filename])
@@ -213,17 +165,18 @@
     example_files = _short_fiber_examples[example_key]
     with tempfile.TemporaryDirectory() as tmpdir:
 
         def get_server_path(filename: str) -> str:
             return _download_and_upload_file(example_files.directory, filename, tmpdir, server)
 
         return ShortFiberCompositesFiles(
-            rst=get_server_path(example_files.files.rst),
+            rst=[get_server_path(filename) for filename in example_files.files.rst],
             dsdat=get_server_path(example_files.files.dsdat),
             engineering_data=get_server_path(example_files.files.engineering_data),
+            files_are_local=False,
         )
 
 
 def get_continuous_fiber_example_files(
     server: dpf.server,
     example_key: str,
 ) -> ContinuousFiberCompositesFiles:
@@ -252,11 +205,12 @@
                 composite_files.mapping = get_server_path(
                     composite_examples_files_for_scope.mapping
                 )
 
             all_composite_files[key] = composite_files
 
         return ContinuousFiberCompositesFiles(
-            rst=get_server_path(example_files.files.rst),
+            rst=[get_server_path(rst_path) for rst_path in example_files.files.rst],
             engineering_data=get_server_path(example_files.files.engineering_data),
             composite=all_composite_files,
+            files_are_local=False,
         )
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/__init__.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module of failure criteria."""
 
 from ._combined_failure_criterion import CombinedFailureCriterion
 from ._core_failure import CoreFailureCriterion
 from ._cuntze import CuntzeCriterion
 from ._face_sheet_wrinkling import FaceSheetWrinklingCriterion
+from ._failure_mode_enum import FailureModeEnum
 from ._hashin import HashinCriterion
 from ._hoffman import HoffmanCriterion
 from ._larc import LaRCCriterion
 from ._max_strain import MaxStrainCriterion
 from ._max_stress import MaxStressCriterion
 from ._puck import PuckCriterion
 from ._shear_crimping import ShearCrimpingCriterion
@@ -26,8 +27,9 @@
     "CuntzeCriterion",
     "FaceSheetWrinklingCriterion",
     "HashinCriterion",
     "LaRCCriterion",
     "PuckCriterion",
     "ShearCrimpingCriterion",
     "VonMisesCriterion",
+    "FailureModeEnum",
 ]
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_core_failure.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_core_failure.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_cuntze.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_cuntze.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hashin.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_hashin.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hoffman.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_hoffman.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_larc.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_larc.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_strain.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_max_strain.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_stress.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_max_stress.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_puck.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_puck.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_von_mises.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/failure_criteria/_von_mises.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/__init__.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,53 @@
 """Helper functions to add lay-up information to a DPF meshed region."""
 from typing import Optional
 from warnings import warn
 
-from ansys.dpf.core import MeshedRegion, Operator
+from ansys.dpf.core import DataSources, MeshedRegion, Operator
 
 from ..data_sources import CompositeDataSources
 from ..unit_system import UnitSystemProvider
 from .material_operators import MaterialOperators
 
 
+def _get_composite_data_sources_for_layup_provider(
+    data_sources: CompositeDataSources, composite_definition_label: Optional[str] = None
+) -> DataSources:
+    """
+    Prepare DataSources of composite for the DPF server.
+
+    Ensure that DataSources object is compatible with the version of the layup provider.
+    """
+    # import is here because of circular dependencies
+    from ..server_helpers import version_older_than
+
+    # pylint: disable=protected-access
+    if version_older_than(data_sources.composite._server, "7.0"):
+        if len(data_sources.old_composite_sources) == 1:
+            return data_sources.composite
+        else:
+            if not composite_definition_label:
+                raise RuntimeError(
+                    "Calling _get_composite_data_sources_for_layup_provider"
+                    " without composite_definition_label is not allowed."
+                )
+
+            if composite_definition_label in data_sources.old_composite_sources.keys():
+                return data_sources.old_composite_sources[composite_definition_label]
+            else:
+                key_strs = ", ".join(data_sources.old_composite_sources.keys())
+                raise RuntimeError(
+                    f"Invalid key {composite_definition_label}."
+                    " Available keys in composite data sources are"
+                    f" {key_strs}."
+                )
+
+    return data_sources.composite
+
+
 def add_layup_info_to_mesh(
     data_sources: CompositeDataSources,
     material_operators: MaterialOperators,
     mesh: MeshedRegion,
     unit_system: Optional[UnitSystemProvider] = None,
     composite_definition_label: Optional[str] = None,
 ) -> Operator:
@@ -37,30 +72,24 @@
         attribute. This parameter is only required for assemblies.
         See the note about assemblies in the description for the :class:`.CompositeModel` class.
     Returns
     -------
     :
         Lay-up provider operator.
     """
-    if composite_definition_label is None:
-        composite_definition_labels = list(data_sources.composite.keys())
-        if len(composite_definition_labels) == 1:
-            composite_definition_label = composite_definition_labels[0]
-        else:
-            raise RuntimeError(
-                f"Multiple composite definition keys exists: {composite_definition_labels}. "
-                f"Please specify a key explicitly."
-            )
+    composite_data_sources = _get_composite_data_sources_for_layup_provider(
+        data_sources, composite_definition_label
+    )
 
     # Set up the lay-up provider.
     # Reads the composite definition file and enriches the mesh
     # with the composite lay-up information.
     layup_provider = Operator("composite::layup_provider_operator")
     layup_provider.inputs.mesh(mesh)
-    layup_provider.inputs.data_sources(data_sources.composite[composite_definition_label])
+    layup_provider.inputs.data_sources(composite_data_sources)
     layup_provider.inputs.abstract_field_support(
         material_operators.material_support_provider.outputs.abstract_field_support
     )
 
     if unit_system is None:
         warn(
             "Calling add_layup_info_to_mesh"
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_layup_info.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/_layup_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 """Lay-up information provider."""
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Collection, Dict, List, Optional, Sequence, Union, cast
+from typing import Any, Collection, Dict, List, Optional, Sequence, Union, cast
 
 import ansys.dpf.core as dpf
 from ansys.dpf.core import DataSources, MeshedRegion, Operator, PropertyField
+from ansys.dpf.core.server_types import BaseServer
 import numpy as np
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
+from numpy.typing import NDArray
 
 from .._indexer import (
     FieldIndexerNoDataPointer,
     FieldIndexerWithDataPointer,
     PropertyFieldIndexerArrayValue,
     PropertyFieldIndexerNoDataPointer,
     PropertyFieldIndexerNoDataPointerNoBoundsCheck,
     PropertyFieldIndexerSingleValue,
     PropertyFieldIndexerWithDataPointer,
     PropertyFieldIndexerWithDataPointerNoBoundsCheck,
 )
+from ..server_helpers import version_older_than
 from ._enums import LayupProperty
 
-_ANALYSIS_PLY_PREFIX = "AnalysisPly:"
+
+def _get_separator(server: BaseServer) -> str:
+    if version_older_than(server, "7.0"):
+        return ":"
+    else:
+        return "::"
+
+
+def _get_analysis_ply_prefix(server: BaseServer) -> str:
+    return "AnalysisPly" + _get_separator(server)
 
 
 def get_all_analysis_ply_names(mesh: MeshedRegion) -> Collection[str]:
     """Get names of all available analysis plies."""
+    prefix = _get_analysis_ply_prefix(mesh._server)  # pylint: disable=protected-access
     return [
-        property_field_name[len(_ANALYSIS_PLY_PREFIX) :]
+        property_field_name[len(prefix) :]
         for property_field_name in mesh.available_property_fields
-        if property_field_name.startswith(_ANALYSIS_PLY_PREFIX)
+        if property_field_name.startswith(prefix)
     ]
 
 
 def _get_analysis_ply(mesh: MeshedRegion, name: str, skip_check: bool = False) -> PropertyField:
-    ANALYSIS_PLY_PREFIX = "AnalysisPly:"
-    property_field_name = ANALYSIS_PLY_PREFIX + name
+    prefix = _get_analysis_ply_prefix(mesh._server)  # pylint: disable=protected-access
+    property_field_name = prefix + name
 
     # Because this test can be slow, it can be skipped
     if not skip_check and property_field_name not in mesh.available_property_fields:
         available_analysis_plies = get_all_analysis_ply_names(mesh)
         raise RuntimeError(
             f"Analysis ply is not available: {name}. "
             f"Available analysis plies: {available_analysis_plies}"
@@ -80,15 +90,15 @@
 
     id: int
     n_layers: int
     n_corner_nodes: int
     n_spots: int
     is_layered: bool
     element_type: int
-    dpf_material_ids: "NDArray[np.int64]"
+    dpf_material_ids: NDArray[np.int64]
     is_shell: bool
     number_of_nodes_per_spot_plane: int
 
 
 _supported_element_types = [181, 281, 185, 186, 187, 190]
 
 """
@@ -108,35 +118,34 @@
 def _is_shell(apdl_element_type: np.int64) -> bool:
     return {181: True, 281: True, 185: False, 186: False, 187: False, 190: False}[
         int(apdl_element_type)
     ]
 
 
 def _get_n_spots(apdl_element_type: np.int64, keyopt_8: np.int64, keyopt_3: np.int64) -> int:
-
     if keyopt_3 == 0:
         if apdl_element_type == 185 or apdl_element_type == 186:
             return 0
 
     try:
         return _n_spots_by_element_type_and_keyopt_dict[int(apdl_element_type)][int(keyopt_8)]
     except KeyError as exc:
         raise RuntimeError(
             f"Unsupported element type keyopt8 combination "
             f"Apdl Element Type: {apdl_element_type} "
             f"keyopt8: {keyopt_8}."
         ) from exc
 
 
-def _get_corner_nodes_by_element_type_array() -> "NDArray[np.int64]":
+def _get_corner_nodes_by_element_type_array() -> NDArray[np.int64]:
     # Precompute n_corner_nodes for all element types
     # corner_nodes_by_element_type by can be indexed by element type to get the number of
     # corner nodes. If negative value is returned number of corner nodes is not available.
     all_element_types = [int(e.value) for e in dpf.element_types if e.value >= 0]
-    corner_nodes_by_element_type: "NDArray[np.int64]" = np.full(
+    corner_nodes_by_element_type: NDArray[np.int64] = np.full(
         np.amax(all_element_types) + 1, -1, dtype=np.int64
     )
 
     corner_nodes_by_element_type[all_element_types] = [
         dpf.element_types.descriptor(element_type).n_corner_nodes
         if dpf.element_types.descriptor(element_type).n_corner_nodes is not None
         else -1
@@ -214,14 +223,17 @@
         for element_id in diff:
             element_id_int = int(element_id)
             element_info = element_info_provider.get_element_info(element_id_int)
             if element_info is not None:
                 layer_index = analysis_ply_info_provider.get_layer_index_by_element_id(
                     element_id_int
                 )
+                assert (
+                    layer_index is not None
+                ), f"No layer index found for element with id {element_id_int}."
                 analysis_ply_to_material_map[analysis_ply_name] = element_info.dpf_material_ids[
                     layer_index
                 ]
                 break
 
     return analysis_ply_to_material_map
 
@@ -237,15 +249,14 @@
     Parameters
     ----------
     mesh
         DPF Meshed region enriched with lay-up information
     """
     analysis_ply_name_to_index_map = {}
     with mesh.property_field("layer_to_analysis_ply").as_local_field() as local_field:
-
         for analysis_ply_name in get_all_analysis_ply_names(mesh):
             analysis_ply_property_field = _get_analysis_ply(
                 mesh, analysis_ply_name, skip_check=True
             )
             first_element_id = analysis_ply_property_field.scoping.id(0)
             analysis_ply_indices: List[int] = local_field.get_entity_data_by_id(first_element_id)
 
@@ -261,14 +272,18 @@
 
     Use :func:`~get_element_info_provider` to create :class:`~ElementInfoProvider`
     objects.
 
     Initialize the class before a loop and
     call :func:`~get_element_info` for each element.
 
+    Note that the :class:`~ElementInfoProvider` class is not fully supported for
+    distributed RST files. The :func:`~get_element_info` method will raise an
+    exception if the DPF server version does not support reading the required
+    information.
 
     Parameters
     ----------
     mesh
     layer_indices
     element_types_apdl
     element_types_dpf
@@ -342,35 +357,38 @@
         keyopt_8 = self.keyopt_8_values.by_id(element_id)
         keyopt_3 = self.keyopt_3_values.by_id(element_id)
         apdl_element_type = self.apdl_element_types.by_id(element_id)
 
         if keyopt_3 is None or keyopt_8 is None or apdl_element_type is None:
             raise RuntimeError(
                 "Could not determine element properties. Probably they were requested for an"
-                f" invalid element id. Element id: {element_id}"
+                f" invalid element id. Element id: {element_id}\n"
+                "Note that creating ElementInfo is not fully supported for distributed RST files."
             )
 
         if int(apdl_element_type) not in _supported_element_types:
             return None
 
         n_spots = _get_n_spots(apdl_element_type, keyopt_8, keyopt_3)
         dpf_material_ids: Any = []
         element_type = self.dpf_element_types.by_id(element_id)
+        if element_type is None:
+            raise IndexError(f"No DPF element type for element with id {element_id}.")
 
         layer_data = self.layer_indices.by_id(element_id)
         if layer_data is not None:
             dpf_material_ids = self.layer_materials.by_id(element_id)
             assert dpf_material_ids is not None
             assert layer_data[0] + 1 == len(layer_data), "Invalid size of layer data"
             n_layers = layer_data[0]
             is_layered = True
 
         corner_nodes_dpf = self.corner_nodes_by_element_type[element_type]
         if corner_nodes_dpf < 0:
-            raise Exception(f"Invalid number of corner nodes for element with type {element_type}")
+            raise ValueError(f"Invalid number of corner nodes for element with type {element_type}")
         is_shell = _is_shell(apdl_element_type)
         number_of_nodes_per_spot_plane = -1
         if is_layered:
             number_of_nodes_per_spot_plane = corner_nodes_dpf if is_shell else corner_nodes_dpf // 2
         return ElementInfo(
             n_layers=n_layers,
             n_corner_nodes=corner_nodes_dpf,
@@ -482,36 +500,36 @@
 
         self._index_to_name_map = get_analysis_ply_index_to_name_map(mesh)
 
         self._analysis_ply_indexer = PropertyFieldIndexerWithDataPointer(
             mesh.property_field("layer_to_analysis_ply")
         )
 
-    def get_layer_angles(self, element_id: int) -> Optional["NDArray[np.double]"]:
+    def get_layer_angles(self, element_id: int) -> Optional[NDArray[np.double]]:
         """Get angles for all layers. Returns None if element is not layered.
 
         Parameters
         ----------
         element_id:
             Element Id/Label
         """
         return self._angle_indexer.by_id(element_id)
 
-    def get_layer_thicknesses(self, element_id: int) -> Optional["NDArray[np.double]"]:
+    def get_layer_thicknesses(self, element_id: int) -> Optional[NDArray[np.double]]:
         """Get thicknesses for all layers. Returns None if element is not layered.
 
         Parameters
         ----------
         element_id:
             Element Id/Label
 
         """
         return self._thickness_indexer.by_id(element_id)
 
-    def get_layer_shear_angles(self, element_id: int) -> Optional["NDArray[np.double]"]:
+    def get_layer_shear_angles(self, element_id: int) -> Optional[NDArray[np.double]]:
         """Get shear angle for all layers. Returns None if element is not layered.
 
         Parameters
         ----------
         element_id:
             Element Id/Label
         """
@@ -524,15 +542,15 @@
         ----------
         element_id:
             Element Id/Label
 
         """
         return self._offset_indexer.by_id(element_id)
 
-    def get_analysis_plies(self, element_id: int) -> Optional[Collection[str]]:
+    def get_analysis_plies(self, element_id: int) -> Optional[Sequence[str]]:
         """Get analysis ply names. Returns None if element is not layered.
 
         Parameters
         ----------
         element_id:
             Element Id/Label
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_operators.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/material_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
     unit_system: Optional[UnitSystemProvider] = None,
 ) -> MaterialOperators:
     """Get material properties related to operators.
 
     Parameters
     ----------
     rst_data_source
-        Data source that contains a RST file.
+        Data source that contains a RST file. Note that multiple (distributed)
+        RST files are not supported.
     engineering_data_source
         Data source that contains the Engineering Data file.
     unit_system:
         Unit System
     ----------
 
     """
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_properties.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/layup_info/material_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/result_definition.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/result_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Object to represent the result definition used by the failure operator in DPF Composites."""
 
 from dataclasses import dataclass, field
 from enum import Enum
 import json
-from typing import Any, Dict, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Union
 
 from ._typing_helper import PATH as _PATH
 from .failure_criteria import CombinedFailureCriterion
 
-__all__ = ("FailureMeasure", "ResultDefinitionScope", "ResultDefinition")
+__all__ = ("FailureMeasureEnum", "ResultDefinitionScope", "ResultDefinition")
 
 
-class FailureMeasure(str, Enum):
+class FailureMeasureEnum(str, Enum):
     """Provides available failure measures."""
 
     # TODO: Add descriptions for each property
     INVERSE_RESERVE_FACTOR: str = "inverse_reserve_factor"
     MARGIN_OF_SAFETY: str = "safety_margin"
     RESERVE_FACTOR: str = "safety_factor"
 
 
 _SUPPORTED_EXPRESSIONS = ["composite_failure"]
-_SUPPORTED_MEASURES = [v.value for v in FailureMeasure]
+_SUPPORTED_MEASURES = [v.value for v in FailureMeasureEnum]
 _SUPPORTED_STRESS_STRAIN_EVAL_MODES = ["rst_file", "mapdl_live"]
 
 
 @dataclass
 class ResultDefinitionScope:
     """Provides the result definition scope."""
 
@@ -52,40 +52,41 @@
 
 
 class ResultDefinition:
     """Represents the result definition of DPF Composites.
 
     This class is used to configure the DPF operators ``composite::failure_evaluator``
     and ``composite::sampling_point_evaluator``.
+
     """
 
     _VERSION = 1
     _ACCUMULATOR = "max"
 
     def __init__(
         self,
         name: str,
         combined_failure_criterion: CombinedFailureCriterion,
         composite_scopes: Sequence[ResultDefinitionScope],
-        rst_file: _PATH,
+        rst_files: Sequence[_PATH],
         material_file: _PATH,
         measure: str = "inverse_reserve_factor",
         stress_strain_eval_mode: str = "rst_file",
         time: Union[float, None] = None,
         expression: str = "composite_failure",
         max_chunk_size: int = 50000,
     ):
         """Create a ResultDefinition object."""
         self._name = name
         self._expression = expression
         self._combined_failure_criterion = combined_failure_criterion
         self._measure = measure
         self._composite_scopes = composite_scopes
         self._material_file = material_file
-        self._rst_file = rst_file
+        self._rst_files = list(rst_files)
         self._stress_strain_eval_mode = stress_strain_eval_mode
         self._time = time
         self._max_chunk_size = max_chunk_size
 
     @property
     def name(self) -> str:
         """Custom name."""
@@ -142,21 +143,21 @@
         return self._composite_scopes
 
     @scopes.setter
     def scopes(self, value: Sequence[ResultDefinitionScope]) -> None:
         self._composite_scopes = value
 
     @property
-    def rst_file(self) -> _PATH:
+    def rst_files(self) -> List[_PATH]:
         """Path of the result (RST) files."""
-        return self._rst_file
+        return self._rst_files
 
-    @rst_file.setter
-    def rst_file(self, value: _PATH) -> None:
-        self._rst_file = value
+    @rst_files.setter
+    def rst_files(self, value: List[_PATH]) -> None:
+        self._rst_files = list(value)
 
     @property
     def material_file(self) -> _PATH:
         """Path of the material files that store the material properties.
 
         Supported formats are XML and ENGD.
         """
@@ -237,36 +238,38 @@
             "max_chunk_size": self.max_chunk_size,
         }
 
         if self.time:
             result_definition["time"] = self.time
 
         def get_scope(
-            result_definition_scope: ResultDefinitionScope, rst_file: _PATH, material_file: _PATH
+            result_definition_scope: ResultDefinitionScope,
+            rst_files: List[_PATH],
+            material_file: _PATH,
         ) -> Dict[str, Any]:
             write_for_full_scope = result_definition_scope.write_data_for_full_element_scope
             mapping_entry = []
             if result_definition_scope.mapping_file is not None:
                 mapping_entry.append(str(result_definition_scope.mapping_file))
             return {
                 "datasources": {
                     "composite_definition": [str(result_definition_scope.composite_definition)],
                     "assembly_mapping_file": mapping_entry,
-                    "rst_file": [str(rst_file)],
+                    "rst_file": [str(filename) for filename in rst_files],
                     "material_file": [str(material_file)],
                 },
                 "write_data_for_full_element_scope": write_for_full_scope,
                 "elements": [int(v) for v in result_definition_scope.element_scope],
                 "ply_ids": result_definition_scope.ply_scope,
                 "named_selections": result_definition_scope.named_selection_scope,
             }
 
         scopes = {
             "scopes": [
-                get_scope(scope, self.rst_file, self.material_file)
+                get_scope(scope, self.rst_files, self.material_file)
                 for scope in self._composite_scopes
             ]
         }
 
         result_definition.update(scopes)
         return result_definition
 
@@ -282,14 +285,19 @@
             and not attr.startswith("_")
             and not callable(getattr(self, attr))
             and attr not in exclude
         ]
 
         return properties
 
+    def check_has_single_scope(self, msg: str) -> None:
+        """Check that the result definition has one scope."""
+        if len(self.scopes) != 1:
+            raise RuntimeError(f"Result definition has multiple scopes. {msg}")
+
     def _short_descr(self) -> str:
         """:return: short description of the object."""
         return f"{self.__class__.__name__}(name='{self.name}')"
 
     def __repr__(self) -> str:
         """:return: string conversion."""
         s_attrs = ", ".join([f"{attr}={getattr(self, attr)}" for attr in self._get_properties()])
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/select_indices.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/select_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Functions to get elementary indices based on filter input."""
-from typing import TYPE_CHECKING, Collection, Optional
+from typing import Collection, Optional
 
 import numpy as np
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
+from numpy.typing import NDArray
 
 from .constants import Spot
 from .layup_info import AnalysisPlyInfoProvider, ElementInfo
 
 __all__ = (
     "get_selected_indices",
     "get_selected_indices_by_dpf_material_ids",
@@ -26,15 +24,15 @@
 
 def get_selected_indices(
     element_info: ElementInfo,
     layers: Optional[Collection[int]] = None,
     nodes: Optional[Collection[int]] = None,
     spots: Optional[Collection[Spot]] = None,
     disable_checks: bool = False,
-) -> "NDArray[np.int64]":
+) -> NDArray[np.int64]:
     """Get elementary indices based on element information, layers, nodes, and spots.
 
     Parameters
     ----------
     element_info
         Lay-up information for the element.
     layers
@@ -123,15 +121,15 @@
                 current_index = current_index + 1
 
     return all_indices
 
 
 def get_selected_indices_by_dpf_material_ids(
     element_info: ElementInfo, dpf_material_ids: Collection[np.int64]
-) -> "NDArray[np.int64]":
+) -> NDArray[np.int64]:
     """Get selected indices by DPF material IDs.
 
     This method selects all indices that are in a layer with one of the selected materials.
 
     Parameters
     ----------
     element_info: ElementInfo
@@ -151,15 +149,15 @@
         if mat_id in dpf_material_ids
     ]
     return get_selected_indices(element_info, layers=layer_indices)
 
 
 def get_selected_indices_by_analysis_ply(
     analysis_ply_info_provider: AnalysisPlyInfoProvider, element_info: ElementInfo
-) -> "NDArray[np.int64]":
+) -> NDArray[np.int64]:
     """Get selected indices by analysis ply.
 
     Selects all indices that are in a layer with the given analysis ply
 
     Parameters
     ----------
     analysis_ply_info_provider: AnalysisPlyInfoProvider
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     raise TimeoutError(f"Timeout is reached: {error_message}")
 
 
 def _wait_until_server_is_up(server: _dpf_server) -> Any:
     # Small hack to check if the server is up.
     # The DPF server should check this in the ``connect_to_server`` function, but
     # that's currently not the case.
-    # https://github.com/pyansys/pydpf-core/issues/414
+    # https://github.com/ansys/pydpf-core/issues/414
     # We use the fact that server.version throws an error if the server
     # is not yet connected.
     _try_until_timeout(
         lambda: server.version, "Failed to connect to the DPF server before timing out."
     )
 
 
@@ -85,18 +85,19 @@
         server = start_local_server(
             ansys_path=ansys_path,
             context=_dpf_server.server_context.ServerContext(
                 server_context.LicensingContextType.premium
             ),
         )
 
+    required_version = "6.0"
     server.check_version(
-        "5.0",
-        f"The DPF Composites plugin requires DPF Server version 5.0 (Ansys 2023 R1) or later."
-        f" Your version is currently {server.version}.",
+        required_version,
+        f"The DPF Composites plugin requires DPF Server version {required_version} "
+        f"(Ansys 2023 R2) or later. Your version is currently {server.version}.",
     )
 
     _wait_until_server_is_up(server)
     # Note: server.ansys_path contains the computed Ansys path from
     # dpf.server.start_local_server. It is None if
     # a connection is made to an existing server.
     load_composites_plugin(server, ansys_path=server.ansys_path)
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_load_plugin.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/server_helpers/_load_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,34 @@
 import os
 import pathlib
 from typing import Optional
 
 import ansys.dpf.core as dpf
 from ansys.dpf.core.misc import get_ansys_path
 from ansys.dpf.core.server_types import BaseServer
+from ansys.dpf.gate.errors import DPFServerException
 
-AWP_ROOT_DOCKER = "/ansys_inc/ansys/dpf/server_2023_2_pre1"
-
-
-def load_composites_plugin(server: BaseServer, ansys_path: Optional[str] = None) -> None:
-    r"""Load composites plugins and its dependencies.
-
-    Parameters
-    ----------
-    server:
-    ansys_path:
-        Ansys root path, for example C:\Program Files\ANSYS Inc\v232.
-        If None, it is assumed that all the plugins and their dependencies
-        are found in the PATH/LD_LIBRARY_PATH. If ansys_path
-        is set, the composite_operators and
-        Ans.Dpf.EngineeringData plugins are loaded from their location
-        in the installer.
-    """
-    # The automatic load of the plug can be disabled by the user and so
-    # all plugins which are required for dpf composites are loaded
-    libs = [
-        "Ans.Dpf.Native",
-        "mapdlOperatorsCore",
-        "Ans.Dpf.FEMutils",
-        "Ans.Dpf.EngineeringData",
-        "composite_operators",
-    ]
+from ._versions import version_older_than
 
+# The automatic load of the plug-in can be disabled by the user and so
+# all plugins which are required for dpf composites are loaded
+_PLUGINS = (
+    "Ans.Dpf.Native",
+    "mapdlOperatorsCore",
+    "Ans.Dpf.FEMutils",
+    "Ans.Dpf.EngineeringData",
+    "composite_operators",
+)
+
+
+def _load_plugins(
+    server: BaseServer,
+    awp_root_docker: str,
+    ansys_path: Optional[str] = None,
+) -> None:
     def get_lib_from_name(name: str) -> str:
         if server.os == "posix":
             return f"lib{name}.so"
         elif server.os == "nt":
             return f"{name}.dll"
         else:
             raise RuntimeError(f"Invalid server os: {server.os}")
@@ -45,33 +37,74 @@
     location_in_installer = {
         "composite_operators": {
             "nt": ["dpf", "plugins", "dpf_composites"],
             "posix": ["dpf", "plugins", "dpf_composites"],
         },
     }
 
-    # March 2023 R.Roos
-    # the dpf load_plugin method requires an absolute path because the dfp_composites
-    # plugin is not in the search path. The logic below should support all cases
-    # except a local gRPC sever on linux (local in-process server on Linux is supported)
-    # DPF core team thinks about to expose ANSYS_ROOT_FOLDER so that the absolute path
-    # can be easily constructed here.
     if not ansys_path:
         if server.ansys_path:
             ansys_path = server.ansys_path
         elif server.os == "posix":
-            ansys_path = AWP_ROOT_DOCKER
+            ansys_path = awp_root_docker
         else:
             ansys_path = get_ansys_path()
 
     if not ansys_path:
         raise RuntimeError("Ansys path is not available. DPF Composites plugin cannot be loaded.")
 
-    for name in libs:
+    for name in _PLUGINS:
         if name in location_in_installer:
             relative_location = location_in_installer[name][server.os]
             library = os.path.join(ansys_path, *relative_location, get_lib_from_name(name))
             if server.os == "posix":
                 library = pathlib.Path(library).as_posix()
         else:
             library = get_lib_from_name(name)
         dpf.load_library(library, name, server=server)
+
+
+def load_composites_plugin(server: BaseServer, ansys_path: Optional[str] = None) -> None:
+    r"""Load composites plugins and its dependencies.
+
+    Parameters
+    ----------
+    server:
+    ansys_path:
+        Ansys root path, for example C:\\Program Files\\ANSYS Inc\\v232.
+        If None, it is assumed that all the plugins and their dependencies
+        are found in the PATH/LD_LIBRARY_PATH. If ansys_path
+        is set, the composite_operators and
+        Ans.Dpf.EngineeringData plugins are loaded from their location
+        in the installer.
+    """
+    if version_older_than(server, "7.0"):
+        # March 2023 R.Roos
+        # the dpf load_plugin method requires an absolute path because the dpf_composites
+        # plugin is not in the search path. The logic below should support all cases
+        # except a local gRPC sever on linux (local in-process server on Linux is supported)
+        # DPF core team thinks about to expose ANSYS_ROOT_FOLDER so that the absolute path
+        # can be easily constructed here.
+        # Different versions have different awp roots. Here we just try to load the plugins
+        # from different roots.
+        possible_awp_roots = [
+            "/ansys_inc/ansys/dpf/server_2023_2_pre1",
+            "/ansys_inc/ansys/dpf/server_2023_2_pre2",
+        ]
+
+        while True:
+            awp_root_docker = possible_awp_roots.pop()
+            try:
+                _load_plugins(server, ansys_path=ansys_path, awp_root_docker=awp_root_docker)
+                return
+            except DPFServerException:
+                if len(possible_awp_roots) == 0:
+                    raise
+    else:
+        for name in _PLUGINS:
+            # Since version 7.0, the dpf load_library method can load the plugins
+            # by passing their name (as defined in the _PLUGIN variable) in place
+            # of the filename.
+            # Note greschd July '23: AFAICT, The 'name' argument needs to be unique
+            # for each plugin. Otherwise, the plugin may not be loaded if another
+            # plugin with the same name is already loaded.
+            dpf.load_library(name, name=name, server=server)
```

### Comparing `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/unit_system.py` & `ansys_dpf_composites-0.3.0/src/ansys/dpf/composites/unit_system.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b2/PKG-INFO` & `ansys_dpf_composites-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-composites
-Version: 0.2b2
+Version: 0.3.0
 Summary: A python wrapper for ansys dpf composites
-Home-page: https://github.com/pyansys/pydpf-composites
+Home-page: https://github.com/ansys/pydpf-composites
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: test
 Requires-Dist: Sphinx (>=5.0.1,<6.0.0) ; extra == "all" or extra == "docs"
 Requires-Dist: ansys-dpf-core (>=0.8,<1)
 Requires-Dist: ansys-sphinx-theme (>=0,<1) ; extra == "all" or extra == "docs"
 Requires-Dist: build (>=0.8.0,<0.9.0) ; extra == "all" or extra == "build"
-Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.8"
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
-Requires-Dist: mypy (>=0.931,<0.932) ; extra == "all" or extra == "pre-commit"
-Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0) ; extra == "all" or extra == "pre-commit"
-Requires-Dist: numpy (>=1.19,<1.22) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: numpy (>=1.22,<2.0) ; python_version >= "3.8"
+Requires-Dist: mypy (>=1.2.0,<2.0.0) ; extra == "all" or extra == "pre-commit"
+Requires-Dist: mypy-extensions (>=1.0.0,<2.0.0) ; extra == "all" or extra == "pre-commit"
+Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: numpydoc (>=1.5,<2.0) ; extra == "all" or extra == "docs"
+Requires-Dist: packaging
 Requires-Dist: pre-commit ; extra == "all" or extra == "pre-commit"
 Requires-Dist: pylint (>=2.13,<3.0) ; extra == "all" or extra == "pre-commit"
 Requires-Dist: pypandoc (>=1.8.1,<2.0.0) ; extra == "all" or extra == "docs"
 Requires-Dist: pytest (>=7.1.2,<8.0.0) ; extra == "all" or extra == "test"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "all" or extra == "test"
-Requires-Dist: pyvista (>=0.36.1,<0.37.0)
+Requires-Dist: pytest-rerunfailures (>=11.1.2,<12.0.0) ; extra == "all" or extra == "test"
+Requires-Dist: pyvista[jupyter] (>=0.36.1,<1) ; extra == "all" or extra == "docs"
+Requires-Dist: scipy (>=1.9.0) ; extra == "all" or extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints (>=1.19,<1.20.2) ; extra == "all" or extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.4,<0.5) ; extra == "all" or extra == "docs"
 Requires-Dist: sphinx-design (>=0.3.0,<0.4.0) ; extra == "all" or extra == "docs"
 Requires-Dist: sphinx_gallery (>=0.11.0,<0.12.0) ; extra == "all" or extra == "docs"
 Requires-Dist: twine (>=4.0.1,<5.0.0) ; extra == "all" or extra == "build"
-Requires-Dist: vtk
 Project-URL: Documentation, https://composites.dpf.docs.pyansys.com
-Project-URL: Repository, https://github.com/pyansys/pydpf-composites
+Project-URL: Repository, https://github.com/ansys/pydpf-composites
 Description-Content-Type: text/x-rst
 
 ****************
 PyDPF Composites
 ****************
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
+.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.8-blue
    :target: https://pypi.org/project/ansys-dpf-composites/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-dpf-composites.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-dpf-composites
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pydpf-composites/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pydpf-composites
+.. |codecov| image:: https://codecov.io/gh/ansys/pydpf-composites/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pydpf-composites
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pydpf-composites/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pydpf-composites/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pydpf-composites/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pydpf-composites/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -86,16 +84,17 @@
    :alt: Black
 
 
 PyDPF Composites is a Python wrapper for Ansys DPF composites. It implements
 classes on top of DPF Composites operators and data accessors for short
 fiber and layered composites (layered shell and solid elements). This module
 can be used to postprocess fiber reinforced plastics and layered composites and
-to implement custom failure criteria and computation. For examples demonstrating
-the behavior and usage of PyDPF Composites, see `PyDPF Composites - Examples`_.
+to implement custom failure criteria and computation. For information demonstrating
+the behavior and usage of PyDPF Composites, see `Examples`_ in the DPF Composite
+documentation.
 
 .. START_MARKER_FOR_SPHINX_DOCS
 
 ----------
 Contribute
 ----------
 
@@ -108,15 +107,15 @@
 Before attempting to contribute to PyDPF Composites, ensure that you are thoroughly
 familiar with the `PyAnsys Developer's Guide`_.
 
 #.  Clone the repository:
 
     .. code:: bash
 
-        git clone https://github.com/pyansys/pydpf-composites
+        git clone https://github.com/ansys/pydpf-composites
         cd pydpf-composites
 
 
 #.  Install dependencies:
 
     .. code:: bash
 
@@ -124,18 +123,20 @@
         pipx ensurepath
         # Minimum required poetry version is 1.2.0
         pipx install poetry
         pipx install pip
         pipx install tox
 
 
-#.  Create a virtual environment and install the package with development
-    dependencies. PyDPF Composites uses `Poetry <https://python-poetry.org>`_
+    PyDPF Composites uses `Poetry <https://python-poetry.org>`_
     to manage the development environment.
 
+#.  Create a virtual environment and install the package with the
+    development dependencies:
+
     .. code:: bash
 
         poetry install --all-extras
 
 
 #.  Activate the virtual environment:
 
@@ -143,77 +144,71 @@
 
         poetry shell
 
 
 Test
 ====
 
-.. note::
-
-   The Docker container referenced in the first option is not yet publicly available.
-
-Set the environment variable `ANSYSLMD_LICENSE_FILE` to configure the licensing or pass it
-as argument (`--license-server=1055@mylicenseserver`) to the pytest call.
-
-There are three ways to run the PyDPF Composites tests, depending on how the DPF
+There are different ways to run the PyDPF Composites tests, depending on how the DPF
 server is started.
 
-#.  Run tests with a Docker container.
+#.  Run tests with a Docker container:
+
+    Follow the steps in `Getting The DPF Server Docker Image`_ to get
+    and run the DPF docker image. Run the tests with the following command
 
     .. code:: bash
 
-        docker pull ghcr.io/pyansys/pydpf-composites:latest
-        pytest .
+        pytest . --port 50052
 
 
 #.  Run tests with a DPF server started from the Ansys installer. The Ansys version must
     be 2023 R2 or later.
 
     .. code:: bash
 
         pytest . --ansys-path "C:\Program Files\Ansys Inc\v232"
 
 
-#.  Run tests with a local gRPC server executable:
+#.  Run tests with a Docker container from Github (Ansys Internal only):
 
     .. code:: bash
 
-        pytest . --server-bin dpf_composites/bin/lib/deps/Ans.Dpf.Grpc.exe
-
-
-    This currently works only on Windows and with the directory structure of the Ansys internal
-    ``dpf_composites`` package. The runtime dependencies of the ``Ans.Dpf.Grpc.exe`` file must be
-    in its folder and the parent folder.
+        docker pull ghcr.io/ansys/pydpf-composites:latest
+        pytest .
 
 
 Build documentation
 ===================
 
-.. note::
-
-    The Docker container referenced in this section is not yet publicly available.
+Follow the description in `Getting The DPF Server Docker Image`_ image to get
+and run the dpf docker image.
 
-
-On Windows, build documentation with this code:
+On Windows, build the documentation with:
 
 .. code:: bash
 
-    docker pull ghcr.io/pyansys/pydpf-composites:latest
-    docker run -d -p 21002:50052 -e ANSYSLMD_LICENSE_FILE=10555@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/pyansys/pydpf-composites:latest
     tox -e doc-windows
 
 
-On Linux, build documentation with this code:
+On Linux, build the documentation with:
 
 .. code:: bash
 
-    docker pull ghcr.io/pyansys/pydpf-composites:latest
-    docker run -d -p 21002:50052 -e ANSYSLMD_LICENSE_FILE=10555@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/pyansys/pydpf-composites:latest
     tox -e doc-linux
 
+Ansys internal only: Build the docs with the latest container from Github:
+
+.. code:: bash
+
+    docker pull ghcr.io/ansys/pydpf-composites:latest
+    docker run -d -p 50052:50052 -e ANSYSLMD_LICENSE_FILE=1055@mylicserver -e ANSYS_DPF_ACCEPT_LA=Y ghcr.io/ansys/pydpf-composites:latest
+    tox -e doc-windows
+
+
 
 Run style checks
 ================
 
 The style checks use `pre-commit`_ and can be run through `tox`_:
 
 .. code:: bash
@@ -224,19 +219,32 @@
 The style checks can also be configured to run automatically before each ``git commit``:
 
 .. code:: bash
 
     pre-commit install
 
 
+View documentation
+-------------------
+Documentation for the latest stable release of PyDPF Composites is hosted at
+`PyDPF Composites Documentation <https://composites.dpf.docs.pyansys.com/version/stable/>`_.
+
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
+
+
+
 .. LINKS AND REFERENCES
 .. _black: https://github.com/psf/black
 .. _flake8: https://flake8.pycqa.org/en/latest/
 .. _isort: https://github.com/PyCQA/isort
 .. _pip: https://pypi.org/project/pip/
 .. _pre-commit: https://pre-commit.com/
 .. _PyAnsys Developer's Guide: https://dev.docs.pyansys.com/
 .. _pytest: https://docs.pytest.org/en/stable/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _tox: https://tox.wiki/
-.. _PyDPF Composites - Examples: https://composites.dpf.docs.pyansys.com/dev/examples/index.html
+.. _Examples: https://composites.dpf.docs.pyansys.com/dev/examples/index.html
+.. _Getting The DPF Server Docker Image: https://composites.dpf.docs.pyansys.com/version/stable/intro.html#getting-the-dpf-server-docker-image
```

