# Comparing `tmp/tequila-basic-1.8.8.tar.gz` & `tmp/tequila-basic-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tequila-basic-1.8.8.tar", last modified: Thu May 25 07:44:51 2023, max compression
+gzip compressed data, was "tequila-basic-1.8.9.tar", last modified: Thu Aug  3 20:31:12 2023, max compression
```

## Comparing `tequila-basic-1.8.8.tar` & `tequila-basic-1.8.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 07:44:50.000000 tequila-basic-1.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/tequila/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/tequila/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/_unary_state_prep_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/adapt/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/adapt/adapt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/krylov/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/krylov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/krylov/krylov.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/robustness/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/unary_state_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/autograd_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/_gates_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/pyzx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/qpic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/grouping/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/binary_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    66415 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/compile_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/ev_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32412 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/fermionic_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/fermionic_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/overlapping_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/hamiltonian/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/paulis.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/paulistring.py
--rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/qubit_hamiltonian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/interface_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/ml_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/utils_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    31763 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/qtensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    32085 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38993 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gpyopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_phoenics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/quantumchemistry/
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/chemistry_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    34407 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/madness_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/orbital_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/psi4_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/pyscf_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    86149 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/qc_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/simulators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24177 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33174 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17220 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_cirq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24240 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_pyquil.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25119 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qibo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23429 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qlm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19546 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs_gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5220 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_symbolic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/qng.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/random_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/joined_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/keymap.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila/wavefunction/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/wavefunction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/wavefunction/qubit_wavefunction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-03 20:31:10.000000 tequila-basic-1.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/_unary_state_prep_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/apps/adapt/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/adapt/adapt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/apps/krylov/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/krylov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/krylov/krylov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/apps/robustness/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/robustness/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24735 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/robustness/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/apps/unary_state_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/autograd_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.977047 tequila-basic-1.8.9/src/tequila/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/_gates_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/pyzx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/circuit/qpic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/grouping/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/binary_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66415 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/compile_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/ev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32412 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/fermionic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/fermionic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/grouping/overlapping_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/hamiltonian/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/hamiltonian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/hamiltonian/paulis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/hamiltonian/paulistring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/hamiltonian/qubit_hamiltonian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/ml/interface_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/ml/ml_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/ml/utils_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/objective/braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31763 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/objective/qtensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32272 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/optimizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38993 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/optimizer_gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/optimizer_gpyopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/optimizer_phoenics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/optimizers/optimizer_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/quantumchemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40939 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/chemistry_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/madness_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/orbital_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/psi4_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/pyscf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91623 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/quantumchemistry/qc_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.981047 tequila-basic-1.8.9/src/tequila/simulators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24172 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33174 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17220 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_cirq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24240 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_pyquil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25095 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_qibo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23429 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_qlm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19728 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_qulacs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_qulacs_gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5220 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/simulators/simulator_symbolic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/src/tequila/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/tools/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/tools/qng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/tools/random_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/src/tequila/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/joined_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/src/tequila/wavefunction/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/wavefunction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-08-03 20:30:56.000000 tequila-basic-1.8.9/src/tequila/wavefunction/qubit_wavefunction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:31:12.985047 tequila-basic-1.8.9/src/tequila_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-08-03 20:31:12.000000 tequila-basic-1.8.9/src/tequila_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-03 20:31:12.000000 tequila-basic-1.8.9/src/tequila_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:31:12.000000 tequila-basic-1.8.9/src/tequila_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 20:31:12.000000 tequila-basic-1.8.9/src/tequila_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 20:31:12.000000 tequila-basic-1.8.9/src/tequila_basic.egg-info/top_level.txt
```

### Comparing `tequila-basic-1.8.8/LICENSE` & `tequila-basic-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/PKG-INFO` & `tequila-basic-1.8.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,132 +1,63 @@
 Metadata-Version: 2.1
 Name: tequila-basic
-Version: 1.8.8
+Version: 1.8.9
 Summary: A High-Level Abstraction Framework for Quantum Algorithms
 Home-page: https://github.com/tequilahub/tequila
 Author: Jakob Kottmann and Sumner Alperin-Lea and Teresa Tamayo-Mendoza and Alba Cervera-Lierta and Cyrille Lavigne and Tzu-Ching Yen and Vladyslav Verteletskyi and Philipp Schleich and Abhinav Anand and Matthias Degroote and Skylar Chaney and Maha Kesibi and Naomi Grace Curnow and Brandon Solo and Georgios Tsilimigkounakis and Claudia Zendejas-Morales and Artur F Izmaylov and Alan Aspuru-Guzik ... 
 Author-email: jakob.kottmann@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENCE) [![DOI](https://zenodo.org/badge/259718912.svg)](https://zenodo.org/badge/latestdoi/259718912) [![PyPI version](https://badge.fury.io/py/tequila-basic.svg)](https://badge.fury.io/py/tequila-basic) ![CI](https://github.com/tequilahub/tequila/actions/workflows/ci_basic.yml/badge.svg)
 
-![Image](docs/all_in_one_example.png)
-
 # Tequila
 
 Tequila is an abstraction framework for (variational) quantum algorithms.  
 It operates on abstract data structures allowing the formulation, combination, automatic differentiation and optimization of generalized objectives.
 Tequila can execute the underlying quantum expectation values on state of the art simulators as well as on real quantum devices.  
 
-Check out this small overview to get a glimpse on [what tequila is,](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
-or, get an overview through different slides and recordings of talks on different level of detail: See [here](https://kottmanj.github.io/talks_and_material/).  
-
-Get started with our [BasicUsage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb) Tutorial or find more in the [Tutorial collection](https://github.com/aspuru-guzik-group/tequila-tutorials)  
-
-or checkout our [overview article](https://arxiv.org/abs/2011.03057)  
-
-# Quantum Backends
-Currently supported
-- [Qulacs](https://github.com/qulacs/qulacs)
-- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
-- [Qiskit](https://github.com/qiskit/qiskit)  
-- [Cirq](https://github.com/quantumlib/cirq)
-- [PyQuil](https://github.com/rigetti/pyquil)
-- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
-
-Tequila detects backends automatically if they are installed on your systems.
-All of them are available over standard pip installation like for example `pip install qulacs`.
-For best performance it is recommended to have `qulacs` installed.
-
-# QuantumChemistry:
-Currently supported
-## [Psi4](https://github.com/psi4/psi4).
-In a conda environment this can be installed with
-```bash
-conda install psi4 -c psi4
-```
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
+- [overview article](https://arxiv.org/abs/2011.03057)   
+- [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
+- [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
+- [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
+- [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
+- [talks and slides](https://kottmanj.github.io/talks_and_material/)  
+
+# Installation
+Recommended Python version is 3.8-3.9.   
+Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.
 
-## [Madness](https://github.com/kottmanj/madness)  
-In a conda environment this can be installed with  
-```bash
-conda install madtequila -c kottmann
-```  
-This installs a modified version of madness ready to use with tequila.  
-Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage.
-
-## [PySCF](https://github.com/pyscf/pyscf)  
-Install with
-```bash
-pip install pyscf
-```  
-Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
-
-# Install from source
+## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
-We recommend installing in editable mode with
-```bash
-git clone https://github.com/tequilahub/tequila.git
-cd tequila
-pip install -e .
-```
-
-You can install `tequila` directly with pip over:
-```bash
-pip install git+https://github.com/tequilahub/tequila.git
-```
-Install from devel branch (most recent updates):
-```bash
-pip install git+https://github.com/tequilahub/tequila.git@devel
-```
-
-Recommended Python version is 3.7.
-Python 3.8 works, but not all (optional) dependencies support it yet (e.g. Psi4).
-Python 3.6 works, but some (optional) dependencies might have issues with numpy >= 1.20.
-
-# Install from PyPi
-**Do not** install like this:
-<strike>`pip install tequila`</strike>
-
-this will install a Minecraft server manager (might be useful for other things, but probably not what you are looking for).
-
 You can install tequila from PyPi as:
 ```bash
 pip install tequila-basic
 ```
 this will install tequila with all essential dependencies.
 We recommend to install some fast quantum backends, like qulacs or qibo, as well.
 Those can be installed before or after you install tequila.
 ```bash
 # install basic tequila
 pip install tequila-basic
 # install qulacs and/or other backends and use it within tequila
 pip install qulacs
 ```
 
-# Install with Windows
+## Install from github 
+You can install `tequila` directly with pip over:
+```bash
+pip install git+https://github.com/tequilahub/tequila.git
+```
+Install from devel branch (most recent updates):
 ```bash
-pip install git+https://github.com/tequilahub/tequila.git@windows
+pip install git+https://github.com/tequilahub/tequila.git@devel
 ```
-See also the troubleshooting below if you want to tweak things manually.  
-The command above will not install the qulacs simulator.  
-You can install it on windows OS, but you need to have cmake and c++ compilers ready (can be installed for example over visual studio).  
-Of course you can also use one of the other backends (see above).  
-
-# Getting Started
-We have a collection of [*tutorials*](https://github.com/tequilahub/tequila-tutorials) covering basic usage of tequila as well as cutting edge research content:
-- Tutorial on [Basic Usage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb)  
-- Chemistry tutorial with psi4: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
-- Chemistry tutorial with madness: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)
-- check the list of research projects below for links to specific examples.  
-- all tutorials: [github/tequilahub/tequila-tutorials](https://github.com/tequilahub/tequila-tutorials).  
 
 ## Tequila Hello World
 ```python
 # optimize a one qubit example
 
 # define a variable
 a = tq.Variable("a")
@@ -143,21 +74,16 @@
 print("optimized wavefunction = ", wfn)
 # plot information about the optimization
 result.history.plot("energies")
 result.history.plot("angles")
 result.history.plot("gradients")
 ```
 
-## Chemistry Hello World (Madness backend)  
-Install backend as
-```bash
-conda install madtequila -c kottmann
-```  
-or see above for more.    
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)  
+## Chemistry Hello World (Madness backend)   
+see below for installation of dependencies  
 ```python
 import tequila as tq
 
 # initialize molecule (also works over .xyz files --> see next example)
 geomstring="Li 0.0 0.0 0.0\nH 0.0 0.0 1.6"
 mol = tq.Molecule(geometry=geomstring)
 
@@ -170,55 +96,48 @@
 # define the expectation value
 E = tq.ExpectationValue(H=H, U=U)
 
 # minimize the expectation value
 result = tq.minimize(E)
 
 # optional:compute classical reference energies
-# needs pyscf
+# needs pyscf as well
 cisd = mol.compute_energy("cisd")
 fci = mol.compute_energy("fci")
 
 print("VQE : {:+2.8}f".format(result.energy))
 print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 
 ```
 
 ## Chemistry Hello World (Psi4 or PySCF backend)
-install backends with
-```bash
-pip install pyscf
-# and/or
-conda install psi4 -c psi4 
-```
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
+see below for installation of dependencies  
 ```python
 # define a molecule within an active space
-active = {"a1": [1], "b1":[0]}
+active_orbitals=[1,2,5]
 molecule = tq.quantumchemistry.Molecule(geometry="lih.xyz", basis_set='6-31g', active_orbitals=active, transformation="bravyi-kitaev")
 
 # get the qubit hamiltonian
 H = molecule.make_hamiltonian()
 
 # create an k-UpCCGSD circuit of order k
-U = molecule.make_upccgsd_ansatz(order=1, include_singles=True)
+U = molecule.make_ansatz(name="UpCCGSD")
 
 # define the expectationvalue
 E = tq.ExpectationValue(H=H, U=U)
 
 # compute reference energies
 fci = molecule.compute_energy("fci")
 cisd = molecule.compute_energy("detci", options={"detci__ex_level": 2})
 
 # optimize
 result = tq.minimize(objective=E, method="BFGS", initial_values=0.0)
 
 print("VQE : {:+2.8}f".format(result.energy))
-print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 ```
 
 Do you want to create your own methods? Check out the [tutorials](https://github.com/tequilahub/tequila-tutorials)!
 
 # Some Research projects using Tequila
 J.S. Kottmann, A. Anand, A. Aspuru-Guzik.  
@@ -325,14 +244,52 @@
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
 Quantum backends are treated in the same way.
 
+## Quantum Backends
+Currently supported
+- [Qulacs](https://github.com/qulacs/qulacs) (recommended)
+- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
+- [Qiskit](https://github.com/qiskit/qiskit)  
+- [Cirq](https://github.com/quantumlib/cirq)
+- [PyQuil](https://github.com/rigetti/pyquil)
+- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
+
+Tequila detects backends automatically if they are installed on your systems.
+All of them are available over standard pip installation like for example `pip install qulacs`.
+For best performance it is recommended to have `qulacs` installed.
+
+## QuantumChemistry:
+Currently supported
+### [Psi4](https://github.com/psi4/psi4).
+In a conda environment this can be installed with
+```bash
+conda install psi4 -c psi4
+```
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
+
+### [Madness](https://github.com/kottmanj/madness)  
+In a conda environment this can be installed with  
+```bash
+conda install madtequila -c kottmann
+```  
+This installs a modified version of madness ready to use with tequila.  
+Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage. For fast performance it is recommended to not use the conda package.
+
+### [PySCF](https://github.com/pyscf/pyscf)  
+Install with
+```bash
+pip install pyscf
+```  
+Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
+
 # Documentation
 You can build the documentation by navigating to `docs` and entering `make html`.
 Open the documentation with a browser over like `firefox docs/build/html/index.html`
 Note that you will need some additional python packages like `sphinx` and `mr2` that are not explicitly listed in the requirements.txt
 
 You can also visit our prebuild online [documentation](https://tequilahub.github.io/tequila/)
 that will correspond to the github master branch
```

### Comparing `tequila-basic-1.8.8/README.md` & `tequila-basic-1.8.9/src/tequila_basic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,63 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENCE) [![DOI](https://zenodo.org/badge/259718912.svg)](https://zenodo.org/badge/latestdoi/259718912) [![PyPI version](https://badge.fury.io/py/tequila-basic.svg)](https://badge.fury.io/py/tequila-basic) ![CI](https://github.com/tequilahub/tequila/actions/workflows/ci_basic.yml/badge.svg)
+Metadata-Version: 2.1
+Name: tequila-basic
+Version: 1.8.9
+Summary: A High-Level Abstraction Framework for Quantum Algorithms
+Home-page: https://github.com/tequilahub/tequila
+Author: Jakob Kottmann and Sumner Alperin-Lea and Teresa Tamayo-Mendoza and Alba Cervera-Lierta and Cyrille Lavigne and Tzu-Ching Yen and Vladyslav Verteletskyi and Philipp Schleich and Abhinav Anand and Matthias Degroote and Skylar Chaney and Maha Kesibi and Naomi Grace Curnow and Brandon Solo and Georgios Tsilimigkounakis and Claudia Zendejas-Morales and Artur F Izmaylov and Alan Aspuru-Guzik ... 
+Author-email: jakob.kottmann@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-![Image](docs/all_in_one_example.png)
+[![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENCE) [![DOI](https://zenodo.org/badge/259718912.svg)](https://zenodo.org/badge/latestdoi/259718912) [![PyPI version](https://badge.fury.io/py/tequila-basic.svg)](https://badge.fury.io/py/tequila-basic) ![CI](https://github.com/tequilahub/tequila/actions/workflows/ci_basic.yml/badge.svg)
 
 # Tequila
 
 Tequila is an abstraction framework for (variational) quantum algorithms.  
 It operates on abstract data structures allowing the formulation, combination, automatic differentiation and optimization of generalized objectives.
 Tequila can execute the underlying quantum expectation values on state of the art simulators as well as on real quantum devices.  
 
-Check out this small overview to get a glimpse on [what tequila is,](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
-or, get an overview through different slides and recordings of talks on different level of detail: See [here](https://kottmanj.github.io/talks_and_material/).  
-
-Get started with our [BasicUsage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb) Tutorial or find more in the [Tutorial collection](https://github.com/aspuru-guzik-group/tequila-tutorials)  
-
-or checkout our [overview article](https://arxiv.org/abs/2011.03057)  
-
-# Quantum Backends
-Currently supported
-- [Qulacs](https://github.com/qulacs/qulacs)
-- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
-- [Qiskit](https://github.com/qiskit/qiskit)  
-- [Cirq](https://github.com/quantumlib/cirq)
-- [PyQuil](https://github.com/rigetti/pyquil)
-- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
-
-Tequila detects backends automatically if they are installed on your systems.
-All of them are available over standard pip installation like for example `pip install qulacs`.
-For best performance it is recommended to have `qulacs` installed.
-
-# QuantumChemistry:
-Currently supported
-## [Psi4](https://github.com/psi4/psi4).
-In a conda environment this can be installed with
-```bash
-conda install psi4 -c psi4
-```
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
-
-## [Madness](https://github.com/kottmanj/madness)  
-In a conda environment this can be installed with  
-```bash
-conda install madtequila -c kottmann
-```  
-This installs a modified version of madness ready to use with tequila.  
-Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage.
-
-## [PySCF](https://github.com/pyscf/pyscf)  
-Install with
-```bash
-pip install pyscf
-```  
-Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
+- [overview article](https://arxiv.org/abs/2011.03057)   
+- [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
+- [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
+- [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
+- [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
+- [talks and slides](https://kottmanj.github.io/talks_and_material/)  
+
+# Installation
+Recommended Python version is 3.8-3.9.   
+Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.
 
-# Install from source
+## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
-We recommend installing in editable mode with
-```bash
-git clone https://github.com/tequilahub/tequila.git
-cd tequila
-pip install -e .
-```
-
-You can install `tequila` directly with pip over:
-```bash
-pip install git+https://github.com/tequilahub/tequila.git
-```
-Install from devel branch (most recent updates):
-```bash
-pip install git+https://github.com/tequilahub/tequila.git@devel
-```
-
-Recommended Python version is 3.7.
-Python 3.8 works, but not all (optional) dependencies support it yet (e.g. Psi4).
-Python 3.6 works, but some (optional) dependencies might have issues with numpy >= 1.20.
-
-# Install from PyPi
-**Do not** install like this:
-<strike>`pip install tequila`</strike>
-
-this will install a Minecraft server manager (might be useful for other things, but probably not what you are looking for).
-
 You can install tequila from PyPi as:
 ```bash
 pip install tequila-basic
 ```
 this will install tequila with all essential dependencies.
 We recommend to install some fast quantum backends, like qulacs or qibo, as well.
 Those can be installed before or after you install tequila.
 ```bash
 # install basic tequila
 pip install tequila-basic
 # install qulacs and/or other backends and use it within tequila
 pip install qulacs
 ```
 
-# Install with Windows
+## Install from github 
+You can install `tequila` directly with pip over:
+```bash
+pip install git+https://github.com/tequilahub/tequila.git
+```
+Install from devel branch (most recent updates):
 ```bash
-pip install git+https://github.com/tequilahub/tequila.git@windows
+pip install git+https://github.com/tequilahub/tequila.git@devel
 ```
-See also the troubleshooting below if you want to tweak things manually.  
-The command above will not install the qulacs simulator.  
-You can install it on windows OS, but you need to have cmake and c++ compilers ready (can be installed for example over visual studio).  
-Of course you can also use one of the other backends (see above).  
-
-# Getting Started
-We have a collection of [*tutorials*](https://github.com/tequilahub/tequila-tutorials) covering basic usage of tequila as well as cutting edge research content:
-- Tutorial on [Basic Usage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb)  
-- Chemistry tutorial with psi4: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
-- Chemistry tutorial with madness: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)
-- check the list of research projects below for links to specific examples.  
-- all tutorials: [github/tequilahub/tequila-tutorials](https://github.com/tequilahub/tequila-tutorials).  
 
 ## Tequila Hello World
 ```python
 # optimize a one qubit example
 
 # define a variable
 a = tq.Variable("a")
@@ -133,21 +74,16 @@
 print("optimized wavefunction = ", wfn)
 # plot information about the optimization
 result.history.plot("energies")
 result.history.plot("angles")
 result.history.plot("gradients")
 ```
 
-## Chemistry Hello World (Madness backend)  
-Install backend as
-```bash
-conda install madtequila -c kottmann
-```  
-or see above for more.    
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)  
+## Chemistry Hello World (Madness backend)   
+see below for installation of dependencies  
 ```python
 import tequila as tq
 
 # initialize molecule (also works over .xyz files --> see next example)
 geomstring="Li 0.0 0.0 0.0\nH 0.0 0.0 1.6"
 mol = tq.Molecule(geometry=geomstring)
 
@@ -160,55 +96,48 @@
 # define the expectation value
 E = tq.ExpectationValue(H=H, U=U)
 
 # minimize the expectation value
 result = tq.minimize(E)
 
 # optional:compute classical reference energies
-# needs pyscf
+# needs pyscf as well
 cisd = mol.compute_energy("cisd")
 fci = mol.compute_energy("fci")
 
 print("VQE : {:+2.8}f".format(result.energy))
 print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 
 ```
 
 ## Chemistry Hello World (Psi4 or PySCF backend)
-install backends with
-```bash
-pip install pyscf
-# and/or
-conda install psi4 -c psi4 
-```
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
+see below for installation of dependencies  
 ```python
 # define a molecule within an active space
-active = {"a1": [1], "b1":[0]}
+active_orbitals=[1,2,5]
 molecule = tq.quantumchemistry.Molecule(geometry="lih.xyz", basis_set='6-31g', active_orbitals=active, transformation="bravyi-kitaev")
 
 # get the qubit hamiltonian
 H = molecule.make_hamiltonian()
 
 # create an k-UpCCGSD circuit of order k
-U = molecule.make_upccgsd_ansatz(order=1, include_singles=True)
+U = molecule.make_ansatz(name="UpCCGSD")
 
 # define the expectationvalue
 E = tq.ExpectationValue(H=H, U=U)
 
 # compute reference energies
 fci = molecule.compute_energy("fci")
 cisd = molecule.compute_energy("detci", options={"detci__ex_level": 2})
 
 # optimize
 result = tq.minimize(objective=E, method="BFGS", initial_values=0.0)
 
 print("VQE : {:+2.8}f".format(result.energy))
-print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 ```
 
 Do you want to create your own methods? Check out the [tutorials](https://github.com/tequilahub/tequila-tutorials)!
 
 # Some Research projects using Tequila
 J.S. Kottmann, A. Anand, A. Aspuru-Guzik.  
@@ -315,14 +244,52 @@
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
 Quantum backends are treated in the same way.
 
+## Quantum Backends
+Currently supported
+- [Qulacs](https://github.com/qulacs/qulacs) (recommended)
+- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
+- [Qiskit](https://github.com/qiskit/qiskit)  
+- [Cirq](https://github.com/quantumlib/cirq)
+- [PyQuil](https://github.com/rigetti/pyquil)
+- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
+
+Tequila detects backends automatically if they are installed on your systems.
+All of them are available over standard pip installation like for example `pip install qulacs`.
+For best performance it is recommended to have `qulacs` installed.
+
+## QuantumChemistry:
+Currently supported
+### [Psi4](https://github.com/psi4/psi4).
+In a conda environment this can be installed with
+```bash
+conda install psi4 -c psi4
+```
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
+
+### [Madness](https://github.com/kottmanj/madness)  
+In a conda environment this can be installed with  
+```bash
+conda install madtequila -c kottmann
+```  
+This installs a modified version of madness ready to use with tequila.  
+Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage. For fast performance it is recommended to not use the conda package.
+
+### [PySCF](https://github.com/pyscf/pyscf)  
+Install with
+```bash
+pip install pyscf
+```  
+Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
+
 # Documentation
 You can build the documentation by navigating to `docs` and entering `make html`.
 Open the documentation with a browser over like `firefox docs/build/html/index.html`
 Note that you will need some additional python packages like `sphinx` and `mr2` that are not explicitly listed in the requirements.txt
 
 You can also visit our prebuild online [documentation](https://tequilahub.github.io/tequila/)
 that will correspond to the github master branch
```

### Comparing `tequila-basic-1.8.8/requirements.txt` & `tequila-basic-1.8.9/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # necessary
 numpy
-scipy >= 1.5 # can in principle be smaller, we recommend >= 1.5 for consistency with our tutorials (numerical gradients mostly)
+scipy < 1.11 # for now, until issues with scipy/pyscf are fixed # can in principle be smaller, we recommend >= 1.5 for consistency with our tutorials (numerical gradients mostly)
 sympy
 #jax
 #jaxlib
 autograd # autograd works better on OSX-ARM64 (M1 and M2) and Windows, feel free to try jax however (no big differences)
 setuptools
 pytest
 openfermion ~= 1.0 # can not be smaller than 1.0 
 #cmake # needed by #qulacs, can be removed otherwise, now in #qulacs requirements
-#qulacs < 0.5.0 # default simulator (best integration), remove if the installation gives you trouble and just install one of the other supported backend. Version restriction only for noise models, otherwise the new version is fine
+#qulacs # default simulator (best integration), remove if the installation gives you trouble and just install one of the other supported backend. Version restriction only for noise models, otherwise the new version is fine
 
 #optional quantum backends
 #cirq >= 0.9.2 #
 #qiskit>=0.30
 #pyquil<3.0 # you also need to install the forest-sdk
 ##qulacs-gpu # you can't have #qulacs and #qulacs-gpu at the same time
 #qibo <= 0.1.1 # can not be installed in the same environment as gpyopt
```

### Comparing `tequila-basic-1.8.8/setup.py` & `tequila-basic-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/__init__.py` & `tequila-basic-1.8.9/src/tequila/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/__init__.py` & `tequila-basic-1.8.9/src/tequila/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/_unary_state_prep_impl.py` & `tequila-basic-1.8.9/src/tequila/apps/_unary_state_prep_impl.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/adapt/adapt.py` & `tequila-basic-1.8.9/src/tequila/apps/adapt/adapt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/krylov/krylov.py` & `tequila-basic-1.8.9/src/tequila/apps/krylov/krylov.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/robustness/helpers.py` & `tequila-basic-1.8.9/src/tequila/apps/robustness/helpers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/apps/robustness/interval.py` & `tequila-basic-1.8.9/src/tequila/apps/robustness/interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             min_eigval = min(p_eigvals)
             max_eigval = max(p_eigvals)
 
             if str(p_str) == 'I' or len(p_str) == 0:
                 pauli_lower_bound = pauli_upper_bound = 1.0
             else:
                 expec_normalized = np.clip(2 * (p_expec - min_eigval) / (max_eigval - min_eigval) - 1, -1, 1,
-                                           dtype=np.float64)
+                                           dtype=float)
 
                 pauli_lower_bound = (max_eigval - min_eigval) / 2.0 * (
                         1 + self._calc_lower_bound(expec_normalized, self.fidelity)) + min_eigval
 
                 pauli_upper_bound = (max_eigval - min_eigval) / 2.0 * (
                         1 + self._calc_upper_bound(expec_normalized, self.fidelity)) + min_eigval
 
@@ -333,15 +333,15 @@
 
     def _compute_bound_grouped(self) -> float:
         bound = 0.0
 
         for eigvals, expec, variance in zip(self._pauligroups_eigenvalues, self._pauligroups_expectations,
                                             self._pauligroups_variances):
             min_eigval = min(eigvals)
-            expec_pos = np.clip(expec - min_eigval, 0, None, dtype=np.float)
+            expec_pos = np.clip(expec - min_eigval, 0, None, dtype=float)
             bound += min_eigval + self._calc_lower_bound(expec_pos, variance, self.fidelity)
 
         return bound
 
     def _compute_expectation(self, group_tems) -> Union[float, RealNumber]:
         if group_tems:
             return float(np.dot(self._pauligroups_coeffs, self._pauligroups_expectations))
```

### Comparing `tequila-basic-1.8.8/src/tequila/apps/unary_state_prep.py` & `tequila-basic-1.8.9/src/tequila/apps/unary_state_prep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/autograd_imports.py` & `tequila-basic-1.8.9/src/tequila/autograd_imports.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/_gates_impl.py` & `tequila-basic-1.8.9/src/tequila/circuit/_gates_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,26 +176,26 @@
 
     @parameter.setter
     def parameter(self, other):
         self._parameter = assign_variable(variable=other)
 
     def __init__(self, name, parameter: UnionParam, target: UnionList, control: UnionList = None,
                 generator: QubitHamiltonian = None):
-        super().__init__(name=name, target=target, control=control, generator=generator)
         # failsafe
         if hasattr(parameter, "shape") and parameter.shape not in [tuple()]: # take care of new numpy conventions where scalars have shape ()
+            self._parameter=None
             raise TequilaException("parameter has to be a scalar. Received {}\n{}\n{}".format(repr(parameter), type(parameter), str(parameter)))
         self._parameter = assign_variable(variable=parameter)
+        super().__init__(name=name, target=target, control=control, generator=generator)
 
     def __str__(self):
         result = str(self.name) + "(target=" + str(self.target)
         if not self.is_single_qubit_gate():
             result += ", control=" + str(self.control)
-
-        result += ", parameter=" + repr(self._parameter)
+        result += ", parameter=" + repr(self.parameter)
         result += ")"
         return result
 
     def __eq__(self, other):
         if not isinstance(other, ParametrizedGateImpl):
             return False
         if not super().__eq__(other):
```

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/circuit.py` & `tequila-basic-1.8.9/src/tequila/circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/compiler.py` & `tequila-basic-1.8.9/src/tequila/circuit/compiler.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/gates.py` & `tequila-basic-1.8.9/src/tequila/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/gradient.py` & `tequila-basic-1.8.9/src/tequila/circuit/gradient.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/noise.py` & `tequila-basic-1.8.9/src/tequila/circuit/noise.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/pyzx.py` & `tequila-basic-1.8.9/src/tequila/circuit/pyzx.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/qasm.py` & `tequila-basic-1.8.9/src/tequila/circuit/qasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,22 +398,27 @@
         try:
             phase = float(angle)
         except ValueError:
             if angle.find('pi') == -1:
                 raise TequilaException("Invalid specification {}".format(name))
             angle = angle.replace('pi', '')
             try:
+                sign = 1
+                div = 1
+                if angle.find('-') != -1:
+                    angle = angle.replace('-', '')
+                    sign = -1
+                if angle.find('/') != -1:
+                    div = float(angle[angle.index('/')+1:])
+                    angle = angle[:angle.index('/')]
                 if angle.find('*') != -1:
                     angle = angle.replace('*', '')
-                    phase = float(angle) * pi
-                elif angle.find('/') != -1:
-                    angle = angle.replace('/', '')
-                    phase = pi / float(angle)
+                    phase = sign * float(angle) * pi / div
                 elif len(angle) == 0:
-                    phase = pi
+                    phase = sign * pi / div
                 else:
-                    phase = float(angle)
+                    phase = sign * float(angle) / div
             except ValueError:
                 raise TequilaException("Invalid specification {}".format(name))
         angles.append(phase)
     return angles
```

### Comparing `tequila-basic-1.8.8/src/tequila/circuit/qpic.py` & `tequila-basic-1.8.9/src/tequila/circuit/qpic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/binary_rep.py` & `tequila-basic-1.8.9/src/tequila/grouping/binary_rep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/binary_utils.py` & `tequila-basic-1.8.9/src/tequila/grouping/binary_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/compile_groups.py` & `tequila-basic-1.8.9/src/tequila/grouping/compile_groups.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/ev_utils.py` & `tequila-basic-1.8.9/src/tequila/grouping/ev_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/fermionic_functions.py` & `tequila-basic-1.8.9/src/tequila/grouping/fermionic_functions.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/fermionic_methods.py` & `tequila-basic-1.8.9/src/tequila/grouping/fermionic_methods.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/grouping/overlapping_methods.py` & `tequila-basic-1.8.9/src/tequila/grouping/overlapping_methods.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/hamiltonian/paulis.py` & `tequila-basic-1.8.9/src/tequila/hamiltonian/paulis.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/hamiltonian/qubit_hamiltonian.py` & `tequila-basic-1.8.9/src/tequila/hamiltonian/qubit_hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
         Returns
         -------
             Hermitian and anti-Hermitian part as tuple
         """
         hermitian = QubitHamiltonian.zero()
         anti_hermitian = QubitHamiltonian.zero()
         for k, v in self.qubit_operator.terms.items():
-            hermitian.qubit_operator.terms[k] = np.float(v.real)
+            hermitian.qubit_operator.terms[k] = v.real
             anti_hermitian.qubit_operator.terms[k] = 1.j * v.imag
 
         return hermitian.simplify(), anti_hermitian.simplify()
 
     def is_antihermitian(self):
         for v in self.values():
             if v.real != 0.0:
```

### Comparing `tequila-basic-1.8.8/src/tequila/ml/interface_torch.py` & `tequila-basic-1.8.9/src/tequila/ml/interface_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             # build up weight and input gradient matrices... see what needs to be done to them.
             grad_outs = [None,None]
             for i, grads in enumerate([i_grads, w_grads]):
                 if grads != {}:
                     g_keys = [j for j in grads.keys()]
                     probe = grads[g_keys[0]]  # first entry will tell us number of output
                     dims = len(g_keys), len(probe)
-                    arr = np.empty(dims, dtype=np.float)
+                    arr = np.empty(dims, dtype=float)
                     for j, key in enumerate(g_keys):
                         line = grads[key]
                         for k, ob in enumerate(line):
                             arr[j, k] = ob(variables=call_args, samples=samples)
                     if back_d >= 0:
                         g_tensor = torch.as_tensor(arr, dtype=grad_backward.dtype, device=back_d)
                     else:
```

### Comparing `tequila-basic-1.8.8/src/tequila/ml/ml_api.py` & `tequila-basic-1.8.9/src/tequila/ml/ml_api.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/ml/utils_ml.py` & `tequila-basic-1.8.9/src/tequila/ml/utils_ml.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/objective/braket.py` & `tequila-basic-1.8.9/src/tequila/objective/braket.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/objective/objective.py` & `tequila-basic-1.8.9/src/tequila/objective/objective.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/objective/qtensor.py` & `tequila-basic-1.8.9/src/tequila/objective/qtensor.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/__init__.py` & `tequila-basic-1.8.9/src/tequila/optimizers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     -------
 
     """
 
     ovtmp=objective.extract_variables()
     fast_return=False
     if ovtmp is None or len(ovtmp) == 0:
-        return OptimizerResults(energy=numpy.float(simulate(objective, *args, **kwargs)), variables={}, history=OptimizerHistory())
+        return OptimizerResults(energy=float(simulate(objective, *args, **kwargs)), variables={}, history=OptimizerHistory())
 
     for k, v in INSTALLED_OPTIMIZERS.items():
         if method.lower() in v.methods or method.upper() in v.methods:
             return v.minimize(
                 objective=objective,
                 method=method,
                 variables=variables,
```

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/_containers.py` & `tequila-basic-1.8.9/src/tequila/optimizers/_containers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_base.py` & `tequila-basic-1.8.9/src/tequila/optimizers/optimizer_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,26 @@
 
     # history of all true iterations (epochs)
     energies: typing.List[numbers.Real] = field(default_factory=list)
     gradients: typing.List[typing.Dict[str, numbers.Real]] = field(default_factory=list)
     angles: typing.List[typing.Dict[str, numbers.Number]] = field(default_factory=list)
 
     # history of all function evaluations
-    energies_calls: typing.List[numbers.Real] = field(default_factory=list)
-    gradients_calls: typing.List[typing.Dict[str, numbers.Real]] = field(default_factory=list)
+    energy_calls: typing.List[numbers.Real] = field(default_factory=list)
+    gradient_calls: typing.List[typing.Dict[str, numbers.Real]] = field(default_factory=list)
     angles_calls: typing.List[typing.Dict[str, numbers.Number]] = field(default_factory=list)
-
+    
+    # backward comp.
+    @property
+    def energies_calls(self):
+        return self.energy_calls
+    @property
+    def energies_evaluations(self):
+        return self.energy_calls
+    
     def __add__(self, other):
         """
         magic method for convenient combination of history objects.
         """
         result = OptimizerHistory()
         result.energies = self.energies + other.energies
         result.gradients = self.gradients + other.gradients
```

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gd.py` & `tequila-basic-1.8.9/src/tequila/optimizers/optimizer_gd.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gpyopt.py` & `tequila-basic-1.8.9/src/tequila/optimizers/optimizer_gpyopt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_phoenics.py` & `tequila-basic-1.8.9/src/tequila/optimizers/optimizer_phoenics.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_scipy.py` & `tequila-basic-1.8.9/src/tequila/optimizers/optimizer_scipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,23 +271,23 @@
 
         # failsafe since callback is not implemented everywhere
         if callback.real_iterations == 0:
             real_iterations = range(len(E.history))
 
         if self.save_history:
             self.history.energies = callback.energies
-            self.history.energy_evaluations = E.history
+            self.history.energy_calls = E.history
             self.history.angles = callback.angles
-            self.history.angles_evaluations = E.history_angles
+            self.history.angles_calls = E.history_angles
             self.history.gradients = callback.gradients
             self.history.hessians = callback.hessians
             if dE is not None and not isinstance(dE, str):
-                self.history.gradients_evaluations = dE.history
+                self.history.gradient_calls = dE.history
             if ddE is not None and not isinstance(ddE, str):
-                self.history.hessians_evaluations = ddE.history
+                self.history.hessian_calls = ddE.history
 
             # some methods like "cobyla" do not support callback functions
             if len(self.history.energies) == 0:
                 self.history.energies = E.history
                 self.history.angles = E.history_angles
 
         # some scipy methods always give back the last value and not the minimum (e.g. cobyla)
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/__init__.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/chemistry_tools.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/chemistry_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -799,15 +799,15 @@
     Manage Basis Integrals of Quantum Chemistry
     All integrals are held in their original basis, the corresponding mo-coefficients have to be passed down
     and are usually held by the QuantumChemistryBaseClass
     """
     _overlap_integrals: numpy.ndarray = None
     _one_body_integrals: numpy.ndarray = None
     _two_body_integrals: NBodyTensor = None
-    _constant_term: numpy.float = None
+    _constant_term: float = None
     _basis_type: str = "unknown"
     _basis_name: str = "unknown"
     _orbital_type: str = "unknown" # e.g. "HF", "PNO", "native"
     _orbital_coefficients: numpy.ndarray = None
     _active_space: ActiveSpaceData = None
     _orbitals: typing.List[OrbitalData] = None
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/encodings.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/encodings.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,23 @@
                  "ReorderedBravyiKitaev": lambda **kwargs: BravyiKitaev(up_then_down=True, **kwargs),
                  "ReorderedBravyiKitaevTree": lambda **kwargs: BravyiKitaevTree(up_then_down=True, **kwargs),
                  }
     return {k.replace("_","").replace("-","").upper():v for k,v in encodings.items()}
 
 class EncodingBase:
 
+    # true if the encoding is fully integrated
+    # false: can only do special things (like building the Hamiltionian)
+    # but is not consistent with UCC gate generation
+    _ucc_support=False
+
+    @property
+    def supports_ucc(self):
+        return self._ucc_support
+
     @property
     def name(self):
         prefix=""
         if self.up_then_down:
             prefix="Reordered"
         if hasattr(self, "_name"):
             return prefix+self._name
@@ -125,14 +134,15 @@
     def __str__(self):
         return type(self).__name__
 
 class JordanWigner(EncodingBase):
     """
     OpenFermion::jordan_wigner
     """
+    _ucc_support=True
 
     def do_transform(self, fermion_operator:openfermion.FermionOperator, *args, **kwargs) -> openfermion.QubitOperator:
         return openfermion.jordan_wigner(fermion_operator, *args, **kwargs)
 
     def map_state(self, state:list, *args, **kwargs):
         state = state + [0]*(self.n_orbitals-len(state))
         result = [0]*len(state)
@@ -148,39 +158,48 @@
         return U
 
 class BravyiKitaev(EncodingBase):
     """
     Uses OpenFermion::bravyi_kitaev
     """
 
+    _ucc_support=True
+
     def do_transform(self, fermion_operator:openfermion.FermionOperator, *args, **kwargs) -> openfermion.QubitOperator:
         return openfermion.bravyi_kitaev(fermion_operator, n_qubits=self.n_orbitals*2)
 
 
 class BravyiKitaevTree(EncodingBase):
     """
     Uses OpenFermion::bravyi_kitaev_tree
     """
 
+    _ucc_support=True
+
     def do_transform(self, fermion_operator:openfermion.FermionOperator, *args, **kwargs) -> openfermion.QubitOperator:
         return openfermion.bravyi_kitaev_tree(fermion_operator, n_qubits=self.n_orbitals*2)
 
 class BravyiKitaevFast(EncodingBase):
     """
     Uses OpenFermion::bravyi_kitaev_tree
     """
 
+    _ucc_support=False
+
     def do_transform(self, fermion_operator:openfermion.FermionOperator, *args, **kwargs) -> openfermion.QubitOperator:
         n_qubits = openfermion.count_qubits(fermion_operator)
         if n_qubits != self.n_orbitals*2:
             raise Exception("BravyiKitaevFast transformation currently only possible for full Hamiltonians (no UCC generators).\nfermion_operator was {}".format(fermion_operator))
         op = openfermion.get_interaction_operator(fermion_operator)
         return openfermion.bravyi_kitaev_fast(op)
 
 class TaperedBravyKitaev(EncodingBase):
+
+    _ucc_support=False
+
     """
     Uses OpenFermion::symmetry_conserving_bravyi_kitaev (tapered bravyi_kitaev_tree arxiv:1701.07072)
     Reduces Hamiltonian by 2 qubits
     See OpenFermion Documentation for more
     Does not work for UCC generators yet
     """
     def __init__(self, n_electrons, n_orbitals, active_fermions=None, active_orbitals=None, *args, **kwargs):
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/madness_interface.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/madness_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,55 @@
         executable = shutil.which("pno_integrals")
         if madness_root_dir is None:
             madness_root_dir = str(os.environ.get("MAD_ROOT_DIR"))
         if executable is None and madness_root_dir is not None:
             executable = shutil.which("{}/src/apps/pno/pno_integrals".format(madness_root_dir))
         return executable
 
+    def plot2cube(self, orbital, filename=None, *args, **kwargs):
+        """
+        plot orbitals to cube file (needs madtequila backend installed)
+        Parameters
+        ----------
+        method: orbital, the orbital index (starting from 0 on the active orbitals)
+                if you want to plot frozen orbitals you can hand in a Tequila Orbital structure with idx_total defined
+        filename: name of the cubefile (default: mra_orbital_X.cube where X is the total index of the active orbital)
+        args: further arguments for plot2cube
+        kwargs further keyword arguments for plot2cube
+
+        see here for more https://github.com/kottmanj/madness/tree/tequila/src/apps/plot
+        """
+
+        plot2cube = shutil.which("plot2cube")
+        if plot2cube is None:
+            raise TequilaMadnessException(
+                "can't plot to cube file. Couldn't find plot2cube executable.\n\nTry installing\n\t conda install madtequila -c kottmann\nand assure the version is >2.3")
+
+        if hasattr(orbital,"idx"):
+            idx = orbital.idx
+        else:
+            idx = self.orbitals[orbital].idx_total
+
+        callist = [plot2cube, "file=mra_orbital_{}".format(idx)]
+
+        if filename is not None:
+            callist.append("outfile={}".format(filename))
+        for k, v in kwargs.items():
+            callist.append("{}={}".format(k, v))
+        for k in args:
+            callist.append("{}".format(k))
+
+        import subprocess
+        try:
+            with open("plot2cube_{}.log".format(orbital), "w") as logfile:
+                subprocess.call(callist, stdout=logfile)
+        except:
+            print("plotting failed ....")
+            print("see plot2cube_{}.log".format(orbital))
+
     def __init__(self, parameters: ParametersQC,
                  transformation: typing.Union[str, typing.Callable] = None,
                  active_orbitals: list = "auto",
                  executable: str = None,
                  n_pno: int = None,
                  n_virt: int = 0,
                  keep_mad_files=False,
@@ -89,36 +130,38 @@
                 self.parameters = parameters
                 status += "madness="
                 madness_status = self.run_madness(*args, **kwargs)
                 if int(madness_status) != 0:
                     warnings.warn("MADNESS did not terminate as expected! status = {}".format(status), TequilaWarning)
                 status += str(madness_status) + "\n"
             except Exception as E:
-                status += "madness_run={}\n".format(str(E))
+                status += str(E) + "\n"
 
             # will read the binary files, convert them and save them with the right name
-            h, g, pinfo= self.convert_madness_output_from_bin_to_npy(name=name, datadir=datadir)
+            h, g, pinfo = self.convert_madness_output_from_bin_to_npy(name=name, datadir=datadir)
             status += "found {}_htensor.npy={}\n".format(name, "failed" not in h)
             status += "found {}_gtensor.npy={}\n".format(name, "failed" not in g)
             status += "found {}_pnoinfo.txt={}\n".format(name, "failed" not in pinfo)
             status += "h_tensor report:\n"
             status += str(h)
             status += "g_tensor report:\n"
             status += str(g)
             status += "pnoinfo report:\n"
             status += str(pinfo)
+
+            solution = "Solution 1: Assuming precomputed files are available:\n    provide {name}_gtensor.npy, {name}_htensor.npy and {name}_pnoinfo.txt\n    and call the Molecule constructor with n_pno='read' keyword \n\nSolution 2: Try installing with conda\n    conda install madtequila -c kottmann\n\nSolution 3: Install from source\n    follow instructions on github.com/kottmanj/madness".format(
+                name=name)
+            if self.executable is not None:
+                solution = "madness executable was found, but calculation did not succeed, check {name}_pno_integrals.out for clues".format(
+                    name=name)
+
             if "failed" in h or "failed" in g:
                 raise TequilaMadnessException("Could not initialize the madness interface\n"
                                               "Status report is\n"
-                                              "{status}\n"
-                                              "either provide {name}_gtensor.npy and {name}_htensor.npy files\n"
-                                              "or provide the number of pnos over by giving the n_pnos keyword to run madness\n"
-                                              "in order for madness to run you need to make sure that the pno_integrals executable can be found in your environment\n"
-                                              "alternatively you can provide the path to the madness_root_dir: the directory where you compiled madness\n".format(
-                    name=name, status=status))
+                                              "{status}\n\n".format(status=status) + solution)
         # get additional information from madness file
         nuclear_repulsion = 0.0
         pairinfo = None
         occinfo = None
         path = parameters.name
         if datadir is not None:
             path = "{}/{}".format(datadir, path)
@@ -138,20 +181,20 @@
                 if pairinfo is not None:
                     break
             except:
                 continue
 
         if pairinfo is None:
             raise TequilaMadnessException("Pairinfo from madness calculation not found\nPlease provide pnoinfo.txt")
-        
+
         n_orbitals_total = h.shape[0]
         if "n_orbitals" in kwargs:
             # this would be the active orbitals
             kwargs.pop("n_orbitals")
-            
+
         assert h.shape[1] == n_orbitals_total
         assert sum(g.shape) == 4 * n_orbitals_total
         assert len(g.shape) == 4
         assert len(h.shape) == 2
 
         g = NBodyTensor(elems=g, ordering='mulliken')
 
@@ -215,16 +258,15 @@
                 if warn:
                     warnings.warn("Found file {} from previous calculation ... deleting it".format(filename),
                                   TequilaWarning)
                 os.remove(filename)
 
     def run_madness(self, *args, **kwargs):
         if self.executable is None:
-            return "pno_integrals executable not found\n" \
-                   "pass over executable keyword or export MAD_ROOT_DIR to system environment"
+            return "\n\n----> pno_integrals executable not found <----\n\n"
         self.write_madness_input(n_pno=self.n_pno, n_virt=self.n_virt, *args, **kwargs)
 
         # prevent reading in old files
         self.cleanup(warn=True, delete_all_files=True)
 
         import subprocess
         import time
@@ -488,23 +530,27 @@
                     idx = self.format_excitation_indices([(x.idx, a.idx)])
                     U += gates.Ry(angle=(idx, "D", label), target=a.idx, control=c[0])
                     U += gates.X(target=c[1], control=a.idx)
                     if hasattr(direct_compiling, "lower") and direct_compiling.lower() == "ladder":
                         c = [a.idx, a.idx]
                     else:
                         c = [x.idx, x.idx]
+
+            alpha_map = {k.idx: self.transformation.up(k.idx) for k in self.orbitals}
+            U = U.map_qubits(alpha_map)
         else:
             for x in pairs:
                 if include_reference:
-                    U += gates.X(x.idx)
+                    U += gates.X(self.transformation.up(x.idx))
                 for a in self.get_pair_orbitals(i=x, j=x):
                     if x == a:
                         continue
                     idx = self.format_excitation_indices([(x.idx, a.idx)])
                     U += self.make_hardcore_boson_excitation_gate(indices=idx, angle=(idx, "D", label))
+
         return U
 
     def make_upccgsd_indices(self, label=None, name="UpCCGD", exclude: list = None, *args, **kwargs):
         """
         :param label: label the angles
         :param generalized: if true the complement to UpCCGD is created (otherwise UpCCD)
         :param exclude: list of indices to exclude
@@ -608,26 +654,28 @@
             # only count active electrons (will not compute pnos for frozen pairs)
             n_core_electrons = self.parameters.get_number_of_core_electrons()
             n_electrons -= n_core_electrons
 
         n_pairs = n_electrons // 2
         if n_orbitals is None:
             n_orbitals = n_electrons  # minimal correlated (each active pair will have one virtual)
-        
+
         if n_pno is None:
             n_pno = n_orbitals - n_pairs
 
         if maxrank is None:
             # need at least maxrank=1, otherwise no PNOs are computed
             # this was a bug in <=v1.8.5 
-            maxrank = max(1,int(numpy.ceil(n_pno // n_pairs)))
-        
-        if maxrank<=0:
-            warnings.warn("maxrank={} in tequila madness backend! No PNOs will be computed. Set the value when initializing the Molecule as tq.Molecule(..., pno={\"maxrank\":1, ...})".format(maxrank), TequilaWarning)
-        
+            maxrank = max(1, int(numpy.ceil(n_pno // n_pairs)))
+
+        if maxrank <= 0:
+            warnings.warn(
+                "maxrank={} in tequila madness backend! No PNOs will be computed. Set the value when initializing the Molecule as tq.Molecule(..., pno={\"maxrank\":1, ...})".format(
+                    maxrank), TequilaWarning)
+
         data = {}
         if self.parameters.multiplicity != 1:
             raise TequilaMadnessException(
                 "Currently only closed shell supported for MRA-PNO-MP2, you demanded multiplicity={} for the surrogate".format(
                     self.parameters.multiplicity))
         data["dft"] = {"charge": self.parameters.charge, "xc": "hf", "k": 7, "econv": 1.e-4, "dconv": 5.e-4,
                        "localize": "boys",
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/orbital_optimizer.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/orbital_optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,26 +33,27 @@
         # use as callback
         if "u" in local_data:
             self.rotation_matrix = copy.deepcopy(local_data["u"])
         self.mcscf_local_data=local_data
         self.iterations += 1
 
 def optimize_orbitals(molecule, circuit=None, vqe_solver=None, pyscf_arguments=None, silent=False,
-                      vqe_solver_arguments=None, initial_guess=None, return_mcscf=False, *args, **kwargs):
+                      vqe_solver_arguments=None, initial_guess=None, return_mcscf=False, use_hcb=False, *args, **kwargs):
     """
 
     Parameters
     ----------
     molecule: The tequila molecule whose orbitals are to be optimized
     circuit: The circuit that defines the ansatz to the wavefunction in the VQE
              can be None, if a customized vqe_solver is passed that can construct a circuit
     vqe_solver: The VQE solver (the default - vqe_solver=None - will take the given circuit and construct an expectationvalue out of molecule.make_hamiltonian and the given circuit)
                 A customized object can be passed that needs to be callable with the following signature: vqe_solver(H=H, circuit=self.circuit, molecule=molecule, **self.vqe_solver_arguments)
     pyscf_arguments: Arguments for the MCSCF structure of PySCF, if None, the defaults are {"max_cycle_macro":10, "max_cycle_micro":3} (see here https://pyscf.org/pyscf_api_docs/pyscf.mcscf.html)
     silent: silence printout
+    use_hcb: indicate if the circuit is in hardcore Boson encoding
     vqe_solver_arguments: Optional arguments for a customized vqe_solver or the default solver
                           for the default solver: vqe_solver_arguments={"optimizer_arguments":A, "restrict_to_hcb":False} where A holds the kwargs for tq.minimize
                           restrict_to_hcb keyword controls if the standard (in whatever encoding the molecule structure has) Hamiltonian is constructed or the hardcore_boson hamiltonian
     initial_guess: Initial guess for the MCSCF module of PySCF (Matrix of orbital rotation coefficients)
                    The default (None) is a unit matrix
                    predefined commands are
                         initial_guess="random"
@@ -82,14 +83,24 @@
     mc = mcscf.CASSCF(mf, pyscf_molecule.n_orbitals, pyscf_molecule.n_electrons)
     mc.callback=result
     c = pyscf_molecule.compute_constant_part()
 
     if circuit is None and vqe_solver is None:
         raise Exception("optimize_orbitals: Either provide a circuit or a callable vqe_solver")
 
+    if use_hcb:
+        if vqe_solver_arguments is None:
+            vqe_solver_arguments={}
+        vqe_solver_arguments["restrict_to_hcb"]=True
+        # consistency check
+        n_qubits = len(circuit.qubits)
+        n_orbitals = molecule.n_orbitals
+        if n_qubits > n_orbitals:
+            warnings.warn("Potential inconsistency in orbital optimization: use_hcb is switched on but we have\n n_qubits={} in the circuit\n n_orbital={} in the molecule\n".format(n_qubits,n_orbitals), TequilaWarning)
+
     wrapper = PySCFVQEWrapper(molecule_arguments=pyscf_molecule.parameters, n_electrons=pyscf_molecule.n_electrons,
                               const_part=c, circuit=circuit, vqe_solver_arguments=vqe_solver_arguments, silent=silent,
                               vqe_solver=vqe_solver, *args, **kwargs)
     mc.fcisolver = wrapper
     mc.internal_rotation = True
     if pyscf_arguments is not None:
         for k, v in pyscf_arguments.items():
@@ -199,26 +210,16 @@
         if hasattr(result, "circuit"):
             # potential adaptive ansatz
             U = result.circuit
             self.circuit = U
         else:
             # static ansatz
             U = self.circuit
-
-        if restrict_to_hcb:
-            # todo: adapt compute_rdms function to operate in HCB encoding -> faster and less measurements
-            U = molecule.hcb_to_me(U=U)
-            warnings.warn("optimize_orbitals: restrict_to_hcb=True, will use HCB for VQE but will map back to JW for the RDMs -> not fully optimized, see lines in code below this warning for potential speedup :-)", TequilaWarning)
-            # should look like this:
-            #rdm1 = .... compute rdm1 from hcb wavefunction
-            #rdm2 = .... compute rdm2 from hcb wavefunction
-            # then wrap the line below to an else statement
             
-        rdm1, rdm2 = molecule.compute_rdms(U=U, variables=result.variables, spin_free=True, get_rdm1=True,
-                                           get_rdm2=True)
+        rdm1, rdm2 = molecule.compute_rdms(U=U, variables=result.variables, spin_free=True, get_rdm1=True, get_rdm2=True, use_hcb=restrict_to_hcb)
         rdm2 = self.reorder(rdm2, 'dirac', 'mulliken')
         if not self.silent:
             print("{:20} : {}".format("energy", result.energy))
             if len(self.history) > 0:
                 print("{:20} : {}".format("deltaE", result.energy - self.history[-1].energy))
                 print("{:20} : {}".format("||delta RDM1||", numpy.linalg.norm(self.rdm1 - rdm1)))
         self.history.append(result)
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/psi4_interface.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/psi4_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         basisset = ref_wfn.basisset()
         mints = psi4.core.MintsHelper(basisset)
 
         # get integrals in atomic basis
         S = numpy.asarray(mints.ao_overlap())
         h = numpy.asarray(wfn.H())
         g = numpy.asarray(mints.ao_eri())
-        c = numpy.float(wfn.variables()['NUCLEAR REPULSION ENERGY'])
+        c = float(wfn.variables()['NUCLEAR REPULSION ENERGY'])
 
         g = NBodyTensor(elems=numpy.asarray(g), ordering='chem')
 
         kwargs["overlap_integrals"] = S
         kwargs["two_body_integrals"] = g
         kwargs["one_body_integrals"] = h
         kwargs["constant_term"] = c
@@ -572,15 +572,15 @@
 
     @property
     def rdm2(self) -> tuple:
         return super().rdm2
 
     def compute_rdms(self, U: QCircuit = None, variables: Variables = None, spin_free: bool = True,
                      get_rdm1: bool = True, get_rdm2: bool = True, psi4_method: str = None,
-                     psi4_options: dict = {}):
+                     psi4_options: dict = {}, *args, **kwargs):
         """
         Same functionality as qc_base.compute_rdms (look there for more information),
         plus the additional option to compute 1- and 2-RDM using psi4 by the keyword psi4_rdms
 
         Parameters
         ----------
         U :
@@ -601,16 +601,16 @@
            If "detci__opdm" for 1-RDM and "detci__tpdm" for 2-RDM are not included, the keywords get_rdm1, get_rdm2 are
            used (if both are specified, prioritizing psi4_options).
 
         Returns
         -------
         """
         if not psi4_method:
-            super().compute_rdms(U=U, variables=variables, spin_free=spin_free,
-                                 get_rdm1=get_rdm1, get_rdm2=get_rdm2)
+            return super().compute_rdms(U=U, variables=variables, spin_free=spin_free,
+                                 get_rdm1=get_rdm1, get_rdm2=get_rdm2, *args, **kwargs)
         else:
             # Get 1- and 2-particle reduced density matrix via Psi4 CISD computation
             # If "cisd" is chosen, change to "detci" (default is excitation level 2 anyhow) to obtain a CIWavefunction
             if psi4_method.lower() == "cisd":
                 print("Changed psi4_method from 'cisd' to 'detci' with ex_level=2 s.th. psi4 returns a CIWavefunction.")
                 psi4_method = "detci"
             # Set options if not handed over
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/pyscf_interface.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/pyscf_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     mol.symmetry = True
                     mol.symmetry_subgroup = point_group
                 else:
                     mol.symmetry = False
             else:
                 mol.symmetry = True
 
-            mol.build()
+            mol.build(parse_arg=False)
 
             # solve restricted HF
             mf = pyscf.scf.RHF(mol)
             mf.kernel()
             self.irreps = mf.get_irrep_nelec()
             orbital_energies = mf.mo_energy
 
@@ -116,15 +116,15 @@
         norb = self.n_orbitals
         nelec = self.n_electrons
 
         mo_coeff = numpy.eye(norb)
         mo_occ = numpy.zeros(norb)
         mo_occ[:nelec // 2] = 2
 
-        pyscf_mol = pyscf.gto.M(verbose=0)
+        pyscf_mol = pyscf.gto.M(verbose=0, parse_arg=False)
         pyscf_mol.nelectron = nelec
         pyscf_mol.incore_anyway = True  # ensure that custom integrals are used
         pyscf_mol.energy_nuc = lambda *args: c
 
         hf = pyscf.scf.RHF(pyscf_mol)
         hf.get_hcore = lambda *args: h1
         hf.get_ovlp = lambda *args: numpy.eye(norb)
```

### Comparing `tequila-basic-1.8.8/src/tequila/quantumchemistry/qc_base.py` & `tequila-basic-1.8.9/src/tequila/quantumchemistry/qc_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import copy
 from dataclasses import dataclass
 from tequila import TequilaException, BitString, TequilaWarning
 from tequila.hamiltonian import QubitHamiltonian
 
-from tequila.hamiltonian.paulis import Sp, Sm
+from tequila.hamiltonian.paulis import Sp, Sm, Zero
 
 from tequila.circuit import QCircuit, gates
 from tequila.objective.objective import Variable, Variables, ExpectationValue
 
 from tequila.simulators.simulator_api import simulate
 from tequila.utils import to_float
 from .chemistry_tools import ActiveSpaceData, FermionicGateImpl, prepare_product_state, ClosedShellAmplitudes, \
-    Amplitudes, ParametersQC, NBodyTensor, IntegralManager, OrbitalData
+    Amplitudes, ParametersQC, NBodyTensor, IntegralManager
 
 from .encodings import known_encodings
 
 import typing, numpy, numbers
 from itertools import product
 
-# if you are experiencing import errors you need to update openfermion
-# required is version >= 1.0
-# otherwise replace with from openfermion.hamiltonians import MolecularData
-import openfermion
+
 
 try:
+    # if you are experiencing import errors you need to update openfermion
+    # required is version >= 1.0
+    # otherwise replace with from openfermion.hamiltonians import MolecularData
+    import openfermion
     from openfermion.chem import MolecularData
 except:
     try:
         from openfermion.hamiltonians import MolecularData
     except Exception as E:
         raise Exception("{}\nIssue with Tequila Chemistry: Please update openfermion".format(str(E)))
 import warnings
@@ -101,14 +102,21 @@
 
 
         self.transformation = self._initialize_transformation(transformation=transformation, *args, **kwargs)
 
         self._rdm1 = None
         self._rdm2 = None
 
+    def supports_ucc(self):
+        """
+        check if the current molecule supports UCC operations
+        (e.g. mol.make_excitation_gate)
+        """
+        return self.transformation.supports_ucc
+
     def _initialize_transformation(self, transformation=None, *args, **kwargs):
         """
         Helper Function to initialize the Fermion-to-Qubit Transformation
         Parameters
         ----------
         transformation: name of the transformation (passed down from __init__
         args
@@ -188,17 +196,16 @@
             if the unitary is controlled this might not be true!
         Returns
         -------
         type
             1j*Transformed qubit excitation operator, depends on self.transformation
         """
 
-        if type(self.transformation).__name__ == "BravyiKitaevFast":
-            raise TequilaException(
-                "The Bravyi-Kitaev-Superfast transformation does not support general FermionOperators yet")
+        if not self.supports_ucc():
+            raise TequilaException("Molecule with transformation {} does not support general UCC operations".format(self.transformation))
 
         # check indices and convert to list of tuples if necessary
         if len(indices) == 0:
             raise TequilaException("make_excitation_operator: no indices given")
         elif not isinstance(indices[0], typing.Iterable):
             if len(indices) % 2 != 0:
                 raise TequilaException("make_excitation_generator: unexpected input format of indices\n"
@@ -300,20 +307,23 @@
         Returns
         -------
 
         """
         target = []
         for pair in indices:
             assert len(pair) == 2
-            target += [pair[0], pair[1]]
-        consistency = [x < self.n_orbitals for x in target]
+            target += [self.transformation.up(pair[0]), self.transformation.up(pair[1])]
+        if self.transformation.up_then_down:
+            consistency = [x < self.n_orbitals for x in target]
+        else:
+            consistency = [x % 2 == 0  for x in target]
         if not all(consistency):
             raise TequilaException(
-                "make_hardcore_boson_excitation_gate: Inconsistencies in indices={}. Should be indexed from 0 ... n_orbitals={}".format(
-                    indices, self.n_orbitals))
+                "make_hardcore_boson_excitation_gate: Inconsistencies in indices={} for encoding: {}".format(
+                    indices, self.transformation))
         return gates.QubitExcitation(angle=angle, target=target, assume_real=assume_real, control=control,
                                      compile_options=compile_options)
     
     def UR(self,i,j,angle=None, label=None, control=None, assume_real=True, *args, **kwargs):
         """
         Convenience function for orbital rotation circuit (rotating spatial orbital i and j) with standard naming of variables
         See arXiv:2207.12421 Eq.6 for UR(0,1)
@@ -400,14 +410,18 @@
                 Numeric or hashable type or tequila objective
             control:
                 List of possible control qubits
             assume_real:
                 Assume that the wavefunction will always stay real.
                 Will reduce potential gradient costs by a factor of 2
         """
+
+        if not self.supports_ucc():
+            raise TequilaException("Molecule with transformation {} does not support general UCC operations".format(self.transformation))
+
         generator = self.make_excitation_generator(indices=indices, remove_constant_term=control is None)
         p0 = self.make_excitation_generator(indices=indices, form="P0", remove_constant_term=control is None)
 
         return QCircuit.wrap_gate(
             FermionicGateImpl(angle=angle, generator=generator, p0=p0,
                               transformation=type(self.transformation).__name__.lower(), indices=indices,
                               assume_real=assume_real,
@@ -552,15 +566,15 @@
         # can not be an instance of a specific backend (otherwise we get inconsistencies with classical methods in the backend)
         if inplace:
             self.integral_manager.transform_to_native_orbitals()
             return self
         else:
             integral_manager = copy.deepcopy(self.integral_manager)
             integral_manager.transform_to_native_orbitals()
-            result = QuantumChemistryBase(parameters=self.parameters, integral_manager=integral_manager, orbital_type="native")
+            result = QuantumChemistryBase(parameters=self.parameters, integral_manager=integral_manager, orbital_type="native", transformation=self.transformation)
             return result
 
 
     def do_make_molecule(self, *args, **kwargs):
         """
         Called by self.make_molecule with args and kwargs passed through
         Override this in derived class if needed
@@ -641,25 +655,24 @@
         try:
             qop = self.transformation(fop)
         except TypeError:
             qop = self.transformation(openfermion.transforms.get_interaction_operator(fop))
         qop.is_hermitian()
         return qop
 
-    def make_hardcore_boson_hamiltonian(self):
+    def make_hardcore_boson_hamiltonian(self, condensed=False):
         """
         Returns
         -------
         Hamiltonian in Hardcore-Boson approximation (electrons are forced into spin-pairs)
         Indepdent of Fermion-to-Qubit mapping
+        condensed: always give Hamiltonian back from qubit 0 to N where N is the number of orbitals
+        if condensed=False then JordanWigner would give back the Hamiltonian defined on even qubits between 0 to 2N
         """
-        if not self.transformation.up_then_down:
-            warnings.warn(
-                "Hardcore-Boson Hamiltonian without reordering will result in non-consecutive Hamiltonians that are eventually not be combinable with other features of tequila. Try transformation=\'ReorderedJordanWigner\' or similar for more consistency",
-                TequilaWarning)
+
         # integrate with QubitEncoding at some point
         n_orbitals = self.n_orbitals
         c, obt, tbt = self.get_integrals()
         h = numpy.zeros(shape=[n_orbitals] * 2)
         g = numpy.zeros(shape=[n_orbitals] * 2)
         for p in range(n_orbitals):
             h[p, p] += 2 * obt[p, p]
@@ -671,14 +684,17 @@
         H = c
         for p in range(n_orbitals):
             for q in range(n_orbitals):
                 up = p
                 uq = q
                 H += h[p, q] * Sm(up) * Sp(uq) + g[p, q] * Sm(up) * Sp(up) * Sm(uq) * Sp(uq)
 
+        if not self.transformation.up_then_down and not condensed:
+            alpha_map = {k.idx:self.transformation.up(k.idx) for k in self.orbitals}
+            H = H.map_qubits(alpha_map)
         return H
 
     def make_molecular_hamiltonian(self, occupied_indices=None, active_indices=None):
         """
         Returns
         -------
         Create a MolecularHamiltonian as openfermion Class
@@ -753,26 +769,27 @@
     def prepare_hardcore_boson_reference(self):
         """
         Prepare reference state in the Hardcore-Boson approximation (eqch qubit represents two spin-paired electrons)
         Returns
         -------
         tq.QCircuit that prepares the HCB reference
         """
-        U = gates.X(target=[i.idx for i in self.reference_orbitals])
+        U = gates.X(target=[self.transformation.up(i.idx) for i in self.reference_orbitals])
         U.n_qubits = self.n_orbitals
         return U
 
-    def hcb_to_me(self, U=None):
+    def hcb_to_me(self, U=None, condensed=False):
         """
         Transform a circuit in the hardcore-boson encoding (HCB)
         to the encoding of this molecule
         HCB is supposed to be encoded on the first n_orbitals qubits
         Parameters
         ----------
         U: HCB circuit (using the alpha qubits)
+        condensed: assume that incoming U is condensed (HCB on the first n_orbitals; and not, as for example in JW on the first n even orbitals)
         Returns
         -------
 
         """
         if U is None:
             U = QCircuit()
 
@@ -780,16 +797,20 @@
         consistency = [x < self.n_orbitals for x in U.qubits]
         if not all(consistency):
             warnings.warn(
                 "hcb_to_me: given circuit is not defined on the first {} qubits. Is this a HCB circuit?".format(
                     self.n_orbitals))
 
         # map to alpha qubits
-        alpha_map = {k: self.transformation.up(k) for k in range(self.n_orbitals)}
-        alpha_U = U.map_qubits(qubit_map=alpha_map)
+        if condensed:
+            alpha_map = {k: self.transformation.up(k) for k in range(self.n_orbitals)}
+            alpha_U = U.map_qubits(qubit_map=alpha_map)
+        else:
+            alpha_U = U
+
         UX = self.transformation.hcb_to_me()
         if UX is None:
             raise TequilaException(
                 "transformation={} has no hcb_to_me function implemented".format(self.transformation))
         return alpha_U + UX
 
     def get_pair_specific_indices(self,
@@ -927,21 +948,21 @@
         if self.n_electrons % 2 != 0:
             raise TequilaException("need even number of electrons for SPA ansatz.\n{} active electrons".format(self.n_electrons))
         # making sure that enough edges are assigned
         n_edges = len(edges)
         if len(edges) != self.n_electrons//2:
             raise TequilaException("number of edges need to be equal to number of active electrons//2\n{} edges given\n{} active electrons\nfrozen core is {}".format(len(edges), self.n_electrons, self.parameters.frozen_core))
         # making sure that orbitals are uniquely assigned to edges
-        for edge in edges:
-            for orbital in edge:
+        for edge_qubits in edges:
+            for q1 in edge_qubits:
                 for edge2 in edges:
-                    if edge2==edge:
+                    if edge2==edge_qubits:
                         continue
-                    elif orbital in edge2:
-                        raise TequilaException("make_spa_ansatz: faulty list of edges, orbitals are overlapping e.g. orbital {} is in edge {} and edge {}".format(orbital, edge, edge2))
+                    elif q1 in edge2:
+                        raise TequilaException("make_spa_ansatz: faulty list of edges, orbitals are overlapping e.g. orbital {} is in edge {} and edge {}".format(q1, edge_qubits, edge2))
         
         # auto assign if the circuit construction is optimized
         # depending on the current qubit encoding (if hcb_to_me is implemnented we can optimize)
         if optimize is None:
             try:
                 have_hcb_to_me = self.hcb_to_me() is not None
             except:
@@ -951,63 +972,74 @@
             else:
                 optimize=False
 
         U = QCircuit()
         
         # construction of the optimized circuit
         if optimize:
-            for edge in edges:
-                U += gates.X(2*edge[0])
-                previous = edge[0]
-                if len(edge)==1:
+            # circuit in HCB representation
+            # depends a bit on the ordering of the spin-orbitals in the encoding
+            # here we transform it to the qubits representing the up-spins
+            # the hcb_to_me sequence will then transfer to the actual encoding later
+            for edge_orbitals in edges:
+                edge_qubits = [self.transformation.up(i) for i in edge_orbitals]
+                U += gates.X(edge_qubits[0])
+                if len(edge_qubits)==1:
                     continue
-                for orbital in edge[1:]:
-                    c=previous
+                for i in range(1,len(edge_qubits)):
+                    q1=edge_qubits[i]
+                    c=edge_qubits[i-1]
                     if not ladder:
-                        c=edge[0]
-                    angle=Variable(name=((c, orbital), "D" ,label))
+                        c=edge_qubits[0]
+                    angle=Variable(name=((edge_orbitals[i-1], edge_orbitals[i]), "D" ,label))
                     if use_units_of_pi:
                         angle=angle*numpy.pi
-                    if previous == edge[0]:
-                        U += gates.Ry(angle=angle, target=2*orbital, control=None)
+                    if i-1 == 0:
+                        U += gates.Ry(angle=angle, target=q1, control=None)
                     else:
-                        U += gates.Ry(angle=angle, target=2*orbital, control=2*c)
-                    U += gates.CNOT(2*orbital,2*c)
-                    previous = orbital
+                        U += gates.Ry(angle=angle, target=q1, control=c)
+                    U += gates.CNOT(q1,c)
+
 
             if not hcb:
                 U += self.hcb_to_me()
         else:
-            # construction of the non-optimized circuit
-            U = self.prepare_reference()
+            # construction of the non-optimized circuit (UpCCD with paired doubles according to edges)
+            if hcb:
+                U = self.prepare_hardcore_boson_reference()
+            else:
+                U = self.prepare_reference()
             # will only work if the first orbitals in the edges are the reference orbitals
             sane = True
             reference_orbitals = self.reference_orbitals
-            for edge in edges:
-                if self.orbitals[edge[0]] not in reference_orbitals:
+            for edge_qubits in edges:
+                if self.orbitals[edge_qubits[0]] not in reference_orbitals:
                     sane=False
-                if len(edge)>1:
-                    for orbital in edge[1:]:
-                        if self.orbitals[orbital] in reference_orbitals:
+                if len(edge_qubits)>1:
+                    for q1 in edge_qubits[1:]:
+                        if self.orbitals[q1] in reference_orbitals:
                             sane=False
             if not sane:
                 raise TequilaException("Non-Optimized SPA (e.g. with encodings that are not JW) will only work if the first orbitals of all SPA edges are occupied reference orbitals and all others are not. You gave edges={} and reference_orbitals are {}".format(edges, reference_orbitals))
 
-            for edge in edges:
-                previous = edge[0]
-                if len(edge)>1:
-                    for orbital in edge[1:]:
+            for edge_qubits in edges:
+                previous = edge_qubits[0]
+                if len(edge_qubits)>1:
+                    for q1 in edge_qubits[1:]:
                         c = previous
                         if not ladder:
-                            c = edge[0]
-                        angle = Variable(name=((c,orbital), "D" ,label))
+                            c = edge_qubits[0]
+                        angle = Variable(name=((c,q1), "D" ,label))
                         if use_units_of_pi:
                             angle=angle*numpy.pi
-                        U += self.make_excitation_gate(indices=[(2*c,2*orbital),(2*c+1,2*orbital+1)], angle=angle)
-                        previous = orbital
+                        if hcb:
+                            U += self.make_hardcore_boson_excitation_gate(indices=[(q1,c)],angle=angle)
+                        else:
+                            U += self.make_excitation_gate(indices=[(2*c,2*q1),(2*c+1,2*q1+1)], angle=angle)
+                        previous = q1
         return U
 
     def make_ansatz(self, name: str, *args, **kwargs):
         """
         Automatically calls the right subroutines to construct ansatze implemented in tequila.chemistry
         name: namne of the ansatz, examples are: UpCCGSD, UpCCD, SPA, UCCSD, SPA+UpCCD, SPA+GS
         """
@@ -1580,15 +1612,15 @@
         if self._rdm2 is not None:
             return self._rdm2
         else:
             print("2-RDM has not been computed. Return None for 2-RDM.")
             return None
 
     def compute_rdms(self, U: QCircuit = None, variables: Variables = None, spin_free: bool = True,
-                     get_rdm1: bool = True, get_rdm2: bool = True, ordering="dirac"):
+                     get_rdm1: bool = True, get_rdm2: bool = True, ordering="dirac", use_hcb: bool = False):
         """
         Computes the one- and two-particle reduced density matrices (rdm1 and rdm2) given
         a unitary U. This method uses the standard ordering in physics as denoted below.
         Note, that the representation of the density matrices depends on the qubit transformation
         used. The Jordan-Wigner encoding corresponds to 'classical' second quantized density
         matrices in the occupation picture.
 
@@ -1615,31 +1647,45 @@
 
         Returns
         -------
         """
         # Check whether unitary circuit is not 0
         if U is None:
             raise TequilaException('Need to specify a Quantum Circuit.')
-
         # Check whether transformation is BKSF.
         # Issue here: when a single operator acts only on a subset of qubits, BKSF might not yield the correct
         # transformation, because it computes the number of qubits incorrectly in this case.
         # A hotfix such as for symmetry_conserving_bravyi_kitaev would require deeper changes, thus omitted for now
         if type(self.transformation).__name__ == "BravyiKitaevFast":
             raise TequilaException(
                 "The Bravyi-Kitaev-Superfast transformation does not support general FermionOperators yet.")
-
         # Set up number of spin-orbitals and molecular orbitals respectively
         n_SOs = 2 * self.n_orbitals
         n_MOs = self.n_orbitals
 
         # Check whether unitary circuit is not 0
         if U is None:
             raise TequilaException('Need to specify a Quantum Circuit.')
 
+        def _get_hcb_op(op_tuple):
+            '''Build the hardcore boson operators: b^\dagger_ib_j + h.c. in qubit encoding '''
+            if (len(op_tuple) == 2):
+                return 2 * Sm(op_tuple[0][0]) * Sp(op_tuple[1][0])
+            elif (len(op_tuple) == 4):
+                if ((op_tuple[0][0] == op_tuple[1][0]) and (op_tuple[2][0] == op_tuple[3][0])):  # iijj uddu+duud
+                    return Sm(op_tuple[0][0]) * Sp(op_tuple[2][0]) + Sm(op_tuple[2][0]) * Sp(op_tuple[0][0])
+                if ((op_tuple[0][0] == op_tuple[2][0]) and (op_tuple[1][0] == op_tuple[3][0]) and (
+                        op_tuple[0][0] != op_tuple[1][0]) and (op_tuple[2][0] != op_tuple[3][0])):  # ijij uuuu+dddd
+                    return 4 * Sm(op_tuple[0][0]) * Sm(op_tuple[1][0]) * Sp(op_tuple[2][0]) * Sp(op_tuple[3][0])
+                if ((op_tuple[0][0] == op_tuple[3][0]) and (op_tuple[1][0] == op_tuple[2][0]) and (
+                        op_tuple[0][0] != op_tuple[1][0]) and (op_tuple[2][0] != op_tuple[3][0])):  # ijji abba
+                    return -2 * Sm(op_tuple[0][0]) * Sm(op_tuple[1][0]) * Sp(op_tuple[2][0]) * Sp(op_tuple[3][0])
+            else:
+                return Zero()
+
         def _get_of_op(operator_tuple):
             """ Returns operator given by a operator tuple as OpenFermion - Fermion operator """
             op = openfermion.FermionOperator(operator_tuple)
             return op
 
         def _get_qop_hermitian(of_operator) -> QubitHamiltonian:
             """ Returns Hermitian part of Fermion operator as QubitHamiltonian """
@@ -1714,17 +1760,15 @@
                     op_tuple = ((2 * p + 1, 1), (2 * q, 1), (2 * s, 0), (2 * r + 1, 0)) if (
                             2 * p + 1 != 2 * q and 2 * r + 1 != 2 * s) else '0.0 []'
                     op += _get_of_op(op_tuple)
                     # Spin bbbb
                     op_tuple = ((2 * p + 1, 1), (2 * q + 1, 1), (2 * s + 1, 0), (2 * r + 1, 0)) if (
                             p != q and r != s) else '0.0 []'
                     op += _get_of_op(op_tuple)
-
                     ops += [op]
-
             return ops
 
         def _assemble_rdm1(evals) -> numpy.ndarray:
             """
             Returns spin-ful or spin-free one-particle RDM built by symmetry conditions
             Same symmetry with or without spin, so we can use the same function
             """
@@ -1779,49 +1823,99 @@
             # Further permutational symmetry: pqrs = qpsr
             for p, q, r, s in product(range(n_MOs), repeat=4):
                 if p >= q or r >= s:
                     rdm2[q, p, s, r] = rdm2[p, q, r, s]
 
             return rdm2
 
+        def _build_1bdy_operators_hcb() -> list:
+            """ Returns hcb one-body operators as a symmetry-reduced list of QubitHamiltonians """
+            # Exploit symmetry pq = qp (not changed by spin-summation)
+            ops = []
+            for p in range(n_MOs):
+                for q in range(p + 1):
+                    if (p == q):
+                        if (self.transformation.up_then_down):
+                            op_tuple = ((p, 1), (p, 0))
+                            op = _get_hcb_op(op_tuple)
+                        else:
+                            op_tuple = ((2 * p, 1), (2 * p, 0))
+                            op = _get_hcb_op(op_tuple)
+                        ops += [op]
+                    else:
+                        ops += [Zero()]
+            return ops
+
+        def _build_2bdy_operators_hcb() -> list:
+            """ Returns hcb two-body operators as a symmetry-reduced list of QubitHamiltonians """
+            # Exploit symmetries pqrs = qpsr (due to spin summation, '-pqsr = -qprs' drops out)
+            #                and      = rspq
+            ops = []
+            scale = 2
+            if self.transformation.up_then_down:
+                scale = 1
+            for p, q, r, s in product(range(n_MOs), repeat=4):
+                if p * n_MOs + q >= r * n_MOs + s and (p >= q or r >= s):
+                    # Spin abba+ baab allow p=q=r=s orb iijj
+                    op_tuple = ((scale * p, 1), (scale * q, 1), (scale * r, 0), (scale * s, 0)) if (
+                            p == q and s == r) else '0.0 []'
+                    op = _get_hcb_op(op_tuple)
+                    # Spin abba+ baab dont allow p=q=r=s orb ijij
+                    op_tuple = ((scale * p, 1), (scale * q, 1), (scale * r, 0), (scale * s, 0)) if (
+                            p != q and r != s and p == r and s == q) else '0.0 []'
+                    op += _get_hcb_op(op_tuple)
+                    # Spin aaaa+ bbbb dont allow p=q=r=s  orb ijji
+                    op_tuple = ((scale * p, 1), (scale * q, 1), (scale * r, 0), (scale * s, 0)) if (
+                            p != q and r != s and p == s and q == r) else '0.0 []'
+                    op += _get_hcb_op(op_tuple)
+                    ops += [op]
+            return ops
+
         # Build operator lists
         qops = []
-        if spin_free:
+        if spin_free and not use_hcb:
             qops += _build_1bdy_operators_spinfree() if get_rdm1 else []
             qops += _build_2bdy_operators_spinfree() if get_rdm2 else []
+        elif use_hcb:
+            qops += _build_1bdy_operators_hcb() if get_rdm1 else []
+            qops += _build_2bdy_operators_hcb() if get_rdm2 else []
         else:
+            if use_hcb:
+                raise TequilaException(
+                    "compute_rdms: spin_free={} and use_hcb={} are not compatible".format(spin_free, use_hcb))
             qops += _build_1bdy_operators_spinful() if get_rdm1 else []
             qops += _build_2bdy_operators_spinful() if get_rdm2 else []
 
         # Transform operator lists to QubitHamiltonians
-        qops = [_get_qop_hermitian(op) for op in qops]
+        if (not use_hcb):
+            qops = [_get_qop_hermitian(op) for op in qops]
         # Compute expected values
         evals = simulate(ExpectationValue(H=qops, U=U, shape=[len(qops)]), variables=variables)
 
         # Assemble density matrices
         # If self._rdm1, self._rdm2 exist, reset them if they are of the other spin-type
         def _reset_rdm(rdm):
             if rdm is not None:
-                if spin_free and rdm.shape[0] != n_MOs:
+                if (spin_free or use_hcb) and rdm.shape[0] != n_MOs:
                     return None
                 if not spin_free and rdm.shape[0] != n_SOs:
                     return None
             return rdm
 
         self._rdm1 = _reset_rdm(self._rdm1)
         self._rdm2 = _reset_rdm(self._rdm2)
         # Split expectation values in 1- and 2-particle expectation values
         if get_rdm1:
-            len_1 = n_MOs * (n_MOs + 1) // 2 if spin_free else n_SOs * (n_SOs + 1) // 2
+            len_1 = n_MOs * (n_MOs + 1) // 2 if (spin_free or use_hcb) else n_SOs * (n_SOs + 1) // 2
         else:
             len_1 = 0
         evals_1, evals_2 = evals[:len_1], evals[len_1:]
         # Build matrices using the expectation values
         self._rdm1 = _assemble_rdm1(evals_1) if get_rdm1 else self._rdm1
-        if spin_free:
+        if spin_free or use_hcb:
             self._rdm2 = _assemble_rdm2_spinfree(evals_2) if get_rdm2 else self._rdm2
         else:
             self._rdm2 = _assemble_rdm2_spinful(evals_2) if get_rdm2 else self._rdm2
 
         if get_rdm2:
             rdm2 = NBodyTensor(elems=self.rdm2, ordering="dirac")
             rdm2.reorder(to=ordering)
```

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_api.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from tequila.objective import Objective, Variable, assign_variable, format_variable_dictionary, QTensor
 from tequila.utils.exceptions import TequilaException, TequilaWarning
 from tequila.simulators.simulator_base import BackendCircuit, BackendExpectationValue
 from tequila.circuit.noise import NoiseModel
 
 SUPPORTED_BACKENDS = ["qulacs_gpu", "qulacs",'qibo', "qiskit", "cirq", "pyquil", "symbolic", "qlm"]
-SUPPORTED_NOISE_BACKENDS = ["qiskit",'qibo', 'cirq', 'pyquil', 'qulacs', "qulacs_gpu"]
+SUPPORTED_NOISE_BACKENDS = ["qiskit", 'cirq', 'pyquil'] # qulacs removed in v.1.9
 BackendTypes = namedtuple('BackendTypes', 'CircType ExpValueType')
 INSTALLED_SIMULATORS = {}
 INSTALLED_SAMPLERS = {}
 
 HAS_QULACS = True
 INSTALLED_NOISE_SAMPLERS = {}
 if typing.TYPE_CHECKING:
```

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_base.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_base.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_cirq.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_cirq.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_pyquil.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_pyquil.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_qibo.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_qibo.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         Returns
         -------
         QubitWaveFunction:
             QubitWaveFunction representing result of the simulation.
         """
         n_qubits = max(self.highest_qubit + 1, self.n_qubits, self.abstract_circuit.max_qubit() + 1)
         if initial_state is not None:
-            if isinstance(initial_state, int) or isinstance(initial_state,np.int):
+            if isinstance(initial_state, (int, np.int64)):
                 wave = QubitWaveFunction.from_int(i=initial_state, n_qubits=n_qubits)
             elif isinstance(initial_state, str):
                 wave = QubitWaveFunction.from_string(string=initial_state).to_array()
             elif isinstance(initial_state, QubitWaveFunction):
                 wave = initial_state
             elif isinstance(initial_state,np.ndarray):
                 wave = QubitWaveFunction.from_array(initial_state)
```

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_qiskit.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_qiskit.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_qlm.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_qlm.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_qulacs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import qulacs
 import numbers, numpy
-from tequila import TequilaException
+import warnings
+
+from tequila import TequilaException, TequilaWarning
 from tequila.utils.bitstrings import BitNumbering, BitString, BitStringLSB
 from tequila.wavefunction.qubit_wavefunction import QubitWaveFunction
 from tequila.simulators.simulator_base import BackendCircuit, BackendExpectationValue, QCircuit, change_basis
 from tequila.utils.keymap import KeyMapRegisterToSubregister
 
 """
 Developer Note:
@@ -87,14 +89,17 @@
             'Exp-Pauli': None
         }
         self.measurements = None
         self.variables = []
         super().__init__(abstract_circuit=abstract_circuit, noise=noise, *args, **kwargs)
         self.has_noise=False
         if noise is not None:
+
+            warnings.warn("Warning: noise in qulacs module will be dropped. Currently only works for qulacs version 0.5 or lower", TequilaWarning)
+
             self.has_noise=True
             self.noise_lookup = {
                 'bit flip': [qulacs.gate.BitFlipNoise],
                 'phase flip': [lambda target, prob: qulacs.gate.Probabilistic([prob],[qulacs.gate.Z(target)])],
                 'phase damp': [lambda target, prob: qulacs.gate.DephasingNoise(target,(1/2)*(1-numpy.sqrt(1-prob)))],
                 'amplitude damp': [qulacs.gate.AmplitudeDampingNoise],
                 'phase-amplitude damp': [qulacs.gate.AmplitudeDampingNoise,
```

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs_gpu.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_qulacs_gpu.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/simulators/simulator_symbolic.py` & `tequila-basic-1.8.9/src/tequila/simulators/simulator_symbolic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/tools/convenience.py` & `tequila-basic-1.8.9/src/tequila/tools/convenience.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/tools/qng.py` & `tequila-basic-1.8.9/src/tequila/tools/qng.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/tools/random_generators.py` & `tequila-basic-1.8.9/src/tequila/tools/random_generators.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/utils/bitstrings.py` & `tequila-basic-1.8.9/src/tequila/utils/bitstrings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/utils/exceptions.py` & `tequila-basic-1.8.9/src/tequila/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/utils/joined_transformation.py` & `tequila-basic-1.8.9/src/tequila/utils/joined_transformation.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/utils/keymap.py` & `tequila-basic-1.8.9/src/tequila/utils/keymap.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/utils/misc.py` & `tequila-basic-1.8.9/src/tequila/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila/wavefunction/qubit_wavefunction.py` & `tequila-basic-1.8.9/src/tequila/wavefunction/qubit_wavefunction.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.8/src/tequila_basic.egg-info/PKG-INFO` & `tequila-basic-1.8.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,132 +1,53 @@
-Metadata-Version: 2.1
-Name: tequila-basic
-Version: 1.8.8
-Summary: A High-Level Abstraction Framework for Quantum Algorithms
-Home-page: https://github.com/tequilahub/tequila
-Author: Jakob Kottmann and Sumner Alperin-Lea and Teresa Tamayo-Mendoza and Alba Cervera-Lierta and Cyrille Lavigne and Tzu-Ching Yen and Vladyslav Verteletskyi and Philipp Schleich and Abhinav Anand and Matthias Degroote and Skylar Chaney and Maha Kesibi and Naomi Grace Curnow and Brandon Solo and Georgios Tsilimigkounakis and Claudia Zendejas-Morales and Artur F Izmaylov and Alan Aspuru-Guzik ... 
-Author-email: jakob.kottmann@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENCE) [![DOI](https://zenodo.org/badge/259718912.svg)](https://zenodo.org/badge/latestdoi/259718912) [![PyPI version](https://badge.fury.io/py/tequila-basic.svg)](https://badge.fury.io/py/tequila-basic) ![CI](https://github.com/tequilahub/tequila/actions/workflows/ci_basic.yml/badge.svg)
 
-![Image](docs/all_in_one_example.png)
-
 # Tequila
 
 Tequila is an abstraction framework for (variational) quantum algorithms.  
 It operates on abstract data structures allowing the formulation, combination, automatic differentiation and optimization of generalized objectives.
 Tequila can execute the underlying quantum expectation values on state of the art simulators as well as on real quantum devices.  
 
-Check out this small overview to get a glimpse on [what tequila is,](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
-or, get an overview through different slides and recordings of talks on different level of detail: See [here](https://kottmanj.github.io/talks_and_material/).  
-
-Get started with our [BasicUsage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb) Tutorial or find more in the [Tutorial collection](https://github.com/aspuru-guzik-group/tequila-tutorials)  
-
-or checkout our [overview article](https://arxiv.org/abs/2011.03057)  
-
-# Quantum Backends
-Currently supported
-- [Qulacs](https://github.com/qulacs/qulacs)
-- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
-- [Qiskit](https://github.com/qiskit/qiskit)  
-- [Cirq](https://github.com/quantumlib/cirq)
-- [PyQuil](https://github.com/rigetti/pyquil)
-- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
-
-Tequila detects backends automatically if they are installed on your systems.
-All of them are available over standard pip installation like for example `pip install qulacs`.
-For best performance it is recommended to have `qulacs` installed.
-
-# QuantumChemistry:
-Currently supported
-## [Psi4](https://github.com/psi4/psi4).
-In a conda environment this can be installed with
-```bash
-conda install psi4 -c psi4
-```
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
-
-## [Madness](https://github.com/kottmanj/madness)  
-In a conda environment this can be installed with  
-```bash
-conda install madtequila -c kottmann
-```  
-This installs a modified version of madness ready to use with tequila.  
-Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
-Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage.
-
-## [PySCF](https://github.com/pyscf/pyscf)  
-Install with
-```bash
-pip install pyscf
-```  
-Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
+- [overview article](https://arxiv.org/abs/2011.03057)   
+- [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
+- [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
+- [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
+- [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
+- [talks and slides](https://kottmanj.github.io/talks_and_material/)  
+
+# Installation
+Recommended Python version is 3.8-3.9.   
+Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.
 
-# Install from source
+## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
-We recommend installing in editable mode with
-```bash
-git clone https://github.com/tequilahub/tequila.git
-cd tequila
-pip install -e .
-```
-
-You can install `tequila` directly with pip over:
-```bash
-pip install git+https://github.com/tequilahub/tequila.git
-```
-Install from devel branch (most recent updates):
-```bash
-pip install git+https://github.com/tequilahub/tequila.git@devel
-```
-
-Recommended Python version is 3.7.
-Python 3.8 works, but not all (optional) dependencies support it yet (e.g. Psi4).
-Python 3.6 works, but some (optional) dependencies might have issues with numpy >= 1.20.
-
-# Install from PyPi
-**Do not** install like this:
-<strike>`pip install tequila`</strike>
-
-this will install a Minecraft server manager (might be useful for other things, but probably not what you are looking for).
-
 You can install tequila from PyPi as:
 ```bash
 pip install tequila-basic
 ```
 this will install tequila with all essential dependencies.
 We recommend to install some fast quantum backends, like qulacs or qibo, as well.
 Those can be installed before or after you install tequila.
 ```bash
 # install basic tequila
 pip install tequila-basic
 # install qulacs and/or other backends and use it within tequila
 pip install qulacs
 ```
 
-# Install with Windows
+## Install from github 
+You can install `tequila` directly with pip over:
+```bash
+pip install git+https://github.com/tequilahub/tequila.git
+```
+Install from devel branch (most recent updates):
 ```bash
-pip install git+https://github.com/tequilahub/tequila.git@windows
+pip install git+https://github.com/tequilahub/tequila.git@devel
 ```
-See also the troubleshooting below if you want to tweak things manually.  
-The command above will not install the qulacs simulator.  
-You can install it on windows OS, but you need to have cmake and c++ compilers ready (can be installed for example over visual studio).  
-Of course you can also use one of the other backends (see above).  
-
-# Getting Started
-We have a collection of [*tutorials*](https://github.com/tequilahub/tequila-tutorials) covering basic usage of tequila as well as cutting edge research content:
-- Tutorial on [Basic Usage](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/BasicUsage.ipynb)  
-- Chemistry tutorial with psi4: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
-- Chemistry tutorial with madness: see [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)
-- check the list of research projects below for links to specific examples.  
-- all tutorials: [github/tequilahub/tequila-tutorials](https://github.com/tequilahub/tequila-tutorials).  
 
 ## Tequila Hello World
 ```python
 # optimize a one qubit example
 
 # define a variable
 a = tq.Variable("a")
@@ -143,21 +64,16 @@
 print("optimized wavefunction = ", wfn)
 # plot information about the optimization
 result.history.plot("energies")
 result.history.plot("angles")
 result.history.plot("gradients")
 ```
 
-## Chemistry Hello World (Madness backend)  
-Install backend as
-```bash
-conda install madtequila -c kottmann
-```  
-or see above for more.    
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb)  
+## Chemistry Hello World (Madness backend)   
+see below for installation of dependencies  
 ```python
 import tequila as tq
 
 # initialize molecule (also works over .xyz files --> see next example)
 geomstring="Li 0.0 0.0 0.0\nH 0.0 0.0 1.6"
 mol = tq.Molecule(geometry=geomstring)
 
@@ -170,55 +86,48 @@
 # define the expectation value
 E = tq.ExpectationValue(H=H, U=U)
 
 # minimize the expectation value
 result = tq.minimize(E)
 
 # optional:compute classical reference energies
-# needs pyscf
+# needs pyscf as well
 cisd = mol.compute_energy("cisd")
 fci = mol.compute_energy("fci")
 
 print("VQE : {:+2.8}f".format(result.energy))
 print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 
 ```
 
 ## Chemistry Hello World (Psi4 or PySCF backend)
-install backends with
-```bash
-pip install pyscf
-# and/or
-conda install psi4 -c psi4 
-```
-more info [here](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb)
+see below for installation of dependencies  
 ```python
 # define a molecule within an active space
-active = {"a1": [1], "b1":[0]}
+active_orbitals=[1,2,5]
 molecule = tq.quantumchemistry.Molecule(geometry="lih.xyz", basis_set='6-31g', active_orbitals=active, transformation="bravyi-kitaev")
 
 # get the qubit hamiltonian
 H = molecule.make_hamiltonian()
 
 # create an k-UpCCGSD circuit of order k
-U = molecule.make_upccgsd_ansatz(order=1, include_singles=True)
+U = molecule.make_ansatz(name="UpCCGSD")
 
 # define the expectationvalue
 E = tq.ExpectationValue(H=H, U=U)
 
 # compute reference energies
 fci = molecule.compute_energy("fci")
 cisd = molecule.compute_energy("detci", options={"detci__ex_level": 2})
 
 # optimize
 result = tq.minimize(objective=E, method="BFGS", initial_values=0.0)
 
 print("VQE : {:+2.8}f".format(result.energy))
-print("CISD: {:+2.8}f".format(cisd))
 print("FCI : {:+2.8}f".format(fci))
 ```
 
 Do you want to create your own methods? Check out the [tutorials](https://github.com/tequilahub/tequila-tutorials)!
 
 # Some Research projects using Tequila
 J.S. Kottmann, A. Anand, A. Aspuru-Guzik.  
@@ -325,14 +234,52 @@
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
 Quantum backends are treated in the same way.
 
+## Quantum Backends
+Currently supported
+- [Qulacs](https://github.com/qulacs/qulacs) (recommended)
+- [Qibo](https://github.com/Quantum-TII/qibo) -- currently needs to be qibo==0.1.1
+- [Qiskit](https://github.com/qiskit/qiskit)  
+- [Cirq](https://github.com/quantumlib/cirq)
+- [PyQuil](https://github.com/rigetti/pyquil)
+- [QLM](https://atos.net/en/solutions/quantum-learning-machine) (works also whith [myQLM](https://myqlm.github.io/index.html))
+
+Tequila detects backends automatically if they are installed on your systems.
+All of them are available over standard pip installation like for example `pip install qulacs`.
+For best performance it is recommended to have `qulacs` installed.
+
+## QuantumChemistry:
+Currently supported
+### [Psi4](https://github.com/psi4/psi4).
+In a conda environment this can be installed with
+```bash
+conda install psi4 -c psi4
+```
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
+
+### [Madness](https://github.com/kottmanj/madness)  
+In a conda environment this can be installed with  
+```bash
+conda install madtequila -c kottmann
+```  
+This installs a modified version of madness ready to use with tequila.  
+Alternatively it can be compiled from the sources provided in this [fork](https://github.com/kottmanj/madness) (follow readme instructions there).  
+Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/MadnessInterface.ipynb) that illustrates the usage. For fast performance it is recommended to not use the conda package.
+
+### [PySCF](https://github.com/pyscf/pyscf)  
+Install with
+```bash
+pip install pyscf
+```  
+Works similar as Psi4. Classical methods are also integrated in the madness interface allowing to use them in a basis-set-free representation.
+
 # Documentation
 You can build the documentation by navigating to `docs` and entering `make html`.
 Open the documentation with a browser over like `firefox docs/build/html/index.html`
 Note that you will need some additional python packages like `sphinx` and `mr2` that are not explicitly listed in the requirements.txt
 
 You can also visit our prebuild online [documentation](https://tequilahub.github.io/tequila/)
 that will correspond to the github master branch
```

### Comparing `tequila-basic-1.8.8/src/tequila_basic.egg-info/SOURCES.txt` & `tequila-basic-1.8.9/src/tequila_basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

